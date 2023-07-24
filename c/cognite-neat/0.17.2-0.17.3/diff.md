# Comparing `tmp/cognite_neat-0.17.2.tar.gz` & `tmp/cognite_neat-0.17.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.17.2.tar", max compression
+gzip compressed data, was "cognite_neat-0.17.3.tar", max compression
```

## Comparing `cognite_neat-0.17.2.tar` & `cognite_neat-0.17.3.tar`

### file list

```diff
@@ -1,120 +1,123 @@
--rw-r--r--   0        0        0    11351 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/LICENSE
--rw-r--r--   0        0        0     8765 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/README.md
--rw-r--r--   0        0        0       61 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/_version.py
--rw-r--r--   0        0        0     9986 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/base_workflows/graph2assets_relationships.py
--rw-r--r--   0        0        0     7037 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/base_workflows/graphs_and_rules.py
--rw-r--r--   0        0        0    14391 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/base_workflows/sheet2cdf.py
--rw-r--r--   0        0        0    11824 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/base_workflows/sme_graph_capture.py
--rw-r--r--   0        0        0      871 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2792 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/app.py
--rw-r--r--   0        0        0     5616 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0        0 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      758 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/exceptions.py
--rw-r--r--   0        0        0      586 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     2837 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/extractors/_exceptions.py
--rw-r--r--   0        0        0        0 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/extractors/cdfcore/__init__.py
--rw-r--r--   0        0        0     2288 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/extractors/cdfcore/labels.py
--rw-r--r--   0        0        0     5048 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/extractors/cdfcore/models.py
--rw-r--r--   0        0        0    39905 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/extractors/cdfcore/rdf_to_assets.py
--rw-r--r--   0        0        0    20940 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/extractors/cdfcore/rdf_to_relationships.py
--rw-r--r--   0        0        0     5516 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/extractors/graph_sheet_to_graph.py
--rw-r--r--   0        0        0       99 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0      938 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/loader/graph_capturing_sheet.py
--rw-r--r--   0        0        0    11407 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0        0 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    12903 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0       73 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9594 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0     2026 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/rules/__init__.py
--rw-r--r--   0        0        0    44399 2023-07-21 10:56:10.040318 cognite_neat-0.17.2/cognite/neat/core/rules/_exceptions.py
--rw-r--r--   0        0        0     3060 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/_loader.py
--rw-r--r--   0        0        0     7054 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/_parser.py
--rw-r--r--   0        0        0     3506 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/_validation.py
--rw-r--r--   0        0        0     4320 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/analysis.py
--rw-r--r--   0        0        0        0 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/exporter/__init__.py
--rw-r--r--   0        0        0       63 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/exporter/cdf/__init__.py
--rw-r--r--   0        0        0       48 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/exporter/cdf/rules2dms.py
--rw-r--r--   0        0        0      615 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/exporter/cdf/rules2labels.py
--rw-r--r--   0        0        0     5420 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/exporter/rules2graph_sheet.py
--rw-r--r--   0        0        0     4989 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/exporter/rules2graphql.py
--rw-r--r--   0        0        0    15289 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/exporter/rules2ontology.py
--rw-r--r--   0        0        0     4029 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/exporter/rules2rules.py
--rw-r--r--   0        0        0      636 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/exporter/rules2triples.py
--rw-r--r--   0        0        0       63 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/importer/__init__.py
--rw-r--r--   0        0        0    12985 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/importer/ontology2excel.py
--rw-r--r--   0        0        0    24271 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/models.py
--rw-r--r--   0        0        0     8231 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/rules/to_rdf_path.py
--rw-r--r--   0        0        0    11890 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0        0 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/utils/__init__.py
--rw-r--r--   0        0        0      314 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/utils/auxiliary.py
--rw-r--r--   0        0        0      741 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/utils/cdf.py
--rw-r--r--   0        0        0    10694 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/utils/utils.py
--rw-r--r--   0        0        0     2650 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      356 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    20733 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17845 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0    11664 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     4882 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      775 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     6977 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0      661 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/examples/__init__.py
--rw-r--r--   0        0        0      286 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
--rw-r--r--   0        0        0    68445 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/examples/graph-sheets/power-grid-example.xlsx
--rw-r--r--   0        0        0    94607 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
--rw-r--r--   0        0        0    14663 2023-07-21 10:57:11.629309 cognite_neat-0.17.2/cognite/neat/examples/ontologies/report.txt
--rw-r--r--   0        0        0    12815 2023-07-21 10:57:11.533301 cognite_neat-0.17.2/cognite/neat/examples/ontologies/transformation_rules.xlsx
--rw-r--r--   0        0        0    64516 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/examples/ontologies/wind-energy.owl
--rw-r--r--   0        0        0    80218 2023-07-21 10:56:10.044319 cognite_neat-0.17.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    77426 2023-07-21 10:56:10.048319 cognite_neat-0.17.2/cognite/neat/examples/rules/power-grid-example.xlsx
--rw-r--r--   0        0        0    75865 2023-07-21 10:56:10.048319 cognite_neat-0.17.2/cognite/neat/examples/rules/rules-template.xlsx
--rw-r--r--   0        0        0    52650 2023-07-21 10:56:10.048319 cognite_neat-0.17.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    79964 2023-07-21 10:56:10.048319 cognite_neat-0.17.2/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1461 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15698 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0     3549 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
--rw-r--r--   0        0        0     2573 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
--rw-r--r--   0        0        0    11456 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0      315 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
--rw-r--r--   0        0        0     8063 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
--rw-r--r--   0        0        0      270 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6668 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0      291 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
--rw-r--r--   0        0        0     6837 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
--rw-r--r--   0        0        0        0 2023-07-21 10:56:10.100323 cognite_neat-0.17.2/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 10:56:10.100323 cognite_neat-0.17.2/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1390 2023-07-21 10:56:10.100323 cognite_neat-0.17.2/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    24068 2023-07-21 10:56:10.100323 cognite_neat-0.17.2/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-07-21 10:56:10.100323 cognite_neat-0.17.2/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-07-21 10:56:10.100323 cognite_neat-0.17.2/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4622 2023-07-21 10:56:10.100323 cognite_neat-0.17.2/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-07-21 10:56:10.052319 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1370103 2023-07-21 10:56:10.060320 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js
--rw-r--r--   0        0        0     2667 2023-07-21 10:56:10.060320 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt
--rw-r--r--   0        0        0  5883237 2023-07-21 10:56:10.092323 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map
--rw-r--r--   0        0        0     2633 2023-07-21 10:56:10.092323 cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-07-21 10:56:10.100323 cognite_neat-0.17.2/cognite/neat/main.py
--rw-r--r--   0        0        0        0 2023-07-21 10:56:10.100323 cognite_neat-0.17.2/cognite/neat/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-07-21 10:56:10.100323 cognite_neat-0.17.2/cognite/neat/migration/wf_manifests.py
--rw-r--r--   0        0        0     2711 2023-07-21 10:56:10.560361 cognite_neat-0.17.2/pyproject.toml
--rw-r--r--   0        0        0    10637 1970-01-01 00:00:00.000000 cognite_neat-0.17.2/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/LICENSE
+-rw-r--r--   0        0        0     8765 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/README.md
+-rw-r--r--   0        0        0       61 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/_version.py
+-rw-r--r--   0        0        0     9986 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/base_workflows/graph2assets_relationships.py
+-rw-r--r--   0        0        0     7037 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/base_workflows/graphs_and_rules.py
+-rw-r--r--   0        0        0    14391 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/base_workflows/sheet2cdf.py
+-rw-r--r--   0        0        0    11824 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/base_workflows/sme_graph_capture.py
+-rw-r--r--   0        0        0      871 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2792 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     5616 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/core/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-07-24 10:01:56.437753 cognite_neat-0.17.3/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0     1276 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/exceptions.py
+-rw-r--r--   0        0        0      586 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     2837 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/extractors/_exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/extractors/cdfcore/__init__.py
+-rw-r--r--   0        0        0     2288 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/extractors/cdfcore/labels.py
+-rw-r--r--   0        0        0     5048 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/extractors/cdfcore/models.py
+-rw-r--r--   0        0        0    39905 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/extractors/cdfcore/rdf_to_assets.py
+-rw-r--r--   0        0        0    20940 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/extractors/cdfcore/rdf_to_relationships.py
+-rw-r--r--   0        0        0     5516 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/extractors/graph_sheet_to_graph.py
+-rw-r--r--   0        0        0       99 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0      938 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/loader/graph_capturing_sheet.py
+-rw-r--r--   0        0        0    11407 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    12903 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0       73 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9594 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0     2026 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/__init__.py
+-rw-r--r--   0        0        0    44399 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/_exceptions.py
+-rw-r--r--   0        0        0     3060 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/_loader.py
+-rw-r--r--   0        0        0     7054 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/_parser.py
+-rw-r--r--   0        0        0     3506 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/_validation.py
+-rw-r--r--   0        0        0     4320 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/analysis.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/exporter/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/exporter/cdf/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/exporter/cdf/rules2dms.py
+-rw-r--r--   0        0        0      615 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/exporter/cdf/rules2labels.py
+-rw-r--r--   0        0        0     5420 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/exporter/rules2graph_sheet.py
+-rw-r--r--   0        0        0     4989 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/exporter/rules2graphql.py
+-rw-r--r--   0        0        0    15289 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/exporter/rules2ontology.py
+-rw-r--r--   0        0        0     4029 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/exporter/rules2rules.py
+-rw-r--r--   0        0        0      636 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/exporter/rules2triples.py
+-rw-r--r--   0        0        0       63 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/importer/__init__.py
+-rw-r--r--   0        0        0    12985 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/importer/ontology2excel.py
+-rw-r--r--   0        0        0    24271 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/models.py
+-rw-r--r--   0        0        0     8231 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/rules/to_rdf_path.py
+-rw-r--r--   0        0        0    11890 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/utils/__init__.py
+-rw-r--r--   0        0        0      314 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/utils/auxiliary.py
+-rw-r--r--   0        0        0      741 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/utils/cdf.py
+-rw-r--r--   0        0        0    10694 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/utils/utils.py
+-rw-r--r--   0        0        0     2650 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      356 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    23380 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17845 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0    11664 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     4907 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0     1008 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/workflow/step_model.py
+-rw-r--r--   0        0        0      775 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     6977 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0      661 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/examples/__init__.py
+-rw-r--r--   0        0        0      286 2023-07-24 10:01:56.441754 cognite_neat-0.17.3/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
+-rw-r--r--   0        0        0    68445 2023-07-24 10:01:56.445754 cognite_neat-0.17.3/cognite/neat/examples/graph-sheets/power-grid-example.xlsx
+-rw-r--r--   0        0        0    94607 2023-07-24 10:01:56.445754 cognite_neat-0.17.3/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
+-rw-r--r--   0        0        0    14663 2023-07-24 10:03:01.617457 cognite_neat-0.17.3/cognite/neat/examples/ontologies/report.txt
+-rw-r--r--   0        0        0    12816 2023-07-24 10:03:01.521452 cognite_neat-0.17.3/cognite/neat/examples/ontologies/transformation_rules.xlsx
+-rw-r--r--   0        0        0    64516 2023-07-24 10:01:56.445754 cognite_neat-0.17.3/cognite/neat/examples/ontologies/wind-energy.owl
+-rw-r--r--   0        0        0    80218 2023-07-24 10:01:56.445754 cognite_neat-0.17.3/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    77426 2023-07-24 10:01:56.445754 cognite_neat-0.17.3/cognite/neat/examples/rules/power-grid-example.xlsx
+-rw-r--r--   0        0        0    75865 2023-07-24 10:01:56.445754 cognite_neat-0.17.3/cognite/neat/examples/rules/rules-template.xlsx
+-rw-r--r--   0        0        0    52650 2023-07-24 10:01:56.445754 cognite_neat-0.17.3/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    79964 2023-07-24 10:01:56.445754 cognite_neat-0.17.3/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1461 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15698 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0     3549 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
+-rw-r--r--   0        0        0     2573 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
+-rw-r--r--   0        0        0    11456 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0      315 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
+-rw-r--r--   0        0        0     8063 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
+-rw-r--r--   0        0        0      270 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6668 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0      291 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
+-rw-r--r--   0        0        0     6837 2023-07-24 10:01:56.449754 cognite_neat-0.17.3/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-07-24 10:01:56.497757 cognite_neat-0.17.3/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:01:56.497757 cognite_neat-0.17.3/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1390 2023-07-24 10:01:56.497757 cognite_neat-0.17.3/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    24068 2023-07-24 10:01:56.497757 cognite_neat-0.17.3/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:01:56.497757 cognite_neat-0.17.3/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-24 10:01:56.497757 cognite_neat-0.17.3/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4622 2023-07-24 10:01:56.497757 cognite_neat-0.17.3/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-07-24 10:01:56.453754 cognite_neat-0.17.3/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-07-24 10:01:56.453754 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-07-24 10:01:56.453754 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-07-24 10:01:56.453754 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-07-24 10:01:56.453754 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-07-24 10:01:56.453754 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-07-24 10:01:56.453754 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-07-24 10:01:56.453754 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-07-24 10:01:56.453754 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-07-24 10:01:56.453754 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-07-24 10:01:56.453754 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1370405 2023-07-24 10:01:56.461755 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.694f3f8e.js
+-rw-r--r--   0        0        0     2667 2023-07-24 10:01:56.461755 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt
+-rw-r--r--   0        0        0  5883860 2023-07-24 10:01:56.493757 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.694f3f8e.js.map
+-rw-r--r--   0        0        0     2633 2023-07-24 10:01:56.493757 cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-07-24 10:01:56.497757 cognite_neat-0.17.3/cognite/neat/main.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:01:56.497757 cognite_neat-0.17.3/cognite/neat/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-07-24 10:01:56.497757 cognite_neat-0.17.3/cognite/neat/migration/wf_manifests.py
+-rw-r--r--   0        0        0      655 2023-07-24 10:01:56.497757 cognite_neat-0.17.3/cognite/neat/steps/data_contracts.py
+-rw-r--r--   0        0        0     1992 2023-07-24 10:01:56.497757 cognite_neat-0.17.3/cognite/neat/steps/steps.py
+-rw-r--r--   0        0        0     2711 2023-07-24 10:01:56.977787 cognite_neat-0.17.3/pyproject.toml
+-rw-r--r--   0        0        0    10637 1970-01-01 00:00:00.000000 cognite_neat-0.17.3/PKG-INFO
```

### Comparing `cognite_neat-0.17.2/LICENSE` & `cognite_neat-0.17.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/README.md` & `cognite_neat-0.17.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/base_workflows/graph2assets_relationships.py` & `cognite_neat-0.17.3/cognite/neat/base_workflows/graph2assets_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/base_workflows/graphs_and_rules.py` & `cognite_neat-0.17.3/cognite/neat/base_workflows/graphs_and_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/base_workflows/sheet2cdf.py` & `cognite_neat-0.17.3/cognite/neat/base_workflows/sheet2cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/base_workflows/sme_graph_capture.py` & `cognite_neat-0.17.3/cognite/neat/base_workflows/sme_graph_capture.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/constants.py` & `cognite_neat-0.17.3/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/app.py` & `cognite_neat-0.17.3/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/configuration.py` & `cognite_neat-0.17.3/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/data_stores/metrics.py` & `cognite_neat-0.17.3/cognite/neat/core/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.17.3/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/extractors/__init__.py` & `cognite_neat-0.17.3/cognite/neat/core/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/extractors/_exceptions.py` & `cognite_neat-0.17.3/cognite/neat/core/extractors/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/extractors/cdfcore/labels.py` & `cognite_neat-0.17.3/cognite/neat/core/extractors/cdfcore/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/extractors/cdfcore/models.py` & `cognite_neat-0.17.3/cognite/neat/core/extractors/cdfcore/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/extractors/cdfcore/rdf_to_assets.py` & `cognite_neat-0.17.3/cognite/neat/core/extractors/cdfcore/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/extractors/cdfcore/rdf_to_relationships.py` & `cognite_neat-0.17.3/cognite/neat/core/extractors/cdfcore/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/extractors/graph_sheet_to_graph.py` & `cognite_neat-0.17.3/cognite/neat/core/extractors/graph_sheet_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/loader/config.py` & `cognite_neat-0.17.3/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/loader/graph.py` & `cognite_neat-0.17.3/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/loader/graph_capturing_sheet.py` & `cognite_neat-0.17.3/cognite/neat/core/loader/graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.17.3/cognite/neat/core/loader/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.17.3/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.17.3/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/__init__.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/_exceptions.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/_loader.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/_parser.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/_parser.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/_validation.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/analysis.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/exporter/cdf/rules2labels.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/exporter/cdf/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/exporter/rules2graph_sheet.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/exporter/rules2graph_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/exporter/rules2graphql.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/exporter/rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/exporter/rules2ontology.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/exporter/rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/exporter/rules2rules.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/exporter/rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/exporter/rules2triples.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/exporter/rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/importer/ontology2excel.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/importer/ontology2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/models.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/rules/to_rdf_path.py` & `cognite_neat-0.17.3/cognite/neat/core/rules/to_rdf_path.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/transformer.py` & `cognite_neat-0.17.3/cognite/neat/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/utils/cdf.py` & `cognite_neat-0.17.3/cognite/neat/core/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/utils/utils.py` & `cognite_neat-0.17.3/cognite/neat/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/validator.py` & `cognite_neat-0.17.3/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/workflow/base.py` & `cognite_neat-0.17.3/cognite/neat/core/workflow/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import inspect
 import json
 import logging
 import threading
 import time
 import traceback
 from threading import Event
+from typing import Type
 
 import yaml
 from cognite.client import CogniteClient
 from prometheus_client import Gauge
 
 from cognite.neat.core.data_stores.metrics import NeatMetricsCollector
+from cognite.neat.core.exceptions import InvalidWorkFlowError
 from cognite.neat.core.utils.utils import retry_decorator
 from cognite.neat.core.workflow import cdf_store
 from cognite.neat.core.workflow.model import (
     FlowMessage,
     StepExecutionStatus,
     StepType,
     WorkflowConfigItem,
@@ -26,14 +29,16 @@
     WorkflowSystemComponent,
 )
 from cognite.neat.core.workflow.tasks import WorkflowTaskBuilder
 
 from ..configuration import Config
 from ..utils.cdf import CogniteClientConfig
 from . import utils
+from .step_model import DataContract
+import cognite.neat.steps.steps
 
 summary_metrics = Gauge("neat_workflow_summary_metrics", "Workflow execution summary metrics", ["wf_name", "name"])
 steps_metrics = Gauge("neat_workflow_steps_metrics", "Workflow step level metrics", ["wf_name", "step_name", "name"])
 timing_metrics = Gauge("neat_workflow_timing_metrics", "Workflow timing metrics", ["wf_name", "component", "name"])
 
 
 class BaseWorkflow:
@@ -68,14 +73,15 @@
             cdf_store.CdfStore(self.cdf_client, data_set_id=self.default_dataset_id)
             if self.default_dataset_id
             else None
         )
         self.metrics = NeatMetricsCollector(self.name, self.cdf_client)
         self.resume_event = Event()
         self.is_ephemeral = False  # if True, workflow will be deleted after completion
+        self.data: dict[str, Type[DataContract]] = {}
 
     def start(self, sync=False, is_ephemeral=False, **kwargs) -> FlowMessage | None:
         """Starts workflow execution.sync=True will block until workflow is completed and
         return last workflow flow message, sync=False will start workflow in a separate thread and return None"""
         if self.state not in [WorkflowState.CREATED, WorkflowState.COMPLETED, WorkflowState.FAILED]:
             logging.error(f"Workflow {self.name} is already running")
             return None
@@ -248,14 +254,52 @@
                     retry_delay=step.retry_delay,
                     component_name=f"wf step runner , step.id = {step.id}",
                 )
                 def method_runner():
                     return method(flow_message)
 
                 new_flow_message = method_runner()
+            elif step.stype == StepType.STD_STEP:
+                for name, step_cls in inspect.getmembers(cognite.neat.steps.steps):
+                    if inspect.isclass(step_cls):
+                        if name == step.method:
+                            step_obj = step_cls(self.metrics)
+                            step_obj.set_global_configs(self.cdf_client, self.data_store_path, self.rules_storage_path)
+                            signature = inspect.signature(step_obj.run)
+                            parameters = signature.parameters
+                            is_valid = True
+                            input_data = []
+                            missing_data = []
+                            for parameter in parameters.values():
+                                try:
+                                    if parameter.annotation.__name__ == "FlowMessage":
+                                        input_data.append(self.flow_message)
+                                    else:
+                                        input_data.append(self.data[parameter.annotation.__name__])
+                                except KeyError:
+                                    is_valid = False
+                                    logging.error(f"Missing data for step {step.id} parameter {parameter.name}")
+                                    missing_data.append(parameter.annotation.__name__)
+                                    continue
+                            if not is_valid:
+                                raise InvalidWorkFlowError(step.id, missing_data)
+                            output = step_obj.run(*input_data)
+                            if output is not None:
+                                if isinstance(output, tuple):
+                                    for i, out_obj in enumerate(output):
+                                        if isinstance(out_obj, FlowMessage):
+                                            new_flow_message = out_obj
+                                        else:
+                                            self.data[type(out_obj).__name__] = out_obj
+                                else:
+                                    if isinstance(output, FlowMessage):
+                                        new_flow_message = output
+                                    else:
+                                        self.data[output.__name__] = output
+                            break
 
             elif step.stype == StepType.START_WORKFLOW_TASK_STEP:
                 if self.task_builder:
                     sync_str = step.params.get("sync", "false")
                     sync = sync_str.lower() == "true" or sync_str == "1"
                     start_status = self.task_builder.start_workflow_task(
                         workflow_name=step.params.get("workflow_name", ""), sync=sync, flow_message=self.flow_message
@@ -282,15 +326,14 @@
                 # reporting workflow execution before waiting for event
                 # self.report_workflow_execution()
                 logging.info(f"Workflow {self.name} is waiting for event")
                 self.resume_event.wait(timeout=timeout)
                 logging.info(f"Workflow {self.name} resumed after event")
                 self.state = WorkflowState.RUNNING
                 self.resume_event.clear()
-
             else:
                 logging.error(f"Workflow step {step.id} has unsupported step type {step.stype}")
 
             stop_time = time.perf_counter()
             elapsed_time = stop_time - start_time
             logging.info(f"Step {step_name} completed in {elapsed_time} seconds")
             step_execution_status = StepExecutionStatus.SUCCESS
```

### Comparing `cognite_neat-0.17.2/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.17.3/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.17.3/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/workflow/model.py` & `cognite_neat-0.17.3/cognite/neat/core/workflow/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         list[str]
     ] = None  # If set, the workflow will skip default route and go to the next step in the list
     step_execution_status: StepExecutionStatus = StepExecutionStatus.UNKNOWN  # The status of the step execution
 
 
 class StepType(StrEnum):
     PYSTEP = "pystep"
+    STD_STEP = "stdstep"
     START_WORKFLOW_TASK_STEP = "start_workflow_task_step"  # Call a workflow from another workflow
     CONTAINER_TASK_STEP = "container_step"  # TODO: implement
     CLI_TASK_STEP = "cli_step"  # TODO: implement
     HTTP_TRIGGER = "http_trigger"
     TIME_TRIGGER = "time_trigger"
     WAIT_FOR_EVENT = "wait_for_event"  # TODO: implement
     EVENT_TRIGGER = "event_trigger"  # TODO: implement
```

### Comparing `cognite_neat-0.17.2/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.17.3/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.17.3/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/__init__.py` & `cognite_neat-0.17.3/cognite/neat/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/graph-sheets/power-grid-example.xlsx` & `cognite_neat-0.17.3/cognite/neat/examples/graph-sheets/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx` & `cognite_neat-0.17.3/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/ontologies/report.txt` & `cognite_neat-0.17.3/cognite/neat/examples/ontologies/report.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/ontologies/transformation_rules.xlsx` & `cognite_neat-0.17.3/cognite/neat/examples/ontologies/transformation_rules.xlsx`

 * *Files 15% similar despite different names*

```diff
@@ -1,801 +1,801 @@
-00000000: 504b 0304 1400 0000 0800 2557 f556 465a  PK........%W.VFZ
+00000000: 504b 0304 1400 0000 0800 6050 f856 465a  PK........`P.VFZ
 00000010: c10c 8200 0000 b100 0000 1000 0000 646f  ..............do
 00000020: 6350 726f 7073 2f61 7070 2e78 6d6c 4d8e  cProps/app.xmlM.
 00000030: 4d0b c230 1044 ff4a e9dd 6e55 f020 3120  M..0.D.J..nU. 1 
 00000040: d4a3 e0c9 7b48 3736 9064 4376 85fc 7c53  ....{H76.dCv..|S
 00000050: c18f db3c de30 8cba 15ca 58c4 2377 3586  ...<.0....X.#w5.
 00000060: c4a7 7e11 c947 00b6 0b46 c343 d3a9 1947  ..~..G...F.C...G
 00000070: 251a 6958 1e40 ce79 8b13 d967 c424 b01b  %.iX.@.y...g.$..
 00000080: c703 6015 4c33 ce9b fc1d ecb5 3ae7 1cbc  ..`.L3......:...
 00000090: 35e2 29e9 abb7 8598 9c74 976a 3128 f897  5.)......t.j1(..
 000000a0: 6bf3 8e85 d7bc 1fb6 6ff9 6105 bf93 fa05  k.......o.a.....
-000000b0: 504b 0304 1400 0000 0800 2557 f556 8547  PK........%W.V.G
-000000c0: 24e6 ea00 0000 cb01 0000 1100 0000 646f  $.............do
-000000d0: 6350 726f 7073 2f63 6f72 652e 786d 6ca5  cProps/core.xml.
-000000e0: 91c1 4ec3 300c 865f 65ea bd75 d30a 2645  ..N.0.._e..u..&E
-000000f0: 5d2e 439c 4042 6212 885b e478 5b44 9346  ].C.@Bb..[.x[D.F
-00000100: 8951 bbb7 a72d 5b07 821b c7f8 fffc d956  .Q...-[........V
-00000110: 1a0c 12bb 484f b10b 14d9 525a 0dae f549  ....HO....RZ...I
-00000120: 62d8 6447 e620 0112 1ec9 e954 8c84 1fc3  b.dG. .....T....
-00000130: 7d17 9de6 f119 0f10 34be eb03 4155 96b7  }.......4...AU..
-00000140: e088 b5d1 ac61 12e6 6131 6667 a5c1 4519  .....a..a1fg..E.
-00000150: 3e62 3b0b 0c02 b5e4 c873 0251 08b8 b24c  >b;......s.Q...L
-00000160: d1a5 3f1b e664 2187 6417 aaef fba2 af67  ..?..d!.d......g
-00000170: 6edc 48c0 ebe3 c3f3 bc7c 6e7d 62ed 9132  n.H......|n}b..2
-00000180: d518 9418 4973 17d5 7451 380d 6d03 df8a  ....Is..tQ8.m...
-00000190: cd79 f657 81cc 6a9c 20f9 1468 935d 9297  .y.W..j. ..h.]..
-000001a0: 7a7b b7bb cf54 5556 755e aef3 4aec 4429  z{...TUVu^..J.D)
-000001b0: 6fd6 5288 b7c9 f5a3 ff2a 749d b17b fb0f  o.R......*t..{..
-000001c0: e345 a01a f8f5 6fea 1350 4b03 0414 0000  .E....o..PK.....
-000001d0: 0008 0025 57f5 5699 5c9c 2310 0600 009c  ...%W.V.\.#.....
-000001e0: 2700 0013 0000 0078 6c2f 7468 656d 652f  '......xl/theme/
-000001f0: 7468 656d 6531 2e78 6d6c ed5a 5b73 da38  theme1.xml.Z[s.8
-00000200: 147e efaf d078 67f6 6d0b c636 81b6 b413  .~...xg.m..6....
-00000210: 7369 76db b499 84ed 4e1f 8511 588d 6c79  siv.....N...X.ly
-00000220: 6491 847f bf47 3610 cb96 0ded 924d ba9b  d....G6......M..
-00000230: 3c04 2ce9 fbce 4547 e7e8 3879 f3ee 2e62  <.,...EG..8y...b
-00000240: e886 8894 f278 60d9 2fdb d6bb b72f dee0  .....x`./..../..
-00000250: 5732 2411 4130 19a7 aff0 c00a a54c 5eb5  W2$.A0.......L^.
-00000260: 5a69 00c3 387d c913 12c3 dc82 8b08 4b78  Zi..8}........Kx
-00000270: 14cb d65c e05b 1a2f 23d6 eab4 dbdd 5684  ...\.[./#.....V.
-00000280: 696c a118 4764 607d 5e2c 6840 d054 515a  il..Gd`}^,h@.TQZ
-00000290: 6f5f 20b4 e51f 33f8 15cb 548d 65a3 0113  o_ ...3...T.e...
-000002a0: 5741 26b9 88b4 f2f9 6cc5 fcda de3e 65cf  WA&.....l....>e.
-000002b0: e93a 1d32 816e 301b 5820 7fce 6fa7 e44e  .:.2.n0.X ..o..N
-000002c0: 5a88 e154 c2c4 c06a 673f 566b c7d1 d248  Z..T...jg?Vk...H
-000002d0: 8082 c97d 9405 ba49 f6a3 d315 0832 0d3b  ...}...I.....2.;
-000002e0: 3a9d 58ce 767c f6c4 ed9f 8cca da74 346d  :.X.v|.......t4m
-000002f0: 1ae0 e3f1 7838 b6cb d28b 701c 04e0 51bb  ....x8....p...Q.
-00000300: 9ec2 9df4 6cbf a441 09b4 a369 d064 d8f6  ....l..A...i.d..
-00000310: daae 91a6 aa8d 534f d3f7 7ddf eb9b 689c  ......SO..}...h.
-00000320: 0a8d 5b4f d36b 77dd d38e 89c6 add0 780d  ..[O.kw.......x.
-00000330: bef1 4f87 c3ae 89c6 abd0 74eb 6926 27fd  ..O.......t.i&'.
-00000340: ae6b a4e9 1668 4246 e3eb 7a12 15b5 e540  .k...hBF..z....@
-00000350: d320 0058 7076 d6cc d203 965e 29fa 7594  . .Xpv.....^).u.
-00000360: 1ad9 1dbb dd41 5cf0 58ee 3989 11fe c6c5  .....A\.X.9.....
-00000370: 04d6 69d2 1996 3446 729d 9005 0e00 37c4  ..i...4Fr.....7.
-00000380: d14c 507c af41 b68a e0c2 92d2 5c90 d6cf  .LP|.A......\...
-00000390: 29b5 501a 089a c881 f547 8221 c5dc affd  ).P......G.!....
-000003a0: f597 bbc9 a433 7a9d 7d3a ce6b 947f 69ab  .....3z.}:.k..i.
-000003b0: 01a7 edbb 9bcf 93fc 73e8 e49f a793 d74d  ........s......M
-000003c0: 42ce 70bc 2c09 f1fb 235b 6187 276e 3b13  B.p.,...#[a.'n;.
-000003d0: 723a 1c67 427c cff6 f691 a525 32cf eff9  r:.gB|.....%2...
-000003e0: 0aeb 4e3c 671f 5696 b05d cfcf e49e 8c72  ..N<g.V..].....r
-000003f0: 23bb ddf6 587d f64f 476e 23d7 a9c0 b322  #...X}.OGn#...."
-00000400: d794 4624 459f c82d bae4 1138 b549 0d32  ..F$E..-...8.I.2
-00000410: 133f 089d 8698 6a50 1c02 a409 3196 a186  .?....jP....1...
-00000420: f8b4 c6ac 11e0 137d b7be 08c8 df8d 88f7  .......}........
-00000430: ab6f 9a3d 57a1 5849 da84 f810 461a e29c  .o.=W.XI....F...
-00000440: 73e6 73d1 6cfb 07a5 46d1 f655 bcdc a397  s.s.l...F..U....
-00000450: 5815 0197 18df 34aa 352c c5d6 7895 c0f1  X.....4.5,..x...
-00000460: ad9c 3c1d 1312 cd94 0b06 4186 9724 2612  ..<.......A..$&.
-00000470: a939 7e4d 4813 fe2b a5da fe9c d340 f094  .9~MH..+.....@..
-00000480: 2f24 fa4a 918f 69b3 23a7 7426 cde8 331a  /$.J..i.#.t&..3.
-00000490: c146 af1b 7587 68d2 3c7a fe05 f99c 350a  .F..u.h.<z....5.
-000004a0: 1c91 1b1d 0267 1bb3 4621 8469 bbf0 1eaf  .....g..F!.i....
-000004b0: 248e 9aad c211 2b42 3e62 1936 1a72 b516  $.....+B>b.6.r..
-000004c0: 81b6 71a9 8460 5a12 c6d1 784e d2b4 11fc  ..q..`Z...xN....
-000004d0: 59ac 3593 3e60 c8ec cd91 75ce d691 0e11  Y.5.>`....u.....
-000004e0: 925e 3742 3e62 ce8b 9011 bf1e 8638 4a9a  .^7B>b.......8J.
-000004f0: eda2 7158 04fd 9e5e c349 c1e8 82cb 66fd  ..qX...^.I....f.
-00000500: b87e 86d5 336c 2c8e f747 d417 4ae4 0f26  .~..3l,..G..J..&
-00000510: a73f e932 3407 a39a 5909 bd84 566a 9faa  .?.24...Y...Vj..
-00000520: 8734 3ea8 1e32 0a05 f1b9 1e3e e57a 780a  .4>..2.....>.zx.
-00000530: 3796 c6bc 50ae 827b 01ff d1da 37c2 abf8  7...P..{....7...
-00000540: 82c0 397f 2e7d cfa5 efb9 f43d a1d2 b737  ..9..}.....=...7
-00000550: 237d 67c1 d38b 5bde 466e 5bc4 fbae 31da  #}g...[.Fn[...1.
-00000560: d734 2e28 6357 72cd c8c7 54af 9329 d839  .4.(cWr...T..).9
-00000570: 9fc0 ecfd 683e 9ef1 edfa d924 84af 9a59  ....h>.....$...Y
-00000580: 2d23 1690 4b81 b341 24b8 fc8b caf0 2ac4  -#..K..A$.....*.
-00000590: 09e8 645b 2509 cb54 d365 378a 129e 421b  ..d[%..T.e7...B.
-000005a0: 6ee9 53f5 4a95 d7e5 afb9 28b8 3c5b e4e9  n.S.J.....(.<[..
-000005b0: afa1 743e 2ccf f93c 5fe7 b4cd 0b33 43b7  ..t>,..<_....3C.
-000005c0: 724b eab6 94be b526 384a f4b1 cc70 4e1e  rK.....&8J...pN.
-000005d0: cb0c 3b67 3c92 1db6 77a0 1d35 fbf6 5d76  ..;g<...w..5..]v
-000005e0: e423 a530 5397 43b8 1a42 be03 6dba 9ddc  .#.0S.C..B..m...
-000005f0: 3a38 9e98 91b9 0ad3 5290 6fc3 f9e9 c578  :8......R.o....x
-00000600: 1ae2 39d9 04b9 7d98 576d e7d8 d1d1 fbe7  ..9...}.Wm......
-00000610: c151 b0a3 ef3c 961d c788 f2a2 21ee a186  .Q...<......!...
-00000620: 98cf c343 8779 7b5f 9867 95c6 5034 146d  ...C.y{_.g..P4.m
-00000630: 6cac 242c 46b7 60b8 d7f1 2c14 e064 602d  l.$,F.`...,..d`-
-00000640: a007 83af 5102 f252 5560 315b c603 2b90  ....Q..RU`1[..+.
-00000650: a27c 4c8c 45e8 70e7 975c 5fe3 d192 e3db  .|L.E.p..\_.....
-00000660: a665 b56e af29 7719 6d22 5239 c269 9813  .e.n.)w.m"R9.i..
-00000670: 67ab cade 65b1 c155 1dcf 555b f2b0 be6a  g...e..U..U[...j
-00000680: 3db4 154e cffe 59ad c89f 0c11 4e16 0b12  =..N..Y.....N...
-00000690: 4863 9417 a64a a2f3 1953 bee7 2b49 c455  Hc...J...S..+I.U
-000006a0: 38bf 4533 b612 9718 bce3 e6c7 714e 53b8  8.E3........qNS.
-000006b0: 1276 b60f 0232 b9bb 39a9 7a65 3167 a6f2  .v...2..9.ze1g..
-000006c0: df2d 0c09 2c5b 8859 12e2 4d5d edd5 e79b  .-..,[.Y..M]....
-000006d0: 9cae 7a22 76fa 9777 c160 f2fd 70c9 470f  ..z"v..w.`..p.G.
-000006e0: e53b e75f f45d 43ae 7ef6 dde3 fa6e 933b  .;._.]C.~....n.;
-000006f0: 484c 9c79 c511 0174 4502 2395 1c06 1617  HL.y...tE.#.....
-00000700: 32e4 50ee 9290 0613 01cd 94c9 44f0 0282  2.P.........D...
-00000710: 64a6 1c80 98fa 0bbd f20c b929 15ce ad3e  d..........)...>
-00000720: 397f 452c 8386 4e5e d225 1214 8ab0 0c05  9.E,..N^.%......
-00000730: 2117 72e3 efef 936a 778c d7fa 2c81 6d84  !.r....jw...,.m.
-00000740: 5432 64d5 17ca 4389 c13d 3372 43d8 5425  T2d...C..=3rC.T%
-00000750: f3ae da26 0b85 dbe2 54cd bb1a be26 604b  ...&....T....&`K
-00000760: c37a 6e9d 2d27 ffdb 5ed4 3db4 173d 46f3  .zn.-'..^.=..=F.
-00000770: a399 e01e b387 739b 7ab8 c245 acff 58d6  ......s.z..E..X.
-00000780: 1ef9 32df 3970 db3a de03 5ee6 132c 43a4  ..2.9p.:..^..,C.
-00000790: 7ec1 7d8a 8a80 11ab 62be baaf 4ff9 259c  ~.}.....b...O.%.
-000007a0: 3bb4 7bf1 8120 9bfc d6db a4f6 dde0 0c7c  ;.{.. .........|
-000007b0: d4ab 5aa5 642b 113f 4b07 7c1f 9206 638c  ..Z.d+.?K.|...c.
-000007c0: 5bf4 345f 8f14 62ad a6b1 adc6 da31 0c79  [.4_..b......1.y
-000007d0: 8058 f30c a166 38df 8745 9a1a 33d5 8bac  .X...f8..E..3...
-000007e0: 398d 0a6f 41d5 40e5 3fdb d40d 68f6 0d34  9..oA.@.?...h..4
-000007f0: 1c91 055e 3199 b636 a3e4 4e0a 3cdc feef  ...^1..6..N.<...
-00000800: 0db0 c2c4 8ee1 ed8b bf01 504b 0304 1400  ..........PK....
-00000810: 0000 0800 2557 f556 e0d9 6c24 3d02 0000  ....%W.V..l$=...
-00000820: a307 0000 1800 0000 786c 2f77 6f72 6b73  ........xl/works
-00000830: 6865 6574 732f 7368 6565 7431 2e78 6d6c  heets/sheet1.xml
-00000840: 8595 db72 9b30 1086 5f85 e101 2ce3 b333  ...r.0.._...,..3
-00000850: 9899 da9d 4e7b 914e 269e 26d7 322c b6c6  ....N{.N&.&.2,..
-00000860: 42a2 d262 d2b7 afa4 38b2 9b82 b842 a7dd  B..b....8....B..
-00000870: 6f0f e257 da4a 75d6 2700 8cde 2a2e f426  o..W.Ju.'...*..&
-00000880: 3e21 d60f 84e8 fc04 15d5 2359 8330 3ba5  >!........#Y.0;.
-00000890: 5415 4533 5547 a26b 05b4 7046 1527 93f1  T.E3UG.k..pF.'..
-000008a0: 7841 2aca 449c a56e ed49 65a9 6c90 3301  xA*.D..n.Ie.l.3.
-000008b0: 4f2a d24d 5551 f567 0b5c b69b 3889 3f16  O*.MUQ.g.\..8.?.
-000008c0: 9ed9 f184 6e81 6469 4d8f b007 fc55 1b03  ....n.diM....U..
-000008d0: 3325 de4f c12a 109a 4911 2928 37f1 97e4  3%.O.*..I.)(7...
-000008e0: 619b cc9c 893b f2c2 a0d5 77e3 c866 7390  a....;....w..fs.
-000008f0: f26c 273f 8a4d 3cb6 4101 871c ad0f 6a3e  .l'?.M<.A.....j>
-00000900: 17d8 01e7 d695 09e5 f7d5 6b7c a35a cbfb  ..........k|.Z..
-00000910: f187 fb6f ae00 26be 03d5 b093 fc95 1578  ...o..&........x
-00000920: dac4 ab38 2aa0 a40d c767 d97e 876b 52f3  ...8*....g.~.kR.
-00000930: 5b88 5f29 d22c 55b2 8d94 cd36 4b73 3b70  [._).,U....6Ks;p
-00000940: 7497 bd39 ce84 add5 1e95 d965 8687 99a0  t..9.......e....
-00000950: 15e8 9ae6 9012 34c1 d845 925f 4db7 7d46  ......4..E._M.}F
-00000960: b671 da74 ee7c 1ce5 f228 18c2 8832 d232  .q.t.|...(...2.2
-00000970: 5190 7fdd 1013 8d0f 69e2 439a 0443 323d  Q.......i.C..C2=
-00000980: 2fd9 5b57 3c93 4f16 ae96 f788 a947 4c83  /.[W<.O......GL.
-00000990: 88c2 94ea 5116 c07f 9af4 bb48 d321 d2cc  ....Q......H.!..
-000009a0: 9366 4152 5e94 7b5b de3e d06c 0834 f7a0  .fAR^.{[.>.l.4..
-000009b0: 7910 7401 656f 6f17 633e c458 78c6 22c8  y.t.eoo.c>.Xx.".
-000009c0: 607a d728 0502 5ffa 610b 677b 3036 972c  `z.(.._.a.g{06.,
-000009d0: 49c9 a5e3 222c 3d6e 19ae 9df9 f911 8a2e  I...",=n........
-000009e0: ca72 28a5 9567 ac82 8ca6 2efa 18ab 21c6  .r(..g........!.
-000009f0: da33 d641 0632 e49d cd5f 0f11 92f1 ed37  .3.A.2..._.....7
-00000a00: 1e87 6f34 e85c b11a 7bba 62ad 0750 778a  ..o4.\..{.b..Pw.
-00000a10: 1196 0cd7 16a9 3a31 9f6d fec7 dc54 2009  ......:1.m...T .
-00000a20: cb40 2e05 2a76 68fa 5083 6290 dcd4 2009  .@..*vh.P.b... .
-00000a30: cb81 b262 aa3b 2983 4290 dc94 2009 4b01  ...b.;).B... .K.
-00000a40: 67b9 7961 ba85 b65f 06c8 9db6 dbc7 eb91  g.ya..._........
-00000a50: aa23 133a e250 1a8b f168 69fe 6ef5 fe18  .#.:.P...hi.n...
-00000a60: bc4f 50d6 2e86 8344 9495 1b9e cc23 0aca  .OP....D.....#..
-00000a70: 1e30 fba5 94e8 2716 e3df e5ec 2f50 4b03  .0....'...../PK.
-00000a80: 0414 0000 0008 0025 57f5 5619 c663 fc00  .......%W.V..c..
-00000a90: 0e00 00bb 8300 0018 0000 0078 6c2f 776f  ...........xl/wo
-00000aa0: 726b 7368 6565 7473 2f73 6865 6574 322e  rksheets/sheet2.
-00000ab0: 786d 6cad 9ddb 72da 4817 855f 85f2 0304  xml...r.H.._....
-00000ac0: 734c 66ca 71d5 60a1 ee74 2687 8a33 99aa  sLf.q.`..t&..3..
-00000ad0: ff4e 8636 a822 2422 449c ccd3 ff12 8969  .N.6."$"D......i
-00000ae0: d9ea 4f4d cbbe 4acc 621f b417 12e2 43b4  ..OM..J.b.....C.
-00000af0: 2eee b2fc eb6e ad75 d1fb b149 d2dd ebb3  .....n.u...I....
-00000b00: 7551 6cff ecf7 778b b5de 44bb 17d9 56a7  uQl...w...D...V.
-00000b10: a572 9be5 9ba8 28ff cc57 fddd 36d7 d1f2  .r....(..W..6...
-00000b20: 10b4 49fa c3f3 f369 7f13 c5e9 d9e5 c5e1  ..I....i........
-00000b30: b18f f9e5 45b6 2f92 38d5 1ff3 de6e bfd9  ....E./.8....n..
-00000b40: 44f9 cf99 4eb2 bbd7 6783 b3fb 073e c5ab  D...N...g....>..
-00000b50: 7571 78a0 7f79 b18d 56fa 5a17 ff6c cb80  uqx..y..V.Z..l..
-00000b60: f2cf fe31 cf32 dee8 7417 6769 2fd7 b7af  ...1.2..t.gi/...
-00000b70: cffe 1afc f9f6 e5f9 21e4 f094 2fb1 bedb  ........!.../...
-00000b80: d5fe dfab b6e6 26cb be56 7fbc 59be 3e3b  ......&..V..Y.>;
-00000b90: af9a d289 5e14 558e a8fc e7bb bed2 4952  ....^.U.......IR
-00000ba0: a52a 5bf9 f63b eb99 a95a 45d6 ff7f 9f3e  .*[..;...ZE....>
-00000bb0: 3c0c a0ec ef26 dae9 ab2c f937 5e16 ebd7  <....&...,.7^...
-00000bc0: 67af ce7a 4b7d 1bed 93e2 5376 27f5 ef8d  g..zK}....Sv'...
-00000bd0: 9a98 1683 a888 2e2f f2ec ae97 575b 7b79  ......./....W[{y
-00000be0: b1a8 fe53 952c 9f18 a7d5 94ae 8bbc 7c3c  ...S.,........|<
-00000bf0: 2e2b 1597 d5d3 7bef b2a5 4e7a 81be 8dd3  .+....{...Nz....
-00000c00: b86a fca2 5f94 2d55 4fe8 2f7e 2798 3d4e  .j.._.-UO./~'.=N
-00000c10: 5015 3c28 57a8 04a8 cca9 9deb 222a b4a5  P.<(W......."*..
-00000c20: 7c88 a904 2a92 8abc 4db3 bb44 2f57 ba34  |...*...M..D/W.4
-00000c30: e8db 3ede 1db6 b997 642b 4be1 3798 5ea1  ..>.....d+K.7.^.
-00000c40: f2d6 a6f4 4b4b 8ebe 0c8f be0c a1c7 ab24  ....KK.........$
-00000c50: daed 6c3e 50c0 fb68 631b dc15 3d3f d0bb  ..l>P..hc...=?..
-00000c60: 451e 6fc1 ee80 c23e 46b9 4e8b 1eb5 37e7  E.o....>F.N...7.
-00000c70: 72e5 4ebc 28cd 5dda dc75 4555 fe04 f657  r.N.(.]..uEU...W
-00000c80: 86a0 d84f 7a9b 440b bdec cd7e 5ac2 2485  ...Oz.D....~Z.$.
-00000c90: 5d67 fb7c 612b f4a6 3da2 374f 8bb8 f8d9  ]g.|a+..=.7O....
-00000ca0: 031f 1445 bf8b 8ac5 da12 f016 5f19 d9a6  ...E........_...
-00000cb0: 3c46 150f 431e bcba 46c7 57d7 0872 8c82  <F..C...F.W..r..
-00000cc0: c32e 6f7b 7d3d 0e31 fb39 2a01 95a9 0e2e  ..o{}=.1.9*.....
-00000cd0: d745 9697 47db 4f7a 7718 d3e7 9f5b db78  .E..G.Ozw....[.x
-00000ce0: e698 3c44 45a0 22a9 a1ea bd66 57be d97c  ..<DE."....fW..|
-00000cf0: 5dbd 5864 abf2 60a7 5f44 71ff 2e4e 977d  ].Xd..`._Dq..N.}
-00000d00: 9be3 fee3 5314 a27f 946f 0636 9b6d 1bf1  ....S....o.6.m..
-00000d10: c0cd f1d1 cd31 e4fe 4be7 7164 35f3 7184  .....1..K.qd5.q.
-00000d20: 3113 9580 aabc 4977 4594 2487 9d91 5cc4  1.....IwE.$...\.
-00000d30: ac21 2a02 1549 9d78 bae8 3d36 4511 68a2  .!*..I.x..=6E.h.
-00000d40: 6d1b 1e98 3839 9a38 a16e 763b 6dcb 3d7b  m...89.8.nv;m.={
-00000d50: 1c60 3c44 25a0 221e 3b24 260f 5111 a848  .`<D%.".;$&.Q..H
-00000d60: 6ac8 d34a dfe1 290a 4027 6d9b f0c0 c9e9  j..J..).@'m.....
-00000d70: d1c9 2935 f323 dec1 5467 8f63 8c99 a804  ..)5.#..Tg.c....
-00000d80: 54e7 df72 4a9f f7f9 4df9 f0d5 3aca cb0d  T..rJ...M...:...
-00000d90: 2a5f d0bb 225e d8ec c4f4 212a 0215 492d  *_.."^....!*..I-
-00000da0: 79da d961 828a 62d0 51db 563c 70f4 e5d1  y..a..b.Q.V<p...
-00000db0: d197 f496 1b84 d59e 83ef 992d 713d 7382  ...........-q=s.
-00000dc0: 6d3b 3b7b 1c69 5c47 658e 4a88 8a40 4552  m;;{.i\Ge.J..@ER
-00000dd0: ef9e 5676 1c9d a238 b4d3 b625 0fec 7c75  ..Vv...8...%..|u
-00000de0: b4f3 159e 4155 6f65 8f4f a17e 59f9 38c6  ....AUoe.O.~Y.8.
-00000df0: eca0 a804 54e7 4b54 bec1 dc24 fabe de3f  ....T.KT...$...?
-00000e00: e514 6dfb 2666 0e51 11a8 48ea c6d3 d00e  ..m.&f.Q..H.....
-00000e10: c353 1483 66da b6e2 8199 7f1c cdfc 83fa  .S..f...........
-00000e20: 29ae f6f9 77eb c1f6 7188 f112 9580 ca54  )...w...q......T
-00000e30: 2fe2 8f79 b6dc 2f0a ebe7 1ecc 18a2 2250  /..y../......."P
-00000e40: 91d4 85a7 87fe 3353 1482 16da 36e2 8185  ......3S....6...
-00000e50: 8373 0321 ce5b a6fb 215f 4569 fcdf e1fc  .s.!.[..!_Ei....
-00000e60: d271 7232 6b24 aad1 0894 022c ef3a 17e2  .qr2k$.....,.:..
-00000e70: 9c21 4b82 2589 9d78 1afc 5c03 5598 087d  .!K.%..x..\.U..}
-00000e80: b76e dd43 e36b f4a9 0d3f b5ec 56b3 4660  .n.C.k...?..V.F`
-00000e90: cde8 16ee 44e5 aa53 a679 aaf3 d5cf 2303  ....D..S.y....#.
-00000ea0: 1279 b4b5 7dfe 9e73 fe90 25c1 92c4 ae7c  .y..}..s..%....|
-00000eb0: 4def 384c 8581 6cb2 9364 0d0c ca1a 20c5  M.8L..l..d.... .
-00000ec0: a93e 75d8 3fdc 3462 6afe a214 b456 f278  .>u.?.4bj....V.x
-00000ed0: d9cf b946 c892 6049 6267 be1e fbcf 5261  ...F..`Ibg....Ra
-00000ee0: 0cdb 6bdb 9087 f61a 9634 783a e599 3572  ..k......4x:..5r
-00000ef0: d4ec 66bc 8495 9df6 3255 6249 b024 b113  ..f.....2UbI.$..
-00000f00: 5f7b 9f3e 4b85 39d8 6e27 6b1a 18d8 3420  _{.>K.9.n'k...4 
-00000f10: 0812 6477 6975 1cb5 facb c089 a500 4b7d  ..dwiu........K}
-00000f20: caca 517c c863 9d16 1180 ea39 e70d 5912  ..Q|.c.....9..Y.
-00000f30: 2c49 ecc6 d7e3 0e03 5418 c4a6 3ad9 d3c0  ,I......T...:...
-00000f40: c0a7 01f1 90f9 f706 52fe ed28 e327 9602  ........R..(.'..
-00000f50: ace3 01a0 387d c892 6049 6253 bec6 fa0e  ....8}..`IbS....
-00000f60: 5161 04bb eae4 5003 03a2 06c4 44e6 3f16  Qa....P.....D.?.
-00000f70: c9be fa36 f37f 596a 3f1e 338f 6229 c07a  ...6..Yj?.3.b).z
-00000f80: 5066 ceb9 4296 044b 123b f0b5 b2eb e414  Pf..B..K.;......
-00000f90: 46b2 a54e 1035 3024 6a40 5c24 8c13 bb93  F..N.50$j@\$....
-00000fa0: 4878 ae58 0ab0 8ccf 7eca 3c8a 25c1 92c4  Hx.X....~.<.%...
-00000fb0: a67c cdf5 9ca1 c200 f6d4 49a3 0606 470d  .|........I...G.
-00000fc0: 088f 84f1 0feb d7a2 b346 44cd 54c6 5158  .........FD.T.QX
-00000fd0: e77a bfdd 6679 513e 547e 42d8 e7ec 2803  .z..fyQ>T~B...(.
-00000fe0: 2996 044b 123b f275 d477 820a 23d8 5227  )..K.;.u.w..#.R'
-00000ff0: 931a 1828 3520 5c12 2659 79c6 92da ae28  ...(5 \.&Yy....(
-00001000: 9835 826a ae32 98c2 5227 bbca 888a 25c1  .5.j.2..R'....%.
-00001010: 92c4 8e7c 5ded 3044 8541 6cac 9354 0d0d  ...|].0D.Al..T..
-00001020: a91a 120f 9159 1eff 9795 e7a3 49f5 2585  .....Y......I.%.
-00001030: f502 0d66 532c 0558 b0e5 bb90 39e7 0b59  ...fS,.X....9..Y
-00001040: 122c 49ec c2d3 d2ee e353 188a c65a b7e7  .,I......S...Z..
-00001050: a1b1 8644 0d89 81bc 995f f135 374c a158  ...D....._.57L.X
-00001060: 0ab0 94d7 1777 5c20 6449 b024 b12d 5f8f  .....w\ dI.$.-_.
-00001070: 3b4c 5261 10bb ebbe 98aa 7635 1521 90fb  ;LRa......v5.!..
-00001080: 9e5e bcb1 facb 148a a5c0 59cc 6a27 1327  .^........Y.j'.'
-00001090: 9604 4b12 bbf0 b5b3 d3e8 1486 b1a1 4ee8  ..K...........N.
-000010a0: 3434 d069 4890 c374 6577 9441 134b 81b3  44.iH..tew.A.K..
-000010b0: 9ad5 5186 4c2c 0996 2476 e1eb 68b7 d929  ..Q.L,..$v..h..)
-000010c0: 8c63 4b9d 6069 68c0 d210 2f30 326d d93d  .cK.`ih.../02m.=
-000010d0: 65b8 c452 e02c 67f5 94a1 124b 8225 895d  e..R.,g....K.%.]
-000010e0: f87a da71 780a 03d9 5427 581a 1ab0 3424  .z.qx...T'X...4$
-000010f0: c251 ef2b b2ba ca80 89a5 e0a4 7a56 6799  .Q.+........zVg.
-00001100: 2ab1 2458 92d8 89af b35d 27a8 3092 ad75  *.$X.....]'.0..u
-00001110: d2a5 a1a1 4b43 221d f5c6 6eac d632 5d62  ....KC"...n..2]b
-00001120: 2938 a99e d55a a64c 2c09 9624 76e2 6b6d  )8...Z.L,..$v.km
-00001130: d709 2a8c 646b 9d94 6968 28d3 9080 47ad  ..*.dk..ih(...G.
-00001140: 31fb 4ecb b489 a5e0 9472 5663 9930 b124  1.N......rVc.0.$
-00001150: 5892 d888 afb1 1de7 a730 907d 7592 a6a1  X........0.}u...
-00001160: 214d 43a2 1eb5 beec 7b2c 0327 9682 53ca  !MC.....{,.'..S.
-00001170: 597d 65ce c492 6049 6223 bebe 769c 9fc2  Y}e...`Ib#..v...
-00001180: 40f6 d589 9b86 0637 0d09 7a98 bebe 586d  @......7..z...Xm
-00001190: 65e2 c452 e0ac 66f5 9429 134b 8225 895d  e..R..f..).K.%.]
-000011a0: f87a da6d 760a e3d8 5227 681a 19d0 3422  .z.mv...R'h...4"
-000011b0: dc61 dab2 1e81 1b71 c652 9682 13aa d94c  .a.....q.R.....L
-000011c0: e58c 214b 8225 897d f8fe 40a3 dbf4 14c6  ..!K.%.}..@.....
-000011d0: f1cf 349c 9069 6420 d3c8 8546 5ed8 0fbf  ..4..id ...F^...
-000011e0: 8db8 9aa9 cc99 4ea8 6635 95c1 124b 8225  ......N.f5...K.%
-000011f0: 897d f89a da6d 7a0a e3d8 5427 5b1a 19b6  .}...mz...T'[...
-00001200: 3442 4092 3abe 656d 44d6 6c65 bc84 f5e8  4B@.:.emD.le....
-00001210: 5b56 ce15 b224 5892 d881 afa1 5d27 a730  [V...$X.....]'.0
-00001220: 922d 75d2 a551 ede7 7148 48dc bf75 9a35  .-u..Q..qHH..u.5
-00001230: 826b aeb6 fc54 8e4a 7a41 612e 10b2 2458  .k...T.JzAa...$X
-00001240: 92d8 96af d54f 98a8 c260 76db 099e 4606  .....O...`v...F.
-00001250: 3c8d 0881 fc1d ddc0 6f21 9938 b114 601d  <.......o!.8..`.
-00001260: dfab 13b9 46c8 9260 4962 67be 2efb 4e52  ....F..`Ibg...NR
-00001270: 6104 5beb c44f 2383 9f46 8440 fe8e d2e5  a.[..O#..F.@....
-00001280: 22fb ae73 abbd 8c9e 580a b096 eb27 029c  "..s....X....'..
-00001290: 3364 49b0 24b1 135f 3bbb 4c4f 6114 5bea  3dI.$.._;.LOa.[.
-000012a0: c44e 2383 9d46 843e de65 6976 b830 d06a  .N#..F.>.eiv.0.j
-000012b0: 2923 2796 02ac 75a8 83bb 27f3 2696 044b  )#'...u...'.&..K
-000012c0: 12db f0f5 b3cb e814 46b1 9f4e d634 32ac  ........F..N.42.
-000012d0: 6944 c8e3 dd3e 2962 3694 4913 4b01 166b  iD...>)b6.I.K..k
-000012e0: 3794 3913 4b82 2589 6df8 1ada 6976 0ac3  7.9.K.%.m...iv..
-000012f0: d851 2765 1a19 ca34 22d8 f13e a36b 231a  .Q'e...4"..>.k#.
-00001300: 2135 3799 2f61 a1b6 6b23 385f c892 6049  !57./a..k#8_..`I
-00001310: 6217 be66 7a8f 4d61 081b e9c4 4a23 8395  b..fz.Ma....J#..
-00001320: 4684 38de 67ed 175f cf1a 9135 3f19 2c61  F.8.g.._...5?.,a
-00001330: bd53 aef7 e6bc 214b 8225 89dd f8fa da75  .S....!K.%.....u
-00001340: 8a0a 23d9 5e27 621a 1bc4 3426 d8f1 3e8b  ..#.^'b...4&..>.
-00001350: 771a 7f3d d908 33de b214 6031 d7d9 11e7  w..=..3...`1....
-00001360: 0c59 122c 49ec c477 f988 4ee3 5318 c68b  .Y.,I..w..N.S...
-00001370: 4838 11d3 d820 a631 c18e f759 3a4b a2a5  H8... .1...Y:K..
-00001380: beff 3069 b596 3913 4b01 97dc 6f6e 74fe  ..0i..9.K...ont.
-00001390: e1f6 50d7 6e2e b326 9604 4b12 7bf1 35f7  ..P.n..&..K.{.5.
-000013a0: 0963 5418 cc16 3b81 d3d8 00a7 31c1 0fe7  .cT...;.....1...
-000013b0: bc67 8dd0 9ac1 4c9c b0a0 179b e002 214b  .g....L.......!K
-000013c0: 8225 896d f97a dd79 9e0a 43d9 6927 871a  .%.m.z.y..C.i'..
-000013d0: 1b0e 3526 f0f1 e1f6 f67a 9de5 f69d 98f9  ..5&.....z......
-000013e0: 134b 0196 3a69 791f c64e 2c09 9624 76e3  .K..:iy..N,..$v.
-000013f0: 6b6d 8701 2a0c 6253 dd8b 35d5 566b 22e4  km..*.bS..5.Vk".
-00001400: f121 654f 5b16 6c6a 59b1 e949 4b36 b5ac  .!eO[.ljY..IK6..
-00001410: d9d4 b268 53cb aa4d cfb5 6c93 fffc 14c6  ...hS..M..l.....
-00001420: b0a5 4ecc 3436 9869 4cc8 e343 9ead aadf  ..N.46.iL..C....
-00001430: 91db 569a 9b35 a26a a632 66c2 5ace 1329  ..V..5.j.2f.Z..)
-00001440: c64c 2c09 9624 76e2 6b68 97e9 298c 624b  .L,..$v.kh..).bK
-00001450: 9d98 696c 30d3 98a8 c7c7 ec4e e77c 72cc  ..il0......N.|r.
-00001460: 9c89 a580 a539 4b21 4b82 2589 1be6 eb5a  .....9K!K.%....Z
-00001470: a701 290c 63db 9c34 696c 68d2 1801 8ffe  ..).c..4ilh.....
-00001480: 75b8 dbad e3ad d538 e649 2c05 58ce 17e9  u......8.I,.X...
-00001490: 738d 9025 c192 c4ce 7c6d ee38 5085 816c  s..%....|m.8P..l
-000014a0: b413 328d 0d64 1a13 fa70 2d35 d008 ac19  ..2..d...p-5....
-000014b0: cda8 09cb 39d6 b19a 73ce 9025 c192 c44e  ....9...s..%...N
-000014c0: 7c8d ed38 4085 816c ac13 3a8d 0d74 1a3f  |..8@..l..:..t.?
-000014d0: 0102 cd1a c135 7399 3b61 49bf cf37 0ca0  .....5s.;aI..7..
-000014e0: 5812 2c49 6ccb d7e9 274c 5461 30bb ed64  X.,Il...'LTa0..d
-000014f0: 5013 c3a0 26b8 f452 0b90 9f35 a28c cd2c  P...&..R...5...,
-00001500: 0558 cbcb 662e 10b2 2458 92d8 96ef 1a98  .X..f...$X......
-00001510: 5d46 a930 8a57 c274 e2a8 89c1 5113 5cd0  ]F.0.W.t....Q.\.
-00001520: 5b7f dbeb d4ba a0f2 ac11 54b3 9731 1496  [.........T..1..
-00001530: f259 dc94 7914 4b82 2589 4df9 9adb 618e  .Y..y.K.%.M...a.
-00001540: 0a83 d85b 2787 9a18 0e35 21f8 711d a7ab  ...['....5!.q...
-00001550: 441f a849 0b6c 6c84 d75c 6616 8545 ddb0  D..I.ll..\f..E..
-00001560: 91b3 862c 0996 24f6 e26b ee93 06a9 309c  ...,..$..k....0.
-00001570: 6d76 42a8 8981 5013 c221 27fe c07c d648  mvB...P..!'..|.H
-00001580: 5033 9a81 1496 f53b 5a33 9962 49b0 24b1  P3.....;Z3.bI.$.
-00001590: 2d5f cf9f 3855 8509 d875 27a5 9a18 4a35  -_..8U...u'...J5
-000015a0: 2162 f279 9d6b f7be cdbc 8aa5 006b 9eb0  !b.y.k.......k..
-000015b0: 6f33 ad62 49b0 24b1 175f 9f9f 3247 85d1  o3.bI.$.._..2G..
-000015c0: 6cb2 7bc9 f1da 9ae3 c450 3ec7 1b7d 5dee  l.{......P>..}].
-000015d0: 5676 735b 561e 6f59 7afc 39d6 1e6f 597c  Vvs[V.oYz.9..oY|
-000015e0: bc65 f5f1 96e5 c79f 6bfd f12e 8354 18c5  .e......k....T..
-000015f0: ee3a 11d6 c420 ac09 a196 6353 d6ef 881a  .:... ....cS....
-00001600: 6135 7b19 6161 3117 96e4 9c21 4b82 2589  a5{.aa1....!K.%.
-00001610: 9df8 7ada 697c 0ac3 d854 27e0 9a18 c035  ..z.i|...T'....5
-00001620: 21ac f2f9 2e73 1e95 9971 b114 60c5 138e  !....s...q..`...
-00001630: ca4c b558 122c 49ec c5d7 dbee 5354 18cb  .L.X.,I.....ST..
-00001640: 063b c1d6 c480 ad09 e115 5825 7cd6 08a8  .;........X%|...
-00001650: b9ca 400b cb9c ba38 39e7 0e59 122c 49ec  ..@....89..Y.,I.
-00001660: c8d7 5bcf 012a 0c60 439d 406b 6280 d684  ..[..*.`C.@kb...
-00001670: 08ca 3f5b 5a2e b311 52b3 9431 1616 3ae5  ..?[Z...R..1..:.
-00001680: f229 ce1b b224 5892 d88d af9d dee3 5318  .)...$X.......S.
-00001690: c286 3a99 d5d4 30ab 2921 93fb 5dc7 6669  ..:...0.)!..].fi
-000016a0: 23c8 58ca 52e0 2ce5 da4b 3977 c892 6049  #.X.R.,..K9w..`I
-000016b0: 6247 beb7 f8e8 3044 8541 7c93 0f27 ac9a  bG....0D.A|..'..
-000016c0: 1a58 3525 5e72 e2b4 678d 0435 9319 5c61  .X5%^r..g..5..\a
-000016d0: 599f 55c9 397f c892 6049 6257 be46 3f71  Y.U.9...`IbW.F?q
-000016e0: a80a 13b0 e94e 8a35 3514 6b4a f4e4 8bce  .....N.55.kJ....
-000016f0: 8b78 c1eb b935 026b 6633 bfc2 726d d72c  .x...5.kf3..rm.,
-00001700: 73be 9025 c192 c42e 7ccd ed38 3c85 816c  s..%....|..8<..l
-00001710: aa93 594d 0db3 9ab6 c1a3 bf8a 24b2 3bca  ..YM........$.;.
-00001720: a08a a500 6bb9 3ef9 70ce 9025 c192 c44e  ....k.>.p..%...N
-00001730: 7c5d ed32 3d85 516c a913 484d 0d90 9a12  |].2=.Ql..HM....
-00001740: 0aa9 9aba 4ae2 8dfd 3690 b346 5ccd 5446  ....J...6..F\.TF
-00001750: 5158 cd69 2a83 2896 044b 123b f135 b5db  QX.i*.(..K.;.5..
-00001760: fc14 c6b1 ad4e 0435 3508 6a4a 0cc4 e3cd  .....N.55.jJ....
-00001770: 6fd6 9aa4 f72b 4bcf dcdd 95f2 5c35 f2d4  o....+K.....\5..
-00001780: 5e10 28cd 590a 5912 2c49 dc1c 5fcb 9f61  ^.(.Y.Y.,I.._..a
-00001790: b60a 93b0 ffee 7be5 d56e 96d7 7617 bb30  ......{..n..v..0
-000017a0: ca37 56bf 5b6e 97d7 72bf bcb6 5227 9f67  .7V.[n..r...R'.g
-000017b0: b5dc 30af e58e 792d b7cc 7bae 7be6 7518  ..0...y-..{.{.u.
-000017c0: a4c2 2036 d709 aba6 0656 4d09 9554 3ddd  .. 6.....VM..T=.
-000017d0: c35e 91c7 d60f c18d e09a c94c abb0 a4f3  .^.........L....
-000017e0: c0cd ac8a 25c1 92c4 4e7c 8d7d c210 1506  ....%...N|.}....
-000017f0: b3c1 4e58 3535 b06a 4ae8 a4f6 259d d55b  ..NX55.jJ...%..[
-00001800: 6656 2c05 add5 4ede 8199 5bb1 2458 92d8  fV,...N...[.$X..
-00001810: 95af cfdd 66a9 308e 2d76 e2ab a9c1 57d3  ....f.0.-v....W.
-00001820: e7b8 386a d6c8 5233 9c89 566b ed93 0d67  ..8j..R3..Vk...g
-00001830: b2c5 9260 4962 57be 863f c764 1566 61fb  ...`IbW..?.d.fa.
-00001840: 9db0 eba5 815d 2f09 b9d0 a236 8d00 e334  .....]/....6...4
-00001850: 4b01 9671 1db6 3967 c892 6049 6227 be37  K..q..9g..`Ib'.7
-00001860: 3ef5 1c9c c200 bee5 29c3 adfe 6ead 7551  >.......)...n.uQ
-00001870: 0def f262 1bad f4bb 285f c5e9 ae97 e8db  ...b....(_......
-00001880: 32e2 fcc5 cbf2 1c2d 8f57 ebe3 1f45 b67d  2......-.W...E.}
-00001890: 7d36 38eb dd64 4591 6d0e ff5d eb68 a9f3  }68..dE.m..].h..
-000018a0: ea09 a57e 9b65 c5f1 8faa cc5d 967f 3d14  ...~.e.....]..=.
-000018b0: b9fc 3f50 4b03 0414 0000 0008 0025 57f5  ..?PK........%W.
-000018c0: 568d 2e97 f3c3 0e00 006f 8b00 0018 0000  V........o......
-000018d0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-000018e0: 6865 6574 332e 786d 6cad 9d5b 779b 4816  heet3.xml..[w.H.
-000018f0: 85ff 8a96 9fa6 5f62 ebe6 24bd 1caf 1549  ......_b..$....I
-00001900: 405d ba92 2cbb 67fa 194b 659b 892c d480  @]..,.g..Ke..,..
-00001910: dac9 fcfa 01f9 0212 7caa 80fc 14db 9ff7  ........|.......
-00001920: a9aa 533b 086f 04ba 788c 93ef e9bd b559  ..S;.o..x......Y
-00001930: efc7 c372 957e 3ab9 cfb2 f5ef a7a7 e9fc  ...r.~:.........
-00001940: de3e 84e9 bb78 6d57 39b9 8d93 8730 cbbf  .>...xmW9....0..
-00001950: 4dee 4ed3 7562 c3c5 56f4 b03c 1d9c 9d9d  M.N.ub..V..<....
-00001960: 9f3e 84d1 eae4 f262 fbb3 6fc9 e545 bcc9  .>.....b..o..E..
-00001970: 96d1 ca7e 4b7a e9e6 e121 4c7e 4eec 327e  ...~Kz...!L~N.2~
-00001980: fc74 d23f 79f9 c155 7477 9f6d 7f70 7a79  .t.?y..Utw.m.pzy
-00001990: b10e efec b5cd febd ce05 f9b7 a7af 7516  ..............u.
-000019a0: d183 5da5 51bc ea25 f6f6 d3c9 e7fe ef5f  ..].Q..%......._
-000019b0: ce07 5bc9 f657 fe13 d9c7 b4f2 75af 58cd  ..[..W......u.X.
-000019c0: 4d1c 7f2f be91 8b4f 2767 c5a4 ecd2 ceb3  M../...O'g......
-000019d0: a246 98ff f38f 9dda e5b2 2895 4fe5 efe7  .F........(.O...
-000019e0: aa27 e5a8 85b2 faf5 4b79 7fdb 807c 7e37  .'......Ky...|~7
-000019f0: 616a a7f1 f2af 6891 dd7f 3af9 70d2 5bd8  aj....h...:.p.[.
-00001a00: db70 b3cc aee2 4761 9f17 352e a738 0bb3  .p....Ga..5..8..
-00001a10: f0f2 2289 1f7b 49b1 dacb 8b79 f145 3164  .."..{I....y.E1d
-00001a20: fe8b d1aa e8d2 7596 e43f 8ff2 91b2 cbe2  ......u..?......
-00001a30: d77b 265e d865 6f66 6fa3 5554 4cfc e234  .{&^.eofo.UTL..4
-00001a40: cba7 54fc c2e9 fcb9 c064 bf40 31e0 964c  ..T......d.@1..L
-00001a50: 91cc 9078 487c 2401 1241 8bbb cec2 cc36  ...xH|$..A.....6
-00001a60: 2c46 6229 8544 d320 7a15 3f2e ede2 cee6  ,Fb).D. z.?.....
-00001a70: dbfd f726 4ab7 1dec 2de3 bb86 81ff c0f2  ...&J...-.......
-00001a80: 06c9 9726 729a 6ff0 eb2e 0f5e 7779 0073  ...&r.o....^wy.s
-00001a90: 9c2e c334 6dda 5512 7c4b f2ff 8749 f6b3  ...4m.U.|K...I..
-00001aa0: 4133 25cd 97f0 a1a9 d933 fafd 994d e749  A3%......3...M.I
-00001ab0: b406 c379 24fb f3e7 ba69 189f 7edf 44ab  ...y$....i..~.D.
-00001ac0: de34 deac b206 5180 a2f0 078a 042f 283f  .4....Q....../(?
-00001ad0: 50cd 73cb 2d9a 3ce7 5215 ae99 35fb 5591  P.s.-.<.R...5.U.
-00001ae0: f6ca ae97 e1dc 2e7a 93a6 9dd2 24bb 8e37  .......z....$..7
-00001af0: c9bc 69a0 3f0e 2b7a de2a 8bb2 9f3d d869  ..i.?.+z.*...=.i
-00001b00: c3dd cce6 f70d 822f e8d7 f821 3f0e ef35  ......./...!?..5
-00001b10: 7fc7 f3c3 57cf 0fe9 3fce 649f bc54 bf0f  ....W...?.d..T..
-00001b20: d3e9 cc1f ceb6 87bd 2687 63c9 1912 0f89  ........&.c.....
-00001b30: 8f24 4022 9048 240a 89c6 46e4 2fbd 69fe  .$@".H$...F./.i.
-00001b40: dafb fdee dd3c becb 8ffd f65d 189d 3e46  .....<.....]..>F
-00001b50: abc5 6993 39ba f6d3 90d0 fec8 5f21 9b7c  ..i.9......._!.|
-00001b60: d1b4 949d ed1f bd6e ff08 b77f 9fec 4eb7  .......n......N.
-00001b70: 78e1 fb9a dc85 abe8 7fdb ff7b 5736 dd7a  x..........{W6.z
-00001b80: 1c0e 2f53 1c67 86c4 43e2 2309 9008 2412  ../S.g..C.#...$.
-00001b90: 8942 a2b1 3bed 3cf1 a64d 3654 0d8d d2b4  .B..;.<..M6T....
-00001ba0: be1d a38c 5f8d 3246 a3ec 93fa 1af2 73c5  ...._.2F......s.
-00001bb0: 264f 60c9 1912 0f89 8f24 4022 9048 240a  &O`......$@".H$.
-00001bc0: 89c6 46b4 f344 d77e 1a12 e2f6 372d 6567  ..F..D.~....7-eg
-00001bd0: fbcf 5fb7 ff1c b77f 9f34 4c37 8b93 fc2f  .._......4L7.../
-00001be0: 06d7 2102 8798 21f1 90f8 4802 2402 8944  ..!...!...H.$..D
-00001bf0: a290 686c 4c3b 3bbc 557f 0d15 427b 342d  ..hlL;;.U...B{4-
-00001c00: 6dc7 1eef 5fed f11e edb1 4f76 a7ef fd53  m..._.....Ov...S
-00001c10: 3b4f 7932 0316 9c21 f190 f848 0224 0289  ;Oy2...!...H.$..
-00001c20: 44a2 9068 6c43 3b33 74eb a621 196e 7dd3  D..hlC;3t..!.n}.
-00001c30: 4276 b6fe c3eb d67f c0ad df27 bb93 f5a3  Bv.........'....
-00001c40: 65e3 6100 ebcd 9078 487c 2401 1281 4422  e.a....xH|$...D"
-00001c50: 5148 3476 a1dd ce77 6aa6 2115 6e7c d33a  QH4v...wj.!.n|.:
-00001c60: 7636 fee3 ebc6 7fc4 8ddf 27bb 73fd 23bc  v6........'.s.#.
-00001c70: 69fe bb01 0bce 9078 487c 2401 1281 4422  i......xH|$...D"
-00001c80: 5148 34b6 a1dd ce77 eba6 2119 6e7d d342  QH4....w..!.n}.B
-00001c90: 76b6 be7f 56e6 6167 b8f9 35b4 3bdf 2bbb  v...V.ag..5.;.+.
-00001ca0: dc9e cba6 f7d1 bac9 045c 79c6 c863 e433  .........\y..c.3
-00001cb0: 0a18 0946 9291 62a4 b92d eddc 705c 7b0d  ...F..b..-..p\{.
-00001cc0: cad1 168d 6bda f545 2527 c51c 6e52 43fb  ....k..E%'..nRC.
-00001cd0: 133f 7c76 c895 678c 3c46 3ea3 8091 6024  .?|v..g.<F>...`$
-00001ce0: 1929 469a dbd2 d217 47b5 d7a0 9c7d e10c  .)F.....G....}..
-00001cf0: 56fb 65b2 dadf 8faa 2abe a014 eb69 e27f  V.e.....*....i..
-00001d00: 460f f6da 2651 b329 b0ec 8c91 c7c8 6714  F...&Q.)......g.
-00001d10: 3012 8c24 23c5 4873 4f5a 9aa2 7b6f 0d6a  0..$#.HsOZ..{o.j
-00001d20: d911 4d0b da75 4499 3bf6 3978 aca1 caac  ..M..uD.;.9x....
-00001d30: 8bbf 77be 25f1 62d3 3885 2957 9d31 f218  ..w.%.b.8.)W.1..
-00001d40: f98c 0246 8291 64a4 1869 6e49 4b43 746e  ...F..d..inIKCtn
-00001d50: ad41 29fb c199 43f6 cb20 b2cf 4964 0d55  .A)...C.. ..Id.U
-00001d60: 26fd 2d7e b4c9 349b 6e92 7fac b159 b8c8  &.-~..4.n....Y..
-00001d70: 17d1 680c 0e20 1979 8c7c 4601 23c1 4832  ..h.. .y.|F.#.H2
-00001d80: 528c 34f7 a6a5 318e efb1 c11a ec10 6700  R.4...1.......g.
-00001d90: d92f 13c8 3e47 9035 5499 fd5f f992 ffdc  ./..>G.5T.._....
-00001da0: 2437 3999 de87 493e 93fc 8897 66d1 bcd1  $79...I>....f...
-00001db0: 269c 4932 f218 f98c 0246 8291 64a4 1869  &.I2.....F..d..i
-00001dc0: 6e50 4b9b bc51 a30d 1662 af38 d3ca 7e19  nPK..Q...b.8..~.
-00001dd0: 57f6 39af aca1 e625 b85e 6838 ad64 e431  W.9....%.^h8.d.1
-00001de0: f219 058c 0423 c948 31d2 dc9d 9646 798b  .....#.H1....Fy.
-00001df0: 2e1b acc2 2e71 8696 fd32 b5ec 736c 5943  .....q...2..slYC
-00001e00: 2f23 4795 8b75 5f6f 1bad c1d9 2523 8f91  /#G..u_o....%#..
-00001e10: cf28 6024 1849 468a 91c6 96b4 b546 e7d6  .(`$.IF......F..
-00001e20: 1a94 b21f 9c49 66bf 8c32 fb9c 65d6 d0ce  .....If..2..e...
-00001e30: a40f 5da8 0393 70cc c9c8 63e4 330a 1809  ..]...p...c.3...
-00001e40: 4692 9162 a4b1 4f6d 4df2 b6fd 3658 8f9d  F..b..OmM...6X..
-00001e50: e38c 42fb 6516 dae7 30b4 866a 2bb9 b619  ..B.e...0..j+...
-00001e60: 9884 1351 461e 239f 51c0 4830 928c 1423  ...QF.#.Q.H0...#
-00001e70: 8d2d 696b 92ce ad35 2865 3f38 f3d1 4199  .-ik...5(e?8..A.
-00001e80: 8f0e 381f ada1 faa4 ebd7 f39a fdc1 a3cc  ..8.............
-00001e90: 1879 8c7c 4601 23c1 4832 528c 34b6 a8a5  .y.|F.#.H2R.4...
-00001ea0: 3fde aed5 064b a15f 1ad7 b7eb 9732 371d  ?....K._.....27.
-00001eb0: 706e 5a43 3b8b d85e f203 7770 62ca c863  pnZC;..^..wpb..c
-00001ec0: e433 0a18 0946 9291 62a4 b121 6ddd d1b1  .3...F..b..!m...
-00001ed0: b106 85ec 05f7 9b50 2bef 42e5 acb4 8676  .......P+.B....v
-00001ee0: a65c 5c04 042b 704e cac8 63e4 330a 1809  .\\..+pN..c.3...
-00001ef0: 4692 9162 a4b1 1f6d add0 adaf 0675 ec04  F..b...m.....u..
-00001f00: 6746 3a28 33d2 0167 a435 b433 e3ed 4541  gF:(3..g.5.3..EA
-00001f10: b002 27a4 8c3c 463e a380 9160 2419 2946  ..'..<F>...`$.)F
-00001f20: 1a1b d2d6 0a1d 1b6b 50c8 5e70 e6a3 8332  .......kP.^p...2
-00001f30: 1f1d 703e 5a43 3b53 ae5e 1104 4b70 36ca  ..p>ZC;S.^..Kp6.
-00001f40: c863 e433 0a18 0946 9291 62a4 b12f 6d2d  .c.3...F..b../m-
-00001f50: 715c 7f0d ead9 19ce 5c74 50e6 a203 ce45  q\......\tP....E
-00001f60: 6b68 6fe6 ce13 4c8e 4319 798c 7c46 0123  kho...L.C.y.|F.#
-00001f70: c148 3252 8c34 f6a5 ad33 8eeb af41 3d3b  .H2R.4...3...A=;
-00001f80: c399 820e ca14 74c0 2968 0ded ccfc f5c2  ......t.)h......
-00001f90: 20d8 82c3 4f46 1e23 9f51 c048 3092 8c14   ...OF.#.Q.H0...
-00001fa0: 238d 4d69 6b8b 239a 6b50 cc9e 7066 9e83  #.Mik.#.kP..pf..
-00001fb0: 32f3 1c70 e659 43e5 b42b 392d 5882 434f  2..p.YC..+9-X.CO
-00001fc0: 461e 239f 51c0 4830 928c 1423 8d3d 696b  F.#.Q.H0...#.=ik
-00001fd0: 89ee bd35 a865 4738 53cf 4199 7a0e 38f5  ...5.eG8S.A.z.8.
-00001fe0: aca1 72d6 78b5 07fc c179 2723 8f91 cf28  ..r.x....y'#...(
-00001ff0: 6024 1849 468a 91c6 0eb5 f5c7 5b75 da60  `$.IF.......[u.`
-00002000: 2576 8b33 e91c 9449 e780 93ce 1a6a 5c83  %v.3...I.....j\.
-00002010: fb50 c2a9 2723 8f91 cf28 6024 1849 468a  .P..'#...(`$.IF.
-00002020: 91c6 f6b4 b5ca 9bb4 d960 19f6 8933 011d  .........`...3..
-00002030: 9609 e890 02b3 cf69 da78 fbca 0415 db57  .......i.x.....W
-00002040: cdad acd9 3028 9469 2f57 f6b6 d25e a376  ....0(.i/W...^.v
-00002050: 86da abe2 bed2 d4ae b2b4 973c 9fe1 f76e  ...........<...n
-00002060: 6cf6 68ed aa17 56ca fe6b 1117 77d3 f7c2  l.h...V..k..w...
-00002070: bb55 5cfc a7ec c537 ffb5 f3ec b75e b85a  .U\....7.....^.Z
-00002080: f49e 59ba b6f3 e8f6 95f5 fe95 6ee6 f7bd  ..Y.........n...
-00002090: 30ed 15fb d57b deb0 dfde 35dd c68b f3ab  0....{....5.....
-000020a0: 6c75 d3ed bc35 5de9 7946 8291 64a4 1869  lu...5].yF..d..i
-000020b0: 9c7e db7b 273b 7ac3 a090 6f9e 74e6 b6c3  .~.{';z...o.t...
-000020c0: 32b7 1d52 14f8 f947 94c2 7b2d 2728 8ad2  2..R...G..{-'(..
-000020d0: 1719 189d 135d 461e 0ee7 b210 c7bd 8c04  .....]F.........
-000020e0: 23c9 4831 d238 fdb6 16ea d875 8342 b690  #.H1.8.....u.B..
-000020f0: 33ee 1d96 71ef 9032 c4e7 775c 353a 0873  3...q..2..w\5:.s
-00002100: cf30 9d66 9368 d5f4 b482 694d 55b1 0fa7  .0.f.h....iMU...
-00002110: c038 569a 25d1 aae9 310d 3e57 0b18 0946  .8V.%...1.>W...F
-00002120: 9291 62a4 b94b 2d9d d3a5 db06 556c 1b67  ..b..K-.....Ul.g
-00002130: 363c acdc b74f 71e3 21db 70b6 593d c97c  6<...Oq.!.p.Y=.|
-00002140: 2a00 87a0 0337 f71f b8bb 9f06 761d 820e  *....7......v...
-00002150: dcfc 7fe0 eeff 03b7 ff1f b8ff ffc0 0300  ................
-00002160: deea 0900 47f7 df60 0976 9533 651e 9629  ....G..`.v.3e..)
-00002170: f390 a24a e94d f129 2828 8ad2 1719 9889  ...J.M.)((......
-00002180: 8367 461e 0ee7 3213 a7d2 8c04 23c9 4831  .gF...2.....#.H1
-00002190: d238 fdb6 66ea d875 8342 b690 338e 1e96  .8..f..u.B..3...
-000021a0: 71f4 9032 4db9 4ab3 70f9 742a 8da7 461c  q..2M.J.p.t*..F.
-000021b0: a8ee cbc1 529c 5833 f270 5897 a538 ce66  ....R.X3.pX..8.f
-000021c0: 2418 4946 8a91 c6e9 b7b5 d491 dd37 5880  $.IF.........7X.
-000021d0: ade5 ccb3 8765 9e3d a468 f4cb e6e1 c626  .....e.=.h.....&
-000021e0: 5f6f 27cb 7061 9b8f 511c c9ee 8ac1 569c  _o'.pa..Q.....V.
-000021f0: 7833 f270 5097 ad38 0e67 2418 4946 8a91  x3.pP..8.g$.IF..
-00002200: c6e9 b7b5 d551 bd37 2867 5339 03f1 6119  .....Q.7(gS9..a.
-00002210: 880f 295d 7dba ed01 cfa5 0edc 8abf 55e2  ..)]}.........U.
-00002220: 5938 27e5 8c3c 1cee c059 3827 e88c 0423  Y8'..<...Y8'...#
-00002230: c948 31d2 dca8 962e ead8 7083 42f6 8f33  .H1.......p.B..3
-00002240: 3e1f 96f1 f990 f256 877f 7e29 f02d 6bc0  >......V..~).-k.
-00002250: 7189 6375 461e 8eed 3a2e 71e6 ce48 3092  q.cuF...:.q..H0.
-00002260: 8c14 238d d36f eba8 b7d8 0283 55d8 5ece  ..#..o......U.^.
-00002270: bc7d 58e6 ed43 8a69 afe2 2c4e be26 915d  .}X..C.i..,N.&.]
-00002280: 6521 3d75 12c5 51ba 2f07 7f71 16cf c8c3  e!=u..Q./..q....
-00002290: 615d fee2 a09e 9160 2419 2946 1aa7 dfd6  a].....`$.)F....
-000022a0: 5f47 76df 6001 b696 33a2 1f95 11fd 08b3  _Gv.`...3.......
-000022b0: ef62 7674 8a8e aae7 55f1 b979 4d59 9a89  .bvt....U..yMY..
-000022c0: 9187 e339 ccc4 2503 4682 9164 a418 699c  ...9..%.F..d..i.
-000022d0: 7edb 27c5 756d bb41 253f 16ce 1981 8fca  ~.'.um.A%?......
-000022e0: 087c 848f 8fb5 7f6f ecaa f141 9913 146d  .|.....o...A...m
-000022f0: f3fc 1725 d888 5370 461e 8ef8 e5fd 60f4  ...%..SpF.....`.
-00002300: f143 7fb1 b0ef cffb a3c5 59ff 66fc d17e  .C........Y.f..~
-00002310: 988f 6e6e 6ede dfce c370 d068 2ece c619  ..nnn....p.h....
-00002320: 0946 9291 62a4 7151 6dcd d57d 3b0c 6ad9  .F..b.qQm..};.j.
-00002330: 5ece 787c 54c6 e323 8a51 af37 eb75 9c64  ^.x|T..#.Q.7.u.d
-00002340: f98f 36f3 6c93 d093 2d26 5820 4a9b 4a80  ..6.l...-&X J.J.
-00002350: e738 3a67 e4e1 d0ae 4317 e7e7 8c04 23c9  .8:g....C.....#.
-00002360: 4831 d238 fdb6 ee7a 831d 3058 846d e68c  H1.8...z..0X.m..
-00002370: d347 659c 3eea 9650 4f50 97ff 5572 e01a  .Ge.>..POP..Ur..
-00002380: e0b4 a6ab 188a 7374 1ced c050 3ed7 0b18  ......st...P>...
-00002390: 0946 9291 62a4 b953 2ddd d4ad e306 756c  .F..b..S-.....ul
-000023a0: 20f7 7374 2b0f d2ed 964a 4f50 f7f4 8816   .st+....JOP....
-000023b0: 7ab7 c4b4 a6ab 18e8 c023 7569 341a c7e7  z........#ui4...
-000023c0: 6201 23c1 4832 528c 34b7 a9a5 7bba b5db  b.#.H2R.4...{...
-000023d0: a08e dde3 0ccd 4765 683e ea16 404f 5057  ......Geh>..@OPW
-000023e0: 2c67 93c9 d5f5 da36 3e4f 7d5a 5356 fcc3  ,g.....6>O}ZSV..
-000023f0: 4139 8e77 bb8c c366 ff70 44ce 4830 928c  A9.w...f.pD.H0..
-00002400: 1423 cd8d 6ae9 9fae 0d37 a864 0739 b3f1  .#..j....7.d.9..
-00002410: 5199 8d8f ba65 cd13 d43d 2de8 eb26 630b  Q....e...=-..&c.
-00002420: 7128 cec8 c301 d942 1c87 3312 8c24 23c5  q(.....B..3..$#.
-00002430: 4873 a75a 5aa8 73c7 0d4a d943 ce28 7c54  Hs.ZZ.s..J.C.(|T
-00002440: 46e1 234a 4a5d 1e3a 10cd cea2 f0c1 6636  F.#JJ].:......f6
-00002450: 6934 1047 e18c 3c1c 8d0d c449 3823 c148  i4.G..<....I8#.H
-00002460: 3252 8c34 b7a9 a581 bab5 dba0 8edd e30c  2R.4............
-00002470: c247 6510 3eea 962a 4f50 972f c7fb 91af  .Ge.>..*OP./....
-00002480: 6515 2e65 f301 88d3 6f46 1e8e 97e2 a514  e..e....oF......
-00002490: ae16 3012 8c24 23c5 4873 a75a 1aa8 6bc7  ..0..$#.Hs.Z..k.
-000024a0: 0d2a d942 ceb0 7b54 86dd a36e c1f1 0475  .*.B..{T...n...u
-000024b0: f982 c4e6 e6e9 839e 1a1d c4f9 3623 0f87  ............6#..
-000024c0: e323 1027 db8c 0423 c948 31d2 dca7 9606  .#.'...#.H1.....
-000024d0: ead8 6f83 42f6 8f33 d11e 9789 f6b8 5b56  ..o.B..3......[V
-000024e0: 3c41 5dbe 9e03 ef7c 9ad6 74a5 7d18 7938  <A]....|..t.}.y8
-000024f0: da81 a17c ae17 3012 8c24 23c5 4873 a75a  ...|..0..$#.Hs.Z
-00002500: 7ec8 45b7 8e1b d4f1 875c 38c3 ec71 1966  ~.E......\8..q.f
-00002510: 8fbb bd57 7a82 ba62 39ee f73d 4d6b fa8a  ...Wz..b9..=Mk..
-00002520: 9138 d3c6 517f 6148 9feb 068c 0423 c948  .8..Q.aH.....#.H
-00002530: 31d2 dcb9 9686 3a6e 070c ead9 58ce 187b  1.....:n....X..{
-00002540: 5cc6 d8e3 6e51 f004 75f9 b24c f8e3 3ade  \...nQ..u..L..:.
-00002550: ac16 db2b d48d aee2 d49a 9187 43e2 ab1b  ...+........C...
-00002560: 170b 1809 4692 9162 a4b9 572d ad74 44cf  ....F..b..W-.tD.
-00002570: 0d8a d947 ce9c 7a5c e6d4 e38e 3935 eaf2  ...G..z\....95..
-00002580: 3539 df3d 37ad a92b 46e2 b41a c774 0ee8  59.=7..+F....t..
-00002590: 73d5 8091 6024 1929 469a bbd6 d251 c774  s...`$.)F....Q.t
-000025a0: dfa0 9a2d e54c aec7 6572 3dee 985c a32e  ...-.L..er=..\..
-000025b0: 5fd4 55f1 318e 7c5c e2ec 9a91 87e3 f171  _.U.1.|\.......q
-000025c0: 89b3 6b46 8291 64a4 1869 6e54 4b17 756d  ..kF..d..inTK.um
-000025d0: b841 253b c8fd d170 95cf 86eb 985e a3ae  .A%;...p.....^..
-000025e0: 5890 fbed 4dd3 9abe e2a3 031f 2147 a3fe  X...M.......!G..
-000025f0: c290 3ed7 0d18 0946 9291 62a4 b973 2d2d  ..>....F..b..s--
-00002600: 75dc 0e18 d4b3 b19c a1f6 b80c b5c7 1d43  u..............C
-00002610: 6dd4 bd2c 0bcf c339 d266 e4e1 7087 c6f2  m..,...9.f..p...
-00002620: b960 c048 3092 8c14 23cd bd6a 69a5 8e3d  .`.H0...#..ji..=
-00002630: 3728 640f 3943 ed71 196a 8f3b 86da a8cb  7(d.9C.q.j.;....
-00002640: d7f3 8bef 3d99 d66a 54ec c401 378e fc8b  ....=..jT...7...
-00002650: c3fa 5c3b 6024 1849 468a 91e6 0eb6 74d6  ..\;`$.IF.....t.
-00002660: f13b 61b0 069b cc99 7d8f cbec 7bdc 31fb  .;a.....}...{.1.
-00002670: 465d b1b4 47bb ce3e 27b6 f1f3 2c6a c28a  F]..G..>'...,j..
-00002680: b338 fac6 e1f8 148a 936f 4682 9164 a418  .8.......oF..d..
-00002690: 69ee 534b 2b75 ecb7 4121 fbc7 197c 8fcb  i.SK+u..A!...|..
-000026a0: e07b dc31 f846 ddde e731 e03d c1d3 5a85  .{.1.F...1.=..Z.
-000026b0: 8a91 3801 c771 7924 9fcb 058c 0423 c948  ..8..qy$.....#.H
-000026c0: 31d2 dcb2 9656 3ab6 f506 2bb0 a79c 61f8  1....V:...+...a.
-000026d0: 7919 869f 770c c351 b7bb b043 9fb6 532b  y...w..Q...C..S+
-000026e0: 519a 8a91 c7c8 6714 3012 8c24 23c5 4873  Q.....g.0..$#.Hs
-000026f0: 6b5a 7ea6 efd1 2d36 5882 3fce d719 849f  kZ~...-6X.?.....
-00002700: 9741 f879 c720 1c75 7b2b 83cf ba9f d6f4  .A.y. .u{+......
-00002710: 15e7 7010 8ea3 a678 4997 ab05 8c04 23c9  ..p....xI.....#.
-00002720: 4831 d2dc af96 8e3a aeef 06f5 6c27 67fc  H1.....:....l'g.
-00002730: 7d5e c6df e71d e36f d4ed 2eeb e0ad 76d3  }^.....o......v.
-00002740: 5a91 8aa7 3806 c7a1 0f0e e673 c580 9160  Z...8......s...`
-00002750: 2419 2946 9a1b d7d2 576f b001 068b b0b9  $.)F....Wo......
-00002760: 3813 3f4d efad cd8a c79b 5d5e acc3 3b6b  8.?M......]^..;k
-00002770: c2e4 2e5a a5bd a5bd cd15 67ef de8f 4f7a  ...Z......g...Oz
-00002780: 4971 fdf9 e59b 2c5e 7f3a c9cd 7a13 6759  Iq....,^.:..z.gY
-00002790: fcb0 fdf2 de86 0b9b 14bf 90f3 db38 ce5e  .............8.^
-000027a0: bf29 8679 8c93 efdb 412e ff0f 504b 0304  .).y....A...PK..
-000027b0: 1400 0000 0800 2557 f556 f7f6 8f09 a702  ......%W.V......
-000027c0: 0000 6d0b 0000 0d00 0000 786c 2f73 7479  ..m.......xl/sty
-000027d0: 6c65 732e 786d 6cdd 56db 8e9b 3010 fd15  les.xml.V...0...
-000027e0: c407 944d 5051 a842 a436 d24a 95da 6aa5  ...MPQ.B.6.J..j.
-000027f0: dd87 be9a 6082 255f a831 ab64 bfbe 33b6  ....`.%_.1.d..3.
-00002800: 1392 ec0e ddf6 b1a0 84f1 1c9f b93b 643d  .............;d=
-00002810: b8a3 e48f 1de7 2e39 28a9 872a ed9c eb3f  .......9(..*...?
-00002820: 65d9 b0eb b862 c307 d373 0d48 6bac 620e  e....b...s.Hk.b.
-00002830: 9676 9f0d bde5 ac19 90a4 64b6 bcbb 2b32  .v........d...+2
-00002840: c584 4e37 6b3d aa7b e586 6467 46ed aaf4  ..N7k=.{..dgF...
-00002850: 2e4d b2cd ba35 7a52 2dd3 a080 bd4c f1e4  .M...5zR-....L..
-00002860: 99c9 2add 3229 6a2b c266 a684 3c06 fdd2  ..*.2)j+.f..<...
-00002870: 6b76 461a 9b38 8886 57e9 c2ab 8697 b061  kvF..8..W......a
-00002880: 1197 186a b4a5 8436 d66b b3e0 267c d791  ...j...6.k..&|..
-00002890: 7089 f8c7 003b 8494 d7f1 8162 b3ee 9973  p....;.....b...s
-000028a0: dcea 7b58 0492 d7be c6a2 fc74 ec21 bebd  ..{X.......t.!..
-000028b0: 65c7 c5f2 637a c1f0 0f70 531b db70 7be5  e...cz...pS..p{.
-000028c0: 28a8 366b c95b 870c 2bf6 9d17 9ce9 f151  (.6k.[..+......Q
-000028d0: 1be7 8c42 a911 6c6f 340b 919c 6857 74df  ...B..lo4...hWt.
-000028e0: c82a 751d 3462 b275 ab45 c3b7 bae8 e556  .*u.4b.u.E.....V
-000028f0: 7d76 1305 4861 c7a5 7cc4 6d3f db73 1e0b  }v..Ha..|.m?.s..
-00002900: c8e3 d026 a1f3 5f1b df74 2cec 4984 e4a3  ...&.._..t,.I...
-00002910: 18cc c405 3ab8 3417 8c5f d85d fe9b dd5e  ....:.4.._.]...^
-00002920: 3c1b f765 848c b45f ff1a 8de3 0f96 b7e2  <..e..._........
-00002930: e0d7 8776 0a80 32bf 20cc 839e f5bd 3c7e  ...v..2. .....<~
-00002940: 9662 af15 0fd9 bfdb e366 cd4e bca4 3356  .b.......f.N..3V
-00002950: bc80 379c c91d 2838 8cec 33b7 4eec 5003  ..7...(8..3.N.P.
-00002960: 4d0a 053a b4b1 4ae7 02f9 725d d5fe ac4d  M..:..J...r]...M
-00002970: f040 55e9 0f3c a8f2 22d1 7a14 d209 1d57  .@U..<..".z....W
-00002980: 9d68 1aae 5fb7 00ec 3b56 c34f c195 03d8  .h.._...;V.O....
-00002990: d5f0 968d d23d 9dc1 2a9d e4ef bc11 a32a  .....=..*......*
-000029a0: cfbb 1eb0 1671 d724 7fc3 515c 14d3 6906  .....q.$..Q\..i.
-000029b0: 6742 37fc c09b 6d5c da7d edc5 0404 701b  gB7...m\.}....p.
-000029c0: af30 c837 d0bd bf08 8864 0590 8010 247d  .0.7.....d....$}
-000029d0: 9161 90ac c023 7dfd 8f79 ade8 bc02 4846  .a...#}..y....HF
-000029e0: b87a 1b5a d1ac 15cd 0abc 37a1 adbf 495f  .z.Z......7...I_
-000029f0: 04ab 848b 48b9 2cf3 bc28 c8f2 6eb7 6f87  ....H.,..(..n.o.
-00002a00: b125 6b58 14f8 210c 9211 2287 f485 defe  .%kX..!...".....
-00002a10: b6f2 3303 3033 367f 980d b2cb b363 43a6  ..3.036......cC.
-00002a20: 3c33 a264 ca33 9547 88a8 2172 ca92 1800  <3.d.3.G..!r....
-00002a30: d217 72c8 a690 1385 4110 be70 d408 569e  ..r.....A..p..V.
-00002a40: 639f c908 c963 3e03 9525 09e1 9012 d35b  c....c>..%.....[
-00002a50: 1454 a10a bc89 7e91 8728 cfcb 9280 1024  .T....~..(.....$
-00002a60: c2c8 7312 c203 3b03 9161 6020 2494 e7e1  ..s...;..a` $...
-00002a70: 457a f33e cb4e efb9 6cfa 83bd f90d 504b  Ez.>.N..l.....PK
-00002a80: 0304 1400 0000 0800 2557 f556 b747 eb8a  ........%W.V.G..
-00002a90: c000 0000 1602 0000 0b00 0000 5f72 656c  ............_rel
-00002aa0: 732f 2e72 656c 739d 924b 6e02 310c 40af  s/.rels..Kn.1.@.
-00002ab0: 1265 5f4c a9c4 0231 acd8 b043 880b b889  .e_L...1...C....
-00002ac0: e7a3 99c4 9163 c4f4 f68d d8c0 2068 114b  .....c...... h.K
-00002ad0: ff9e 9e2d af0f 34a0 761c 73db a56c c630  ...-..4.v.s..l.0
-00002ae0: c45c d956 35ad 00b2 6b29 609e 71a2 582a  .\.V5...k)`.q.X*
-00002af0: 354b 402d a134 90d0 f5d8 102c e6f3 25c8  5K@-.4.....,..%.
-00002b00: 2dc3 6ed6 b74c 73fc 49f4 0a91 ebba 73b4  -.n..Ls.I.....s.
-00002b10: 6577 0a14 f501 f8ae c39a 234a 435a d971  ew........#JCZ.q
-00002b20: 8033 4bff cddc cf0a d49a 9daf acec fca7  .3K.............
-00002b30: 35f0 a6cc f3f5 2090 a247 4570 2cf4 91a4  5..... ..GEp,...
-00002b40: 4c8b 7694 af3e 9edd bea4 f3a5 6362 b478  L.v..>......cb.x
-00002b50: dfe8 fff3 d0a8 143d f9bf 9d30 a589 d2d7  .......=...0....
-00002b60: 4509 266f b0f9 0550 4b03 0414 0000 0008  E.&o...PK.......
-00002b70: 0025 57f5 56b9 489c 7652 0100 00ae 0200  .%W.V.H.vR......
-00002b80: 000f 0000 0078 6c2f 776f 726b 626f 6f6b  .....xl/workbook
-00002b90: 2e78 6d6c 8d91 dd4e 8340 1085 5f85 ec03  .xml...N.@.._...
-00002ba0: 08a5 dac4 a6f4 a68d dac4 bf58 e3fd 0043  ...........X...C
-00002bb0: 9974 7fc8 eed0 6a9f de5d 088a 69d2 78b5  .t....j..]..i.x.
-00002bc0: cc99 d98f 3967 1747 63f7 b931 fbe8 5349  ....9g.Gc..1..SI
-00002bd0: ede6 3613 3573 338f 6357 d4a8 c05d 9906  ..6.5s3.cW...]..
-00002be0: b5ef 55c6 2a60 5fda 5d6c aa8a 0a5c 9ba2  ..U.*`_.]l...\..
-00002bf0: 55a8 394e 9364 165b 94c0 64b4 aba9 71a2  U.9N.d.[..d...q.
-00002c00: a7fd 87e5 1a8b 50ba 1a91 95ec 510a 488b  ......P.....Q.H.
-00002c10: e562 d8ec d546 f1b8 328c 45f8 5350 83f2  .b...F..2.E.SP..
-00002c20: 4178 74bf 03a1 8c0e e428 2749 fc95 89ee  Axt......('I....
-00002c30: 5ba2 8814 6952 74c2 3213 8988 5c6d 8e0f  [...iRt.2...\m..
-00002c40: c6d2 c968 06b9 2dac 9132 1393 bef1 8196  ...h..-..2......
-00002c50: a938 93b7 61cd 77c8 5da7 30e4 6fc1 7326  .8..a.w.].0.o.s&
-00002c60: 6689 0756 641d 7713 1d1f fc92 07f4 c37d  f..Vd.w........}
-00002c70: d5b2 b923 c968 d7c0 786f 4ddb 90de 7518  ...#.h..xoM...u.
-00002c80: 6f23 1ef9 e8a2 18ce 4883 c24c 3c21 4309  o#......H..L<!C.
-00002c90: 0c61 0baf 6eca 7e23 f6a8 913f 3b27 dfb0  .a..n.~#...?;'..
-00002ca0: 9bb2 878e 012b 09ce a11b dd4f 2fdc 4fcf  .....+.....O/.O.
-00002cb0: eefb d49b 10c9 1fc4 f402 62da fb1a cc94  ..........b.....
-00002cc0: 5891 c6f2 d9c3 5c68 f868 0bff aee1 e8cc  X.....\h.h......
-00002cd0: a4d7 3793 5b1f 612b e5ca 6b2f fad1 40f9  ..7.[.a+..k/..@.
-00002ce0: 93ce f0b4 cb6f 504b 0304 1400 0000 0800  .....oPK........
-00002cf0: 2557 f556 0b08 5d06 bc00 0000 1f03 0000  %W.V..].........
-00002d00: 1a00 0000 786c 2f5f 7265 6c73 2f77 6f72  ....xl/_rels/wor
-00002d10: 6b62 6f6f 6b2e 786d 6c2e 7265 6c73 cd93  kbook.xml.rels..
-00002d20: 390e 8330 1045 af62 f900 0c4b 9222 8254  9..0.E.b...K.".T
-00002d30: 6968 232e 60c1 b088 c596 67a2 c0ed 83a0  ih#.`.....g.....
-00002d40: 004b 29d2 a0a4 b2fe 587e ff15 e3f8 819d  .K).....X~......
-00002d50: e246 0f54 3786 c4d8 7703 25b2 6636 5700  .F.T7...w.%.f6W.
-00002d60: ca6b ec15 79da e030 df94 daf6 8ae7 682b  .k..y..0......h+
-00002d70: 302a 6f55 8510 fafe 05ec 9e21 6ff1 9e29  0*oU.......!o..)
-00002d80: b2c9 e037 445d 964d 8e77 9d3f 7b1c f803  ...7D].M.w.?{...
-00002d90: 185e dab6 5423 b214 99b2 1572 2261 ecb6  .^..T#.....r"a..
-00002da0: 31c1 7204 de4c 9622 2d12 69d3 2290 027e  1.r..L."-.i."..~
-00002db0: 6d14 3a46 e11f 1845 8e51 74a4 11f1 d421  m.:F...E.Qt....!
-00002dc0: 6d3a 6b76 fa4f 47f6 f3fc 16b7 fa25 ae43  m:kv.OG......%.C
-00002dd0: 7751 ce8b 0438 ffe1 f606 504b 0304 1400  wQ...8....PK....
-00002de0: 0000 0800 2557 f556 dbfb ce8f 2401 0000  ....%W.V....$...
-00002df0: e904 0000 1300 0000 5b43 6f6e 7465 6e74  ........[Content
-00002e00: 5f54 7970 6573 5d2e 786d 6ccd 54cb 4ec3  _Types].xml.T.N.
-00002e10: 3010 fc95 c8d7 2a71 2912 07d4 f402 5ca1  0.....*q).....\.
-00002e20: 077e c024 9bc6 8a5f f26e 4bfa f76c 121a  .~.$..._.nK..l..
-00002e30: 0954 5aaa 20d1 4bac 7867 67c6 3bb2 97af  .TZ. .K.xgg.;...
-00002e40: fb00 98b4 d638 cc45 4d14 eea5 c4a2 06ab  .....8.EM.......
-00002e50: 30f3 011c 572a 1fad 22fe 8d1b 1954 d1a8  0...W*.."....T..
-00002e60: 0dc8 c57c 7e27 0bef 081c a5d4 7188 d5f2  ...|~'......q...
-00002e70: 112a b535 943c b5bc 8dda bb5c 4430 2892  .*.5.<.....\D0(.
-00002e80: 8701 d869 e542 8560 74a1 88eb 72e7 ca6f  ...i.B.`t...r..o
-00002e90: 2ae9 a742 c69d 3d06 6b1d 70c6 0091 c8a3  *..B..=.k.p.....
-00002ea0: 127d e947 8543 e3cb 0e62 d425 246b 15e9  .}.G.C...b.%$k..
-00002eb0: 5959 86c9 d648 a4bd 01cc 4e73 1c71 e9ab  YY...H....Ns.q..
-00002ec0: 4a17 50fa 626b b925 c310 4195 5803 9035  J.P.bk.%..A.X..5
-00002ed0: d940 3a3b 234d 3c64 18be 3793 0df4 3427  .@:;#M<d..7...4'
-00002ee0: 1519 ba8e 3e20 a716 e172 bd43 2c5d 771a  ....> ...r.C,]w.
-00002ef0: 9808 22e9 3387 1c25 997b f209 a14b bc84  ..".3..%.{...K..
-00002f00: f2b7 e23c e177 1f9b 3e13 94fd 327d cc5f  ...<.w..>...2}._
-00002f10: 731e f92f 35b2 b816 23b7 ff69 e4cd fbe6  s../5...#..i....
-00002f20: af6f 5eb7 6656 6937 1a90 fd0b b7fa 0050  .o^.fVi7.......P
-00002f30: 4b01 0214 0314 0000 0008 0025 57f5 5646  K..........%W.VF
-00002f40: 5ac1 0c82 0000 00b1 0000 0010 0000 0000  Z...............
-00002f50: 0000 0000 0000 0080 0100 0000 0064 6f63  .............doc
-00002f60: 5072 6f70 732f 6170 702e 786d 6c50 4b01  Props/app.xmlPK.
-00002f70: 0214 0314 0000 0008 0025 57f5 5685 4724  .........%W.V.G$
-00002f80: e6ea 0000 00cb 0100 0011 0000 0000 0000  ................
-00002f90: 0000 0000 0080 01b0 0000 0064 6f63 5072  ...........docPr
-00002fa0: 6f70 732f 636f 7265 2e78 6d6c 504b 0102  ops/core.xmlPK..
-00002fb0: 1403 1400 0000 0800 2557 f556 995c 9c23  ........%W.V.\.#
-00002fc0: 1006 0000 9c27 0000 1300 0000 0000 0000  .....'..........
-00002fd0: 0000 0000 8001 c901 0000 786c 2f74 6865  ..........xl/the
-00002fe0: 6d65 2f74 6865 6d65 312e 786d 6c50 4b01  me/theme1.xmlPK.
-00002ff0: 0214 0314 0000 0008 0025 57f5 56e0 d96c  .........%W.V..l
-00003000: 243d 0200 00a3 0700 0018 0000 0000 0000  $=..............
-00003010: 0000 0000 0080 810a 0800 0078 6c2f 776f  ...........xl/wo
-00003020: 726b 7368 6565 7473 2f73 6865 6574 312e  rksheets/sheet1.
-00003030: 786d 6c50 4b01 0214 0314 0000 0008 0025  xmlPK..........%
-00003040: 57f5 5619 c663 fc00 0e00 00bb 8300 0018  W.V..c..........
-00003050: 0000 0000 0000 0000 0000 0080 817d 0a00  .............}..
-00003060: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00003070: 6865 6574 322e 786d 6c50 4b01 0214 0314  heet2.xmlPK.....
-00003080: 0000 0008 0025 57f5 568d 2e97 f3c3 0e00  .....%W.V.......
-00003090: 006f 8b00 0018 0000 0000 0000 0000 0000  .o..............
-000030a0: 0080 81b3 1800 0078 6c2f 776f 726b 7368  .......xl/worksh
-000030b0: 6565 7473 2f73 6865 6574 332e 786d 6c50  eets/sheet3.xmlP
-000030c0: 4b01 0214 0314 0000 0008 0025 57f5 56f7  K..........%W.V.
-000030d0: f68f 09a7 0200 006d 0b00 000d 0000 0000  .......m........
-000030e0: 0000 0000 0000 0080 01ac 2700 0078 6c2f  ..........'..xl/
-000030f0: 7374 796c 6573 2e78 6d6c 504b 0102 1403  styles.xmlPK....
-00003100: 1400 0000 0800 2557 f556 b747 eb8a c000  ......%W.V.G....
-00003110: 0000 1602 0000 0b00 0000 0000 0000 0000  ................
-00003120: 0000 8001 7e2a 0000 5f72 656c 732f 2e72  ....~*.._rels/.r
-00003130: 656c 7350 4b01 0214 0314 0000 0008 0025  elsPK..........%
-00003140: 57f5 56b9 489c 7652 0100 00ae 0200 000f  W.V.H.vR........
-00003150: 0000 0000 0000 0000 0000 0080 0167 2b00  .............g+.
-00003160: 0078 6c2f 776f 726b 626f 6f6b 2e78 6d6c  .xl/workbook.xml
-00003170: 504b 0102 1403 1400 0000 0800 2557 f556  PK..........%W.V
-00003180: 0b08 5d06 bc00 0000 1f03 0000 1a00 0000  ..].............
-00003190: 0000 0000 0000 0000 8001 e62c 0000 786c  ...........,..xl
-000031a0: 2f5f 7265 6c73 2f77 6f72 6b62 6f6f 6b2e  /_rels/workbook.
-000031b0: 786d 6c2e 7265 6c73 504b 0102 1403 1400  xml.relsPK......
-000031c0: 0000 0800 2557 f556 dbfb ce8f 2401 0000  ....%W.V....$...
-000031d0: e904 0000 1300 0000 0000 0000 0000 0000  ................
-000031e0: 8001 da2d 0000 5b43 6f6e 7465 6e74 5f54  ...-..[Content_T
-000031f0: 7970 6573 5d2e 786d 6c50 4b05 0600 0000  ypes].xmlPK.....
-00003200: 000b 000b 00ca 0200 002f 2f00 0000 00    .........//....
+000000b0: 504b 0304 1400 0000 0800 6050 f856 db74  PK........`P.V.t
+000000c0: 89e1 ec00 0000 cb01 0000 1100 0000 646f  ..............do
+000000d0: 6350 726f 7073 2f63 6f72 652e 786d 6c95  cProps/core.xml.
+000000e0: 91c1 4ec3 300c 865f 65ca bd75 da22 90a2  ..N.0.._e..u."..
+000000f0: 2e97 214e 2021 3109 c42d 4abc 2da2 69a2  ..!N !1..-J.-.i.
+00000100: c4a8 dddb 9396 ad1b 820b c7f8 fffc d956  ...............V
+00000110: 5a1d 84f6 119f a30f 18c9 625a 8dae eb93  Z.........bZ....
+00000120: d061 cd0e 4441 0024 7d40 a752 9989 3e87  .a..DA.$}@.R..>.
+00000130: 3b1f 9da2 fc8c 7b08 4a7f a83d 42cd f92d  ;.....{.J..=B..-
+00000140: 3824 6514 2998 8445 588c eca4 347a 5186  8$e.)..EX...4zQ.
+00000150: cfd8 cd02 a301 3b74 d853 82aa ace0 c212  ......;t.S......
+00000160: 4697 fe6c 9893 851c 935d a861 18ca a199  F..l.....].a....
+00000170: b9bc 5105 6f4f 8f2f f3f2 85ed 13a9 5e23  ..Q.oO./......^#
+00000180: 93ad d142 4754 e4a3 9c2e 0ac7 b16b e1aa  ...BGT.......k..
+00000190: d89e 667f 17d0 acf2 0441 c780 6b76 4e5e  ..f......A..kvN^
+000001a0: 9bcd fdf6 81c9 9ad7 4dc1 ef8a fa66 5b71  ........M....f[q
+000001b0: c11b c1f9 fbe4 fad1 7f11 3a6f ecce fed3  ..........:o....
+000001c0: 585d 19cf 02d9 c2af 7f93 5f50 4b03 0414  X]........_PK...
+000001d0: 0000 0008 0060 50f8 5699 5c9c 2310 0600  .....`P.V.\.#...
+000001e0: 009c 2700 0013 0000 0078 6c2f 7468 656d  ..'......xl/them
+000001f0: 652f 7468 656d 6531 2e78 6d6c ed5a 5b73  e/theme1.xml.Z[s
+00000200: da38 147e efaf d078 67f6 6d0b c636 81b6  .8.~...xg.m..6..
+00000210: b413 7369 76db b499 84ed 4e1f 8511 588d  ..siv.....N...X.
+00000220: 6c79 6491 847f bf47 3610 cb96 0ded 924d  lyd....G6......M
+00000230: ba9b 3c04 2ce9 fbce 4547 e7e8 3879 f3ee  ..<.,...EG..8y..
+00000240: 2e62 e886 8894 f278 60d9 2fdb d6bb b72f  .b.....x`./..../
+00000250: dee0 5732 2411 4130 19a7 aff0 c00a a54c  ..W2$.A0.......L
+00000260: 5eb5 5a69 00c3 387d c913 12c3 dc82 8b08  ^.Zi..8}........
+00000270: 4b78 14cb d65c e05b 1a2f 23d6 eab4 dbdd  Kx...\.[./#.....
+00000280: 5684 696c a118 4764 607d 5e2c 6840 d054  V.il..Gd`}^,h@.T
+00000290: 515a 6f5f 20b4 e51f 33f8 15cb 548d 65a3  QZo_ ...3...T.e.
+000002a0: 0113 5741 26b9 88b4 f2f9 6cc5 fcda de3e  ..WA&.....l....>
+000002b0: 65cf e93a 1d32 816e 301b 5820 7fce 6fa7  e..:.2.n0.X ..o.
+000002c0: e44e 5a88 e154 c2c4 c06a 673f 566b c7d1  .NZ..T...jg?Vk..
+000002d0: d248 8082 c97d 9405 ba49 f6a3 d315 0832  .H...}...I.....2
+000002e0: 0d3b 3a9d 58ce 767c f6c4 ed9f 8cca da74  .;:.X.v|.......t
+000002f0: 346d 1ae0 e3f1 7838 b6cb d28b 701c 04e0  4m....x8....p...
+00000300: 51bb 9ec2 9df4 6cbf a441 09b4 a369 d064  Q.....l..A...i.d
+00000310: d8f6 daae 91a6 aa8d 534f d3f7 7ddf eb9b  ........SO..}...
+00000320: 689c 0a8d 5b4f d36b 77dd d38e 89c6 add0  h...[O.kw.......
+00000330: 780d bef1 4f87 c3ae 89c6 abd0 74eb 6926  x...O.......t.i&
+00000340: 27fd ae6b a4e9 1668 4246 e3eb 7a12 15b5  '..k...hBF..z...
+00000350: e540 d320 0058 7076 d6cc d203 965e 29fa  .@. .Xpv.....^).
+00000360: 7594 1ad9 1dbb dd41 5cf0 58ee 3989 11fe  u......A\.X.9...
+00000370: c6c5 04d6 69d2 1996 3446 729d 9005 0e00  ....i...4Fr.....
+00000380: 37c4 d14c 507c af41 b68a e0c2 92d2 5c90  7..LP|.A......\.
+00000390: d6cf 29b5 501a 089a c881 f547 8221 c5dc  ..).P......G.!..
+000003a0: affd f597 bbc9 a433 7a9d 7d3a ce6b 947f  .......3z.}:.k..
+000003b0: 69ab 01a7 edbb 9bcf 93fc 73e8 e49f a793  i.........s.....
+000003c0: d74d 42ce 70bc 2c09 f1fb 235b 6187 276e  .MB.p.,...#[a.'n
+000003d0: 3b13 723a 1c67 427c cff6 f691 a525 32cf  ;.r:.gB|.....%2.
+000003e0: eff9 0aeb 4e3c 671f 5696 b05d cfcf e49e  ....N<g.V..]....
+000003f0: 8c72 23bb ddf6 587d f64f 476e 23d7 a9c0  .r#...X}.OGn#...
+00000400: b322 d794 4624 459f c82d bae4 1138 b549  ."..F$E..-...8.I
+00000410: 0d32 133f 089d 8698 6a50 1c02 a409 3196  .2.?....jP....1.
+00000420: a186 f8b4 c6ac 11e0 137d b7be 08c8 df8d  .........}......
+00000430: 88f7 ab6f 9a3d 57a1 5849 da84 f810 461a  ...o.=W.XI....F.
+00000440: e29c 73e6 73d1 6cfb 07a5 46d1 f655 bcdc  ..s.s.l...F..U..
+00000450: a397 5815 0197 18df 34aa 352c c5d6 7895  ..X.....4.5,..x.
+00000460: c0f1 ad9c 3c1d 1312 cd94 0b06 4186 9724  ....<.......A..$
+00000470: 2612 a939 7e4d 4813 fe2b a5da fe9c d340  &..9~MH..+.....@
+00000480: f094 2f24 fa4a 918f 69b3 23a7 7426 cde8  ../$.J..i.#.t&..
+00000490: 331a c146 af1b 7587 68d2 3c7a fe05 f99c  3..F..u.h.<z....
+000004a0: 350a 1c91 1b1d 0267 1bb3 4621 8469 bbf0  5......g..F!.i..
+000004b0: 1eaf 248e 9aad c211 2b42 3e62 1936 1a72  ..$.....+B>b.6.r
+000004c0: b516 81b6 71a9 8460 5a12 c6d1 784e d2b4  ....q..`Z...xN..
+000004d0: 11fc 59ac 3593 3e60 c8ec cd91 75ce d691  ..Y.5.>`....u...
+000004e0: 0e11 925e 3742 3e62 ce8b 9011 bf1e 8638  ...^7B>b.......8
+000004f0: 4a9a eda2 7158 04fd 9e5e c349 c1e8 82cb  J...qX...^.I....
+00000500: 66fd b87e 86d5 336c 2c8e f747 d417 4ae4  f..~..3l,..G..J.
+00000510: 0f26 a73f e932 3407 a39a 5909 bd84 566a  .&.?.24...Y...Vj
+00000520: 9faa 8734 3ea8 1e32 0a05 f1b9 1e3e e57a  ...4>..2.....>.z
+00000530: 780a 3796 c6bc 50ae 827b 01ff d1da 37c2  x.7...P..{....7.
+00000540: abf8 82c0 397f 2e7d cfa5 efb9 f43d a1d2  ....9..}.....=..
+00000550: b737 237d 67c1 d38b 5bde 466e 5bc4 fbae  .7#}g...[.Fn[...
+00000560: 31da d734 2e28 6357 72cd c8c7 54af 9329  1..4.(cWr...T..)
+00000570: d839 9fc0 ecfd 683e 9ef1 edfa d924 84af  .9....h>.....$..
+00000580: 9a59 2d23 1690 4b81 b341 24b8 fc8b caf0  .Y-#..K..A$.....
+00000590: 2ac4 09e8 645b 2509 cb54 d365 378a 129e  *...d[%..T.e7...
+000005a0: 421b 6ee9 53f5 4a95 d7e5 afb9 28b8 3c5b  B.n.S.J.....(.<[
+000005b0: e4e9 afa1 743e 2ccf f93c 5fe7 b4cd 0b33  ....t>,..<_....3
+000005c0: 43b7 724b eab6 94be b526 384a f4b1 cc70  C.rK.....&8J...p
+000005d0: 4e1e cb0c 3b67 3c92 1db6 77a0 1d35 fbf6  N...;g<...w..5..
+000005e0: 5d76 e423 a530 5397 43b8 1a42 be03 6dba  ]v.#.0S.C..B..m.
+000005f0: 9ddc 3a38 9e98 91b9 0ad3 5290 6fc3 f9e9  ..:8......R.o...
+00000600: c578 1ae2 39d9 04b9 7d98 576d e7d8 d1d1  .x..9...}.Wm....
+00000610: fbe7 c151 b0a3 ef3c 961d c788 f2a2 21ee  ...Q...<......!.
+00000620: a186 98cf c343 8779 7b5f 9867 95c6 5034  .....C.y{_.g..P4
+00000630: 146d 6cac 242c 46b7 60b8 d7f1 2c14 e064  .ml.$,F.`...,..d
+00000640: 602d a007 83af 5102 f252 5560 315b c603  `-....Q..RU`1[..
+00000650: 2b90 a27c 4c8c 45e8 70e7 975c 5fe3 d192  +..|L.E.p..\_...
+00000660: e3db a665 b56e af29 7719 6d22 5239 c269  ...e.n.)w.m"R9.i
+00000670: 9813 67ab cade 65b1 c155 1dcf 555b f2b0  ..g...e..U..U[..
+00000680: be6a 3db4 154e cffe 59ad c89f 0c11 4e16  .j=..N..Y.....N.
+00000690: 0b12 4863 9417 a64a a2f3 1953 bee7 2b49  ..Hc...J...S..+I
+000006a0: c455 38bf 4533 b612 9718 bce3 e6c7 714e  .U8.E3........qN
+000006b0: 53b8 1276 b60f 0232 b9bb 39a9 7a65 3167  S..v...2..9.ze1g
+000006c0: a6f2 df2d 0c09 2c5b 8859 12e2 4d5d edd5  ...-..,[.Y..M]..
+000006d0: e79b 9cae 7a22 76fa 9777 c160 f2fd 70c9  ....z"v..w.`..p.
+000006e0: 470f e53b e75f f45d 43ae 7ef6 dde3 fa6e  G..;._.]C.~....n
+000006f0: 933b 484c 9c79 c511 0174 4502 2395 1c06  .;HL.y...tE.#...
+00000700: 1617 32e4 50ee 9290 0613 01cd 94c9 44f0  ..2.P.........D.
+00000710: 0282 64a6 1c80 98fa 0bbd f20c b929 15ce  ..d..........)..
+00000720: ad3e 397f 452c 8386 4e5e d225 1214 8ab0  .>9.E,..N^.%....
+00000730: 0c05 2117 72e3 efef 936a 778c d7fa 2c81  ..!.r....jw...,.
+00000740: 6d84 5432 64d5 17ca 4389 c13d 3372 43d8  m.T2d...C..=3rC.
+00000750: 5425 f3ae da26 0b85 dbe2 54cd bb1a be26  T%...&....T....&
+00000760: 604b c37a 6e9d 2d27 ffdb 5ed4 3db4 173d  `K.zn.-'..^.=..=
+00000770: 46f3 a399 e01e b387 739b 7ab8 c245 acff  F.......s.z..E..
+00000780: 58d6 1ef9 32df 3970 db3a de03 5ee6 132c  X...2.9p.:..^..,
+00000790: 43a4 7ec1 7d8a 8a80 11ab 62be baaf 4ff9  C.~.}.....b...O.
+000007a0: 259c 3bb4 7bf1 8120 9bfc d6db a4f6 dde0  %.;.{.. ........
+000007b0: 0c7c d4ab 5aa5 642b 113f 4b07 7c1f 9206  .|..Z.d+.?K.|...
+000007c0: 638c 5bf4 345f 8f14 62ad a6b1 adc6 da31  c.[.4_..b......1
+000007d0: 0c79 8058 f30c a166 38df 8745 9a1a 33d5  .y.X...f8..E..3.
+000007e0: 8bac 398d 0a6f 41d5 40e5 3fdb d40d 68f6  ..9..oA.@.?...h.
+000007f0: 0d34 1c91 055e 3199 b636 a3e4 4e0a 3cdc  .4...^1..6..N.<.
+00000800: feef 0db0 c2c4 8ee1 ed8b bf01 504b 0304  ............PK..
+00000810: 1400 0000 0800 6050 f856 e0d9 6c24 3d02  ......`P.V..l$=.
+00000820: 0000 a307 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
+00000830: 6b73 6865 6574 732f 7368 6565 7431 2e78  ksheets/sheet1.x
+00000840: 6d6c 8595 db72 9b30 1086 5f85 e101 2ce3  ml...r.0.._...,.
+00000850: b333 9899 da9d 4e7b 914e 269e 26d7 322c  .3....N{.N&.&.2,
+00000860: b6c6 42a2 d262 d2b7 afa4 38b2 9b82 b842  ..B..b....8....B
+00000870: a7dd 6f0f e257 da4a 75d6 2700 8cde 2a2e  ..o..W.Ju.'...*.
+00000880: f426 3e21 d60f 84e8 fc04 15d5 2359 8330  .&>!........#Y.0
+00000890: 3ba5 5415 4533 5547 a26b 05b4 7046 1527  ;.T.E3UG.k..pF.'
+000008a0: 93f1 7841 2aca 449c a56e ed49 65a9 6c90  ..xA*.D..n.Ie.l.
+000008b0: 3301 4f2a d24d 5551 f567 0b5c b69b 3889  3.O*.MUQ.g.\..8.
+000008c0: 3f16 9ed9 f184 6e81 6469 4d8f b007 fc55  ?.....n.diM....U
+000008d0: 1b03 3325 de4f c12a 109a 4911 2928 37f1  ..3%.O.*..I.)(7.
+000008e0: 97e4 619b cc9c 893b f2c2 a0d5 77e3 c866  ..a....;....w..f
+000008f0: 7390 f26c 273f 8a4d 3cb6 4101 871c ad0f  s..l'?.M<.A.....
+00000900: 6a3e 17d8 01e7 d695 09e5 f7d5 6b7c a35a  j>..........k|.Z
+00000910: cbfb f187 fb6f ae00 26be 03d5 b093 fc95  .....o..&.......
+00000920: 1578 dac4 ab38 2aa0 a40d c767 d97e 876b  .x...8*....g.~.k
+00000930: 52f3 5b88 5f29 d22c 55b2 8d94 cd36 4b73  R.[._).,U....6Ks
+00000940: 3b70 7497 bd39 ce84 add5 1e95 d965 8687  ;pt..9.......e..
+00000950: 99a0 15e8 9ae6 9012 34c1 d845 925f 4db7  ........4..E._M.
+00000960: 7d46 b671 da74 ee7c 1ce5 f228 18c2 8832  }F.q.t.|...(...2
+00000970: d232 5190 7fdd 1013 8d0f 69e2 439a 0443  .2Q.......i.C..C
+00000980: 323d 2fd9 5b57 3c93 4f16 ae96 f788 a947  2=/.[W<.O......G
+00000990: 4c83 88c2 94ea 5116 c07f 9af4 bb48 d321  L.....Q......H.!
+000009a0: d2cc 9366 4152 5e94 7b5b de3e d06c 0834  ...fAR^.{[.>.l.4
+000009b0: f7a0 7910 7401 656f 6f17 633e c458 78c6  ..y.t.eoo.c>.Xx.
+000009c0: 22c8 607a d728 0502 5ffa 610b 677b 3036  ".`z.(.._.a.g{06
+000009d0: 972c 49c9 a5e3 222c 3d6e 19ae 9df9 f911  .,I...",=n......
+000009e0: 8a2e ca72 28a5 9567 ac82 8ca6 2efa 18ab  ...r(..g........
+000009f0: 21c6 da33 d641 0632 e49d cd5f 0f11 92f1  !..3.A.2..._....
+00000a00: ed37 1e87 6f34 e85c b11a 7bba 62ad 0750  .7..o4.\..{.b..P
+00000a10: 778a 1196 0cd7 16a9 3a31 9f6d fec7 dc54  w.......:1.m...T
+00000a20: 2009 cb40 2e05 2a76 68fa 5083 6290 dcd4   ..@..*vh.P.b...
+00000a30: 2009 cb81 b262 aa3b 2983 4290 dc94 2009   ....b.;).B... .
+00000a40: 4b01 67b9 7961 ba85 b65f 06c8 9db6 dbc7  K.g.ya..._......
+00000a50: eb91 aa23 133a e250 1a8b f168 69fe 6ef5  ...#.:.P...hi.n.
+00000a60: fe18 bc4f 50d6 2e86 8344 9495 1b9e cc23  ...OP....D.....#
+00000a70: 0aca 1e30 fba5 94e8 2716 e3df e5ec 2f50  ...0....'...../P
+00000a80: 4b03 0414 0000 0008 0060 50f8 5619 c663  K........`P.V..c
+00000a90: fc00 0e00 00bb 8300 0018 0000 0078 6c2f  .............xl/
+00000aa0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00000ab0: 322e 786d 6cad 9ddb 72da 4817 855f 85f2  2.xml...r.H.._..
+00000ac0: 0304 734c 66ca 71d5 60a1 ee74 2687 8a33  ..sLf.q.`..t&..3
+00000ad0: 99aa ff4e 8636 a822 2422 449c ccd3 ff12  ...N.6."$"D.....
+00000ae0: 8969 d9ea 4f4d cbbe 4acc 621f b417 12e2  .i..OM..J.b.....
+00000af0: 43b4 2eee b2fc eb6e ad75 d1fb b149 d2dd  C......n.u...I..
+00000b00: ebb3 7551 6cff ecf7 778b b5de 44bb 17d9  ..uQl...w...D...
+00000b10: 56a7 a572 9be5 9ba8 28ff cc57 fddd 36d7  V..r....(..W..6.
+00000b20: d1f2 10b4 49fa c3f3 f369 7f13 c5e9 d9e5  ....I....i......
+00000b30: c5e1 b18f f9e5 45b6 2f92 38d5 1ff3 de6e  ......E./.8....n
+00000b40: bfd9 44f9 cf99 4eb2 bbd7 6783 b3fb 073e  ..D...N...g....>
+00000b50: c5ab 7571 78a0 7f79 b18d 56fa 5a17 ff6c  ..uqx..y..V.Z..l
+00000b60: cb80 f2cf fe31 cf32 dee8 7417 6769 2fd7  .....1.2..t.gi/.
+00000b70: b7af cffe 1afc f9f6 e5f9 21e4 f094 2fb1  ..........!.../.
+00000b80: bedb d5fe dfab b6e6 26cb be56 7fbc 59be  ........&..V..Y.
+00000b90: 3e3b af9a d289 5e14 558e a8fc e7bb bed2  >;....^.U.......
+00000ba0: 4952 a52a 5bf9 f63b eb99 a95a 45d6 ff7f  IR.*[..;...ZE...
+00000bb0: 9f3e 3c0c a0ec ef26 dae9 ab2c f937 5e16  .><....&...,.7^.
+00000bc0: ebd7 67af ce7a 4b7d 1bed 93e2 5376 27f5  ..g..zK}....Sv'.
+00000bd0: ef8d 9a98 1683 a888 2e2f f2ec ae97 575b  ........./....W[
+00000be0: 7b79 b1a8 fe53 952c 9f18 a7d5 94ae 8bbc  {y...S.,........
+00000bf0: 7c3c 2e2b 1597 d5d3 7bef b2a5 4e7a 81be  |<.+....{...Nz..
+00000c00: 8dd3 b86a fca2 5f94 2d55 4fe8 2f7e 2798  ...j.._.-UO./~'.
+00000c10: 3d4e 5015 3c28 57a8 04a8 cca9 9deb 222a  =NP.<(W......."*
+00000c20: b4a5 7c88 a904 2a92 8abc 4db3 bb44 2f57  ..|...*...M..D/W
+00000c30: ba34 e8db 3ede 1db6 b997 642b 4be1 3798  .4..>.....d+K.7.
+00000c40: 5ea1 f2d6 a6f4 4b4b 8ebe 0c8f be0c a1c7  ^.....KK........
+00000c50: ab24 daed 6c3e 50c0 fb68 631b dc15 3d3f  .$..l>P..hc...=?
+00000c60: d0bb 451e 6fc1 ee80 c23e 46b9 4e8b 1eb5  ..E.o....>F.N...
+00000c70: 37e7 72e5 4ebc 28cd 5dda dc75 4555 fe04  7.r.N.(.]..uEU..
+00000c80: f657 86a0 d84f 7a9b 440b bdec cd7e 5ac2  .W...Oz.D....~Z.
+00000c90: 2485 5d67 fb7c 612b f4a6 3da2 374f 8bb8  $.]g.|a+..=.7O..
+00000ca0: f8d9 031f 1445 bf8b 8ac5 da12 f016 5f19  .....E........_.
+00000cb0: d9a6 3c46 150f 431e bcba 46c7 57d7 0872  ..<F..C...F.W..r
+00000cc0: 8c82 c32e 6f7b 7d3d 0e31 fb39 2a01 95a9  ....o{}=.1.9*...
+00000cd0: 0e2e d745 9697 47db 4f7a 7718 d3e7 9f5b  ...E..G.Ozw....[
+00000ce0: db78 e698 3c44 45a0 22a9 a1ea bd66 57be  .x..<DE."....fW.
+00000cf0: d97c 5dbd 5864 abf2 60a7 5f44 71ff 2e4e  .|].Xd..`._Dq..N
+00000d00: 977d 9be3 fee3 5314 a27f 946f 0636 9b6d  .}....S....o.6.m
+00000d10: 1bf1 c0cd f1d1 cd31 e4fe 4be7 7164 35f3  .......1..K.qd5.
+00000d20: 7184 3113 9580 aabc 4977 4594 2487 9d91  q.1.....IwE.$...
+00000d30: 5cc4 ac21 2a02 1549 9d78 bae8 3d36 4511  \..!*..I.x..=6E.
+00000d40: 68a2 6d1b 1e98 3839 9a38 a16e 763b 6dcb  h.m...89.8.nv;m.
+00000d50: 3d7b 1c60 3c44 25a0 221e 3b24 260f 5111  ={.`<D%.".;$&.Q.
+00000d60: a848 6ac8 d34a dfe1 290a 4027 6d9b f0c0  .Hj..J..).@'m...
+00000d70: c9e9 d1c9 2935 f323 dec1 5467 8f63 8c99  ....)5.#..Tg.c..
+00000d80: a804 54e7 df72 4a9f f7f9 4df9 f0d5 3aca  ..T..rJ...M...:.
+00000d90: cb0d 2a5f d0bb 225e d8ec c4f4 212a 0215  ..*_.."^....!*..
+00000da0: 492d 79da d961 828a 62d0 51db 563c 70f4  I-y..a..b.Q.V<p.
+00000db0: e5d1 d197 f496 1b84 d59e 83ef 992d 713d  .............-q=
+00000dc0: 7382 6d3b 3b7b 1c69 5c47 658e 4a88 8a40  s.m;;{.i\Ge.J..@
+00000dd0: 4552 ef9e 5676 1c9d a238 b4d3 b625 0fec  ER..Vv...8...%..
+00000de0: 7c75 b4f3 159e 4155 6f65 8f4f a17e 59f9  |u....AUoe.O.~Y.
+00000df0: 38c6 eca0 a804 54e7 4b54 bec1 dc24 fabe  8.....T.KT...$..
+00000e00: de3f e514 6dfb 2666 0e51 11a8 48ea c6d3  .?..m.&f.Q..H...
+00000e10: d00e c353 1483 66da b6e2 8199 7f1c cdfc  ...S..f.........
+00000e20: 83fa 29ae f6f9 77eb c1f6 7188 f112 9580  ..)...w...q.....
+00000e30: ca54 2fe2 8f79 b6dc 2f0a ebe7 1ecc 18a2  .T/..y../.......
+00000e40: 2250 91d4 85a7 87fe 3353 1482 16da 36e2  "P......3S....6.
+00000e50: 8185 8373 0321 ce5b a6fb 215f 4569 fcdf  ...s.!.[..!_Ei..
+00000e60: e1fc d271 7232 6b24 aad1 0894 022c ef3a  ...qr2k$.....,.:
+00000e70: 17e2 9c21 4b82 2589 9d78 1afc 5c03 5598  ...!K.%..x..\.U.
+00000e80: 087d b76e dd43 e36b f4a9 0d3f b5ec 56b3  .}.n.C.k...?..V.
+00000e90: 4660 cde8 16ee 44e5 aa53 a679 aaf3 d5cf  F`....D..S.y....
+00000ea0: 2303 1279 b4b5 7dfe 9e73 fe90 25c1 92c4  #..y..}..s..%...
+00000eb0: ae7c 4def 384c 8581 6cb2 9364 0d0c ca1a  .|M.8L..l..d....
+00000ec0: 20c5 a93e 75d8 3fdc 3462 6afe a214 b456   ..>u.?.4bj....V
+00000ed0: f278 d9cf b946 c892 6049 6267 be1e fbcf  .x...F..`Ibg....
+00000ee0: 5261 0cdb 6bdb 9087 f61a 9634 783a e599  Ra..k......4x:..
+00000ef0: 3572 d4ec 66bc 8495 9df6 3255 6249 b024  5r..f.....2UbI.$
+00000f00: b113 5f7b 9f3e 4b85 39d8 6e27 6b1a 18d8  .._{.>K.9.n'k...
+00000f10: 3420 0812 6477 6975 1cb5 facb c089 a500  4 ..dwiu........
+00000f20: 4b7d caca 517c c863 9d16 1180 ea39 e70d  K}..Q|.c.....9..
+00000f30: 5912 2c49 ecc6 d7e3 0e03 5418 c4a6 3ad9  Y.,I......T...:.
+00000f40: d3c0 c0a7 01f1 90f9 f706 52fe ed28 e327  ..........R..(.'
+00000f50: 9602 ace3 01a0 387d c892 6049 6253 bec6  ......8}..`IbS..
+00000f60: fa0e 5161 04bb eae4 5003 03a2 06c4 44e6  ..Qa....P.....D.
+00000f70: 3f16 c9be fa36 f37f 596a 3f1e 338f 6229  ?....6..Yj?.3.b)
+00000f80: c07a 5066 ceb9 4296 044b 123b f0b5 b2eb  .zPf..B..K.;....
+00000f90: e414 46b2 a54e 1035 3024 6a40 5c24 8c13  ..F..N.50$j@\$..
+00000fa0: bb93 4878 ae58 0ab0 8ccf 7eca 3c8a 25c1  ..Hx.X....~.<.%.
+00000fb0: 92c4 a67c cdf5 9ca1 c200 f6d4 49a3 0606  ...|........I...
+00000fc0: 470d 088f 84f1 0feb d7a2 b346 44cd 54c6  G..........FD.T.
+00000fd0: 5158 e77a bfdd 6679 513e 547e 42d8 e7ec  QX.z..fyQ>T~B...
+00000fe0: 2803 2996 044b 123b f275 d477 820a 23d8  (.)..K.;.u.w..#.
+00000ff0: 5227 931a 1828 3520 5c12 2659 79c6 92da  R'...(5 \.&Yy...
+00001000: ae28 9835 826a ae32 98c2 5227 bbca 888a  .(.5.j.2..R'....
+00001010: 25c1 92c4 8e7c 5ded 3044 8541 6cac 9354  %....|].0D.Al..T
+00001020: 0d0d a91a 120f 9159 1eff 9795 e7a3 49f5  .......Y......I.
+00001030: 2585 f502 0d66 532c 0558 b0e5 bb90 39e7  %....fS,.X....9.
+00001040: 0b59 122c 49ec c2d3 d2ee e353 188a c65a  .Y.,I......S...Z
+00001050: b7e7 a1b1 8644 0d89 81bc 995f f135 374c  .....D....._.57L
+00001060: a158 0ab0 94d7 1777 5c20 6449 b024 b12d  .X.....w\ dI.$.-
+00001070: 5f8f 3b4c 5261 10bb ebbe 98aa 7635 1521  _.;LRa......v5.!
+00001080: 90fb 9e5e bcb1 facb 148a a5c0 59cc 6a27  ...^........Y.j'
+00001090: 1327 9604 4b12 bbf0 b5b3 d3e8 1486 b1a1  .'..K...........
+000010a0: 4ee8 3434 d069 4890 c374 6577 9441 134b  N.44.iH..tew.A.K
+000010b0: 81b3 9ad5 5186 4c2c 0996 2476 e1eb 68b7  ....Q.L,..$v..h.
+000010c0: d929 8c63 4b9d 6069 68c0 d210 2f30 326d  .).cK.`ih.../02m
+000010d0: d93d 65b8 c452 e02c 67f5 94a1 124b 8225  .=e..R.,g....K.%
+000010e0: 895d f87a da71 780a 03d9 5427 581a 1ab0  .].z.qx...T'X...
+000010f0: 3424 c251 ef2b b2ba ca80 89a5 e0a4 7a56  4$.Q.+........zV
+00001100: 6799 2ab1 2458 92d8 89af b35d 27a8 3092  g.*.$X.....]'.0.
+00001110: ad75 d2a5 a1a1 4b43 221d f5c6 6eac d632  .u....KC"...n..2
+00001120: 5d62 2938 a99e d55a a64c 2c09 9624 76e2  ]b)8...Z.L,..$v.
+00001130: 6b6d d709 2a8c 646b 9d94 6968 28d3 9080  km..*.dk..ih(...
+00001140: 47ad 31fb 4ecb b489 a5e0 9472 5663 9930  G.1.N......rVc.0
+00001150: b124 5892 d888 afb1 1de7 a730 907d 7592  .$X........0.}u.
+00001160: a6a1 214d 43a2 1eb5 beec 7b2c 0327 9682  ..!MC.....{,.'..
+00001170: 53ca 597d 65ce c492 6049 6223 bebe 769c  S.Y}e...`Ib#..v.
+00001180: 9fc2 40f6 d589 9b86 0637 0d09 7a98 bebe  ..@......7..z...
+00001190: 586d 65e2 c452 e0ac 66f5 9429 134b 8225  Xme..R..f..).K.%
+000011a0: 895d f87a da6d 760a e3d8 5227 681a 19d0  .].z.mv...R'h...
+000011b0: 3422 dc61 dab2 1e81 1b71 c652 9682 13aa  4".a.....q.R....
+000011c0: d94c e58c 214b 8225 897d f8fe 40a3 dbf4  .L..!K.%.}..@...
+000011d0: 14c6 f1cf 349c 9069 6420 d3c8 8546 5ed8  ....4..id ...F^.
+000011e0: 0fbf 8db8 9aa9 cc99 4ea8 6635 95c1 124b  ........N.f5...K
+000011f0: 8225 897d f89a da6d 7a0a e3d8 5427 5b1a  .%.}...mz...T'[.
+00001200: 19b6 3442 4092 3abe 656d 44d6 6c65 bc84  ..4B@.:.emD.le..
+00001210: f5e8 5b56 ce15 b224 5892 d881 afa1 5d27  ..[V...$X.....]'
+00001220: a730 922d 75d2 a551 ede7 7148 48dc bf75  .0.-u..Q..qHH..u
+00001230: 9a35 826b aeb6 fc54 8e4a 7a41 612e 10b2  .5.k...T.JzAa...
+00001240: 2458 92d8 96af d54f 98a8 c260 76db 099e  $X.....O...`v...
+00001250: 4606 3c8d 0881 fc1d ddc0 6f21 9938 b114  F.<.......o!.8..
+00001260: 601d dfab 13b9 46c8 9260 4962 67be 2efb  `.....F..`Ibg...
+00001270: 4e52 6104 5beb c44f 2383 9f46 8440 fe8e  NRa.[..O#..F.@..
+00001280: d2e5 22fb ae73 abbd 8c9e 580a b096 eb27  .."..s....X....'
+00001290: 029c 3364 49b0 24b1 135f 3bbb 4c4f 6114  ..3dI.$.._;.LOa.
+000012a0: 5bea c44e 2383 9d46 843e de65 6976 b830  [..N#..F.>.eiv.0
+000012b0: d06a 2923 2796 02ac 75a8 83bb 27f3 2696  .j)#'...u...'.&.
+000012c0: 044b 12db f0f5 b3cb e814 46b1 9f4e d634  .K........F..N.4
+000012d0: 32ac 6944 c8e3 dd3e 2962 3694 4913 4b01  2.iD...>)b6.I.K.
+000012e0: 166b 3794 3913 4b82 2589 6df8 1ada 6976  .k7.9.K.%.m...iv
+000012f0: 0ac3 d851 2765 1a19 ca34 22d8 f13e a36b  ...Q'e...4"..>.k
+00001300: 231a 2135 3799 2f61 a1b6 6b23 385f c892  #.!57./a..k#8_..
+00001310: 6049 6217 be66 7a8f 4d61 081b e9c4 4a23  `Ib..fz.Ma....J#
+00001320: 8395 4684 38de 67ed 175f cf1a 9135 3f19  ..F.8.g.._...5?.
+00001330: 2c61 bd53 aef7 e6bc 214b 8225 89dd f8fa  ,a.S....!K.%....
+00001340: da75 8a0a 23d9 5e27 621a 1bc4 3426 d8f1  .u..#.^'b...4&..
+00001350: 3e8b 771a 7f3d d908 33de b214 6031 d7d9  >.w..=..3...`1..
+00001360: 11e7 0c59 122c 49ec c477 f988 4ee3 5318  ...Y.,I..w..N.S.
+00001370: c68b 4838 11d3 d820 a631 c18e f759 3a4b  ..H8... .1...Y:K
+00001380: a2a5 beff 3069 b596 3913 4b01 97dc 6f6e  ....0i..9.K...on
+00001390: 74fe e1f6 50d7 6e2e b326 9604 4b12 7bf1  t...P.n..&..K.{.
+000013a0: 35f7 0963 5418 cc16 3b81 d3d8 00a7 31c1  5..cT...;.....1.
+000013b0: 0fe7 bc67 8dd0 9ac1 4c9c b0a0 179b e002  ...g....L.......
+000013c0: 214b 8225 896d f97a dd79 9e0a 43d9 6927  !K.%.m.z.y..C.i'
+000013d0: 871a 1b0e 3526 f0f1 e1f6 f67a 9de5 f69d  ....5&.....z....
+000013e0: 98f9 134b 0196 3a69 791f c64e 2c09 9624  ...K..:iy..N,..$
+000013f0: 76e3 6b6d 8701 2a0c 6253 dd8b 35d5 566b  v.km..*.bS..5.Vk
+00001400: 22e4 f121 654f 5b16 6c6a 59b1 e949 4b36  "..!eO[.ljY..IK6
+00001410: b5ac d9d4 b268 53cb aa4d cfb5 6c93 fffc  .....hS..M..l...
+00001420: 14c6 b0a5 4ecc 3436 9869 4cc8 e343 9ead  ....N.46.iL..C..
+00001430: aadf 91db 569a 9b35 a26a a632 66c2 5ace  ....V..5.j.2f.Z.
+00001440: 1329 c64c 2c09 9624 76e2 6b68 97e9 298c  .).L,..$v.kh..).
+00001450: 624b 9d98 696c 30d3 98a8 c7c7 ec4e e77c  bK..il0......N.|
+00001460: 72cc 9c89 a580 a539 4b21 4b82 2589 1be6  r......9K!K.%...
+00001470: eb5a a701 290c 63db 9c34 696c 68d2 1801  .Z..).c..4ilh...
+00001480: 8ffe 75b8 dbad e3ad d538 e649 2c05 58ce  ..u......8.I,.X.
+00001490: 17e9 738d 9025 c192 c4ce 7c6d ee38 5085  ..s..%....|m.8P.
+000014a0: 816c b413 328d 0d64 1a13 fa70 2d35 d008  .l..2..d...p-5..
+000014b0: ac19 cda8 09cb 39d6 b19a 73ce 9025 c192  ......9...s..%..
+000014c0: c44e 7c8d ed38 4085 816c ac13 3a8d 0d74  .N|..8@..l..:..t
+000014d0: 1a3f 0102 cd1a c135 7399 3b61 49bf cf37  .?.....5s.;aI..7
+000014e0: 0ca0 5812 2c49 6ccb d7e9 274c 5461 30bb  ..X.,Il...'LTa0.
+000014f0: ed64 5013 c3a0 26b8 f452 0b90 9f35 a28c  .dP...&..R...5..
+00001500: cd2c 0558 cbcb 662e 10b2 2458 92d8 96ef  .,.X..f...$X....
+00001510: 1a98 5d46 a930 8a57 c274 e2a8 89c1 5113  ..]F.0.W.t....Q.
+00001520: 5cd0 5b7f dbeb d4ba a0f2 ac11 54b3 9731  \.[.........T..1
+00001530: 1496 f259 dc94 7914 4b82 2589 4df9 9adb  ...Y..y.K.%.M...
+00001540: 618e 0a83 d85b 2787 9a18 0e35 21f8 711d  a....['....5!.q.
+00001550: a7ab 441f a849 0b6c 6c84 d75c 6616 8545  ..D..I.ll..\f..E
+00001560: ddb0 91b3 862c 0996 24f6 e26b ee93 06a9  .....,..$..k....
+00001570: 309c 6d76 42a8 8981 5013 c221 27fe c07c  0.mvB...P..!'..|
+00001580: d648 5033 9a81 1496 f53b 5a33 9962 49b0  .HP3.....;Z3.bI.
+00001590: 24b1 2d5f cf9f 3855 8509 d875 27a5 9a18  $.-_..8U...u'...
+000015a0: 4a35 2162 f279 9d6b f7be cdbc 8aa5 006b  J5!b.y.k.......k
+000015b0: 9eb0 6f33 ad62 49b0 24b1 175f 9f9f 3247  ..o3.bI.$.._..2G
+000015c0: 85d1 6cb2 7bc9 f1da 9ae3 c450 3ec7 1b7d  ..l.{......P>..}
+000015d0: 5dee 5676 735b 561e 6f59 7afc 39d6 1e6f  ].Vvs[V.oYz.9..o
+000015e0: 597c bc65 f5f1 96e5 c79f 6bfd f12e 8354  Y|.e......k....T
+000015f0: 18c5 ee3a 11d6 c420 ac09 a196 6353 d6ef  ...:... ....cS..
+00001600: 881a 6135 7b19 6161 3117 96e4 9c21 4b82  ..a5{.aa1....!K.
+00001610: 2589 9df8 7ada 697c 0ac3 d854 27e0 9a18  %...z.i|...T'...
+00001620: c035 21ac f2f9 2e73 1e95 9971 b114 60c5  .5!....s...q..`.
+00001630: 138e ca4c b558 122c 49ec c5d7 dbee 5354  ...L.X.,I.....ST
+00001640: 18cb 063b c1d6 c480 ad09 e115 5825 7cd6  ...;........X%|.
+00001650: 08a8 b9ca 400b cb9c ba38 39e7 0e59 122c  ....@....89..Y.,
+00001660: 49ec c8d7 5bcf 012a 0c60 439d 406b 6280  I...[..*.`C.@kb.
+00001670: d684 08ca 3f5b 5a2e b311 52b3 9431 1616  ....?[Z...R..1..
+00001680: 3ae5 f229 ce1b b224 5892 d88d af9d dee3  :..)...$X.......
+00001690: 5318 c286 3a99 d5d4 30ab 2921 93fb 5dc7  S...:...0.)!..].
+000016a0: 6669 23c8 58ca 52e0 2ce5 da4b 3977 c892  fi#.X.R.,..K9w..
+000016b0: 6049 6247 beb7 f8e8 3044 8541 7c93 0f27  `IbG....0D.A|..'
+000016c0: ac9a 1a58 3525 5e72 e2b4 678d 0435 9319  ...X5%^r..g..5..
+000016d0: 5c61 599f 55c9 397f c892 6049 6257 be46  \aY.U.9...`IbW.F
+000016e0: 3f71 a80a 13b0 e94e 8a35 3514 6b4a f4e4  ?q.....N.55.kJ..
+000016f0: 8bce 8b78 c1eb b935 026b 6633 bfc2 726d  ...x...5.kf3..rm
+00001700: d72c 73be 9025 c192 c42e 7ccd ed38 3c85  .,s..%....|..8<.
+00001710: 816c aa93 594d 0db3 9ab6 c1a3 bf8a 24b2  .l..YM........$.
+00001720: 3bca a08a a500 6bb9 3ef9 70ce 9025 c192  ;.....k.>.p..%..
+00001730: c44e 7c5d ed32 3d85 516c a913 484d 0d90  .N|].2=.Ql..HM..
+00001740: 9a12 0aa9 9aba 4ae2 8dfd 3690 b346 5ccd  ......J...6..F\.
+00001750: 5446 5158 cd69 2a83 2896 044b 123b f135  TFQX.i*.(..K.;.5
+00001760: b5db fc14 c6b1 ad4e 0435 3508 6a4a 0cc4  .......N.55.jJ..
+00001770: e3cd 6fd6 9aa4 f72b 4bcf dcdd 95f2 5c35  ..o....+K.....\5
+00001780: f2d4 5e10 28cd 590a 5912 2c49 dc1c 5fcb  ..^.(.Y.Y.,I.._.
+00001790: 9f61 b60a 93b0 ffee 7be5 d56e 96d7 7617  .a......{..n..v.
+000017a0: bb30 ca37 56bf 5b6e 97d7 72bf bcb6 5227  .0.7V.[n..r...R'
+000017b0: 9f67 b5dc 30af e58e 792d b7cc 7bae 7be6  .g..0...y-..{.{.
+000017c0: 7518 a4c2 2036 d709 aba6 0656 4d09 9554  u... 6.....VM..T
+000017d0: 3ddd c35e 91c7 d60f c18d e09a c94c abb0  =..^.........L..
+000017e0: a4f3 c0cd ac8a 25c1 92c4 4e7c 8d7d c210  ......%...N|.}..
+000017f0: 1506 b3c1 4e58 3535 b06a 4ae8 a4f6 259d  ....NX55.jJ...%.
+00001800: d55b 6656 2c05 add5 4ede 8199 5bb1 2458  .[fV,...N...[.$X
+00001810: 92d8 95af cfdd 66a9 308e 2d76 e2ab a9c1  ......f.0.-v....
+00001820: 57d3 e7b8 386a d6c8 5233 9c89 566b ed93  W...8j..R3..Vk..
+00001830: 0d67 b2c5 9260 4962 57be 863f c764 1566  .g...`IbW..?.d.f
+00001840: 61fb 9db0 eba5 815d 2f09 b9d0 a236 8d00  a......]/....6..
+00001850: e334 4b01 9671 1db6 3967 c892 6049 6227  .4K..q..9g..`Ib'
+00001860: be37 3ef5 1c9c c200 bee5 29c3 adfe 6ead  .7>.......)...n.
+00001870: 7551 0def f262 1bad f4bb 285f c5e9 ae97  uQ...b....(_....
+00001880: e8db 32e2 fcc5 cbf2 1c2d 8f57 ebe3 1f45  ..2......-.W...E
+00001890: b67d 7d36 38eb dd64 4591 6d0e ff5d eb68  .}}68..dE.m..].h
+000018a0: a9f3 ea09 a57e 9b65 c5f1 8faa cc5d 967f  .....~.e.....]..
+000018b0: 3d14 b9fc 3f50 4b03 0414 0000 0008 0060  =...?PK........`
+000018c0: 50f8 560e 2fc9 cfc2 0e00 006f 8b00 0018  P.V./......o....
+000018d0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+000018e0: 2f73 6865 6574 332e 786d 6cad 9d5b 779b  /sheet3.xml..[w.
+000018f0: 4816 85ff 8a96 9fa6 5f62 ebe6 24bd 1caf  H......._b..$...
+00001900: 1549 405d ba92 2cbb 67fa 194b 659b 892c  .I@]..,.g..Ke..,
+00001910: d480 dac9 fcfa 01f9 0212 7caa 80fc 14db  ..........|.....
+00001920: 9ff7 a9aa 533b 086f 04ba 788c 93ef e9bd  ....S;.o..x.....
+00001930: b559 efc7 c372 957e 3ab9 cfb2 f5ef a7a7  .Y...r.~:.......
+00001940: e9fc de3e 84e9 bb78 6d57 39b9 8d93 8730  ...>...xmW9....0
+00001950: cbbf 4dee 4ed3 7562 c3c5 56f4 b03c 1d9c  ..M.N.ub..V..<..
+00001960: 9d9d 9f3e 84d1 eae4 f262 fbb3 6fc9 e545  ...>.....b..o..E
+00001970: bcc9 96d1 ca7e 4b7a e9e6 e121 4c7e 4eec  .....~Kz...!L~N.
+00001980: 327e fc74 d23f 79f9 c155 7477 9f6d 7f70  2~.t.?y..Utw.m.p
+00001990: 7a79 b10e efec b5cd febd ce05 f9b7 a7af  zy..............
+000019a0: 7516 d183 5da5 51bc ea25 f6f6 d3c9 e7fe  u...].Q..%......
+000019b0: ef5f ce07 5bc9 f657 fe13 d9c7 b4f2 75af  ._..[..W......u.
+000019c0: 58cd 4d1c 7f2f be91 8b4f 2767 c5a4 ecd2  X.M../...O'g....
+000019d0: ceb3 a246 98ff f38f 9dda e5b2 2895 4fe5  ...F........(.O.
+000019e0: efe7 aa27 e5a8 85b2 faf5 4b79 7fdb 807c  ...'......Ky...|
+000019f0: 7e37 616a a7f1 f2af 6891 dd7f 3af9 70d2  ~7aj....h...:.p.
+00001a00: 5bd8 db70 b3cc aee2 4761 9f17 352e a738  [..p....Ga..5..8
+00001a10: 0bb3 f0f2 2289 1f7b 49b1 dacb 8b79 f145  ...."..{I....y.E
+00001a20: 3164 fe8b d1aa e8d2 7596 e43f 8ff2 91b2  1d......u..?....
+00001a30: cbe2 d77b 265e d865 6f66 6fa3 5554 4cfc  ...{&^.eofo.UTL.
+00001a40: e234 cba7 54fc c2e9 fcb9 c064 bf40 31e0  .4..T......d.@1.
+00001a50: 964c 91cc 9078 487c 2401 1241 8bbb cec2  .L...xH|$..A....
+00001a60: cc36 2c46 6229 8544 d320 7a15 3f2e ede2  .6,Fb).D. z.?...
+00001a70: cee6 dbfd f726 4ab7 1dec 2de3 bb86 81ff  .....&J...-.....
+00001a80: c0f2 06c9 9726 729a 6ff0 eb2e 0f5e 7779  .....&r.o....^wy
+00001a90: 0073 9c2e c334 6dda 5512 7c4b f2ff 8749  .s...4m.U.|K...I
+00001aa0: f6b3 4133 25cd 97f0 a1a9 d933 fafd 994d  ..A3%......3...M
+00001ab0: e749 b406 c379 24fb f3e7 ba69 189f 7edf  .I...y$....i..~.
+00001ac0: 44ab de34 deac b206 5180 a2f0 078a 042f  D..4....Q....../
+00001ad0: 283f 50cd 73cb 2d9a 3ce7 5215 ae99 35fb  (?P.s.-.<.R...5.
+00001ae0: 5591 f6ca ae97 e1dc 2e7a 93a6 9dd2 24bb  U........z....$.
+00001af0: 8e37 c9bc 69a0 3f0e 2b7a de2a 8bb2 9f3d  .7..i.?.+z.*...=
+00001b00: d869 c3dd cce6 f70d 822f e8d7 f821 3f0e  .i......./...!?.
+00001b10: ef35 7fc7 f3c3 57cf 0fe9 3fce 649f bc54  .5....W...?.d..T
+00001b20: bf0f d3e9 cc1f ceb6 87bd 2687 63c9 1912  ..........&.c...
+00001b30: 0f89 8f24 4022 9048 240a 89c6 46e4 2fbd  ...$@".H$...F./.
+00001b40: 69fe dafb fdee dd3c becb 8ffd f65d 189d  i......<.....]..
+00001b50: 3e46 abc5 6993 39ba f6d3 90d0 fec8 5f21  >F..i.9......._!
+00001b60: 9b7c d1b4 949d ed1f bd6e ff08 b77f 9fec  .|.......n......
+00001b70: 4eb7 78e1 fb9a dc85 abe8 7fdb ff7b 5736  N.x..........{W6
+00001b80: dd7a 1c0e 2f53 1c67 86c4 43e2 2309 9008  .z../S.g..C.#...
+00001b90: 2412 8942 a2b1 3bed 3cf1 a64d 3654 0d8d  $..B..;.<..M6T..
+00001ba0: d2b4 be1d a38c 5f8d 3246 a3ec 93fa 1af2  ......_.2F......
+00001bb0: 73c5 264f 60c9 1912 0f89 8f24 4022 9048  s.&O`......$@".H
+00001bc0: 240a 89c6 46b4 f344 d77e 1a12 e2f6 372d  $...F..D.~....7-
+00001bd0: 6567 fbcf 5fb7 ff1c b77f 9f34 4c37 8b93  eg.._......4L7..
+00001be0: fc2f 06d7 2102 8798 21f1 90f8 4802 2402  ./..!...!...H.$.
+00001bf0: 8944 a290 686c 4c3b 3bbc 557f 0d15 427b  .D..hlL;;.U...B{
+00001c00: 342d 6dc7 1eef 5fed f11e edb1 4f76 a7ef  4-m..._.....Ov..
+00001c10: fd53 3b4f 7932 0316 9c21 f190 f848 0224  .S;Oy2...!...H.$
+00001c20: 0289 44a2 9068 6c43 3b33 74eb a621 196e  ..D..hlC;3t..!.n
+00001c30: 7dd3 4276 b6fe c3eb d67f c0ad df27 bb93  }.Bv.........'..
+00001c40: f5a3 65e3 6100 ebcd 9078 487c 2401 1281  ..e.a....xH|$...
+00001c50: 4422 5148 3476 a1dd ce77 6aa6 2115 6e7c  D"QH4v...wj.!.n|
+00001c60: d33a 7636 fee3 ebc6 7fc4 8ddf 27bb 73fd  .:v6........'.s.
+00001c70: 23bc 69fe bb01 0bce 9078 487c 2401 1281  #.i......xH|$...
+00001c80: 4422 5148 34b6 a1dd ce77 eba6 2119 6e7d  D"QH4....w..!.n}
+00001c90: d342 76b6 be7f 56e6 6167 b8f9 35b4 3bdf  .Bv...V.ag..5.;.
+00001ca0: 2bbb dc9e cba6 f7d1 bac9 045c 79c6 c863  +..........\y..c
+00001cb0: e433 0a18 0946 9291 62a4 b92d eddc 705c  .3...F..b..-..p\
+00001cc0: 7b0d cad1 168d 6bda f545 2527 c51c 6e52  {.....k..E%'..nR
+00001cd0: 43fb 133f 7c76 c895 678c 3c46 3ea3 8091  C..?|v..g.<F>...
+00001ce0: 6024 1929 469a dbd2 d217 47b5 d7a0 9c7d  `$.)F.....G....}
+00001cf0: e10c 56fb 65b2 dadf 8faa 2abe a014 eb69  ..V.e.....*....i
+00001d00: e27f 460f f6da 2651 b329 b0ec 8c91 c7c8  ..F...&Q.)......
+00001d10: 6714 3012 8c24 23c5 4873 4f5a 9aa2 7b6f  g.0..$#.HsOZ..{o
+00001d20: 0d6a d911 4d0b da75 4499 3bf6 3978 aca1  .j..M..uD.;.9x..
+00001d30: caac 8bbf 77be 25f1 62d3 3885 2957 9d31  ....w.%.b.8.)W.1
+00001d40: f218 f98c 0246 8291 64a4 1869 6e49 4b43  .....F..d..inIKC
+00001d50: 746e ad41 29fb c199 43f6 cb20 b2cf 4964  tn.A)...C.. ..Id
+00001d60: 0d55 26fd 2d7e b4c9 349b 6e92 7fac b159  .U&.-~..4.n....Y
+00001d70: b8c8 17d1 680c 0e20 1979 8c7c 4601 23c1  ....h.. .y.|F.#.
+00001d80: 4832 528c 34f7 a6a5 318e efb1 c11a ec10  H2R.4...1.......
+00001d90: 6700 d92f 13c8 3e47 9035 5499 fd5f f992  g../..>G.5T.._..
+00001da0: ffdc 2437 3999 de87 493e 93fc 8897 66d1  ..$79...I>....f.
+00001db0: bcd1 269c 4932 f218 f98c 0246 8291 64a4  ..&.I2.....F..d.
+00001dc0: 1869 6e50 4b9b bc51 a30d 1662 af38 d3ca  .inPK..Q...b.8..
+00001dd0: 7e19 57f6 39af aca1 e625 b85e 6838 ad64  ~.W.9....%.^h8.d
+00001de0: e431 f219 058c 0423 c948 31d2 dc9d 9646  .1.....#.H1....F
+00001df0: 798b 2e1b acc2 2e71 8696 fd32 b5ec 736c  y......q...2..sl
+00001e00: 5943 2f23 4795 8b75 5f6f 1bad c1d9 2523  YC/#G..u_o....%#
+00001e10: 8f91 cf28 6024 1849 468a 91c6 96b4 b546  ...(`$.IF......F
+00001e20: e7d6 1a94 b21f 9c49 66bf 8c32 fb9c 65d6  .......If..2..e.
+00001e30: d0ce a40f 5da8 0393 70cc c9c8 63e4 330a  ....]...p...c.3.
+00001e40: 1809 4692 9162 a4b1 4f6d 4df2 b6fd 3658  ..F..b..OmM...6X
+00001e50: 8f9d e38c 42fb 6516 dae7 30b4 866a 2bb9  ....B.e...0..j+.
+00001e60: b619 9884 1351 461e 239f 51c0 4830 928c  .....QF.#.Q.H0..
+00001e70: 1423 8d2d 696b 92ce ad35 2865 3f38 f3d1  .#.-ik...5(e?8..
+00001e80: 4199 8f0e 381f ada1 faa4 ebd7 f39a fdc1  A...8...........
+00001e90: a3cc 1879 8c7c 4601 23c1 4832 528c 34b6  ...y.|F.#.H2R.4.
+00001ea0: a8a5 3fde aed5 064b a15f 1ad7 b7eb 9732  ..?....K._.....2
+00001eb0: 371d 706e 5a43 3b8b d85e f203 7770 62ca  7.pnZC;..^..wpb.
+00001ec0: c863 e433 0a18 0946 9291 62a4 b121 6ddd  .c.3...F..b..!m.
+00001ed0: d1b1 b106 85ec 05f7 9b50 2bef 42e5 acb4  .........P+.B...
+00001ee0: 8676 a65c 5c04 042b 704e cac8 63e4 330a  .v.\\..+pN..c.3.
+00001ef0: 1809 4692 9162 a4b1 1f6d add0 adaf 0675  ..F..b...m.....u
+00001f00: ec04 6746 3a28 33d2 0167 a435 b433 e3ed  ..gF:(3..g.5.3..
+00001f10: 4541 b002 27a4 8c3c 463e a380 9160 2419  EA..'..<F>...`$.
+00001f20: 2946 1a1b d2d6 0a1d 1b6b 50c8 5e70 e6a3  )F.......kP.^p..
+00001f30: 8332 1f1d 703e 5a43 3b53 ae5e 1104 4b70  .2..p>ZC;S.^..Kp
+00001f40: 36ca c863 e433 0a18 0946 9291 62a4 b12f  6..c.3...F..b../
+00001f50: 6d2d 715c 7f0d ead9 19ce 5c74 50e6 a203  m-q\......\tP...
+00001f60: ce45 6b68 6fe6 ce13 4c8e 4319 798c 7c46  .Ekho...L.C.y.|F
+00001f70: 0123 c148 3252 8c34 f6a5 ad33 8eeb af41  .#.H2R.4...3...A
+00001f80: 3d3b c399 820e ca14 74c0 2968 0ded ccfc  =;......t.)h....
+00001f90: f5c2 20d8 82c3 4f46 1e23 9f51 c048 3092  .. ...OF.#.Q.H0.
+00001fa0: 8c14 238d 4d69 6b8b 239a 6b50 cc9e 7066  ..#.Mik.#.kP..pf
+00001fb0: 9e83 32f3 1c70 e659 43e5 b42b 392d 5882  ..2..p.YC..+9-X.
+00001fc0: 434f 461e 239f 51c0 4830 928c 1423 8d3d  COF.#.Q.H0...#.=
+00001fd0: 696b 89ee bd35 a865 4738 53cf 4199 7a0e  ik...5.eG8S.A.z.
+00001fe0: 38f5 aca1 72d6 78b5 07fc c179 2723 8f91  8...r.x....y'#..
+00001ff0: cf28 6024 1849 468a 91c6 0eb5 f5c7 5b75  .(`$.IF.......[u
+00002000: da60 2576 8b33 e91c 9449 e780 93ce 1a6a  .`%v.3...I.....j
+00002010: 5c83 fb50 c2a9 2723 8f91 cf28 6024 1849  \..P..'#...(`$.I
+00002020: 468a 91c6 f6b4 b5ca 9bb4 d960 19f6 8933  F..........`...3
+00002030: 011d 9609 e890 02b3 cf69 da78 fbca 0415  .........i.x....
+00002040: db57 cdad acd9 3028 9469 2f57 f6b6 d25e  .W....0(.i/W...^
+00002050: a376 86da abe2 bed2 d4ae b2b4 973c 9fe1  .v...........<..
+00002060: f76e 6cf6 68ed aa17 56ca fe6b 1117 77d3  .nl.h...V..k..w.
+00002070: f7c2 bb55 5cfc a7ec c537 ffb5 f3ec b75e  ...U\....7.....^
+00002080: b85a f49e 59ba b6f3 e8f6 95f5 fe95 6ee6  .Z..Y.........n.
+00002090: f7bd 30ed 15fb d57b deb0 dfde 35dd c68b  ..0....{....5...
+000020a0: f3ab 6c75 d3ed bc35 5de9 7946 8291 64a4  ..lu...5].yF..d.
+000020b0: 1869 9c7e db7b 273b 7ac3 a090 6f9e 74e6  .i.~.{';z...o.t.
+000020c0: b6c3 32b7 1d52 14f8 f947 94c2 7b2d 2728  ..2..R...G..{-'(
+000020d0: 8ad2 1719 189d 135d 461e 0ee7 b210 c7bd  .......]F.......
+000020e0: 8c04 23c9 4831 d238 fdb6 16ea d875 8342  ..#.H1.8.....u.B
+000020f0: b690 33ee 1d96 71ef 9032 c4e7 775c 353a  ..3...q..2..w\5:
+00002100: 0873 cf30 9d66 9368 d5f4 b482 694d 55b1  .s.0.f.h....iMU.
+00002110: 0fa7 c038 569a 25d1 aae9 310d 3e57 0b18  ...8V.%...1.>W..
+00002120: 0946 9291 62a4 b94b 2d9d d3a5 db06 556c  .F..b..K-.....Ul
+00002130: 1b67 363c acdc b74f 71e3 21db 70b6 593d  .g6<...Oq.!.p.Y=
+00002140: c97c 2a00 87a0 0337 f71f b8bb 9f06 761d  .|*....7......v.
+00002150: 820e dcfc 7fe0 eeff 03b7 ff1f b8ff ffc0  ................
+00002160: 0300 deea 0900 47f7 df60 0976 9533 651e  ......G..`.v.3e.
+00002170: 9629 f390 a24a e94d f129 2828 8ad2 1719  .)...J.M.)((....
+00002180: 9889 8367 461e 0ee7 3213 a7d2 8c04 23c9  ...gF...2.....#.
+00002190: 4831 d238 fdb6 66ea d875 8342 b690 338e  H1.8..f..u.B..3.
+000021a0: 1e96 71f4 9032 4db9 4ab3 70f9 742a 8da7  ..q..2M.J.p.t*..
+000021b0: 461c a8ee cbc1 529c 5833 f270 5897 a538  F.....R.X3.pX..8
+000021c0: ce66 2418 4946 8a91 c6e9 b7b5 d491 dd37  .f$.IF.........7
+000021d0: 5880 ade5 ccb3 8765 9e3d a468 f4cb e6e1  X......e.=.h....
+000021e0: c626 5f6f 27cb 7061 9b8f 511c c9ee 8ac1  .&_o'.pa..Q.....
+000021f0: 569c 7833 f270 5097 ad38 0e67 2418 4946  V.x3.pP..8.g$.IF
+00002200: 8a91 c6e9 b7b5 d551 bd37 2867 5339 03f1  .......Q.7(gS9..
+00002210: 6119 880f 295d 7dba ed01 cfa5 0edc 8abf  a...)]}.........
+00002220: 55e2 5938 27e5 8c3c 1cee c059 3827 e88c  U.Y8'..<...Y8'..
+00002230: 0423 c948 31d2 dca8 962e ead8 7083 42f6  .#.H1.......p.B.
+00002240: 8f33 3e1f 96f1 f990 f256 877f 7e29 f02d  .3>......V..~).-
+00002250: 6bc0 7189 6375 461e 8eed 3a2e 71e6 ce48  k.q.cuF...:.q..H
+00002260: 3092 8c14 238d d36f eba8 b7d8 0283 55d8  0...#..o......U.
+00002270: 5ece bc7d 58e6 ed43 8a69 afe2 2c4e be26  ^..}X..C.i..,N.&
+00002280: 915d 6521 3d75 12c5 51ba 2f07 7f71 16cf  .]e!=u..Q./..q..
+00002290: c8c3 615d fee2 a09e 9160 2419 2946 1aa7  ..a].....`$.)F..
+000022a0: dfd6 5f47 76df 6001 b696 33a2 1f95 11fd  .._Gv.`...3.....
+000022b0: 08b3 ef62 7674 8a8e aae7 55f1 b979 4d59  ...bvt....U..yMY
+000022c0: 9a89 9187 e339 ccc4 2503 4682 9164 a418  .....9..%.F..d..
+000022d0: 699c 7edb 27c5 756d bb41 253f 16ce 1981  i.~.'.um.A%?....
+000022e0: 8fca 087c 848f 8fb5 7f6f ecaa f141 9913  ...|.....o...A..
+000022f0: 146d f3fc 1725 d888 5370 461e 8ef8 e56c  .m...%..SpF....l
+00002300: f8de 7e1c dc0c 071f 6f6e 47e3 0fb7 3703  ..~.....onG...7.
+00002310: 3b0a df87 37ef 3f7c 08fb 67c3 6673 7136  ;...7.?|..g.fsq6
+00002320: ce48 3092 8c14 238d 8b6a 6bae eedb 6150  .H0...#..jk...aP
+00002330: cbf6 72c6 e3a3 321e 1f51 8c7a bd59 afe3  ..r...2..Q.z.Y..
+00002340: 24cb 7fb4 9967 9b84 9e6c 31c1 0251 da54  $....g...l1..Q.T
+00002350: 023c c7d1 3923 0f87 761d ba38 3f67 2418  .<..9#..v..8?g$.
+00002360: 4946 8a91 c6e9 b775 d71b ec80 c122 6c33  IF.....u....."l3
+00002370: 679c 3e2a e3f4 51b7 847a 82ba fcaf 9203  g.>*..Q..z......
+00002380: d700 a735 5dc5 509c a3e3 6807 86f2 b95e  ...5].P...h....^
+00002390: c048 3092 8c14 23cd 9d6a e9a6 6e1d 37a8  .H0...#..j..n.7.
+000023a0: 6303 b99f a35b 7990 6eb7 547a 82ba a747  c....[y.n.Tz...G
+000023b0: b4d0 bb25 a635 5dc5 4007 1ea9 4ba3 d138  ...%.5].@...K..8
+000023c0: 3e17 0b18 0946 9291 62a4 b94d 2ddd d3ad  >....F..b..M-...
+000023d0: dd06 75ec 1e67 683e 2a43 f351 b700 7a82  ..u..gh>*C.Q..z.
+000023e0: ba62 399b 4cae aed7 b6f1 79ea d39a b2e2  .b9.L.....y.....
+000023f0: 1f0e ca71 bcdb 651c 36fb 8723 7246 8291  ...q..e.6..#rF..
+00002400: 64a4 1869 6e54 4bff 746d b841 253b c899  d..inTK.tm.A%;..
+00002410: 8d8f ca6c 7cd4 2d6b 9ea0 ee69 415f 3719  ...l|.-k...iA_7.
+00002420: 5b88 4371 461e 0ec8 16e2 389c 9160 2419  [.CqF.....8..`$.
+00002430: 2946 9a3b d5d2 429d 3b6e 50ca 1e72 46e1  )F.;..B.;nP..rF.
+00002440: a332 0a1f 5152 eaf2 d081 6876 1685 0f36  .2..QR....hv...6
+00002450: b349 a381 380a 67e4 e168 6c20 4ec2 1909  .I..8.g..hl N...
+00002460: 4692 9162 a4b9 4d2d 0dd4 addd 0675 ec1e  F..b..M-.....u..
+00002470: 6710 3e2a 83f0 51b7 5479 82ba 7c39 de8f  g.>*..Q.Ty..|9..
+00002480: 7c2d ab70 299b 0f40 9c7e 33f2 70bc 142f  |-.p)..@.~3.p../
+00002490: a570 b580 9160 2419 2946 9a3b d5d2 405d  .p...`$.)F.;..@]
+000024a0: 3b6e 50c9 1672 86dd a332 ec1e 750b 8e27  ;nP..r...2..u..'
+000024b0: a8cb 1724 3637 4f1f f4d4 e820 ceb7 1979  ...$67O.... ...y
+000024c0: 381c 1f81 38d9 6624 1849 468a 91e6 3eb5  8...8.f$.IF...>.
+000024d0: 3450 c77e 1b14 b27f 9c89 f6b8 4cb4 c7dd  4P.~........L...
+000024e0: b2e2 09ea f2f5 1c78 e7d3 b4a6 2bed c3c8  .......x....+...
+000024f0: c3d1 0e0c e573 bd80 9160 2419 2946 9a3b  .....s...`$.)F.;
+00002500: d5f2 432e ba75 dca0 8e3f e4c2 1966 8fcb  ..C..u...?...f..
+00002510: 307b dced bdd2 13d4 15cb 71bf ef69 5ad3  0{........q..iZ.
+00002520: 578c c499 368e fa0b 43fa 5c37 6024 1849  W...6...C.\7`$.I
+00002530: 468a 91e6 ceb5 34d4 713b 6050 cfc6 72c6  F.....4.q;`P..r.
+00002540: d8e3 32c6 1e77 8b82 27a8 cb97 65c2 1fd7  ..2..w..'...e...
+00002550: f166 b5d8 5ea1 6e74 15a7 d68c 3c1c 125f  .f..^.nt....<.._
+00002560: ddb8 58c0 4830 928c 1423 cdbd 6a69 a523  ..X.H0...#..ji.#
+00002570: 7a6e 50cc 3e72 e6d4 e332 a71e 77cc a951  znP.>r...2..w..Q
+00002580: 97af c9f9 eeb9 694d 5d31 12a7 d538 a673  ......iM]1...8.s
+00002590: 409f ab06 8c04 23c9 4831 d2dc b596 8e3a  @.....#.H1.....:
+000025a0: a6fb 06d5 6c29 6772 3d2e 93eb 71c7 e41a  ....l)gr=...q...
+000025b0: 75f9 a2ae 8a8f 71e4 e312 67d7 8c3c 1c8f  u.....q...g..<..
+000025c0: 8f4b 9c5d 3312 8c24 23c5 4873 a35a baa8  .K.]3..$#.Hs.Z..
+000025d0: 6bc3 0d2a d941 ee8f 86ab 7c36 5cc7 f41a  k..*.A....|6\...
+000025e0: 75c5 82dc 6f6f 9ad6 f415 1f1d f808 391a  u...oo........9.
+000025f0: f517 86f4 b96e c048 3092 8c14 23cd 9d6b  .....n.H0...#..k
+00002600: 69a9 e376 c0a0 9e8d e50c b5c7 65a8 3dee  i..v........e.=.
+00002610: 186a a3ee 6559 781e ce91 3623 0f87 3b34  .j..eYx...6#..;4
+00002620: 96cf 0503 4682 9164 a418 69ee 554b 2b75  ....F..d..i.UK+u
+00002630: ecb9 4121 7bc8 196a 8fcb 507b dc31 d446  ..A!{..j..P{.1.F
+00002640: 5dbe 9e5f 7cef c9b4 56a3 6227 0eb8 71e4  ].._|...V.b'..q.
+00002650: 5f1c d6e7 da01 23c1 4832 528c 3477 b0a5  _.....#.H2R.4w..
+00002660: b38e df09 8335 d864 ceec 7b5c 66df e38e  .....5.d..{\f...
+00002670: d937 ea8a a53d da75 f639 b18d 9f67 5113  .7...=.u.9...gQ.
+00002680: 569c c5d1 370e c7a7 509c 7c33 128c 2423  V...7...P.|3..$#
+00002690: c548 739f 5a5a a963 bf0d 0ad9 3fce e07b  .Hs.ZZ.c....?..{
+000026a0: 5c06 dfe3 8ec1 37ea f63e 8f01 ef09 9ed6  \.....7..>......
+000026b0: 2a54 8cc4 0938 8ecb 23f9 5c2e 6024 1849  *T...8..#.\.`$.I
+000026c0: 468a 91e6 96b5 b4d2 b1ad 3758 813d e50c  F.........7X.=..
+000026d0: c3cf cb30 fcbc 6318 8eba dd85 1dfa b49d  ...0..c.........
+000026e0: 5a89 d254 8c3c 463e a380 9160 2419 2946  Z..T.<F>...`$.)F
+000026f0: 9a5b d3f2 337d 8f6e b1c1 12fc 71be ce20  .[..3}.n....q.. 
+00002700: fcbc 0cc2 cf3b 06e1 a8db 5b19 7cd6 fdb4  .....;....[.|...
+00002710: a6af 3887 8370 1c35 c54b ba5c 2d60 2418  ..8..p.5.K.\-`$.
+00002720: 4946 8a91 e67e b574 d471 7d37 a867 3b39  IF...~.t.q}7.g;9
+00002730: e3ef f332 fe3e ef18 7fa3 6e77 5907 6fb5  ...2.>....nwY.o.
+00002740: 9bd6 8a54 3cc5 3138 0e7d 7030 9f2b 068c  ...T<.18.}p0.+..
+00002750: 0423 c948 31d2 dcb8 96be 7a83 0d30 5884  .#.H1.....z..0X.
+00002760: cdc5 99f8 697a 6f6d 563c deec f262 1dde  ....izomV<...b..
+00002770: 5913 2677 d12a ed2d ed6d ae38 7bf7 7e7c  Y.&w.*.-.m.8{.~|
+00002780: d24b 8aeb cf2f df64 f1fa d349 6ed6 9b38  .K.../.d...In..8
+00002790: cbe2 87ed 97f7 365c d8a4 f885 9cdf c671  ......6\.......q
+000027a0: f6fa 4d31 cc63 9c7c df0e 72f9 7f50 4b03  ..M1.c.|..r..PK.
+000027b0: 0414 0000 0008 0060 50f8 56f7 f68f 09a7  .......`P.V.....
+000027c0: 0200 006d 0b00 000d 0000 0078 6c2f 7374  ...m.......xl/st
+000027d0: 796c 6573 2e78 6d6c dd56 db8e 9b30 10fd  yles.xml.V...0..
+000027e0: 15c4 0794 4d50 51a8 42a4 36d2 4a95 da6a  ....MPQ.B.6.J..j
+000027f0: a5dd 87be 9a60 8225 5fa8 31ab 64bf be33  .....`.%_.1.d..3
+00002800: b613 92ec 0edd f6b1 a084 f11c 9fb9 3b64  ..............;d
+00002810: 3db8 a3e4 8f1d e72e 3928 a987 2aed 9ceb  =.......9(..*...
+00002820: 3f65 d9b0 ebb8 62c3 07d3 730d 486b ac62  ?e....b...s.Hk.b
+00002830: 0e96 769f 0dbd e5ac 1990 a464 b6bc bb2b  ..v........d...+
+00002840: 32c5 844e 376b 3daa 7be5 8664 6746 edaa  2..N7k=.{..dgF..
+00002850: f42e 4db2 cdba 357a 522d d3a0 80bd 4cf1  ..M...5zR-....L.
+00002860: e499 c92a dd32 296a 2bc2 66a6 843c 06fd  ...*.2)j+.f..<..
+00002870: d26b 7646 1a9b 3888 8657 e9c2 ab86 97b0  .kvF..8..W......
+00002880: 6111 9718 6ab4 a584 36d6 6bb3 e026 7cd7  a...j...6.k..&|.
+00002890: 9170 89f8 c700 3b84 94d7 f181 62b3 ee99  .p....;.....b...
+000028a0: 73dc ea7b 5804 92d7 bec6 a2fc 74ec 21be  s..{X.......t.!.
+000028b0: bd65 c7c5 f263 7ac1 f00f 7053 1bdb 707b  .e...cz...pS..p{
+000028c0: e528 a836 6bc9 5b87 0c2b f69d 179c e9f1  .(.6k.[..+......
+000028d0: 511b e78c 42a9 116c 6f34 0b91 9c68 5774  Q...B..lo4...hWt
+000028e0: dfc8 2a75 1d34 62b2 75ab 45c3 b7ba e8e5  ..*u.4b.u.E.....
+000028f0: 567d 7613 0548 61c7 a57c c46d 3fdb 731e  V}v..Ha..|.m?.s.
+00002900: 0bc8 e3d0 26a1 f35f 1bdf 742c ec49 84e4  ....&.._..t,.I..
+00002910: a318 ccc4 053a b834 178c 5fd8 5dfe 9bdd  .....:.4.._.]...
+00002920: 5e3c 1bf7 6584 8cb4 5fff 1a8d e30f 96b7  ^<..e..._.......
+00002930: e2e0 d787 760a 8032 bf20 cc83 9ef5 bd3c  ....v..2. .....<
+00002940: 7e96 62af 150f d9bf dbe3 66cd 4ebc a433  ~.b.......f.N..3
+00002950: 56bc 8037 9cc9 1d28 388c ec33 b74e ec50  V..7...(8..3.N.P
+00002960: 034d 0a05 3ab4 b14a e702 f972 5dd5 feac  .M..:..J...r]...
+00002970: 4df0 4055 e90f 3ca8 f222 d17a 14d2 091d  M.@U..<..".z....
+00002980: 579d 681a ae5f b700 ec3b 56c3 4fc1 9503  W.h.._...;V.O...
+00002990: d8d5 f096 8dd2 3d9d c12a 9de4 efbc 11a3  ......=..*......
+000029a0: 2acf bb1e b016 71d7 247f c351 5c14 d369  *.....q.$..Q\..i
+000029b0: 0667 4237 fcc0 9b6d 5cda 7ded c504 0470  .gB7...m\.}....p
+000029c0: 1baf 30c8 37d0 bdbf 0888 6405 9080 1024  ..0.7.....d....$
+000029d0: 7d91 6190 acc0 237d fd8f 79ad e8bc 0248  }.a...#}..y....H
+000029e0: 46b8 7a1b 5ad1 ac15 cd0a bc37 a1ad bf49  F.z.Z......7...I
+000029f0: 5f04 ab84 8b48 b92c f3bc 28c8 f26e b76f  _....H.,..(..n.o
+00002a00: 87b1 256b 5814 f821 0c92 1122 87f4 85de  ..%kX..!..."....
+00002a10: feb6 f233 0330 3336 7f98 0db2 cbb3 6343  ...3.036......cC
+00002a20: a63c 33a2 64ca 3395 4788 a821 72ca 9218  .<3.d.3.G..!r...
+00002a30: 00d2 1772 c8a6 9013 8541 10be 70d4 0856  ...r.....A..p..V
+00002a40: 9e63 9fc9 08c9 633e 0395 2509 e190 12d3  .c....c>..%.....
+00002a50: 5b14 54a1 0abc 897e 9187 28cf cb92 8010  [.T....~..(.....
+00002a60: 24c2 c873 12c2 033b 0391 6160 2024 94e7  $..s...;..a` $..
+00002a70: e145 7af3 3ecb 4eef b96c fa83 bdf9 0d50  .Ez.>.N..l.....P
+00002a80: 4b03 0414 0000 0008 0060 50f8 56b7 47eb  K........`P.V.G.
+00002a90: 8ac0 0000 0016 0200 000b 0000 005f 7265  ............._re
+00002aa0: 6c73 2f2e 7265 6c73 9d92 4b6e 0231 0c40  ls/.rels..Kn.1.@
+00002ab0: af12 655f 4ca9 c402 31ac d8b0 4388 0bb8  ..e_L...1...C...
+00002ac0: 89e7 a399 c491 63c4 f4f6 8dd8 c020 6811  ......c...... h.
+00002ad0: 4bff 9e9e 2daf 0f34 a076 1c73 dba5 6cc6  K...-..4.v.s..l.
+00002ae0: 30c4 5cd9 5635 ad00 b26b 2960 9e71 a258  0.\.V5...k)`.q.X
+00002af0: 2a35 4b40 2da1 3490 d0f5 d810 2ce6 f325  *5K@-.4.....,..%
+00002b00: c82d c36e d6b7 4c73 fc49 f40a 91eb ba73  .-.n..Ls.I.....s
+00002b10: b465 770a 14f5 01f8 aec3 9a23 4a43 5ad9  .ew........#JCZ.
+00002b20: 7180 334b ffcd dccf 0ad4 9a9d afac ecfc  q.3K............
+00002b30: a735 f0a6 ccf3 f520 90a2 4745 702c f491  .5..... ..GEp,..
+00002b40: a44c 8b76 94af 3e9e ddbe a4f3 a563 62b4  .L.v..>......cb.
+00002b50: 78df e8ff f3d0 a814 3df9 bf9d 30a5 89d2  x.......=...0...
+00002b60: d745 0926 6fb0 f905 504b 0304 1400 0000  .E.&o...PK......
+00002b70: 0800 6050 f856 b948 9c76 5201 0000 ae02  ..`P.V.H.vR.....
+00002b80: 0000 0f00 0000 786c 2f77 6f72 6b62 6f6f  ......xl/workboo
+00002b90: 6b2e 786d 6c8d 91dd 4e83 4010 855f 85ec  k.xml...N.@.._..
+00002ba0: 0308 a5da c4a6 f4a6 8dda c4bf 58e3 fd00  ............X...
+00002bb0: 4399 747f c8ee d06a 9fde 5d08 8a69 d278  C.t....j..]..i.x
+00002bc0: b5cc 99d9 8f39 6717 4763 f7b9 31fb e853  .....9g.Gc..1..S
+00002bd0: 49ed e636 1335 7333 8f63 57d4 a8c0 5d99  I..6.5s3.cW...].
+00002be0: 06b5 ef55 c62a 605f da5d 6caa 8a0a 5c9b  ...U.*`_.]l...\.
+00002bf0: a255 a839 4e93 6416 5b94 c064 b4ab a971  .U.9N.d.[..d...q
+00002c00: a2a7 fd87 e51a 8b50 ba1a 9195 ec51 0a48  .......P.....Q.H
+00002c10: 8be5 62d8 ecd5 46f1 b832 8c45 f853 5083  ..b...F..2.E.SP.
+00002c20: f241 7874 bf03 a18c 0ee4 2827 49fc 9589  .Axt......('I...
+00002c30: ee5b a288 1469 5274 c232 1389 885c 6d8e  .[...iRt.2...\m.
+00002c40: 0fc6 d2c9 6806 b92d ac91 3213 93be f181  ....h..-..2.....
+00002c50: 96a9 3893 b761 cd77 c85d a730 e46f c173  ..8..a.w.].0.o.s
+00002c60: 2666 8907 5664 1d77 131d 1ffc 9207 f4c3  &f..Vd.w........
+00002c70: 7dd5 b2b9 23c9 68d7 c078 6f4d db90 de75  }...#.h..xoM...u
+00002c80: 186f 231e f9e8 a218 ce48 83c2 4c3c 2143  .o#......H..L<!C
+00002c90: 090c 610b af6e ca7e 23f6 a891 3f3b 27df  ..a..n.~#...?;'.
+00002ca0: b09b b287 8e01 2b09 cea1 1bdd 4f2f dc4f  ......+.....O/.O
+00002cb0: cfee fbd4 9b10 c91f c4f4 0262 dafb 1acc  ...........b....
+00002cc0: 9458 91c6 f2d9 c35c 68f8 680b ffae e1e8  .X.....\h.h.....
+00002cd0: cca4 d737 935b 1f61 2be5 ca6b 2ffa d140  ...7.[.a+..k/..@
+00002ce0: f993 cef0 b4cb 6f50 4b03 0414 0000 0008  ......oPK.......
+00002cf0: 0060 50f8 560b 085d 06bc 0000 001f 0300  .`P.V..]........
+00002d00: 001a 0000 0078 6c2f 5f72 656c 732f 776f  .....xl/_rels/wo
+00002d10: 726b 626f 6f6b 2e78 6d6c 2e72 656c 73cd  rkbook.xml.rels.
+00002d20: 9339 0e83 3010 45af 62f9 000c 4b92 2282  .9..0.E.b...K.".
+00002d30: 5469 6823 2e60 c1b0 88c5 9667 a2c0 ed83  Tih#.`.....g....
+00002d40: a000 4b29 d2a0 a4b2 fe58 7eff 15e3 f881  ..K).....X~.....
+00002d50: 9de2 460f 5437 86c4 d877 0325 b266 3657  ..F.T7...w.%.f6W
+00002d60: 00ca 6bec 1579 dae0 30df 94da f68a e768  ..k..y..0......h
+00002d70: 2b30 2a6f 5585 10fa fe05 ec9e 216f f19e  +0*oU.......!o..
+00002d80: 29b2 c9e0 3744 5d96 4d8e 779d 3f7b 1cf8  )...7D].M.w.?{..
+00002d90: 0318 5eda b654 23b2 1499 b215 7222 61ec  ..^..T#.....r"a.
+00002da0: b631 c172 04de 4c96 222d 1269 d322 9002  .1.r..L."-.i."..
+00002db0: 7e6d 143a 46e1 1f18 458e 5174 a411 f1d4  ~m.:F...E.Qt....
+00002dc0: 216d 3a6b 76fa 4f47 f6f3 fc16 b7fa 25ae  !m:kv.OG......%.
+00002dd0: 4377 51ce 8b04 38ff e1f6 0650 4b03 0414  CwQ...8....PK...
+00002de0: 0000 0008 0060 50f8 56db fbce 8f24 0100  .....`P.V....$..
+00002df0: 00e9 0400 0013 0000 005b 436f 6e74 656e  .........[Conten
+00002e00: 745f 5479 7065 735d 2e78 6d6c cd54 cb4e  t_Types].xml.T.N
+00002e10: c330 10fc 95c8 d72a 7129 1207 d4f4 025c  .0.....*q).....\
+00002e20: a107 7ec0 249b c68a 5ff2 6e4b faf7 6c12  ..~.$..._.nK..l.
+00002e30: 1a09 545a aa20 d14b ac78 6767 c63b b297  ..TZ. .K.xgg.;..
+00002e40: affb 0098 b4d6 38cc 454d 14ee a5c4 a206  ......8.EM......
+00002e50: ab30 f301 1c57 2a1f ad22 fe8d 1b19 54d1  .0...W*.."....T.
+00002e60: a80d c8c5 7c7e 270b ef08 1ca5 d471 88d5  ....|~'......q..
+00002e70: f211 2ab5 3594 3cb5 bc8d dabb 5c44 3028  ..*.5.<.....\D0(
+00002e80: 9287 01d8 69e5 4285 6074 a188 eb72 e7ca  ....i.B.`t...r..
+00002e90: 6f2a e9a7 42c6 9d3d 066b 1d70 c600 91c8  o*..B..=.k.p....
+00002ea0: a312 7de9 4785 43e3 cb0e 62d4 2524 6b15  ..}.G.C...b.%$k.
+00002eb0: e959 5986 c9d6 48a4 bd01 cc4e 731c 71e9  .YY...H....Ns.q.
+00002ec0: ab4a 1750 fa62 6bb9 25c3 1041 9558 0390  .J.P.bk.%..A.X..
+00002ed0: 35d9 403a 3b23 4d3c 6418 be37 930d f434  5.@:;#M<d..7...4
+00002ee0: 2715 19ba 8e3e 20a7 16e1 72bd 432c 5d77  '....> ...r.C,]w
+00002ef0: 1a98 0822 e933 871c 2599 7bf2 09a1 4bbc  ...".3..%.{...K.
+00002f00: 84f2 b7e2 3ce1 771f 9b3e 1394 fd32 7dcc  ....<.w..>...2}.
+00002f10: 5f73 1ef9 2f35 b2b8 1623 b7ff 69e4 cdfb  _s../5...#..i...
+00002f20: e6af 6f5e b766 5669 371a 90fd 0bb7 fa00  ..o^.fVi7.......
+00002f30: 504b 0102 1403 1400 0000 0800 6050 f856  PK..........`P.V
+00002f40: 465a c10c 8200 0000 b100 0000 1000 0000  FZ..............
+00002f50: 0000 0000 0000 0000 8001 0000 0000 646f  ..............do
+00002f60: 6350 726f 7073 2f61 7070 2e78 6d6c 504b  cProps/app.xmlPK
+00002f70: 0102 1403 1400 0000 0800 6050 f856 db74  ..........`P.V.t
+00002f80: 89e1 ec00 0000 cb01 0000 1100 0000 0000  ................
+00002f90: 0000 0000 0000 8001 b000 0000 646f 6350  ............docP
+00002fa0: 726f 7073 2f63 6f72 652e 786d 6c50 4b01  rops/core.xmlPK.
+00002fb0: 0214 0314 0000 0008 0060 50f8 5699 5c9c  .........`P.V.\.
+00002fc0: 2310 0600 009c 2700 0013 0000 0000 0000  #.....'.........
+00002fd0: 0000 0000 0080 01cb 0100 0078 6c2f 7468  ...........xl/th
+00002fe0: 656d 652f 7468 656d 6531 2e78 6d6c 504b  eme/theme1.xmlPK
+00002ff0: 0102 1403 1400 0000 0800 6050 f856 e0d9  ..........`P.V..
+00003000: 6c24 3d02 0000 a307 0000 1800 0000 0000  l$=.............
+00003010: 0000 0000 0000 8081 0c08 0000 786c 2f77  ............xl/w
+00003020: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+00003030: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+00003040: 6050 f856 19c6 63fc 000e 0000 bb83 0000  `P.V..c.........
+00003050: 1800 0000 0000 0000 0000 0000 8081 7f0a  ................
+00003060: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00003070: 7368 6565 7432 2e78 6d6c 504b 0102 1403  sheet2.xmlPK....
+00003080: 1400 0000 0800 6050 f856 0e2f c9cf c20e  ......`P.V./....
+00003090: 0000 6f8b 0000 1800 0000 0000 0000 0000  ..o.............
+000030a0: 0000 8081 b518 0000 786c 2f77 6f72 6b73  ........xl/works
+000030b0: 6865 6574 732f 7368 6565 7433 2e78 6d6c  heets/sheet3.xml
+000030c0: 504b 0102 1403 1400 0000 0800 6050 f856  PK..........`P.V
+000030d0: f7f6 8f09 a702 0000 6d0b 0000 0d00 0000  ........m.......
+000030e0: 0000 0000 0000 0000 8001 ad27 0000 786c  ...........'..xl
+000030f0: 2f73 7479 6c65 732e 786d 6c50 4b01 0214  /styles.xmlPK...
+00003100: 0314 0000 0008 0060 50f8 56b7 47eb 8ac0  .......`P.V.G...
+00003110: 0000 0016 0200 000b 0000 0000 0000 0000  ................
+00003120: 0000 0080 017f 2a00 005f 7265 6c73 2f2e  ......*.._rels/.
+00003130: 7265 6c73 504b 0102 1403 1400 0000 0800  relsPK..........
+00003140: 6050 f856 b948 9c76 5201 0000 ae02 0000  `P.V.H.vR.......
+00003150: 0f00 0000 0000 0000 0000 0000 8001 682b  ..............h+
+00003160: 0000 786c 2f77 6f72 6b62 6f6f 6b2e 786d  ..xl/workbook.xm
+00003170: 6c50 4b01 0214 0314 0000 0008 0060 50f8  lPK..........`P.
+00003180: 560b 085d 06bc 0000 001f 0300 001a 0000  V..]............
+00003190: 0000 0000 0000 0000 0080 01e7 2c00 0078  ............,..x
+000031a0: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
+000031b0: 2e78 6d6c 2e72 656c 7350 4b01 0214 0314  .xml.relsPK.....
+000031c0: 0000 0008 0060 50f8 56db fbce 8f24 0100  .....`P.V....$..
+000031d0: 00e9 0400 0013 0000 0000 0000 0000 0000  ................
+000031e0: 0080 01db 2d00 005b 436f 6e74 656e 745f  ....-..[Content_
+000031f0: 5479 7065 735d 2e78 6d6c 504b 0506 0000  Types].xmlPK....
+00003200: 0000 0b00 0b00 ca02 0000 302f 0000 0000  ..........0/....
```

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/ontologies/wind-energy.owl` & `cognite_neat-0.17.3/cognite/neat/examples/ontologies/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.17.3/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/rules/power-grid-example.xlsx` & `cognite_neat-0.17.3/cognite/neat/examples/rules/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/rules/rules-template.xlsx` & `cognite_neat-0.17.3/cognite/neat/examples/rules/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.17.3/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.17.3/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.17.3/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.17.3/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.17.3/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.17.3/cognite/neat/examples/workflows/default/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.17.3/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py` & `cognite_neat-0.17.3/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml` & `cognite_neat-0.17.3/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.17.3/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.17.3/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml` & `cognite_neat-0.17.3/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.17.3/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml` & `cognite_neat-0.17.3/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.17.3/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer/explorer.py` & `cognite_neat-0.17.3/cognite/neat/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.17.3/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="./favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="NEAT controll panel"/><link rel="apple-touch-icon" href="./logo192.png"/><link rel="manifest" href="./manifest.json"/><title>React App</title><script defer="defer" src="./static/js/main.16555d84.js"></script><link href="./static/css/main.38a62222.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="./favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="NEAT controll panel"/><link rel="apple-touch-icon" href="./logo192.png"/><link rel="manifest" href="./manifest.json"/><title>React App</title><script defer="defer" src="./static/js/main.694f3f8e.js"></script><link href="./static/css/main.38a62222.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js` & `cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.694f3f8e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.16555d84.js.LICENSE.txt */ ! function() {
+/*! For license information please see main.694f3f8e.js.LICENSE.txt */ ! function() {
     var e = {
             3361: function(e, t, n) {
                 "use strict";
                 n.d(t, {
                     Z: function() {
                         return oe
                     }
@@ -58690,15 +58690,15 @@
                     return (0, e.useEffect)((function() {
                         t({
                             rightClickNode: function(e) {
                                 console.log("clickNode", e.event, e.node), console.log("node id: " + e.node), j("update"), C(e.node),
                                     function(e) {
                                         var t = "",
                                             n = localStorage.getItem("nodeNameProperty");
-                                        t = n ? "SELECT ?node_name (?linked_obj_type  AS ?node_class) (?dst_object_ref AS ?node_id) ?src_object_ref ?dst_object_ref WHERE {\n          BIND( <" + e + "> AS ?src_object_ref )\n          { \n           ?src_object_ref ?rel_propery ?dst_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type .\n           ?dst_object_ref " + n + " ?node_name . \n          }\n          UNION \n          {\n           ?dst_object_ref ?rel_propery ?src_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type . \n           ?dst_object_ref " + n + " ?node_name .\n          }             \n          } " : "SELECT (?dst_object_ref AS ?node_name) (?linked_obj_type  AS ?node_class) (?dst_object_ref AS ?node_id) ?src_object_ref ?dst_object_ref WHERE {\n          BIND( <" + e + "> AS ?src_object_ref )\n          { \n           ?src_object_ref ?rel_propery ?dst_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type \n          }\n          UNION \n          {\n           ?dst_object_ref ?rel_propery ?src_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type . \n          }             \n          }  ", console.log("requesting linked nodes"), M(t)
+                                        t = n ? "SELECT ?node_name (?linked_obj_type  AS ?node_class) (?dst_object_ref AS ?node_id) ?src_object_ref ?dst_object_ref WHERE {\n          BIND( <" + e + "> AS ?src_object_ref )\n          {\n           ?src_object_ref ?rel_propery ?dst_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type .\n           ?dst_object_ref " + n + " ?node_name .\n          }\n          UNION\n          {\n           ?dst_object_ref ?rel_propery ?src_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type .\n           ?dst_object_ref " + n + " ?node_name .\n          }\n          } " : "SELECT (?dst_object_ref AS ?node_name) (?linked_obj_type  AS ?node_class) (?dst_object_ref AS ?node_id) ?src_object_ref ?dst_object_ref WHERE {\n          BIND( <" + e + "> AS ?src_object_ref )\n          {\n           ?src_object_ref ?rel_propery ?dst_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type\n          }\n          UNION\n          {\n           ?dst_object_ref ?rel_propery ?src_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type .\n          }\n          }  ", console.log("requesting linked nodes"), M(t)
                                     }(e.node), n.getGraph().setNodeAttribute(e.node, "highlighted", !0)
                             },
                             doubleClickNode: function(e) {
                                 C(e.node), y(!0)
                             },
                             mouseup: function(e) {
                                 a && (l(null), n.getGraph().removeNodeAttribute(a, "highlighted"))
@@ -59321,15 +59321,15 @@
                                 onClick: function(t) {
                                     K(e.value)
                                 },
                                 children: "Table "
                             }), " ", (0, E.jsx)(Kn, {
                                 onClick: function(t) {
                                     ! function(e) {
-                                        A(2), q = localStorage.getItem("nodeNameProperty"), V(q ? "SELECT ?node_name ?node_class (?inst AS ?node_id) WHERE { \n        BIND( <" + e + "> AS ?inst)\n        ?inst " + q + " ?node_name .\n        ?inst rdf:type ?node_class . \n        } " : "SELECT (?inst AS ?node_name) ?node_class (?inst AS ?node_id) WHERE { \n        BIND( <" + e + "> AS ?inst)\n        ?inst rdf:type ?node_class . \n        } ")
+                                        A(2), q = localStorage.getItem("nodeNameProperty"), V(q ? "SELECT ?node_name ?node_class (?inst AS ?node_id) WHERE {\n        BIND( <" + e + "> AS ?inst)\n        ?inst " + q + " ?node_name .\n        ?inst rdf:type ?node_class .\n        } " : "SELECT (?inst AS ?node_name) ?node_class (?inst AS ?node_id) WHERE {\n        BIND( <" + e + "> AS ?inst)\n        ?inst rdf:type ?node_class .\n        } ")
                                     }(e.value)
                                 },
                                 children: "Graph "
                             })]
                         });
                         if (null !== (n = e.value) && void 0 !== n && n.includes("#") && R) {
                             var i = An(e.value);
@@ -60439,14 +60439,17 @@
                                 label: "Step type",
                                 size: "small",
                                 variant: "outlined",
                                 onChange: function(e) {
                                     x("stype", e.target.value)
                                 },
                                 children: [(0, E.jsx)(gv, {
+                                    value: "stdstep",
+                                    children: "Step from standard library"
+                                }), (0, E.jsx)(gv, {
                                     value: "pystep",
                                     children: "Python function"
                                 }), (0, E.jsx)(gv, {
                                     value: "http_trigger",
                                     children: "HTTP trigger"
                                 }), (0, E.jsx)(gv, {
                                     value: "time_trigger",
@@ -60489,14 +60492,27 @@
                                 label: "Time interval",
                                 size: "small",
                                 variant: "outlined",
                                 value: null === s || void 0 === s ? void 0 : s.params.interval,
                                 onChange: function(e) {
                                     x("time-interval", e.target.value)
                                 }
+                            }), "stdstep" == (null === s || void 0 === s ? void 0 : s.stype) && (0, E.jsx)(fg, {
+                                sx: {
+                                    marginTop: 1
+                                },
+                                id: "step-stdstep-method",
+                                fullWidth: !0,
+                                label: "Name of the step",
+                                size: "small",
+                                variant: "outlined",
+                                value: null === s || void 0 === s ? void 0 : s.method,
+                                onChange: function(e) {
+                                    x("method", e.target.value)
+                                }
                             }), "pystep" == (null === s || void 0 === s ? void 0 : s.stype) && (0, E.jsx)(fg, {
                                 sx: {
                                     marginTop: 1
                                 },
                                 id: "step-pystep-method",
                                 fullWidth: !0,
                                 label: "Override function name (optional)",
@@ -62154,8 +62170,8 @@
                 })
             };
             r.createRoot(document.getElementById("root")).render((0, E.jsxs)(e.Fragment, {
                 children: [(0, E.jsx)(dO, {}), (0, E.jsx)(uO, {})]
             }))
         }()
 }();
-//# sourceMappingURL=main.16555d84.js.map
+//# sourceMappingURL=main.694f3f8e.js.map
```

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt` & `cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map` & `cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.694f3f8e.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8565203859321506%*

 * *Differences: {"'file'": "'static/js/main.694f3f8e.js'",*

 * * "'mappings'": "';sFAqDA,IAAIA,EAA0B,WAE5B,SAASA,EAAWC,GAClB,IAAIC,EAAQC,KAEZA,KAAKC,WAAa,SAAUC,GAC1B,IAAIC,EAIAA,EAFsB,IAAtBJ,EAAMK,KAAKC,OACTN,EAAMO,eACCP,EAAMO,eAAeC,YACrBR,EAAMS,QACNT,EAAMU,UAAUC,WAEhBX,EAAMI,OAGRJ,EAAMK,KAAKL,EAAMK,KAAKC,OAAS,GAAGE,YAG7CR,EAAMU,UAAUE,aAAaT,EAAKC,GAElCJ,EAAMK,KAAKQ,KAAKV,EAClB,EAEAF,KAAKa,cAA8BC,IAAnBhB,EAAQiB,QAA+DjB,EAAQiB,OAC/Ff,KAAKI,KAAO,GACZJ,KAAKgB,IAAM,EACXhB,KAAKiB,MAAQnB,EAAQmB,MAErBjB,KAAKkB,IAAMpB,EAAQoB,IACnBlB,KAA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.16555d84.js",
+    "file": "static/js/main.694f3f8e.js",
     "names": [
         "StyleSheet",
         "options",
         "_this",
         "this",
         "_insertTag",
         "tag",
@@ -12045,15 +12045,15 @@
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getTableRowUtilityClass(slot) {\n  return generateUtilityClass('MuiTableRow', slot);\n}\nconst tableRowClasses = generateUtilityClasses('MuiTableRow', ['root', 'selected', 'hover', 'head', 'footer']);\nexport default tableRowClasses;",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\nimport _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nconst _excluded = [\"className\", \"component\", \"hover\", \"selected\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport { alpha } from '@mui/system';\nimport Tablelvl2Context from '../Table/Tablelvl2Context';\nimport useThemeProps from '../styles/useThemeProps';\nimport styled from '../styles/styled';\nimport tableRowClasses, { getTableRowUtilityClass } from './tableRowClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    classes,\n    selected,\n    hover,\n    head,\n    footer\n  } = ownerState;\n  const slots = {\n    root: ['root', selected && 'selected', hover && 'hover', head && 'head', footer && 'footer']\n  };\n  return composeClasses(slots, getTableRowUtilityClass, classes);\n};\nconst TableRowRoot = styled('tr', {\n  name: 'MuiTableRow',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.root, ownerState.head && styles.head, ownerState.footer && styles.footer];\n  }\n})(({\n  theme\n}) => ({\n  color: 'inherit',\n  display: 'table-row',\n  verticalAlign: 'middle',\n  // We disable the focus ring for mouse, touch and keyboard users.\n  outline: 0,\n  [`&.${tableRowClasses.hover}:hover`]: {\n    backgroundColor: (theme.vars || theme).palette.action.hover\n  },\n  [`&.${tableRowClasses.selected}`]: {\n    backgroundColor: theme.vars ? `rgba(${theme.vars.palette.primary.mainChannel} / ${theme.vars.palette.action.selectedOpacity})` : alpha(theme.palette.primary.main, theme.palette.action.selectedOpacity),\n    '&:hover': {\n      backgroundColor: theme.vars ? `rgba(${theme.vars.palette.primary.mainChannel} / calc(${theme.vars.palette.action.selectedOpacity} + ${theme.vars.palette.action.hoverOpacity}))` : alpha(theme.palette.primary.main, theme.palette.action.selectedOpacity + theme.palette.action.hoverOpacity)\n    }\n  }\n}));\nconst defaultComponent = 'tr';\n/**\n * Will automatically set dynamic row height\n * based on the material table element parent (head, body, etc).\n */\nconst TableRow = /*#__PURE__*/React.forwardRef(function TableRow(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiTableRow'\n  });\n  const {\n      className,\n      component = defaultComponent,\n      hover = false,\n      selected = false\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const tablelvl2 = React.useContext(Tablelvl2Context);\n  const ownerState = _extends({}, props, {\n    component,\n    hover,\n    selected,\n    head: tablelvl2 && tablelvl2.variant === 'head',\n    footer: tablelvl2 && tablelvl2.variant === 'footer'\n  });\n  const classes = useUtilityClasses(ownerState);\n  return /*#__PURE__*/_jsx(TableRowRoot, _extends({\n    as: component,\n    ref: ref,\n    className: clsx(classes.root, className),\n    role: component === defaultComponent ? null : 'row',\n    ownerState: ownerState\n  }, other));\n});\nprocess.env.NODE_ENV !== \"production\" ? TableRow.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * Should be valid <tr> children such as `TableCell`.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n  /**\n   * If `true`, the table row will shade on hover.\n   * @default false\n   */\n  hover: PropTypes.bool,\n  /**\n   * If `true`, the table row will have the selected shading.\n   * @default false\n   */\n  selected: PropTypes.bool,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nexport default TableRow;",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getTypographyUtilityClass(slot) {\n  return generateUtilityClass('MuiTypography', slot);\n}\nconst typographyClasses = generateUtilityClasses('MuiTypography', ['root', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'subtitle1', 'subtitle2', 'body1', 'body2', 'inherit', 'button', 'caption', 'overline', 'alignLeft', 'alignRight', 'alignCenter', 'alignJustify', 'noWrap', 'gutterBottom', 'paragraph']);\nexport default typographyClasses;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"align\", \"className\", \"component\", \"gutterBottom\", \"noWrap\", \"paragraph\", \"variant\", \"variantMapping\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_extendSxProp as extendSxProp } from '@mui/system';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport styled from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nimport capitalize from '../utils/capitalize';\nimport { getTypographyUtilityClass } from './typographyClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    align,\n    gutterBottom,\n    noWrap,\n    paragraph,\n    variant,\n    classes\n  } = ownerState;\n  const slots = {\n    root: ['root', variant, ownerState.align !== 'inherit' && `align${capitalize(align)}`, gutterBottom && 'gutterBottom', noWrap && 'noWrap', paragraph && 'paragraph']\n  };\n  return composeClasses(slots, getTypographyUtilityClass, classes);\n};\nexport const TypographyRoot = styled('span', {\n  name: 'MuiTypography',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.root, ownerState.variant && styles[ownerState.variant], ownerState.align !== 'inherit' && styles[`align${capitalize(ownerState.align)}`], ownerState.noWrap && styles.noWrap, ownerState.gutterBottom && styles.gutterBottom, ownerState.paragraph && styles.paragraph];\n  }\n})(({\n  theme,\n  ownerState\n}) => _extends({\n  margin: 0\n}, ownerState.variant && theme.typography[ownerState.variant], ownerState.align !== 'inherit' && {\n  textAlign: ownerState.align\n}, ownerState.noWrap && {\n  overflow: 'hidden',\n  textOverflow: 'ellipsis',\n  whiteSpace: 'nowrap'\n}, ownerState.gutterBottom && {\n  marginBottom: '0.35em'\n}, ownerState.paragraph && {\n  marginBottom: 16\n}));\nconst defaultVariantMapping = {\n  h1: 'h1',\n  h2: 'h2',\n  h3: 'h3',\n  h4: 'h4',\n  h5: 'h5',\n  h6: 'h6',\n  subtitle1: 'h6',\n  subtitle2: 'h6',\n  body1: 'p',\n  body2: 'p',\n  inherit: 'p'\n};\n\n// TODO v6: deprecate these color values in v5.x and remove the transformation in v6\nconst colorTransformations = {\n  primary: 'primary.main',\n  textPrimary: 'text.primary',\n  secondary: 'secondary.main',\n  textSecondary: 'text.secondary',\n  error: 'error.main'\n};\nconst transformDeprecatedColors = color => {\n  return colorTransformations[color] || color;\n};\nconst Typography = /*#__PURE__*/React.forwardRef(function Typography(inProps, ref) {\n  const themeProps = useThemeProps({\n    props: inProps,\n    name: 'MuiTypography'\n  });\n  const color = transformDeprecatedColors(themeProps.color);\n  const props = extendSxProp(_extends({}, themeProps, {\n    color\n  }));\n  const {\n      align = 'inherit',\n      className,\n      component,\n      gutterBottom = false,\n      noWrap = false,\n      paragraph = false,\n      variant = 'body1',\n      variantMapping = defaultVariantMapping\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const ownerState = _extends({}, props, {\n    align,\n    color,\n    className,\n    component,\n    gutterBottom,\n    noWrap,\n    paragraph,\n    variant,\n    variantMapping\n  });\n  const Component = component || (paragraph ? 'p' : variantMapping[variant] || defaultVariantMapping[variant]) || 'span';\n  const classes = useUtilityClasses(ownerState);\n  return /*#__PURE__*/_jsx(TypographyRoot, _extends({\n    as: Component,\n    ref: ref,\n    ownerState: ownerState,\n    className: clsx(classes.root, className)\n  }, other));\n});\nprocess.env.NODE_ENV !== \"production\" ? Typography.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * Set the text-align on the component.\n   * @default 'inherit'\n   */\n  align: PropTypes.oneOf(['center', 'inherit', 'justify', 'left', 'right']),\n  /**\n   * The content of the component.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n  /**\n   * If `true`, the text will have a bottom margin.\n   * @default false\n   */\n  gutterBottom: PropTypes.bool,\n  /**\n   * If `true`, the text will not wrap, but instead will truncate with a text overflow ellipsis.\n   *\n   * Note that text overflow can only happen with block or inline-block level elements\n   * (the element needs to have a width in order to overflow).\n   * @default false\n   */\n  noWrap: PropTypes.bool,\n  /**\n   * If `true`, the element will be a paragraph element.\n   * @default false\n   */\n  paragraph: PropTypes.bool,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object]),\n  /**\n   * Applies the theme typography styles.\n   * @default 'body1'\n   */\n  variant: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['body1', 'body2', 'button', 'caption', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'inherit', 'overline', 'subtitle1', 'subtitle2']), PropTypes.string]),\n  /**\n   * The component maps the variant prop to a range of different HTML element types.\n   * For instance, subtitle1 to `<h6>`.\n   * If you wish to change that mapping, you can provide your own.\n   * Alternatively, you can use the `component` prop.\n   * @default {\n   *   h1: 'h1',\n   *   h2: 'h2',\n   *   h3: 'h3',\n   *   h4: 'h4',\n   *   h5: 'h5',\n   *   h6: 'h6',\n   *   subtitle1: 'h6',\n   *   subtitle2: 'h6',\n   *   body1: 'p',\n   *   body2: 'p',\n   *   inherit: 'p',\n   * }\n   */\n  variantMapping: PropTypes /* @typescript-to-proptypes-ignore */.object\n} : void 0;\nexport default Typography;",
         "// Inspired by https://github.com/material-components/material-components-ios/blob/bca36107405594d5b7b16265a5b0ed698f85a5ee/components/Elevation/src/UIColor%2BMaterialElevation.m#L61\nconst getOverlayAlpha = elevation => {\n  let alphaValue;\n  if (elevation < 1) {\n    alphaValue = 5.11916 * elevation ** 2;\n  } else {\n    alphaValue = 4.5 * Math.log(elevation + 1) + 2;\n  }\n  return (alphaValue / 100).toFixed(2);\n};\nexport default getOverlayAlpha;",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getPaperUtilityClass(slot) {\n  return generateUtilityClass('MuiPaper', slot);\n}\nconst paperClasses = generateUtilityClasses('MuiPaper', ['root', 'rounded', 'outlined', 'elevation', 'elevation0', 'elevation1', 'elevation2', 'elevation3', 'elevation4', 'elevation5', 'elevation6', 'elevation7', 'elevation8', 'elevation9', 'elevation10', 'elevation11', 'elevation12', 'elevation13', 'elevation14', 'elevation15', 'elevation16', 'elevation17', 'elevation18', 'elevation19', 'elevation20', 'elevation21', 'elevation22', 'elevation23', 'elevation24']);\nexport default paperClasses;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"className\", \"component\", \"elevation\", \"square\", \"variant\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { chainPropTypes, integerPropType } from '@mui/utils';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport { alpha } from '@mui/system';\nimport styled from '../styles/styled';\nimport getOverlayAlpha from '../styles/getOverlayAlpha';\nimport useThemeProps from '../styles/useThemeProps';\nimport useTheme from '../styles/useTheme';\nimport { getPaperUtilityClass } from './paperClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    square,\n    elevation,\n    variant,\n    classes\n  } = ownerState;\n  const slots = {\n    root: ['root', variant, !square && 'rounded', variant === 'elevation' && `elevation${elevation}`]\n  };\n  return composeClasses(slots, getPaperUtilityClass, classes);\n};\nconst PaperRoot = styled('div', {\n  name: 'MuiPaper',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.root, styles[ownerState.variant], !ownerState.square && styles.rounded, ownerState.variant === 'elevation' && styles[`elevation${ownerState.elevation}`]];\n  }\n})(({\n  theme,\n  ownerState\n}) => {\n  var _theme$vars$overlays;\n  return _extends({\n    backgroundColor: (theme.vars || theme).palette.background.paper,\n    color: (theme.vars || theme).palette.text.primary,\n    transition: theme.transitions.create('box-shadow')\n  }, !ownerState.square && {\n    borderRadius: theme.shape.borderRadius\n  }, ownerState.variant === 'outlined' && {\n    border: `1px solid ${(theme.vars || theme).palette.divider}`\n  }, ownerState.variant === 'elevation' && _extends({\n    boxShadow: (theme.vars || theme).shadows[ownerState.elevation]\n  }, !theme.vars && theme.palette.mode === 'dark' && {\n    backgroundImage: `linear-gradient(${alpha('#fff', getOverlayAlpha(ownerState.elevation))}, ${alpha('#fff', getOverlayAlpha(ownerState.elevation))})`\n  }, theme.vars && {\n    backgroundImage: (_theme$vars$overlays = theme.vars.overlays) == null ? void 0 : _theme$vars$overlays[ownerState.elevation]\n  }));\n});\nconst Paper = /*#__PURE__*/React.forwardRef(function Paper(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiPaper'\n  });\n  const {\n      className,\n      component = 'div',\n      elevation = 1,\n      square = false,\n      variant = 'elevation'\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const ownerState = _extends({}, props, {\n    component,\n    elevation,\n    square,\n    variant\n  });\n  const classes = useUtilityClasses(ownerState);\n  if (process.env.NODE_ENV !== 'production') {\n    // eslint-disable-next-line react-hooks/rules-of-hooks\n    const theme = useTheme();\n    if (theme.shadows[elevation] === undefined) {\n      console.error([`MUI: The elevation provided <Paper elevation={${elevation}}> is not available in the theme.`, `Please make sure that \\`theme.shadows[${elevation}]\\` is defined.`].join('\\n'));\n    }\n  }\n  return /*#__PURE__*/_jsx(PaperRoot, _extends({\n    as: component,\n    ownerState: ownerState,\n    className: clsx(classes.root, className),\n    ref: ref\n  }, other));\n});\nprocess.env.NODE_ENV !== \"production\" ? Paper.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * The content of the component.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n  /**\n   * Shadow depth, corresponds to `dp` in the spec.\n   * It accepts values between 0 and 24 inclusive.\n   * @default 1\n   */\n  elevation: chainPropTypes(integerPropType, props => {\n    const {\n      elevation,\n      variant\n    } = props;\n    if (elevation > 0 && variant === 'outlined') {\n      return new Error(`MUI: Combining \\`elevation={${elevation}}\\` with \\`variant=\"${variant}\"\\` has no effect. Either use \\`elevation={0}\\` or use a different \\`variant\\`.`);\n    }\n    return null;\n  }),\n  /**\n   * If `true`, rounded corners are disabled.\n   * @default false\n   */\n  square: PropTypes.bool,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object]),\n  /**\n   * The variant to use.\n   * @default 'elevation'\n   */\n  variant: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['elevation', 'outlined']), PropTypes.string])\n} : void 0;\nexport default Paper;",
-        "\n\nexport function getSelectedWorkflowName() {\n  let workflowName = localStorage.getItem(\"selectedWorkflowName\");\n  if (workflowName == null) {\n    workflowName = \"default\";\n  }\n  return workflowName;\n}\nexport function setSelectedWorkflowName(workflowName: string) {\n  localStorage.setItem(\"selectedWorkflowName\", workflowName);\n}\n\nexport function getNeatApiRootUrl() {\n  let url = localStorage.getItem(\"neatApiRootUrl\");\n  if (url == null) {\n    // url = \"http://localhost:8000\";\n    const protocol = window.location.protocol;\n    const domain = window.location.hostname;\n    const port = window.location.port;\n    url = protocol + \"//\" + domain + \":\" + port;\n  }\n  return url;\n}\n\nexport function convertMillisToStr(millis) {\n  const date = new Date(millis);\n  const isoString = date.toISOString();\n  return isoString;\n}\n\nexport function getShortenedString(str,len) {\n  str = RemoveNsPrefix(str);\n  if (str.length <= len) {\n    return str;\n  } else {\n    return str.slice(0,len)+\"...\"+ str.slice(-len);\n  }\n}\n\nexport default function RemoveNsPrefix(strWithPrefix: string) {\n\n  if (strWithPrefix.includes(\"#\"))\n  {\n    const strPlit = strWithPrefix.split(\"#\")\n    if (strPlit.length > 1) {\n      return strPlit[1]\n    }\n  }else if (strWithPrefix.includes(\"/\")) {\n    const strPlit = strWithPrefix.split(\"/\")\n    if (strPlit.length > 1) {\n      return strPlit[strPlit.length-1]\n    }\n  }\n\n  return strWithPrefix;\n}\n\n",
+        "\n\nexport function getSelectedWorkflowName() {\n  let workflowName = localStorage.getItem(\"selectedWorkflowName\");\n  if (workflowName == null) {\n    workflowName = \"default\";\n  }\n  return workflowName;\n}\nexport function setSelectedWorkflowName(workflowName: string) {\n  localStorage.setItem(\"selectedWorkflowName\", workflowName);\n}\n\nexport function getNeatApiRootUrl() {\n  let url = localStorage.getItem(\"neatApiRootUrl\");\n  if (url == null) {\n    // url = \"http://localhost:8000\";\n    const protocol = window.location.protocol;\n    const domain = window.location.hostname;\n    const port = window.location.port;\n    url = protocol + \"//\" + domain + \":\" + port;\n  }\n  return url;\n}\n\nexport function convertMillisToStr(millis) {\n  const date = new Date(millis);\n  const isoString = date.toISOString();\n  return isoString;\n}\n\nexport function getShortenedString(str,len) {\n  str = RemoveNsPrefix(str);\n  if (str.length <= len) {\n    return str;\n  } else {\n    return str.slice(0,len)+\"...\"+ str.slice(-len);\n  }\n}\n\nexport default function RemoveNsPrefix(strWithPrefix: string) {\n\n  if (strWithPrefix.includes(\"#\"))\n  {\n    const strPlit = strWithPrefix.split(\"#\")\n    if (strPlit.length > 1) {\n      return strPlit[1]\n    }\n  }else if (strWithPrefix.includes(\"/\")) {\n    const strPlit = strWithPrefix.split(\"/\")\n    if (strPlit.length > 1) {\n      return strPlit[strPlit.length-1]\n    }\n  }\n\n  return strWithPrefix;\n}\n",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getButtonUtilityClass(slot) {\n  return generateUtilityClass('MuiButton', slot);\n}\nconst buttonClasses = generateUtilityClasses('MuiButton', ['root', 'text', 'textInherit', 'textPrimary', 'textSecondary', 'textSuccess', 'textError', 'textInfo', 'textWarning', 'outlined', 'outlinedInherit', 'outlinedPrimary', 'outlinedSecondary', 'outlinedSuccess', 'outlinedError', 'outlinedInfo', 'outlinedWarning', 'contained', 'containedInherit', 'containedPrimary', 'containedSecondary', 'containedSuccess', 'containedError', 'containedInfo', 'containedWarning', 'disableElevation', 'focusVisible', 'disabled', 'colorInherit', 'textSizeSmall', 'textSizeMedium', 'textSizeLarge', 'outlinedSizeSmall', 'outlinedSizeMedium', 'outlinedSizeLarge', 'containedSizeSmall', 'containedSizeMedium', 'containedSizeLarge', 'sizeMedium', 'sizeSmall', 'sizeLarge', 'fullWidth', 'startIcon', 'endIcon', 'iconSizeSmall', 'iconSizeMedium', 'iconSizeLarge']);\nexport default buttonClasses;",
         "import * as React from 'react';\n/**\n * @ignore - internal component.\n */\nconst ButtonGroupContext = /*#__PURE__*/React.createContext({});\nif (process.env.NODE_ENV !== 'production') {\n  ButtonGroupContext.displayName = 'ButtonGroupContext';\n}\nexport default ButtonGroupContext;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"children\", \"color\", \"component\", \"className\", \"disabled\", \"disableElevation\", \"disableFocusRipple\", \"endIcon\", \"focusVisibleClassName\", \"fullWidth\", \"size\", \"startIcon\", \"type\", \"variant\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { internal_resolveProps as resolveProps } from '@mui/utils';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport { alpha } from '@mui/system';\nimport styled, { rootShouldForwardProp } from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nimport ButtonBase from '../ButtonBase';\nimport capitalize from '../utils/capitalize';\nimport buttonClasses, { getButtonUtilityClass } from './buttonClasses';\nimport ButtonGroupContext from '../ButtonGroup/ButtonGroupContext';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    color,\n    disableElevation,\n    fullWidth,\n    size,\n    variant,\n    classes\n  } = ownerState;\n  const slots = {\n    root: ['root', variant, `${variant}${capitalize(color)}`, `size${capitalize(size)}`, `${variant}Size${capitalize(size)}`, color === 'inherit' && 'colorInherit', disableElevation && 'disableElevation', fullWidth && 'fullWidth'],\n    label: ['label'],\n    startIcon: ['startIcon', `iconSize${capitalize(size)}`],\n    endIcon: ['endIcon', `iconSize${capitalize(size)}`]\n  };\n  const composedClasses = composeClasses(slots, getButtonUtilityClass, classes);\n  return _extends({}, classes, composedClasses);\n};\nconst commonIconStyles = ownerState => _extends({}, ownerState.size === 'small' && {\n  '& > *:nth-of-type(1)': {\n    fontSize: 18\n  }\n}, ownerState.size === 'medium' && {\n  '& > *:nth-of-type(1)': {\n    fontSize: 20\n  }\n}, ownerState.size === 'large' && {\n  '& > *:nth-of-type(1)': {\n    fontSize: 22\n  }\n});\nconst ButtonRoot = styled(ButtonBase, {\n  shouldForwardProp: prop => rootShouldForwardProp(prop) || prop === 'classes',\n  name: 'MuiButton',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.root, styles[ownerState.variant], styles[`${ownerState.variant}${capitalize(ownerState.color)}`], styles[`size${capitalize(ownerState.size)}`], styles[`${ownerState.variant}Size${capitalize(ownerState.size)}`], ownerState.color === 'inherit' && styles.colorInherit, ownerState.disableElevation && styles.disableElevation, ownerState.fullWidth && styles.fullWidth];\n  }\n})(({\n  theme,\n  ownerState\n}) => {\n  var _theme$palette$getCon, _theme$palette;\n  return _extends({}, theme.typography.button, {\n    minWidth: 64,\n    padding: '6px 16px',\n    borderRadius: (theme.vars || theme).shape.borderRadius,\n    transition: theme.transitions.create(['background-color', 'box-shadow', 'border-color', 'color'], {\n      duration: theme.transitions.duration.short\n    }),\n    '&:hover': _extends({\n      textDecoration: 'none',\n      backgroundColor: theme.vars ? `rgba(${theme.vars.palette.text.primaryChannel} / ${theme.vars.palette.action.hoverOpacity})` : alpha(theme.palette.text.primary, theme.palette.action.hoverOpacity),\n      // Reset on touch devices, it doesn't add specificity\n      '@media (hover: none)': {\n        backgroundColor: 'transparent'\n      }\n    }, ownerState.variant === 'text' && ownerState.color !== 'inherit' && {\n      backgroundColor: theme.vars ? `rgba(${theme.vars.palette[ownerState.color].mainChannel} / ${theme.vars.palette.action.hoverOpacity})` : alpha(theme.palette[ownerState.color].main, theme.palette.action.hoverOpacity),\n      // Reset on touch devices, it doesn't add specificity\n      '@media (hover: none)': {\n        backgroundColor: 'transparent'\n      }\n    }, ownerState.variant === 'outlined' && ownerState.color !== 'inherit' && {\n      border: `1px solid ${(theme.vars || theme).palette[ownerState.color].main}`,\n      backgroundColor: theme.vars ? `rgba(${theme.vars.palette[ownerState.color].mainChannel} / ${theme.vars.palette.action.hoverOpacity})` : alpha(theme.palette[ownerState.color].main, theme.palette.action.hoverOpacity),\n      // Reset on touch devices, it doesn't add specificity\n      '@media (hover: none)': {\n        backgroundColor: 'transparent'\n      }\n    }, ownerState.variant === 'contained' && {\n      backgroundColor: (theme.vars || theme).palette.grey.A100,\n      boxShadow: (theme.vars || theme).shadows[4],\n      // Reset on touch devices, it doesn't add specificity\n      '@media (hover: none)': {\n        boxShadow: (theme.vars || theme).shadows[2],\n        backgroundColor: (theme.vars || theme).palette.grey[300]\n      }\n    }, ownerState.variant === 'contained' && ownerState.color !== 'inherit' && {\n      backgroundColor: (theme.vars || theme).palette[ownerState.color].dark,\n      // Reset on touch devices, it doesn't add specificity\n      '@media (hover: none)': {\n        backgroundColor: (theme.vars || theme).palette[ownerState.color].main\n      }\n    }),\n    '&:active': _extends({}, ownerState.variant === 'contained' && {\n      boxShadow: (theme.vars || theme).shadows[8]\n    }),\n    [`&.${buttonClasses.focusVisible}`]: _extends({}, ownerState.variant === 'contained' && {\n      boxShadow: (theme.vars || theme).shadows[6]\n    }),\n    [`&.${buttonClasses.disabled}`]: _extends({\n      color: (theme.vars || theme).palette.action.disabled\n    }, ownerState.variant === 'outlined' && {\n      border: `1px solid ${(theme.vars || theme).palette.action.disabledBackground}`\n    }, ownerState.variant === 'contained' && {\n      color: (theme.vars || theme).palette.action.disabled,\n      boxShadow: (theme.vars || theme).shadows[0],\n      backgroundColor: (theme.vars || theme).palette.action.disabledBackground\n    })\n  }, ownerState.variant === 'text' && {\n    padding: '6px 8px'\n  }, ownerState.variant === 'text' && ownerState.color !== 'inherit' && {\n    color: (theme.vars || theme).palette[ownerState.color].main\n  }, ownerState.variant === 'outlined' && {\n    padding: '5px 15px',\n    border: '1px solid currentColor'\n  }, ownerState.variant === 'outlined' && ownerState.color !== 'inherit' && {\n    color: (theme.vars || theme).palette[ownerState.color].main,\n    border: theme.vars ? `1px solid rgba(${theme.vars.palette[ownerState.color].mainChannel} / 0.5)` : `1px solid ${alpha(theme.palette[ownerState.color].main, 0.5)}`\n  }, ownerState.variant === 'contained' && {\n    color: theme.vars ?\n    // this is safe because grey does not change between default light/dark mode\n    theme.vars.palette.text.primary : (_theme$palette$getCon = (_theme$palette = theme.palette).getContrastText) == null ? void 0 : _theme$palette$getCon.call(_theme$palette, theme.palette.grey[300]),\n    backgroundColor: (theme.vars || theme).palette.grey[300],\n    boxShadow: (theme.vars || theme).shadows[2]\n  }, ownerState.variant === 'contained' && ownerState.color !== 'inherit' && {\n    color: (theme.vars || theme).palette[ownerState.color].contrastText,\n    backgroundColor: (theme.vars || theme).palette[ownerState.color].main\n  }, ownerState.color === 'inherit' && {\n    color: 'inherit',\n    borderColor: 'currentColor'\n  }, ownerState.size === 'small' && ownerState.variant === 'text' && {\n    padding: '4px 5px',\n    fontSize: theme.typography.pxToRem(13)\n  }, ownerState.size === 'large' && ownerState.variant === 'text' && {\n    padding: '8px 11px',\n    fontSize: theme.typography.pxToRem(15)\n  }, ownerState.size === 'small' && ownerState.variant === 'outlined' && {\n    padding: '3px 9px',\n    fontSize: theme.typography.pxToRem(13)\n  }, ownerState.size === 'large' && ownerState.variant === 'outlined' && {\n    padding: '7px 21px',\n    fontSize: theme.typography.pxToRem(15)\n  }, ownerState.size === 'small' && ownerState.variant === 'contained' && {\n    padding: '4px 10px',\n    fontSize: theme.typography.pxToRem(13)\n  }, ownerState.size === 'large' && ownerState.variant === 'contained' && {\n    padding: '8px 22px',\n    fontSize: theme.typography.pxToRem(15)\n  }, ownerState.fullWidth && {\n    width: '100%'\n  });\n}, ({\n  ownerState\n}) => ownerState.disableElevation && {\n  boxShadow: 'none',\n  '&:hover': {\n    boxShadow: 'none'\n  },\n  [`&.${buttonClasses.focusVisible}`]: {\n    boxShadow: 'none'\n  },\n  '&:active': {\n    boxShadow: 'none'\n  },\n  [`&.${buttonClasses.disabled}`]: {\n    boxShadow: 'none'\n  }\n});\nconst ButtonStartIcon = styled('span', {\n  name: 'MuiButton',\n  slot: 'StartIcon',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.startIcon, styles[`iconSize${capitalize(ownerState.size)}`]];\n  }\n})(({\n  ownerState\n}) => _extends({\n  display: 'inherit',\n  marginRight: 8,\n  marginLeft: -4\n}, ownerState.size === 'small' && {\n  marginLeft: -2\n}, commonIconStyles(ownerState)));\nconst ButtonEndIcon = styled('span', {\n  name: 'MuiButton',\n  slot: 'EndIcon',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.endIcon, styles[`iconSize${capitalize(ownerState.size)}`]];\n  }\n})(({\n  ownerState\n}) => _extends({\n  display: 'inherit',\n  marginRight: -4,\n  marginLeft: 8\n}, ownerState.size === 'small' && {\n  marginRight: -2\n}, commonIconStyles(ownerState)));\nconst Button = /*#__PURE__*/React.forwardRef(function Button(inProps, ref) {\n  // props priority: `inProps` > `contextProps` > `themeDefaultProps`\n  const contextProps = React.useContext(ButtonGroupContext);\n  const resolvedProps = resolveProps(contextProps, inProps);\n  const props = useThemeProps({\n    props: resolvedProps,\n    name: 'MuiButton'\n  });\n  const {\n      children,\n      color = 'primary',\n      component = 'button',\n      className,\n      disabled = false,\n      disableElevation = false,\n      disableFocusRipple = false,\n      endIcon: endIconProp,\n      focusVisibleClassName,\n      fullWidth = false,\n      size = 'medium',\n      startIcon: startIconProp,\n      type,\n      variant = 'text'\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const ownerState = _extends({}, props, {\n    color,\n    component,\n    disabled,\n    disableElevation,\n    disableFocusRipple,\n    fullWidth,\n    size,\n    type,\n    variant\n  });\n  const classes = useUtilityClasses(ownerState);\n  const startIcon = startIconProp && /*#__PURE__*/_jsx(ButtonStartIcon, {\n    className: classes.startIcon,\n    ownerState: ownerState,\n    children: startIconProp\n  });\n  const endIcon = endIconProp && /*#__PURE__*/_jsx(ButtonEndIcon, {\n    className: classes.endIcon,\n    ownerState: ownerState,\n    children: endIconProp\n  });\n  return /*#__PURE__*/_jsxs(ButtonRoot, _extends({\n    ownerState: ownerState,\n    className: clsx(contextProps.className, classes.root, className),\n    component: component,\n    disabled: disabled,\n    focusRipple: !disableFocusRipple,\n    focusVisibleClassName: clsx(classes.focusVisible, focusVisibleClassName),\n    ref: ref,\n    type: type\n  }, other, {\n    classes: classes,\n    children: [startIcon, children, endIcon]\n  }));\n});\nprocess.env.NODE_ENV !== \"production\" ? Button.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * The content of the component.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The color of the component.\n   * It supports both default and custom theme colors, which can be added as shown in the\n   * [palette customization guide](https://mui.com/material-ui/customization/palette/#adding-new-colors).\n   * @default 'primary'\n   */\n  color: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['inherit', 'primary', 'secondary', 'success', 'error', 'info', 'warning']), PropTypes.string]),\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n  /**\n   * If `true`, the component is disabled.\n   * @default false\n   */\n  disabled: PropTypes.bool,\n  /**\n   * If `true`, no elevation is used.\n   * @default false\n   */\n  disableElevation: PropTypes.bool,\n  /**\n   * If `true`, the  keyboard focus ripple is disabled.\n   * @default false\n   */\n  disableFocusRipple: PropTypes.bool,\n  /**\n   * If `true`, the ripple effect is disabled.\n   *\n   * \u26a0\ufe0f Without a ripple there is no styling for :focus-visible by default. Be sure\n   * to highlight the element by applying separate styles with the `.Mui-focusVisible` class.\n   * @default false\n   */\n  disableRipple: PropTypes.bool,\n  /**\n   * Element placed after the children.\n   */\n  endIcon: PropTypes.node,\n  /**\n   * @ignore\n   */\n  focusVisibleClassName: PropTypes.string,\n  /**\n   * If `true`, the button will take up the full width of its container.\n   * @default false\n   */\n  fullWidth: PropTypes.bool,\n  /**\n   * The URL to link to when the button is clicked.\n   * If defined, an `a` element will be used as the root node.\n   */\n  href: PropTypes.string,\n  /**\n   * The size of the component.\n   * `small` is equivalent to the dense button styling.\n   * @default 'medium'\n   */\n  size: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['small', 'medium', 'large']), PropTypes.string]),\n  /**\n   * Element placed before the children.\n   */\n  startIcon: PropTypes.node,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object]),\n  /**\n   * @ignore\n   */\n  type: PropTypes.oneOfType([PropTypes.oneOf(['button', 'reset', 'submit']), PropTypes.string]),\n  /**\n   * The variant to use.\n   * @default 'text'\n   */\n  variant: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['contained', 'outlined', 'text']), PropTypes.string])\n} : void 0;\nexport default Button;",
         "import * as React from 'react';\nimport {useState,useEffect} from 'react';\n\nimport { DataGrid, GridColDef, GridRenderCellParams } from '@mui/x-data-grid';\nimport parsePrometheusTextFormat from 'parse-prometheus-text-format';\nimport Box from '@mui/material/Box';\nimport Collapse from '@mui/material/Collapse';\nimport IconButton from '@mui/material/IconButton';\nimport Table from '@mui/material/Table';\nimport TableBody from '@mui/material/TableBody';\nimport TableCell from '@mui/material/TableCell';\nimport TableContainer from '@mui/material/TableContainer';\nimport TableHead from '@mui/material/TableHead';\nimport TableRow from '@mui/material/TableRow';\nimport Typography from '@mui/material/Typography';\nimport Paper from '@mui/material/Paper';\nimport KeyboardArrowDownIcon from '@mui/icons-material/KeyboardArrowDown';\nimport KeyboardArrowUpIcon from '@mui/icons-material/KeyboardArrowUp';\nimport { getNeatApiRootUrl } from 'components/Utils';\nimport { Button } from '@mui/material';\n\nfunction Row(props: { row: any }) {\n  const { row } = props;\n  const [open, setOpen] = React.useState(false);\n\n  return (\n    <React.Fragment>\n      <TableRow sx={{ '& > *': { borderBottom: 'unset' } }}>\n        <TableCell>\n          <IconButton\n            aria-label=\"expand row\"\n            size=\"small\"\n            onClick={() => setOpen(!open)}\n          >\n            {open ? <KeyboardArrowUpIcon /> : <KeyboardArrowDownIcon />}\n          </IconButton>\n        </TableCell>\n        <TableCell component=\"th\" scope=\"row\">\n          {row.name}\n        </TableCell>\n        <TableCell align=\"right\">{row.type}</TableCell>\n        <TableCell align=\"right\">{row.documentation}</TableCell>\n      </TableRow>\n      <TableRow>\n        <TableCell style={{ paddingBottom: 0, paddingTop: 0 }} colSpan={6}>\n          <Collapse in={open} timeout=\"auto\" unmountOnExit>\n            <Box sx={{ margin: 1 }}>\n              <Typography variant=\"h6\" gutterBottom component=\"div\">\n                Metrics\n              </Typography>\n              <Table size=\"small\" aria-label=\"purchases\">\n                <TableHead>\n                  <TableRow>\n                    <TableCell>Labels</TableCell>\n                    <TableCell>Value</TableCell>\n                  </TableRow>\n                </TableHead>\n                <TableBody>\n                  {row.samples.map((metric) => (\n                    <TableRow key={JSON.stringify(metric[0])}>\n                      <TableCell component=\"th\" scope=\"row\">\n                        {JSON.stringify(metric[1])}\n                      </TableCell>\n                      { row.type == \"gauge\" &&(<TableCell>{metric[2]}</TableCell>)}\n                      { row.type == \"counter\" &&(<TableCell>{metric[2]}</TableCell>)}\n                      { row.type == \"summary\" &&(<TableCell>Count : {metric[2]} Sum : { metric[3] } sec Avg : {metric[2]/metric[3]} sec </TableCell>)}\n                    </TableRow>\n                  ))}\n                </TableBody>\n              </Table>\n            </Box>\n          </Collapse>\n        </TableCell>\n      </TableRow>\n    </React.Fragment>\n  );\n}\n\nexport default function MetricsTable() {\n  const neatApiRootUrl = getNeatApiRootUrl();\n  const [data, setData] = useState(Array<any>);\n  const columns: GridColDef[] = [\n    {field: 'id', headerName: 'ID', width: 70},\n    {field: 'name', headerName: 'Name', width: 130},\n    {field: 'value', headerName: 'Value', type: 'number', width: 90},\n  ];\n\n  useEffect(() => {\n    loadDataset();\n  }, []);\n\n  const loadDataset = () => {\n    let url = neatApiRootUrl+\"/api/metrics\"\n    fetch(url)\n    .then((response) => {\n      return response.json();\n    }).then((jdata) => {\n      // console.log(text);\n      // const parsed = parsePrometheusTextFormat(text);\n      setData(jdata.prom_metrics);\n      console.dir(jdata.prom_metrics);\n\n    }\n  )}\n  return (\n    <div>\n    <TableContainer component={Paper}>\n      <Table aria-label=\"collapsible table\">\n        <TableHead>\n          <TableRow>\n            <TableCell />\n            <TableCell>Name</TableCell>\n            <TableCell align=\"right\">Type</TableCell>\n            <TableCell align=\"right\">Help</TableCell>\n          </TableRow>\n        </TableHead>\n        <TableBody>\n          {data.map((row:any) => (\n            <Row key={row.name} row={row} />\n          ))}\n        </TableBody>\n      </Table>\n\n    </TableContainer>\n    <Button variant=\"outlined\" sx={{ marginTop: 2, marginRight: 1 }}  onClick={loadDataset}>Reload</Button>\n    <p>  <a href='{neatApiRootUrl}/metrics'>Prometheus metrics endpoint</a> </p>\n    </div>\n  );\n}\n",
         "import _typeof from \"./typeof.js\";\nexport default function _regeneratorRuntime() {\n  \"use strict\"; /*! regenerator-runtime -- Copyright (c) 2014-present, Facebook, Inc. -- license (MIT): https://github.com/facebook/regenerator/blob/main/LICENSE */\n  _regeneratorRuntime = function _regeneratorRuntime() {\n    return exports;\n  };\n  var exports = {},\n    Op = Object.prototype,\n    hasOwn = Op.hasOwnProperty,\n    defineProperty = Object.defineProperty || function (obj, key, desc) {\n      obj[key] = desc.value;\n    },\n    $Symbol = \"function\" == typeof Symbol ? Symbol : {},\n    iteratorSymbol = $Symbol.iterator || \"@@iterator\",\n    asyncIteratorSymbol = $Symbol.asyncIterator || \"@@asyncIterator\",\n    toStringTagSymbol = $Symbol.toStringTag || \"@@toStringTag\";\n  function define(obj, key, value) {\n    return Object.defineProperty(obj, key, {\n      value: value,\n      enumerable: !0,\n      configurable: !0,\n      writable: !0\n    }), obj[key];\n  }\n  try {\n    define({}, \"\");\n  } catch (err) {\n    define = function define(obj, key, value) {\n      return obj[key] = value;\n    };\n  }\n  function wrap(innerFn, outerFn, self, tryLocsList) {\n    var protoGenerator = outerFn && outerFn.prototype instanceof Generator ? outerFn : Generator,\n      generator = Object.create(protoGenerator.prototype),\n      context = new Context(tryLocsList || []);\n    return defineProperty(generator, \"_invoke\", {\n      value: makeInvokeMethod(innerFn, self, context)\n    }), generator;\n  }\n  function tryCatch(fn, obj, arg) {\n    try {\n      return {\n        type: \"normal\",\n        arg: fn.call(obj, arg)\n      };\n    } catch (err) {\n      return {\n        type: \"throw\",\n        arg: err\n      };\n    }\n  }\n  exports.wrap = wrap;\n  var ContinueSentinel = {};\n  function Generator() {}\n  function GeneratorFunction() {}\n  function GeneratorFunctionPrototype() {}\n  var IteratorPrototype = {};\n  define(IteratorPrototype, iteratorSymbol, function () {\n    return this;\n  });\n  var getProto = Object.getPrototypeOf,\n    NativeIteratorPrototype = getProto && getProto(getProto(values([])));\n  NativeIteratorPrototype && NativeIteratorPrototype !== Op && hasOwn.call(NativeIteratorPrototype, iteratorSymbol) && (IteratorPrototype = NativeIteratorPrototype);\n  var Gp = GeneratorFunctionPrototype.prototype = Generator.prototype = Object.create(IteratorPrototype);\n  function defineIteratorMethods(prototype) {\n    [\"next\", \"throw\", \"return\"].forEach(function (method) {\n      define(prototype, method, function (arg) {\n        return this._invoke(method, arg);\n      });\n    });\n  }\n  function AsyncIterator(generator, PromiseImpl) {\n    function invoke(method, arg, resolve, reject) {\n      var record = tryCatch(generator[method], generator, arg);\n      if (\"throw\" !== record.type) {\n        var result = record.arg,\n          value = result.value;\n        return value && \"object\" == _typeof(value) && hasOwn.call(value, \"__await\") ? PromiseImpl.resolve(value.__await).then(function (value) {\n          invoke(\"next\", value, resolve, reject);\n        }, function (err) {\n          invoke(\"throw\", err, resolve, reject);\n        }) : PromiseImpl.resolve(value).then(function (unwrapped) {\n          result.value = unwrapped, resolve(result);\n        }, function (error) {\n          return invoke(\"throw\", error, resolve, reject);\n        });\n      }\n      reject(record.arg);\n    }\n    var previousPromise;\n    defineProperty(this, \"_invoke\", {\n      value: function value(method, arg) {\n        function callInvokeWithMethodAndArg() {\n          return new PromiseImpl(function (resolve, reject) {\n            invoke(method, arg, resolve, reject);\n          });\n        }\n        return previousPromise = previousPromise ? previousPromise.then(callInvokeWithMethodAndArg, callInvokeWithMethodAndArg) : callInvokeWithMethodAndArg();\n      }\n    });\n  }\n  function makeInvokeMethod(innerFn, self, context) {\n    var state = \"suspendedStart\";\n    return function (method, arg) {\n      if (\"executing\" === state) throw new Error(\"Generator is already running\");\n      if (\"completed\" === state) {\n        if (\"throw\" === method) throw arg;\n        return doneResult();\n      }\n      for (context.method = method, context.arg = arg;;) {\n        var delegate = context.delegate;\n        if (delegate) {\n          var delegateResult = maybeInvokeDelegate(delegate, context);\n          if (delegateResult) {\n            if (delegateResult === ContinueSentinel) continue;\n            return delegateResult;\n          }\n        }\n        if (\"next\" === context.method) context.sent = context._sent = context.arg;else if (\"throw\" === context.method) {\n          if (\"suspendedStart\" === state) throw state = \"completed\", context.arg;\n          context.dispatchException(context.arg);\n        } else \"return\" === context.method && context.abrupt(\"return\", context.arg);\n        state = \"executing\";\n        var record = tryCatch(innerFn, self, context);\n        if (\"normal\" === record.type) {\n          if (state = context.done ? \"completed\" : \"suspendedYield\", record.arg === ContinueSentinel) continue;\n          return {\n            value: record.arg,\n            done: context.done\n          };\n        }\n        \"throw\" === record.type && (state = \"completed\", context.method = \"throw\", context.arg = record.arg);\n      }\n    };\n  }\n  function maybeInvokeDelegate(delegate, context) {\n    var methodName = context.method,\n      method = delegate.iterator[methodName];\n    if (undefined === method) return context.delegate = null, \"throw\" === methodName && delegate.iterator[\"return\"] && (context.method = \"return\", context.arg = undefined, maybeInvokeDelegate(delegate, context), \"throw\" === context.method) || \"return\" !== methodName && (context.method = \"throw\", context.arg = new TypeError(\"The iterator does not provide a '\" + methodName + \"' method\")), ContinueSentinel;\n    var record = tryCatch(method, delegate.iterator, context.arg);\n    if (\"throw\" === record.type) return context.method = \"throw\", context.arg = record.arg, context.delegate = null, ContinueSentinel;\n    var info = record.arg;\n    return info ? info.done ? (context[delegate.resultName] = info.value, context.next = delegate.nextLoc, \"return\" !== context.method && (context.method = \"next\", context.arg = undefined), context.delegate = null, ContinueSentinel) : info : (context.method = \"throw\", context.arg = new TypeError(\"iterator result is not an object\"), context.delegate = null, ContinueSentinel);\n  }\n  function pushTryEntry(locs) {\n    var entry = {\n      tryLoc: locs[0]\n    };\n    1 in locs && (entry.catchLoc = locs[1]), 2 in locs && (entry.finallyLoc = locs[2], entry.afterLoc = locs[3]), this.tryEntries.push(entry);\n  }\n  function resetTryEntry(entry) {\n    var record = entry.completion || {};\n    record.type = \"normal\", delete record.arg, entry.completion = record;\n  }\n  function Context(tryLocsList) {\n    this.tryEntries = [{\n      tryLoc: \"root\"\n    }], tryLocsList.forEach(pushTryEntry, this), this.reset(!0);\n  }\n  function values(iterable) {\n    if (iterable) {\n      var iteratorMethod = iterable[iteratorSymbol];\n      if (iteratorMethod) return iteratorMethod.call(iterable);\n      if (\"function\" == typeof iterable.next) return iterable;\n      if (!isNaN(iterable.length)) {\n        var i = -1,\n          next = function next() {\n            for (; ++i < iterable.length;) if (hasOwn.call(iterable, i)) return next.value = iterable[i], next.done = !1, next;\n            return next.value = undefined, next.done = !0, next;\n          };\n        return next.next = next;\n      }\n    }\n    return {\n      next: doneResult\n    };\n  }\n  function doneResult() {\n    return {\n      value: undefined,\n      done: !0\n    };\n  }\n  return GeneratorFunction.prototype = GeneratorFunctionPrototype, defineProperty(Gp, \"constructor\", {\n    value: GeneratorFunctionPrototype,\n    configurable: !0\n  }), defineProperty(GeneratorFunctionPrototype, \"constructor\", {\n    value: GeneratorFunction,\n    configurable: !0\n  }), GeneratorFunction.displayName = define(GeneratorFunctionPrototype, toStringTagSymbol, \"GeneratorFunction\"), exports.isGeneratorFunction = function (genFun) {\n    var ctor = \"function\" == typeof genFun && genFun.constructor;\n    return !!ctor && (ctor === GeneratorFunction || \"GeneratorFunction\" === (ctor.displayName || ctor.name));\n  }, exports.mark = function (genFun) {\n    return Object.setPrototypeOf ? Object.setPrototypeOf(genFun, GeneratorFunctionPrototype) : (genFun.__proto__ = GeneratorFunctionPrototype, define(genFun, toStringTagSymbol, \"GeneratorFunction\")), genFun.prototype = Object.create(Gp), genFun;\n  }, exports.awrap = function (arg) {\n    return {\n      __await: arg\n    };\n  }, defineIteratorMethods(AsyncIterator.prototype), define(AsyncIterator.prototype, asyncIteratorSymbol, function () {\n    return this;\n  }), exports.AsyncIterator = AsyncIterator, exports.async = function (innerFn, outerFn, self, tryLocsList, PromiseImpl) {\n    void 0 === PromiseImpl && (PromiseImpl = Promise);\n    var iter = new AsyncIterator(wrap(innerFn, outerFn, self, tryLocsList), PromiseImpl);\n    return exports.isGeneratorFunction(outerFn) ? iter : iter.next().then(function (result) {\n      return result.done ? result.value : iter.next();\n    });\n  }, defineIteratorMethods(Gp), define(Gp, toStringTagSymbol, \"Generator\"), define(Gp, iteratorSymbol, function () {\n    return this;\n  }), define(Gp, \"toString\", function () {\n    return \"[object Generator]\";\n  }), exports.keys = function (val) {\n    var object = Object(val),\n      keys = [];\n    for (var key in object) keys.push(key);\n    return keys.reverse(), function next() {\n      for (; keys.length;) {\n        var key = keys.pop();\n        if (key in object) return next.value = key, next.done = !1, next;\n      }\n      return next.done = !0, next;\n    };\n  }, exports.values = values, Context.prototype = {\n    constructor: Context,\n    reset: function reset(skipTempReset) {\n      if (this.prev = 0, this.next = 0, this.sent = this._sent = undefined, this.done = !1, this.delegate = null, this.method = \"next\", this.arg = undefined, this.tryEntries.forEach(resetTryEntry), !skipTempReset) for (var name in this) \"t\" === name.charAt(0) && hasOwn.call(this, name) && !isNaN(+name.slice(1)) && (this[name] = undefined);\n    },\n    stop: function stop() {\n      this.done = !0;\n      var rootRecord = this.tryEntries[0].completion;\n      if (\"throw\" === rootRecord.type) throw rootRecord.arg;\n      return this.rval;\n    },\n    dispatchException: function dispatchException(exception) {\n      if (this.done) throw exception;\n      var context = this;\n      function handle(loc, caught) {\n        return record.type = \"throw\", record.arg = exception, context.next = loc, caught && (context.method = \"next\", context.arg = undefined), !!caught;\n      }\n      for (var i = this.tryEntries.length - 1; i >= 0; --i) {\n        var entry = this.tryEntries[i],\n          record = entry.completion;\n        if (\"root\" === entry.tryLoc) return handle(\"end\");\n        if (entry.tryLoc <= this.prev) {\n          var hasCatch = hasOwn.call(entry, \"catchLoc\"),\n            hasFinally = hasOwn.call(entry, \"finallyLoc\");\n          if (hasCatch && hasFinally) {\n            if (this.prev < entry.catchLoc) return handle(entry.catchLoc, !0);\n            if (this.prev < entry.finallyLoc) return handle(entry.finallyLoc);\n          } else if (hasCatch) {\n            if (this.prev < entry.catchLoc) return handle(entry.catchLoc, !0);\n          } else {\n            if (!hasFinally) throw new Error(\"try statement without catch or finally\");\n            if (this.prev < entry.finallyLoc) return handle(entry.finallyLoc);\n          }\n        }\n      }\n    },\n    abrupt: function abrupt(type, arg) {\n      for (var i = this.tryEntries.length - 1; i >= 0; --i) {\n        var entry = this.tryEntries[i];\n        if (entry.tryLoc <= this.prev && hasOwn.call(entry, \"finallyLoc\") && this.prev < entry.finallyLoc) {\n          var finallyEntry = entry;\n          break;\n        }\n      }\n      finallyEntry && (\"break\" === type || \"continue\" === type) && finallyEntry.tryLoc <= arg && arg <= finallyEntry.finallyLoc && (finallyEntry = null);\n      var record = finallyEntry ? finallyEntry.completion : {};\n      return record.type = type, record.arg = arg, finallyEntry ? (this.method = \"next\", this.next = finallyEntry.finallyLoc, ContinueSentinel) : this.complete(record);\n    },\n    complete: function complete(record, afterLoc) {\n      if (\"throw\" === record.type) throw record.arg;\n      return \"break\" === record.type || \"continue\" === record.type ? this.next = record.arg : \"return\" === record.type ? (this.rval = this.arg = record.arg, this.method = \"return\", this.next = \"end\") : \"normal\" === record.type && afterLoc && (this.next = afterLoc), ContinueSentinel;\n    },\n    finish: function finish(finallyLoc) {\n      for (var i = this.tryEntries.length - 1; i >= 0; --i) {\n        var entry = this.tryEntries[i];\n        if (entry.finallyLoc === finallyLoc) return this.complete(entry.completion, entry.afterLoc), resetTryEntry(entry), ContinueSentinel;\n      }\n    },\n    \"catch\": function _catch(tryLoc) {\n      for (var i = this.tryEntries.length - 1; i >= 0; --i) {\n        var entry = this.tryEntries[i];\n        if (entry.tryLoc === tryLoc) {\n          var record = entry.completion;\n          if (\"throw\" === record.type) {\n            var thrown = record.arg;\n            resetTryEntry(entry);\n          }\n          return thrown;\n        }\n      }\n      throw new Error(\"illegal catch attempt\");\n    },\n    delegateYield: function delegateYield(iterable, resultName, nextLoc) {\n      return this.delegate = {\n        iterator: values(iterable),\n        resultName: resultName,\n        nextLoc: nextLoc\n      }, \"next\" === this.method && (this.arg = undefined), ContinueSentinel;\n    }\n  }, exports;\n}",
         "function asyncGeneratorStep(gen, resolve, reject, _next, _throw, key, arg) {\n  try {\n    var info = gen[key](arg);\n    var value = info.value;\n  } catch (error) {\n    reject(error);\n    return;\n  }\n  if (info.done) {\n    resolve(value);\n  } else {\n    Promise.resolve(value).then(_next, _throw);\n  }\n}\nexport default function _asyncToGenerator(fn) {\n  return function () {\n    var self = this,\n      args = arguments;\n    return new Promise(function (resolve, reject) {\n      var gen = fn.apply(self, args);\n      function _next(value) {\n        asyncGeneratorStep(gen, resolve, reject, _next, _throw, \"next\", value);\n      }\n      function _throw(err) {\n        asyncGeneratorStep(gen, resolve, reject, _next, _throw, \"throw\", err);\n      }\n      _next(undefined);\n    });\n  };\n}",
         "export default function cc(names) {\n  if (typeof names === \"string\" || typeof names === \"number\") return \"\" + names\n\n  let out = \"\"\n\n  if (Array.isArray(names)) {\n    for (let i = 0, tmp; i < names.length; i++) {\n      if ((tmp = cc(names[i])) !== \"\") {\n        out += (out && \" \") + tmp\n      }\n    }\n  } else {\n    for (let k in names) {\n      if (names[k]) out += (out && \" \") + k\n    }\n  }\n\n  return out\n}\n",
@@ -12627,17 +12627,17 @@
         "export default \"data:image/svg+xml,%3Csvg%20aria-hidden%3D%22true%22%20focusable%3D%22false%22%20data-prefix%3D%22fas%22%20data-icon%3D%22stop%22%20class%3D%22svg-inline--fa%20fa-stop%20fa-w-14%22%20role%3D%22img%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%20448%20512%22%3E%3Cpath%20fill%3D%22currentColor%22%20d%3D%22M400%2032H48C21.5%2032%200%2053.5%200%2080v352c0%2026.5%2021.5%2048%2048%2048h352c26.5%200%2048-21.5%2048-48V80c0-26.5-21.5-48-48-48z%22%3E%3C%2Fpath%3E%3C%2Fsvg%3E\"",
         "import React, { useEffect, CSSProperties } from \"react\";\n\nimport { useSigma } from \"@react-sigma/core\";\nimport { ReactComponent as StartLayoutIcon } from \"./assets/icons/play-solid.svg\";\nimport { ReactComponent as StopLayoutIcon } from \"./assets/icons/stop-solid.svg\";\nimport { LayoutWorkerHook } from \"./useWorkerLayoutFactory\";\n\n/**\n * Properties for `WorkerLayoutControl` component\n */\nexport interface WorkerLayoutControlProps<T> {\n  /**\n   * HTML id\n   */\n  id?: string;\n\n  /**\n   * HTML class\n   */\n  className?: string;\n\n  /**\n   * HTML CSS style\n   */\n  style?: CSSProperties;\n\n  /**\n   * The layout hook to use\n   */\n  layout: LayoutWorkerHook<T>;\n\n  /**\n   * Settings of the layout.\n   */\n  settings: T;\n\n  /**\n   * Option to tell what we do when the component is mounted\n   *  - <code>-1</code> means that we do nothing (it's the same as no value)\n   *  - <code>0</code> means that we start the algo (and don't auto stop it)\n   *  - <code>X</code> mans that we start the algo, and stop it after X milliseconds\n   */\n  autoRunFor?: number;\n\n  /**\n   * It's possible to customize the button, by passing to JSX Element.\n   * First one is for the \"start layout\", and the second to \"stop layout\".\n   * Example :\n   * ```jsx\n   * <FullScreenControl>\n   *   <>\n   *     <BiFullscreen />\n   *     <BiExitFullscreen />\n   *   </>\n   * </FullScreenControl>\n   * ```\n   */\n  children?: [JSX.Element, JSX.Element];\n}\n\nexport function WorkerLayoutControl<T>({\n  id,\n  className,\n  style,\n  layout,\n  settings,\n  autoRunFor,\n  children,\n}: WorkerLayoutControlProps<T>) {\n  // Get Sigma\n  const sigma = useSigma();\n  // Get layout\n  const { stop, start, isRunning } = layout(settings);\n  // Common html props for the div\n  const props = {\n    className: `react-sigma-control ${className || \"\"}`,\n    id,\n    style,\n  };\n\n  /**\n   * Init component when Sigma or component settings change.\n   */\n  useEffect(() => {\n    if (!sigma) {\n      return;\n    }\n\n    // we run the algo\n    let timeout: number | null = null;\n    if (autoRunFor !== undefined && autoRunFor > -1 && sigma.getGraph().order > 0) {\n      start();\n      // set a timeout to stop it\n      timeout =\n        autoRunFor > 0\n          ? window.setTimeout(() => {\n              stop();\n            }, autoRunFor)\n          : null;\n    }\n\n    //cleaning\n    return () => {\n      if (timeout) {\n        clearTimeout(timeout);\n      }\n    };\n  }, [autoRunFor, start, stop, sigma]);\n\n  return (\n    <div {...props}>\n      <button\n        onClick={() => (isRunning ? stop() : start())}\n        title={isRunning ? \"Stop the layout animation\" : \"Start the layout animation\"}\n      >\n        {children && !isRunning && children[0]}\n        {children && isRunning && children[1]}\n        {!children && !isRunning && <StartLayoutIcon style={{ width: \"1em\" }} />}\n        {!children && isRunning && <StopLayoutIcon style={{ width: \"1em\" }} />}\n      </button>\n    </div>\n  );\n}\n",
         "import FA2Layout from \"graphology-layout-forceatlas2/worker\";\nimport { ForceAtlas2LayoutParameters } from \"graphology-layout-forceatlas2\";\n\nimport { useWorkerLayoutFactory } from \"@react-sigma/layout-core\";\n\n/**\n * React hook that helps you to manage worker of [force atlas2 layout](https://graphology.github.io/standard-library/layout-forceatlas2.html).\n *\n * ```typescript\n * const { stop, start } = useWorkerLayoutForceAtlas2(...);\n *```\n * @category Hook\n */\nexport const useWorkerLayoutForceAtlas2 = useWorkerLayoutFactory<ForceAtlas2LayoutParameters>(FA2Layout);\n",
         "import forceAtlas2, { ForceAtlas2SynchronousLayoutParameters } from \"graphology-layout-forceatlas2\";\n\nimport { useLayoutFactory } from \"@react-sigma/layout-core\";\n\n/**\n * React hook that helps you to manage [force atlas2 layout](https://graphology.github.io/standard-library/layout-forceatlas2.html).\n *\n * ```typescript\n * const { positions, assign } = useLayoutForceAtlas2(...);\n *```\n * @category Hook\n */\nexport const useLayoutForceAtlas2 = useLayoutFactory<ForceAtlas2SynchronousLayoutParameters>(forceAtlas2, {\n  iterations: 100,\n});\n",
         "import { isEqual } from \"lodash\";\nimport { useCallback, useRef, useState, useEffect } from \"react\";\nimport Graph from \"graphology\";\n\nimport { useSigma } from \"@react-sigma/core\";\n\nexport type LayoutWorkerHook<T> = (\n  settings: T,\n) => {\n  stop: () => void;\n  start: () => void;\n  kill: () => void;\n  isRunning: boolean;\n};\n\ninterface GraphologyWorkerLayout {\n  stop: () => void;\n  start: () => void;\n  kill: () => void;\n}\n\ninterface GraphologyWorkerLayoutConstructor<T> {\n  new (graph: Graph, settings: T): GraphologyWorkerLayout;\n}\n\nexport function useWorkerLayoutFactory<T>(worker: GraphologyWorkerLayoutConstructor<T>): LayoutWorkerHook<T> {\n  const hook: LayoutWorkerHook<T> = (parameter: T) => {\n    const sigma = useSigma();\n    const [isRunning, setIsRunning] = useState<boolean>(false);\n    const [layout, setLayout] = useState<GraphologyWorkerLayout | null>(null);\n    const settings = useRef<T>();\n    if (!isEqual(settings.current, parameter)) settings.current = parameter;\n\n    useEffect(() => {\n      setIsRunning(false);\n      let newLayout: GraphologyWorkerLayout | null = null;\n      if (settings.current) newLayout = new worker(sigma.getGraph(), settings.current);\n      setLayout(newLayout);\n      return () => {\n        if (newLayout !== null) newLayout.kill();\n      };\n    }, [sigma, settings, setLayout, setIsRunning]);\n\n    const stop = useCallback(() => {\n      if (layout) {\n        layout.stop();\n        setIsRunning(false);\n      }\n    }, [layout, setIsRunning]);\n\n    const start = useCallback(() => {\n      if (layout) {\n        layout.start();\n        setIsRunning(true);\n      }\n    }, [layout, setIsRunning]);\n\n    const kill = useCallback(() => {\n      if (layout) {\n        layout.kill();\n      }\n      setIsRunning(false);\n    }, [layout, setIsRunning]);\n\n    return { stop, start, kill, isRunning };\n  };\n  return hook;\n}\n",
         "import React from \"react\";\nimport { ForceAtlas2LayoutParameters } from \"graphology-layout-forceatlas2\";\n\nimport { WorkerLayoutControlProps, WorkerLayoutControl } from \"@react-sigma/layout-core\";\nimport { useWorkerLayoutForceAtlas2 } from \"./useWorkerLayoutForceAtlas2\";\n\n/**\n * Properties for `LayoutForceAtlas2Control` component\n */\nexport type LayoutForceAtlas2ControlProps = Omit<\n  WorkerLayoutControlProps<ForceAtlas2LayoutParameters>,\n  \"layout\" | \"settings\"\n> & {\n  settings?: ForceAtlas2LayoutParameters;\n};\n\n/**\n * @category Component\n */\nexport const LayoutForceAtlas2Control: React.FC<LayoutForceAtlas2ControlProps> = ({\n  id,\n  className,\n  style,\n  settings = {},\n  autoRunFor,\n  children,\n}) => {\n  const workerLayoutProps = { id, className, style, settings, autoRunFor, layout: useWorkerLayoutForceAtlas2 };\n  return <WorkerLayoutControl {...workerLayoutProps}>{children}</WorkerLayoutControl>;\n};\n",
         "import circular, { CircularLayoutOptions } from \"graphology-layout/circular\";\n\nimport { useLayoutFactory } from \"@react-sigma/layout-core\";\n\n/**\n * React hook that helps you to manage [circle layout](https://graphology.github.io/standard-library/layout.html#circular).\n *\n * ```typescript\n * const { positions, assign } = useLayoutCircular(...);\n *```\n * @category Hook\n */\nexport const useLayoutCircular = useLayoutFactory<CircularLayoutOptions>(circular, {});\n",
-        "import * as React from 'react';\nimport {useState,useEffect, useRef, useImperativeHandle,FC} from 'react';\nimport Box from '@mui/material/Box';\nimport Graph from \"graphology\";\nimport { SigmaContainer, useLoadGraph,useRegisterEvents } from \"@react-sigma/core\";\n\nimport \"@react-sigma/core/lib/react-sigma.min.css\";\nimport { ControlsContainer, useSigma } from \"@react-sigma/core\";\nimport { ExplorerContext } from 'components/Context';\nimport RemoveNsPrefix, { getNeatApiRootUrl, getSelectedWorkflowName } from 'components/Utils';\nimport TextField from '@mui/material/TextField';\nimport Button from '@mui/material/Button';\nimport NodeViewer from 'components/NodeViewer';\nimport LinearProgress from '@mui/material/LinearProgress';\nimport { useWorkerLayoutForceAtlas2,useLayoutForceAtlas2, LayoutForceAtlas2Control } from \"@react-sigma/layout-forceatlas2\";\nimport { useLayoutCircular } from \"@react-sigma/layout-circular\";\n\nexport function LoadGraph(props:{filters:Array<string>,nodeNameProperty:string,sparqlQuery:string,reloader:number,mode:string,limit:number}) {\n    const neatApiRootUrl = getNeatApiRootUrl();\n    const {hiddenNsPrefixModeCtx, graphNameCtx} = React.useContext(ExplorerContext);\n    const [graphName, setGraphName] = graphNameCtx;\n    const [hiddenNsPrefixMode, setHiddenNsPrefixMode ] = hiddenNsPrefixModeCtx;\n    const loadGraph = useLoadGraph();\n    // const { positions, assign } = useLayoutForceAtlas2({settings:{strongGravityMode:true},iterations:10});\n    const { positions, assign } = useLayoutCircular();\n    const { start, stop,kill } = useWorkerLayoutForceAtlas2({ settings: { slowDown: 5 } });\n    const [ bigGraph, setBigGraph] = useState<Graph>();\n    const [ loading, setLoading] = useState(false);\n\n\n    useEffect(() => {\n      loadDataset();\n    //   start();\n      return () => {\n        // Kill FA2 on unmount\n        kill();\n      };\n\n    }, [loadGraph,start,kill]);\n\n    useEffect(() => {\n      if (props.reloader || props.sparqlQuery) {\n        loadDataset();\n      }\n    }, [props.reloader,props.sparqlQuery]);\n\n    const loadDataset = () => {\n        setLoading(true);\n         console.log(\"loading dataset\");\n        //TODO - this is a hack to get the node name property for the solution graph. Make this configurable.\n        let nodeNameProperty = localStorage.getItem('nodeNameProperty');\n        // if(!props.nodeNameProperty) {\n        //   if (graphName == \"solution\") {\n        //       nodeNameProperty = \"\"\n        //   }else {\n        //       nodeNameProperty = \"\"\n        //   }\n        // }\n        let graph = new Graph();\n\n        if (props.mode== \"update\"){\n          graph = bigGraph;\n        }\n\n        const url = neatApiRootUrl+\"/api/get-nodes-and-edges\";\n        const workflowName = getSelectedWorkflowName();\n\n        const requestFilter = {\n            \"graph_name\": graphName,\n            \"workflow_name\":workflowName,\n            \"node_class_filter\": props.filters,\n            \"src_edge_filter\": props.filters,\n            \"dst_edge_filter\": props.filters,\n            \"node_name_property\": nodeNameProperty,\n            \"sparql_query\": props.sparqlQuery,\n            \"cache\": false,\n            \"limit\": props.limit\n        }\n        fetch(url,{ method:\"post\",body:JSON.stringify(requestFilter),headers: {\n            'Content-Type': 'application/json;charset=utf-8'\n          }}).then((response) => response.json()).then((data) => {\n            console.dir(data)\n            const addedNodes : string[] = [];\n            let graphSize = graph.size+data.nodes.length;\n            data.nodes.forEach((node) => {\n                let nodeClassName = RemoveNsPrefix(node.node_class);\n                const nodeLabel = node.node_name+\" (\"+nodeClassName+\")\";\n                if (!addedNodes.includes(node.node_id)) {\n                    addedNodes.push(node.node_id);\n                    graph.mergeNode(node.node_id,{label:nodeLabel,x:1,y:1,color:getColor(nodeClassName), size:getSize(nodeClassName,graphSize)});\n\n                }\n                \n            });\n            data.edges.forEach((edge) => {\n              if (props.mode== \"update\"){\n                graph.mergeEdge(edge.src_object_ref,edge.dst_object_ref);\n              }else {\n                if (addedNodes.includes(edge.src_object_ref) && addedNodes.includes(edge.dst_object_ref)) {\n                  graph.mergeEdge(edge.src_object_ref,edge.dst_object_ref);\n                }\n              }\n\n            });\n            // loadGraph(graph);\n            setBigGraph(graph);\n            loadGraph(graph);\n            assign();\n            // if (props.mode== \"update\"){\n            // }else {\n            //   assign();\n            // }\n            console.log(\"graph loaded\");\n          }).catch((error) => {\n            console.log('Error:', error);\n          }).finally(() => { \n            setLoading(false);\n           });\n    }\n\n    return (loading &&( <LinearProgress />) );\n  };\n\n\nexport default function GraphExplorer(props:{filters:Array<string>,sparqlQuery:string}) {\n    const [nodeNameProperty, setNodeNameProperty] = useState(localStorage.getItem('nodeNameProperty'));\n    const [reloader, setReloader] = useState(0);\n    const loaderCompRef = useRef()\n    const [limitRecordsInResponse, setLimitRecordsInResponse] = useState(5000);\n    const [openNodeViewer, setOpenNodeViewer] = useState(false);\n    const [selectedNodeId, setSelectedNodeId] = useState(\"\");\n    const [sparqlQuery, setSparqlQuery] = useState(\"\");\n    const [loaderMode, setLoaderMode] = useState(\"create\");\n    \n    const handleNodeNameProperty = (event: React.ChangeEvent<HTMLInputElement>) => {\n        setNodeNameProperty(event.target.value);\n        localStorage.setItem('nodeNameProperty',event.target.value);\n        reload();\n    };\n\n    const handleResponseLimitChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n        setLimitRecordsInResponse(parseInt(event.target.value));\n    };  \n    const reload = () => {\n          setReloader(reloader+1);\n    }\n\n    useEffect(() => {\n      console.log(\"sparqlQuery changed\");\n      setNodeNameProperty(localStorage.getItem('nodeNameProperty'));\n      setSparqlQuery(props.sparqlQuery);\n    }, [props.sparqlQuery]);\n\n\n    const onViewerClose = () => {\n      setOpenNodeViewer(false);\n    }\n\n    const loadLinkedNodes = (nodeRef:string) => {\n      let query = \"\"\n      const nodeNameProperty = localStorage.getItem('nodeNameProperty')\n      if (!nodeNameProperty) {\n\n        query = `SELECT (?dst_object_ref AS ?node_name) (?linked_obj_type  AS ?node_class) (?dst_object_ref AS ?node_id) ?src_object_ref ?dst_object_ref WHERE {\n          BIND( <`+nodeRef+`> AS ?src_object_ref )\n          { \n           ?src_object_ref ?rel_propery ?dst_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type \n          }\n          UNION \n          {\n           ?dst_object_ref ?rel_propery ?src_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type . \n          }             \n          }  `\n      }else {\n        query = `SELECT ?node_name (?linked_obj_type  AS ?node_class) (?dst_object_ref AS ?node_id) ?src_object_ref ?dst_object_ref WHERE {\n          BIND( <`+nodeRef+`> AS ?src_object_ref )\n          { \n           ?src_object_ref ?rel_propery ?dst_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type .\n           ?dst_object_ref `+nodeNameProperty+` ?node_name . \n          }\n          UNION \n          {\n           ?dst_object_ref ?rel_propery ?src_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type . \n           ?dst_object_ref `+nodeNameProperty+` ?node_name .\n          }             \n          } `\n      }  \n      console.log(\"requesting linked nodes\");\n      \n      setSparqlQuery(query);\n    }\n\n    const GraphEvents: React.FC = () => {\n      const registerEvents = useRegisterEvents();\n      const sigma = useSigma();\n      const [draggedNode, setDraggedNode] = useState<string | null>(null);\n      useEffect(() => {\n        // Register the events\n        registerEvents({\n          // node events\n          rightClickNode: (event) => {\n            // event.preventSigmaDefault();\n            console.log(\"clickNode\", event.event, event.node )\n            console.log(\"node id: \"+event.node);\n            setLoaderMode(\"update\");\n            setSelectedNodeId(event.node);\n            loadLinkedNodes(event.node);\n            sigma.getGraph().setNodeAttribute(event.node, \"highlighted\", true);\n         \n          },\n          doubleClickNode: (event) => {\n            setSelectedNodeId(event.node);\n            setOpenNodeViewer(true);\n          },\n          mouseup: (e) => {\n            if (draggedNode) {\n              setDraggedNode(null);\n              sigma.getGraph().removeNodeAttribute(draggedNode, \"highlighted\");\n            }\n          },\n          mousedown: (e) => {\n            // Disable the autoscale at the first down interaction\n            if (!sigma.getCustomBBox()) sigma.setCustomBBox(sigma.getBBox());\n          },\n          mousemove: (e) => {\n            if (draggedNode) {\n              // Get new position of node\n              console.log(\"draggedNode\",draggedNode);\n              const pos = sigma.viewportToGraph(e);\n              sigma.getGraph().setNodeAttribute(draggedNode, \"x\", pos.x);\n              sigma.getGraph().setNodeAttribute(draggedNode, \"y\", pos.y);\n\n              // Prevent sigma to move camera:\n              e.preventSigmaDefault();\n              e.original.preventDefault();\n              e.original.stopPropagation();\n            }\n          },\n          downNode: (e) => {\n            setDraggedNode(e.node);\n            sigma.getGraph().setNodeAttribute(e.node, \"highlighted\", true);\n          },\n          // rightClickNode: (event) => console.log(\"rightClickNode\", event.event, event.node, event.preventSigmaDefault),\n          // wheelNode: (event) => console.log(\"wheelNode\", event.event, event.node, event.preventSigmaDefault),\n          // downNode: (event) => console.log(\"downNode\", event.event, event.node, event.preventSigmaDefault),\n          // enterNode: (event) => console.log(\"enterNode\", event.node),\n          // leaveNode: (event) => console.log(\"leaveNode\", event.node),\n          // // edge events\n          // clickEdge: (event) => console.log(\"clickEdge\", event.event, event.edge, event.preventSigmaDefault),\n          // doubleClickEdge: (event) => console.log(\"doubleClickEdge\", event.event, event.edge, event.preventSigmaDefault),\n          // rightClickEdge: (event) => console.log(\"rightClickEdge\", event.event, event.edge, event.preventSigmaDefault),\n          // wheelEdge: (event) => console.log(\"wheelEdge\", event.event, event.edge, event.preventSigmaDefault),\n          // downEdge: (event) => console.log(\"downEdge\", event.event, event.edge, event.preventSigmaDefault),\n          // enterEdge: (event) => console.log(\"enterEdge\", event.edge),\n          // leaveEdge: (event) => console.log(\"leaveEdge\", event.edge),\n          // // stage events\n          // clickStage: (event) => console.log(\"clickStage\", event.event, event.preventSigmaDefault),\n          // doubleClickStage: (event) => console.log(\"doubleClickStage\", event.event, event.preventSigmaDefault),\n          // rightClickStage: (event) => console.log(\"rightClickStage\", event.event, event.preventSigmaDefault),\n          // wheelStage: (event) => console.log(\"wheelStage\", event.event, event.preventSigmaDefault),\n          // downStage: (event) => console.log(\"downStage\", event.event, event.preventSigmaDefault),\n          // // default mouse events\n          // click: (event) => console.log(\"click\", event.x, event.y),\n          // doubleClick: (event) => console.log(\"doubleClick\", event.x, event.y),\n          // wheel: (event) => console.log(\"wheel\", event.x, event.y, event.delta),\n          // rightClick: (event) => console.log(\"rightClick\", event.x, event.y),\n          // mouseup: (event) => console.log(\"mouseup\", event.x, event.y),\n          // mousedown: (event) => console.log(\"mousedown\", event.x, event.y),\n          // mousemove: (event) => console.log(\"mousemove\", event.x, event.y),\n          // // default touch events\n          // touchup: (event) => console.log(\"touchup\", event.touches),\n          // touchdown: (event) => console.log(\"touchdown\", event.touches),\n          // touchmove: (event) => console.log(\"touchmove\", event.touches),\n          // // sigma kill\n          // kill: () => console.log(\"kill\"),\n          // resize: () => console.log(\"resize\"),\n          // beforeRender: () => console.log(\"beforeRender\"),\n          // afterRender: () => console.log(\"afterRender\"),\n          // // sigma camera update\n          // updated: (event) => console.log(\"updated\", event.x, event.y, event.angle, event.ratio),\n        });\n      }, [registerEvents, sigma, draggedNode]);\n\n      return null;\n    };\n    return (\n        <Box>\n            <TextField id=\"propery_name\" label=\"Property to use as node name. Examples neat:Name or <http://purl.org/cognite/tnt/IdentifiedObject.name>\" value={nodeNameProperty} size='small' sx={{width:500}} variant=\"outlined\" onChange={handleNodeNameProperty}  />\n            <TextField id=\"response_limit\" label=\"Limit max nodes in response\" value={limitRecordsInResponse} size='small' type='number' sx={{width:150 , marginLeft:2}} variant=\"outlined\" onChange={handleResponseLimitChange}  />\n            <Button sx={{ marginLeft: 2 }} onClick={() => reload()  } variant=\"contained\"> Reload </Button>\n            <SigmaContainer style={{ height: \"70vh\", width: \"100%\" }}>\n                <LoadGraph filters={props.filters} nodeNameProperty={nodeNameProperty} reloader={reloader} sparqlQuery={sparqlQuery} mode={loaderMode} limit={limitRecordsInResponse}/>\n                <ControlsContainer position={\"top-right\"}>\n                    <LayoutForceAtlas2Control settings={{ settings: { slowDown: 10 } }} />\n                </ControlsContainer>\n                <GraphEvents />\n            </SigmaContainer>\n            <NodeViewer open={openNodeViewer} nodeId={selectedNodeId} onClose={onViewerClose} />\n        </Box>\n    );\n    }\n\n    const colorMap = {\n      \"Substation\": \"#42f557\",\n      \"Bay\": \"#4842f5\",\n      \"Line\": \"#f59b42\",\n      \"PowerTransformer\": \"#f54e42\",\n      \"HydroGeneratingUnit\": \"##0335fc\",\n      \"WindGeneratingUnit\": \"#03f0fc\",\n      \"SynchronousMachine\": \"#8d9191\",\n      \"plant\": \"#42f598\",\n      \"reservoir\": \"#4263f5\",\n      \"generator\": \"#f5c542\",\n      \"gate\": \"#889c6e\",\n      \"pump\": \"#f58a42\",\n    }\n\n    const sizeMap = {\n      \"plant\": 8,\n      \"reservoir\": 5,\n      \"gate\": 3,\n      \"generator\": 3,\n      \"pump\": 3,\n    }\n\n    function getSize(nodeClass:string,graphSize:number) {\n      if (nodeClass in sizeMap) {\n        return sizeMap[nodeClass];\n      } else\n        // calculate size based on graph size (from 1 to 15). max size for small graphs\n        if (graphSize < 15)\n          return 15;\n        if (graphSize >= 15 && graphSize < 100)\n          return 10;\n        else\n          return 5;\n    }\n\n    function getColor(nodeClass:string) {\n      if (nodeClass in colorMap) {\n        return colorMap[nodeClass];\n      } else\n        return \"#c0c4c4\";\n    }\n",
+        "import * as React from 'react';\nimport {useState,useEffect, useRef, useImperativeHandle,FC} from 'react';\nimport Box from '@mui/material/Box';\nimport Graph from \"graphology\";\nimport { SigmaContainer, useLoadGraph,useRegisterEvents } from \"@react-sigma/core\";\n\nimport \"@react-sigma/core/lib/react-sigma.min.css\";\nimport { ControlsContainer, useSigma } from \"@react-sigma/core\";\nimport { ExplorerContext } from 'components/Context';\nimport RemoveNsPrefix, { getNeatApiRootUrl, getSelectedWorkflowName } from 'components/Utils';\nimport TextField from '@mui/material/TextField';\nimport Button from '@mui/material/Button';\nimport NodeViewer from 'components/NodeViewer';\nimport LinearProgress from '@mui/material/LinearProgress';\nimport { useWorkerLayoutForceAtlas2,useLayoutForceAtlas2, LayoutForceAtlas2Control } from \"@react-sigma/layout-forceatlas2\";\nimport { useLayoutCircular } from \"@react-sigma/layout-circular\";\n\nexport function LoadGraph(props:{filters:Array<string>,nodeNameProperty:string,sparqlQuery:string,reloader:number,mode:string,limit:number}) {\n    const neatApiRootUrl = getNeatApiRootUrl();\n    const {hiddenNsPrefixModeCtx, graphNameCtx} = React.useContext(ExplorerContext);\n    const [graphName, setGraphName] = graphNameCtx;\n    const [hiddenNsPrefixMode, setHiddenNsPrefixMode ] = hiddenNsPrefixModeCtx;\n    const loadGraph = useLoadGraph();\n    // const { positions, assign } = useLayoutForceAtlas2({settings:{strongGravityMode:true},iterations:10});\n    const { positions, assign } = useLayoutCircular();\n    const { start, stop,kill } = useWorkerLayoutForceAtlas2({ settings: { slowDown: 5 } });\n    const [ bigGraph, setBigGraph] = useState<Graph>();\n    const [ loading, setLoading] = useState(false);\n\n\n    useEffect(() => {\n      loadDataset();\n    //   start();\n      return () => {\n        // Kill FA2 on unmount\n        kill();\n      };\n\n    }, [loadGraph,start,kill]);\n\n    useEffect(() => {\n      if (props.reloader || props.sparqlQuery) {\n        loadDataset();\n      }\n    }, [props.reloader,props.sparqlQuery]);\n\n    const loadDataset = () => {\n        setLoading(true);\n         console.log(\"loading dataset\");\n        //TODO - this is a hack to get the node name property for the solution graph. Make this configurable.\n        let nodeNameProperty = localStorage.getItem('nodeNameProperty');\n        // if(!props.nodeNameProperty) {\n        //   if (graphName == \"solution\") {\n        //       nodeNameProperty = \"\"\n        //   }else {\n        //       nodeNameProperty = \"\"\n        //   }\n        // }\n        let graph = new Graph();\n\n        if (props.mode== \"update\"){\n          graph = bigGraph;\n        }\n\n        const url = neatApiRootUrl+\"/api/get-nodes-and-edges\";\n        const workflowName = getSelectedWorkflowName();\n\n        const requestFilter = {\n            \"graph_name\": graphName,\n            \"workflow_name\":workflowName,\n            \"node_class_filter\": props.filters,\n            \"src_edge_filter\": props.filters,\n            \"dst_edge_filter\": props.filters,\n            \"node_name_property\": nodeNameProperty,\n            \"sparql_query\": props.sparqlQuery,\n            \"cache\": false,\n            \"limit\": props.limit\n        }\n        fetch(url,{ method:\"post\",body:JSON.stringify(requestFilter),headers: {\n            'Content-Type': 'application/json;charset=utf-8'\n          }}).then((response) => response.json()).then((data) => {\n            console.dir(data)\n            const addedNodes : string[] = [];\n            let graphSize = graph.size+data.nodes.length;\n            data.nodes.forEach((node) => {\n                let nodeClassName = RemoveNsPrefix(node.node_class);\n                const nodeLabel = node.node_name+\" (\"+nodeClassName+\")\";\n                if (!addedNodes.includes(node.node_id)) {\n                    addedNodes.push(node.node_id);\n                    graph.mergeNode(node.node_id,{label:nodeLabel,x:1,y:1,color:getColor(nodeClassName), size:getSize(nodeClassName,graphSize)});\n\n                }\n\n            });\n            data.edges.forEach((edge) => {\n              if (props.mode== \"update\"){\n                graph.mergeEdge(edge.src_object_ref,edge.dst_object_ref);\n              }else {\n                if (addedNodes.includes(edge.src_object_ref) && addedNodes.includes(edge.dst_object_ref)) {\n                  graph.mergeEdge(edge.src_object_ref,edge.dst_object_ref);\n                }\n              }\n\n            });\n            // loadGraph(graph);\n            setBigGraph(graph);\n            loadGraph(graph);\n            assign();\n            // if (props.mode== \"update\"){\n            // }else {\n            //   assign();\n            // }\n            console.log(\"graph loaded\");\n          }).catch((error) => {\n            console.log('Error:', error);\n          }).finally(() => {\n            setLoading(false);\n           });\n    }\n\n    return (loading &&( <LinearProgress />) );\n  };\n\n\nexport default function GraphExplorer(props:{filters:Array<string>,sparqlQuery:string}) {\n    const [nodeNameProperty, setNodeNameProperty] = useState(localStorage.getItem('nodeNameProperty'));\n    const [reloader, setReloader] = useState(0);\n    const loaderCompRef = useRef()\n    const [limitRecordsInResponse, setLimitRecordsInResponse] = useState(5000);\n    const [openNodeViewer, setOpenNodeViewer] = useState(false);\n    const [selectedNodeId, setSelectedNodeId] = useState(\"\");\n    const [sparqlQuery, setSparqlQuery] = useState(\"\");\n    const [loaderMode, setLoaderMode] = useState(\"create\");\n\n    const handleNodeNameProperty = (event: React.ChangeEvent<HTMLInputElement>) => {\n        setNodeNameProperty(event.target.value);\n        localStorage.setItem('nodeNameProperty',event.target.value);\n        reload();\n    };\n\n    const handleResponseLimitChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n        setLimitRecordsInResponse(parseInt(event.target.value));\n    };\n    const reload = () => {\n          setReloader(reloader+1);\n    }\n\n    useEffect(() => {\n      console.log(\"sparqlQuery changed\");\n      setNodeNameProperty(localStorage.getItem('nodeNameProperty'));\n      setSparqlQuery(props.sparqlQuery);\n    }, [props.sparqlQuery]);\n\n\n    const onViewerClose = () => {\n      setOpenNodeViewer(false);\n    }\n\n    const loadLinkedNodes = (nodeRef:string) => {\n      let query = \"\"\n      const nodeNameProperty = localStorage.getItem('nodeNameProperty')\n      if (!nodeNameProperty) {\n\n        query = `SELECT (?dst_object_ref AS ?node_name) (?linked_obj_type  AS ?node_class) (?dst_object_ref AS ?node_id) ?src_object_ref ?dst_object_ref WHERE {\n          BIND( <`+nodeRef+`> AS ?src_object_ref )\n          {\n           ?src_object_ref ?rel_propery ?dst_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type\n          }\n          UNION\n          {\n           ?dst_object_ref ?rel_propery ?src_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type .\n          }\n          }  `\n      }else {\n        query = `SELECT ?node_name (?linked_obj_type  AS ?node_class) (?dst_object_ref AS ?node_id) ?src_object_ref ?dst_object_ref WHERE {\n          BIND( <`+nodeRef+`> AS ?src_object_ref )\n          {\n           ?src_object_ref ?rel_propery ?dst_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type .\n           ?dst_object_ref `+nodeNameProperty+` ?node_name .\n          }\n          UNION\n          {\n           ?dst_object_ref ?rel_propery ?src_object_ref .\n           ?dst_object_ref rdf:type ?linked_obj_type .\n           ?dst_object_ref `+nodeNameProperty+` ?node_name .\n          }\n          } `\n      }\n      console.log(\"requesting linked nodes\");\n\n      setSparqlQuery(query);\n    }\n\n    const GraphEvents: React.FC = () => {\n      const registerEvents = useRegisterEvents();\n      const sigma = useSigma();\n      const [draggedNode, setDraggedNode] = useState<string | null>(null);\n      useEffect(() => {\n        // Register the events\n        registerEvents({\n          // node events\n          rightClickNode: (event) => {\n            // event.preventSigmaDefault();\n            console.log(\"clickNode\", event.event, event.node )\n            console.log(\"node id: \"+event.node);\n            setLoaderMode(\"update\");\n            setSelectedNodeId(event.node);\n            loadLinkedNodes(event.node);\n            sigma.getGraph().setNodeAttribute(event.node, \"highlighted\", true);\n\n          },\n          doubleClickNode: (event) => {\n            setSelectedNodeId(event.node);\n            setOpenNodeViewer(true);\n          },\n          mouseup: (e) => {\n            if (draggedNode) {\n              setDraggedNode(null);\n              sigma.getGraph().removeNodeAttribute(draggedNode, \"highlighted\");\n            }\n          },\n          mousedown: (e) => {\n            // Disable the autoscale at the first down interaction\n            if (!sigma.getCustomBBox()) sigma.setCustomBBox(sigma.getBBox());\n          },\n          mousemove: (e) => {\n            if (draggedNode) {\n              // Get new position of node\n              console.log(\"draggedNode\",draggedNode);\n              const pos = sigma.viewportToGraph(e);\n              sigma.getGraph().setNodeAttribute(draggedNode, \"x\", pos.x);\n              sigma.getGraph().setNodeAttribute(draggedNode, \"y\", pos.y);\n\n              // Prevent sigma to move camera:\n              e.preventSigmaDefault();\n              e.original.preventDefault();\n              e.original.stopPropagation();\n            }\n          },\n          downNode: (e) => {\n            setDraggedNode(e.node);\n            sigma.getGraph().setNodeAttribute(e.node, \"highlighted\", true);\n          },\n          // rightClickNode: (event) => console.log(\"rightClickNode\", event.event, event.node, event.preventSigmaDefault),\n          // wheelNode: (event) => console.log(\"wheelNode\", event.event, event.node, event.preventSigmaDefault),\n          // downNode: (event) => console.log(\"downNode\", event.event, event.node, event.preventSigmaDefault),\n          // enterNode: (event) => console.log(\"enterNode\", event.node),\n          // leaveNode: (event) => console.log(\"leaveNode\", event.node),\n          // // edge events\n          // clickEdge: (event) => console.log(\"clickEdge\", event.event, event.edge, event.preventSigmaDefault),\n          // doubleClickEdge: (event) => console.log(\"doubleClickEdge\", event.event, event.edge, event.preventSigmaDefault),\n          // rightClickEdge: (event) => console.log(\"rightClickEdge\", event.event, event.edge, event.preventSigmaDefault),\n          // wheelEdge: (event) => console.log(\"wheelEdge\", event.event, event.edge, event.preventSigmaDefault),\n          // downEdge: (event) => console.log(\"downEdge\", event.event, event.edge, event.preventSigmaDefault),\n          // enterEdge: (event) => console.log(\"enterEdge\", event.edge),\n          // leaveEdge: (event) => console.log(\"leaveEdge\", event.edge),\n          // // stage events\n          // clickStage: (event) => console.log(\"clickStage\", event.event, event.preventSigmaDefault),\n          // doubleClickStage: (event) => console.log(\"doubleClickStage\", event.event, event.preventSigmaDefault),\n          // rightClickStage: (event) => console.log(\"rightClickStage\", event.event, event.preventSigmaDefault),\n          // wheelStage: (event) => console.log(\"wheelStage\", event.event, event.preventSigmaDefault),\n          // downStage: (event) => console.log(\"downStage\", event.event, event.preventSigmaDefault),\n          // // default mouse events\n          // click: (event) => console.log(\"click\", event.x, event.y),\n          // doubleClick: (event) => console.log(\"doubleClick\", event.x, event.y),\n          // wheel: (event) => console.log(\"wheel\", event.x, event.y, event.delta),\n          // rightClick: (event) => console.log(\"rightClick\", event.x, event.y),\n          // mouseup: (event) => console.log(\"mouseup\", event.x, event.y),\n          // mousedown: (event) => console.log(\"mousedown\", event.x, event.y),\n          // mousemove: (event) => console.log(\"mousemove\", event.x, event.y),\n          // // default touch events\n          // touchup: (event) => console.log(\"touchup\", event.touches),\n          // touchdown: (event) => console.log(\"touchdown\", event.touches),\n          // touchmove: (event) => console.log(\"touchmove\", event.touches),\n          // // sigma kill\n          // kill: () => console.log(\"kill\"),\n          // resize: () => console.log(\"resize\"),\n          // beforeRender: () => console.log(\"beforeRender\"),\n          // afterRender: () => console.log(\"afterRender\"),\n          // // sigma camera update\n          // updated: (event) => console.log(\"updated\", event.x, event.y, event.angle, event.ratio),\n        });\n      }, [registerEvents, sigma, draggedNode]);\n\n      return null;\n    };\n    return (\n        <Box>\n            <TextField id=\"propery_name\" label=\"Property to use as node name. Examples neat:Name or <http://purl.org/cognite/tnt/IdentifiedObject.name>\" value={nodeNameProperty} size='small' sx={{width:500}} variant=\"outlined\" onChange={handleNodeNameProperty}  />\n            <TextField id=\"response_limit\" label=\"Limit max nodes in response\" value={limitRecordsInResponse} size='small' type='number' sx={{width:150 , marginLeft:2}} variant=\"outlined\" onChange={handleResponseLimitChange}  />\n            <Button sx={{ marginLeft: 2 }} onClick={() => reload()  } variant=\"contained\"> Reload </Button>\n            <SigmaContainer style={{ height: \"70vh\", width: \"100%\" }}>\n                <LoadGraph filters={props.filters} nodeNameProperty={nodeNameProperty} reloader={reloader} sparqlQuery={sparqlQuery} mode={loaderMode} limit={limitRecordsInResponse}/>\n                <ControlsContainer position={\"top-right\"}>\n                    <LayoutForceAtlas2Control settings={{ settings: { slowDown: 10 } }} />\n                </ControlsContainer>\n                <GraphEvents />\n            </SigmaContainer>\n            <NodeViewer open={openNodeViewer} nodeId={selectedNodeId} onClose={onViewerClose} />\n        </Box>\n    );\n    }\n\n    const colorMap = {\n      \"Substation\": \"#42f557\",\n      \"Bay\": \"#4842f5\",\n      \"Line\": \"#f59b42\",\n      \"PowerTransformer\": \"#f54e42\",\n      \"HydroGeneratingUnit\": \"##0335fc\",\n      \"WindGeneratingUnit\": \"#03f0fc\",\n      \"SynchronousMachine\": \"#8d9191\",\n      \"plant\": \"#42f598\",\n      \"reservoir\": \"#4263f5\",\n      \"generator\": \"#f5c542\",\n      \"gate\": \"#889c6e\",\n      \"pump\": \"#f58a42\",\n    }\n\n    const sizeMap = {\n      \"plant\": 8,\n      \"reservoir\": 5,\n      \"gate\": 3,\n      \"generator\": 3,\n      \"pump\": 3,\n    }\n\n    function getSize(nodeClass:string,graphSize:number) {\n      if (nodeClass in sizeMap) {\n        return sizeMap[nodeClass];\n      } else\n        // calculate size based on graph size (from 1 to 15). max size for small graphs\n        if (graphSize < 15)\n          return 15;\n        if (graphSize >= 15 && graphSize < 100)\n          return 10;\n        else\n          return 5;\n    }\n\n    function getColor(nodeClass:string) {\n      if (nodeClass in colorMap) {\n        return colorMap[nodeClass];\n      } else\n        return \"#c0c4c4\";\n    }\n",
         "import { useCallback } from \"react\";\nimport Graph from \"graphology\";\n\nimport { useSigma } from \"./useSigma\";\n\n/**\n * React hook that helps you to load a graph.\n * If a graph was previously loaded in Sigma/Graphology, per default it is cleared.\n * You can change this behaviour by settings the parameter `clear` to false.\n *\n * ```typescript\n * const loadGraph = useLoadGraph();\n * loadGraph(erdosRenyi(UndirectedGraph, { order: 100, probability: 0.2 }), true);\n *```\n * @category Hook\n */\nexport function useLoadGraph(): (graph: Graph, clear?: boolean) => void {\n  const sigma = useSigma();\n\n  return useCallback(\n    (graph: Graph, clear = true) => {\n      if (sigma && graph) {\n        if (clear && sigma.getGraph().order > 0) sigma.getGraph().clear();\n        sigma.getGraph().import(graph);\n        sigma.refresh();\n      }\n    },\n    [sigma],\n  );\n}\n",
-        "import * as React from 'react';\nimport {useState,useEffect} from 'react';\nimport Box from '@mui/material/Box';\nimport InputLabel from '@mui/material/InputLabel';\nimport MenuItem from '@mui/material/MenuItem';\nimport FormControl from '@mui/material/FormControl';\nimport Select, { SelectChangeEvent } from '@mui/material/Select';\nimport Button from '@mui/material/Button';\nimport TextareaAutosize from '@mui/material/TextareaAutosize';\nimport { DataGrid, GridColDef, GridRenderCellParams } from '@mui/x-data-grid';\nimport LinearProgress from '@mui/material/LinearProgress';\nimport Typography from '@mui/material/Typography';\nimport Collapse from '@mui/material/Collapse';\nimport Alert from '@mui/material/Alert';\nimport IconButton from '@mui/material/IconButton';\nimport CloseIcon from '@mui/icons-material/Close';\nimport Breadcrumbs from '@mui/material/Breadcrumbs';\nimport Link from '@mui/material/Link';\nimport TextField from '@mui/material/TextField';\nimport Switch from '@mui/material/Switch';\nimport FormControlLabel from '@mui/material/FormControlLabel';\nimport Tabs from '@mui/material/Tabs';\nimport Tab from '@mui/material/Tab';\nimport TabPanel from 'components/TabPanel';\nimport OverviewRow from './OverviewView';\nimport OverviewTable from './OverviewView';\nimport { ExplorerContext } from '../components/Context';\nimport RemoveNsPrefix, { getNeatApiRootUrl, getSelectedWorkflowName,getShortenedString } from '../components/Utils';\nimport Chip from '@mui/material/Chip';\nimport OutlinedInput from '@mui/material/OutlinedInput';\nimport { Theme, useTheme } from '@mui/material/styles';\nimport GraphExplorer from './GraphView';\nimport AlertTitle from '@mui/material/AlertTitle';\n\n\nfunction handleClick(event: React.MouseEvent<HTMLDivElement, MouseEvent>) {\n  event.preventDefault();\n  console.info('You clicked a breadcrumb.');\n}\n\nexport function NavBreadcrumbs( props:{bhistory:Array<string>,selectedHandler:Function} ) {\n  if (props.bhistory)\n  {\n  return (\n    <div role=\"presentation\" onClick={handleClick}>\n      <Breadcrumbs aria-label=\"breadcrumb\">\n        {props.bhistory.map((item => (\n        <Link underline=\"hover\" color=\"inherit\" onClick={()=>{props.selectedHandler(item)}}>\n          {item}\n        </Link>\n        )))}\n      </Breadcrumbs>\n\n    </div>\n  );} else\n    return ( <Breadcrumbs aria-label=\"breadcrumb\"></Breadcrumbs>);\n }\n\nexport function QuerySelector(props:{selectedHandler:Function,settingsUpdateHandler:Function}) {\n    const neatApiRootUrl = getNeatApiRootUrl();\n    const [query, setQuery] = useState('');\n    const [rule, setRule] = useState('');\n    const [data, setData] = useState([]);\n    const [advancedMode, setAdvancedMode] = useState(false);\n\n    const {hiddenNsPrefixModeCtx, graphNameCtx} = React.useContext(ExplorerContext);\n    const [graphName, setGraphName] = graphNameCtx;\n    const [hiddenNsPrefixMode, setHiddenNsPrefixMode ] = hiddenNsPrefixModeCtx;\n\n    const handleTemplateChange = (event: SelectChangeEvent) => {\n      setQuery(event.target.value as string);\n    };\n\n    const handleGraphChange = (event: SelectChangeEvent) => {\n      console.log(\"handleGraphChange\",event.target.value);\n      setGraphName(event.target.value);\n    };\n\n    const handleQueryChange = (event: React.ChangeEvent<HTMLTextAreaElement>) => {\n      setQuery(event.target.value);\n    };\n\n    const handleRuleChange = (event: React.ChangeEvent<HTMLTextAreaElement>) => {\n      setRule(event.target.value);\n    };\n\n    const handleAdvancedChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n      setAdvancedMode(event.target.checked);\n    };\n    const handleHiddenNsPrefixModeChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n      console.log(\"hiddenNsPrefixMode\",event.target.checked);\n      setHiddenNsPrefixMode(event.target.checked);\n      props.settingsUpdateHandler();\n    };\n\n    useEffect(() => {\n      fetch(neatApiRootUrl+`/api/list-queries`)\n       .then((response) => response.json())\n        .then((data) => setData(data));\n     }, []);\n\n    return (\n      <Box sx={{ minWidth: 400  }}>\n        <FormControlLabel sx={{marginBottom:2}}  control={<Switch value={advancedMode} onChange={handleAdvancedChange} />} label=\"Advanced mode\" />\n        <FormControlLabel sx={{marginBottom:2}}  control={<Switch value={hiddenNsPrefixMode} onChange={handleHiddenNsPrefixModeChange} defaultChecked />} label=\"Hidden NS Prefix mode\" />\n        <Box>\n        <FormControl sx={{width:500,marginBottom:2}} >\n          <InputLabel id=\"graphSelectorLabel\">Graph to query</InputLabel>\n            <Select\n              labelId=\"graphSelectorLabel\"\n              id=\"graphSelector\"\n              value={graphName}\n              label=\"Graph to query\"\n              size='small'\n              onChange={handleGraphChange}\n            >\n              <MenuItem value=\"source\" >Source graph </MenuItem>\n              <MenuItem value=\"solution\" >Solution graph </MenuItem>\n            </Select>\n        </FormControl>\n        </Box>\n        {advancedMode && (\n        <React.Fragment>\n        <FormControl sx={{width:\"80vw\"}}>\n          <InputLabel id=\"queryTemplateSelectorLabel\">Query template</InputLabel>\n          <Select\n            labelId=\"queryTemplateSelectorLabel\"\n            id=\"queryTemplateSelector\"\n            value={query}\n            size='small'\n            label=\"Query template\"\n            onChange={handleTemplateChange}\n          >\n          {\n            data && data.map((item,i) => (\n              <MenuItem value={item.query} key={i}>{item.name} </MenuItem>\n            ))\n          }\n          </Select>\n        </FormControl>\n        <div style={{margin:\"10px\"}}> </div>\n        <Box>\n        <TextareaAutosize  aria-label=\"SPARQL query\" minRows={2} value = {query} placeholder=\"SPARQL query\" style={{width:\"80vw\"}}  onChange={handleQueryChange} />\n        <Button sx={{ margin: \"5px\" }} variant=\"contained\" onClick={()=>{ props.selectedHandler(query,\"query\") }}> Run query </Button>\n        </Box>\n        <Box>\n         <TextField id=\"rule\" label=\"Rule\" value = {rule} size='small' sx={{width:\"80vw\"}} variant=\"outlined\" onChange={handleRuleChange}  />\n         <Button sx={{ margin: \"5px\" }} variant=\"contained\" onClick={()=>{ props.selectedHandler(rule,\"rule\") }}> Execute rule </Button>\n         </Box>\n        </React.Fragment>\n)}\n        <Box>\n\n        </Box>\n      </Box>\n    );\n  }\n\nexport function SearchBar(props:{searchButtonHandler:Function}) {\n    const [searchStr, setSearchStr] = useState('');\n    const [searchType,setSearchType] = useState(\"value_exact_match\");\n\n    const handleSearchTypeChange = (event: SelectChangeEvent) => {\n      setSearchType(event.target.value);\n    };\n    const handleSearchStrChange = (event: React.ChangeEvent<HTMLTextAreaElement>) => {\n      setSearchStr(event.target.value);\n    };\n\n\n    return (\n        <Box sx={{marginBottom:1,marginTop:1}}>\n         <TextField id=\"search\" label=\"Search\" value={searchStr} size='small' sx={{width:500}} variant=\"outlined\" onChange={handleSearchStrChange}  />\n         <FormControl sx={{width:180 , marginLeft:2}} >\n          <InputLabel id=\"graphSearchTypeLabel\">type</InputLabel>\n            <Select\n              labelId=\"graphSearcTypehLabel\"\n              id=\"graphSearchType\"\n              value={searchType}\n              label=\"type\"\n              size='small'\n              onChange={handleSearchTypeChange}\n            >\n              <MenuItem value=\"value_exact_match\" > Exact match </MenuItem>\n              <MenuItem value=\"value_regexp\" > Free search </MenuItem>\n              <MenuItem value=\"reference\" > Object reference </MenuItem>\n            </Select>\n        </FormControl>\n         <Button sx={{ marginLeft: 2 }} variant=\"contained\" onClick={()=>{props.searchButtonHandler(searchStr,searchType)}}> Search </Button>\n        </Box>\n    );\n  }\n\nconst ITEM_HEIGHT = 48;\nconst ITEM_PADDING_TOP = 8;\nconst MenuProps = {\n    PaperProps: {\n      style: {\n        maxHeight: ITEM_HEIGHT * 4.5 + ITEM_PADDING_TOP,\n        width: 250,\n      },\n    },\n};\n\nfunction getStyles(name: string, personName: readonly string[], theme: Theme) {\n  return {\n    fontWeight:\n      personName.indexOf(name) === -1\n        ? theme.typography.fontWeightRegular\n        : theme.typography.fontWeightMedium,\n  };\n}\n\nexport function FilterBar(props:{filterChangeHandler:Function}) {\n    const neatApiRootUrl = getNeatApiRootUrl();\n    const [filters, setFilters] = React.useState<string[]>([]);\n    const theme = useTheme();\n    const {hiddenNsPrefixModeCtx, graphNameCtx} = React.useContext(ExplorerContext);\n    const [graphName, setGraphName] = graphNameCtx;\n    const [hiddenNsPrefixMode, setHiddenNsPrefixMode ] = hiddenNsPrefixModeCtx;\n\n    const [filterOptions, setFilterOptions] = React.useState([]);\n    const [alertMsg, setAlertMsg] = useState(\"\");\n\n    useEffect(() => {\n      loadClassSummary();\n    }, [graphName]);\n\n    const handleChange = (event: SelectChangeEvent<typeof filters>) => {\n      const { target: { value }, } = event;\n      setFilters(\n        // On autofill we get a stringified value.\n        typeof value === 'string' ? value.split(',') : value,\n      );\n      props.filterChangeHandler(filters)\n    };\n\n    function sortArrayOfObjectsByName(arr) {\n      return\n    }\n\n    const loadClassSummary = () => {\n      const workflowName = getSelectedWorkflowName();\n      const url = neatApiRootUrl+\"/api/get-classes?\"+new URLSearchParams({\"graph_name\":graphName,\"cache\":\"false\",\"workflow_name\":workflowName}).toString();\n\n      fetch(url).then((response) => response.json()).then((data) => {\n        if (data.error) {\n          setAlertMsg(\"The workflow is missing or has uninitialized graph stores. Please ensure that you add a graph store and/or run the workflow before proceeding. Error msg: \"+data.error);\n          return;\n        }\n        let options = [];\n        data.rows.forEach((row) => {\n          let vClass = \"\";\n          if (hiddenNsPrefixMode) {\n            vClass = RemoveNsPrefix(row.class);\n          }else {\n            vClass = row.class;\n          }\n\n          // vClass = row.class;\n          setAlertMsg(\"\");\n          options.push({class:vClass,ns_class:row.class});\n        });\n        options = options.sort((a, b) => a.class.localeCompare(b.class));\n        setFilterOptions(options);\n      }).catch((error) => {\n        console.error('Error:', error);\n        setAlertMsg(\"The workflow is missing or has uninitialized graph stores. Please ensure that you add a graph store and/or run the workflow before proceeding. Error msg: \"+error);\n      }).finally(() => {\n       });\n    }\n\n    return (\n      <div>\n    {alertMsg != \"\" && (<Alert severity=\"warning\">\n          <AlertTitle>Warning</AlertTitle>\n          {alertMsg}\n    </Alert> )}\n      <FormControl sx={{ m: 0, width: \"94vw\" }}>\n        <InputLabel id=\"demo-multiple-chip-label\">Filter</InputLabel>\n        <Select\n          labelId=\"demo-multiple-chip-label\"\n          id=\"demo-multiple-chip\"\n          multiple\n          value={filters}\n          size='small'\n          onChange={handleChange}\n          input={<OutlinedInput id=\"select-multiple-chip\" label=\"Chip\" />}\n          renderValue={(selected) => (\n            <Box sx={{ display: 'flex', flexWrap: 'wrap', gap: 0.5 }}>\n              {selected.map((value) => (\n                <Chip key={value} label={value} />\n              ))}\n            </Box>\n          )}\n          MenuProps={MenuProps}\n        >\n          {filterOptions.map((item) => (\n            <MenuItem\n              key={item.ns_class}\n              value={item.ns_class}\n              style={getStyles(item.ns_class, filters, theme)}\n            >\n              {item.class}\n            </MenuItem>\n          ))}\n        </Select>\n      </FormControl>\n    </div>\n    );\n}\n\nfunction reshapeData(data) {\n    data.rows.map((item,i) => {\n      item[\"id\"] = i;\n    });\n    return;\n  }\n\nfunction a11yProps(index: number) {\n    return {\n      id: `simple-tab-${index}`,\n      'aria-controls': `simple-tabpanel-${index}`,\n    };\n}\n\n\nexport default function QDataTable() {\n  const neatApiRootUrl = getNeatApiRootUrl();\n  const [loading, setLoading] = React.useState(false);\n  const [data, setData] = useState({\"fields\": [], \"rows\": [] , \"query\": \"\" ,\"elapsed_time_sec\":0, \"error\": \"\"});\n  const [columns, setColumns] = useState([]);\n  const [openAlert, setOpenAlert] = React.useState(false);\n  const [alertMsg, setAlertMsg] = useState(\"\");\n\n  const [graphName, setGraphName] = React.useState(\"source\");\n  const [hiddenNsPrefixMode, setHiddenNsPrefixMode] = useState(true);\n\n  const [bhistory, setBhistory] = useState(Array<string>);\n  const [tabValue, setTabValue] = React.useState(0);\n  const [filters , setFilters] = React.useState(Array<string>);\n  const [sparqlQuery, setSparqlQuery] = React.useState(\"\");\n\n  // const {hiddenNsPrefixModeCtx, graphNameCtx} = React.useContext(ExplorerContext);\n  // const [graphName, setGraphName] = graphNameCtx;\n  // const [hiddenNsPrefixMode, setHiddenNsPrefixMode ] = hiddenNsPrefixModeCtx;\n  let nodeNameProperty = \"\"\n\n  \n  const getColumnDefs = (fields:[string]) => {\n    const columns: GridColDef[] = [];\n    columns.push({field: 'id', headerName: 'ID', width: 70});\n    fields.map((field) => {\n      columns.push({field: field, headerName: field,renderCell: renderCellExpand , flex:0.5});\n    });\n    return columns;\n  }\n\n  const loadObjectAsGraph = (reference:string) => {\n    setTabValue(2);\n    nodeNameProperty = localStorage.getItem('nodeNameProperty')\n    let query = ``\n    if (!nodeNameProperty) {\n      query = `SELECT (?inst AS ?node_name) ?node_class (?inst AS ?node_id) WHERE { \n        BIND( <`+reference+`> AS ?inst)\n        ?inst rdf:type ?node_class . \n        } `\n    } else {\n      query = `SELECT ?node_name ?node_class (?inst AS ?node_id) WHERE { \n        BIND( <`+reference+`> AS ?inst)\n        ?inst `+nodeNameProperty+` ?node_name .\n        ?inst rdf:type ?node_class . \n        } `\n    }   \n\n    setSparqlQuery(query);  \n    // loadDataset(sparqlQuery,\"query\");\n  }\n\n  const loadObjectProperties = (reference:string) => {\n    const newHistory  = bhistory.slice();\n    let deleteFlag = false;\n    for (const [index, value] of newHistory.entries()) {\n      if (value == reference) {\n         deleteFlag = true;\n         bhistory.splice(index);\n         break;\n      }\n      console.log(\"somethiong here\");\n    }\n    bhistory.push(reference);\n    const workflowName = getSelectedWorkflowName();\n    fetch(neatApiRootUrl+`/api/object-properties?`+new URLSearchParams({\"reference\":reference,\"graph_name\":graphName,\"workflow_name\":workflowName}).toString())\n     .then((response) => response.json())\n      .then((rdata) => {\n        reshapeData(rdata);\n        const cm = getColumnDefs(rdata.fields)\n        setColumns(cm);\n        setData(rdata)\n        setLoading(false);\n        setOpenAlert(true);\n      }).catch((error) => {\n        console.error('Error:', error);\n        setData({\"fields\": [], \"rows\": [] , \"query\": \"\" ,\"elapsed_time_sec\":0, \"error\": error.message})\n        setLoading(false);\n        setOpenAlert(true);\n      });\n   }\n\n   const searchObjects = (searchStr:string,searchType:string) => {\n      setTabValue(1);\n      setLoading(true);\n      const workflowName = getSelectedWorkflowName();\n      fetch(neatApiRootUrl+`/api/search?`+new URLSearchParams({\"search_str\":searchStr,\"graph_name\":graphName,\"search_type\":searchType,\"workflow_name\":workflowName}).toString())\n      .then((response) => response.json())\n        .then((rdata) => {\n          reshapeData(rdata);\n          const cm = getColumnDefs(rdata.fields)\n          setColumns(cm);\n          setData(rdata)\n          setLoading(false);\n          setOpenAlert(true);\n        }).catch((error) => {\n          console.error('Error:', error);\n          setData({\"fields\": [], \"rows\": [] , \"query\": \"\" ,\"elapsed_time_sec\":0, \"error\": error.message})\n          setLoading(false);\n          setOpenAlert(true);\n        });\n   }\n\n   const handleFilterChange = (filters:string[]) => {\n    console.log(\"handleFilterChange\",filters);\n    setFilters(filters);\n   }\n  const renderCellExpand = (params) => {\n    console.log(hiddenNsPrefixMode);\n    if (params.value?.includes(\"#_\")) {\n      return <Box>{getShortenedString(params.value,10)} <Button onClick={(e)=> {loadObjectProperties(params.value)}}>Table </Button> <Button onClick={(e)=> {loadObjectAsGraph(params.value)}}>Graph </Button></Box>  \n\n      } else if (params.value?.includes(\"#\") && hiddenNsPrefixMode) {\n      const value = RemoveNsPrefix(params.value);\n\n      return <Box sx={{ display: 'flex' }}> {value}</Box>\n    } else\n    return (\n       <Box sx={{ display: 'flex' }}> {params.value}</Box>\n    );\n  }\n\n  const settingsUpdateHandler = (settings:any) => {\n    console.log(\"settingsUpdateHandler\",settings);\n    if (settings) {\n      setGraphName(settings.graphName);\n      setHiddenNsPrefixMode(settings.hiddenNsPrefixMode);\n    }\n  }\n\n  const handleRunQueryCommand = (q:string,qtype:string) => {\n    setSparqlQuery(q);\n    if (tabValue == 0) {\n      // switching from Overview tab to Table tab\n      setTabValue(1);\n    }\n    if (tabValue != 2) {\n      // non-graph tab\n      loadDataset(q,qtype);\n    }\n    \n  };\n\n  const loadDataset = (q:string,qtype:string) => {\n    let query = {}\n    let url = \"\"\n\n    console.log('reseting history');\n    setLoading(true);\n    const workflowName = getSelectedWorkflowName();\n    if (qtype == \"query\") {\n      query = {\"query\":q,\"graph_name\":graphName,\"workflow_name\":workflowName}\n      url = neatApiRootUrl+\"/api/query\"\n    } else if (qtype == \"rule\") {\n      query = {\"rule\":q,\"rule_type\":\"rdfpath\",\"graph_name\":graphName,\"workflow_name\":workflowName}\n      url = neatApiRootUrl+\"/api/execute-rule\"\n    }\n\n    fetch(url,{ method:\"post\",body:JSON.stringify(query),headers: {\n      'Content-Type': 'application/json;charset=utf-8'\n    }})\n    .then((response) => response.json()).then((rdata) => {\n      console.dir(rdata)\n      reshapeData(rdata);\n      const cm = getColumnDefs(rdata.fields)\n      setColumns(cm);\n      setData(rdata)\n      setLoading(false);\n      setOpenAlert(true);\n    }).catch((error) => {\n      console.error('Error:', error);\n      setData({\"fields\": [], \"rows\": [] , \"query\": \"\" ,\"elapsed_time_sec\":0, \"error\": error.message})\n      setLoading(false);\n      setOpenAlert(true);\n    });\n  }\n\n  const handleTabChange = (event: React.SyntheticEvent, newValue: number) => {\n    console.log(\"handleTabChange\",newValue);\n    setTabValue(newValue);\n  };\n\n  const activateTable= (className:string) => {\n    setTabValue(1);\n    let sparqlQuery = `SELECT ?instance ?property ?value  WHERE {\n      ?instance rdf:type <`+className+`> .\n      ?instance ?property ?value\n     } LIMIT 10000`\n    loadDataset(sparqlQuery,\"query\");\n  }\n\n  return (\n    <div>\n\n    <ExplorerContext.Provider value={{hiddenNsPrefixModeCtx:[hiddenNsPrefixMode, setHiddenNsPrefixMode],graphNameCtx:[graphName, setGraphName]}}>\n    {alertMsg != \"\" && (<Alert severity=\"warning\">\n          <AlertTitle>Warning</AlertTitle>\n            {alertMsg}\n    </Alert> )}\n    <QuerySelector selectedHandler={handleRunQueryCommand} settingsUpdateHandler={settingsUpdateHandler}/>\n    <SearchBar searchButtonHandler={searchObjects} />\n    <FilterBar filterChangeHandler={handleFilterChange}/>\n    { loading &&( <LinearProgress />) }\n    <Box sx={{ width: '100%' }}>\n      <Tabs value={tabValue} onChange={handleTabChange} aria-label=\"Explorer tabls\">\n        <Tab label=\"Overview\" {...a11yProps(0)} />\n        <Tab label=\"Table\" {...a11yProps(1)} />\n        <Tab label=\"Graph\" {...a11yProps(2)} />\n      </Tabs>\n      <TabPanel value={tabValue} index={0}>\n       <OverviewTable onItemClick={activateTable}/>\n      </TabPanel>\n      <TabPanel value={tabValue} index={1} >\n        <NavBreadcrumbs bhistory={bhistory} selectedHandler={loadObjectProperties}/>\n        <div style={{ height: '70vh', width: '100%' }}>\n          <DataGrid\n              rows={data.rows}\n              columns={columns}\n              pageSize={100}\n              rowsPerPageOptions={[5]}\n            />\n        </div>\n      </TabPanel>\n      <TabPanel value={tabValue} index={2}>\n        <GraphExplorer filters={filters} sparqlQuery={sparqlQuery}/>\n      </TabPanel>\n      <Collapse in={openAlert}>\n            <Alert\n              action={\n                <IconButton aria-label=\"close\" color=\"inherit\" size=\"small\" onClick={() => { setOpenAlert(false); }} >\n                  <CloseIcon fontSize=\"inherit\" />\n                </IconButton>\n              } sx={{ mb: 2 }}>\n              Elapsed time: {data.elapsed_time_sec*1000} ms. Number of rows: {data.rows.length} . <Box> SPARQL query : {data.query } </Box>\n              {data.error &&(<Box> Error: {data.error} </Box>) }\n            </Alert>\n        </Collapse>\n    </Box>\n\n    </ExplorerContext.Provider>\n    </div>\n  );\n}\n",
+        "import * as React from 'react';\nimport {useState,useEffect} from 'react';\nimport Box from '@mui/material/Box';\nimport InputLabel from '@mui/material/InputLabel';\nimport MenuItem from '@mui/material/MenuItem';\nimport FormControl from '@mui/material/FormControl';\nimport Select, { SelectChangeEvent } from '@mui/material/Select';\nimport Button from '@mui/material/Button';\nimport TextareaAutosize from '@mui/material/TextareaAutosize';\nimport { DataGrid, GridColDef, GridRenderCellParams } from '@mui/x-data-grid';\nimport LinearProgress from '@mui/material/LinearProgress';\nimport Typography from '@mui/material/Typography';\nimport Collapse from '@mui/material/Collapse';\nimport Alert from '@mui/material/Alert';\nimport IconButton from '@mui/material/IconButton';\nimport CloseIcon from '@mui/icons-material/Close';\nimport Breadcrumbs from '@mui/material/Breadcrumbs';\nimport Link from '@mui/material/Link';\nimport TextField from '@mui/material/TextField';\nimport Switch from '@mui/material/Switch';\nimport FormControlLabel from '@mui/material/FormControlLabel';\nimport Tabs from '@mui/material/Tabs';\nimport Tab from '@mui/material/Tab';\nimport TabPanel from 'components/TabPanel';\nimport OverviewRow from './OverviewView';\nimport OverviewTable from './OverviewView';\nimport { ExplorerContext } from '../components/Context';\nimport RemoveNsPrefix, { getNeatApiRootUrl, getSelectedWorkflowName,getShortenedString } from '../components/Utils';\nimport Chip from '@mui/material/Chip';\nimport OutlinedInput from '@mui/material/OutlinedInput';\nimport { Theme, useTheme } from '@mui/material/styles';\nimport GraphExplorer from './GraphView';\nimport AlertTitle from '@mui/material/AlertTitle';\n\n\nfunction handleClick(event: React.MouseEvent<HTMLDivElement, MouseEvent>) {\n  event.preventDefault();\n  console.info('You clicked a breadcrumb.');\n}\n\nexport function NavBreadcrumbs( props:{bhistory:Array<string>,selectedHandler:Function} ) {\n  if (props.bhistory)\n  {\n  return (\n    <div role=\"presentation\" onClick={handleClick}>\n      <Breadcrumbs aria-label=\"breadcrumb\">\n        {props.bhistory.map((item => (\n        <Link underline=\"hover\" color=\"inherit\" onClick={()=>{props.selectedHandler(item)}}>\n          {item}\n        </Link>\n        )))}\n      </Breadcrumbs>\n\n    </div>\n  );} else\n    return ( <Breadcrumbs aria-label=\"breadcrumb\"></Breadcrumbs>);\n }\n\nexport function QuerySelector(props:{selectedHandler:Function,settingsUpdateHandler:Function}) {\n    const neatApiRootUrl = getNeatApiRootUrl();\n    const [query, setQuery] = useState('');\n    const [rule, setRule] = useState('');\n    const [data, setData] = useState([]);\n    const [advancedMode, setAdvancedMode] = useState(false);\n\n    const {hiddenNsPrefixModeCtx, graphNameCtx} = React.useContext(ExplorerContext);\n    const [graphName, setGraphName] = graphNameCtx;\n    const [hiddenNsPrefixMode, setHiddenNsPrefixMode ] = hiddenNsPrefixModeCtx;\n\n    const handleTemplateChange = (event: SelectChangeEvent) => {\n      setQuery(event.target.value as string);\n    };\n\n    const handleGraphChange = (event: SelectChangeEvent) => {\n      console.log(\"handleGraphChange\",event.target.value);\n      setGraphName(event.target.value);\n    };\n\n    const handleQueryChange = (event: React.ChangeEvent<HTMLTextAreaElement>) => {\n      setQuery(event.target.value);\n    };\n\n    const handleRuleChange = (event: React.ChangeEvent<HTMLTextAreaElement>) => {\n      setRule(event.target.value);\n    };\n\n    const handleAdvancedChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n      setAdvancedMode(event.target.checked);\n    };\n    const handleHiddenNsPrefixModeChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n      console.log(\"hiddenNsPrefixMode\",event.target.checked);\n      setHiddenNsPrefixMode(event.target.checked);\n      props.settingsUpdateHandler();\n    };\n\n    useEffect(() => {\n      fetch(neatApiRootUrl+`/api/list-queries`)\n       .then((response) => response.json())\n        .then((data) => setData(data));\n     }, []);\n\n    return (\n      <Box sx={{ minWidth: 400  }}>\n        <FormControlLabel sx={{marginBottom:2}}  control={<Switch value={advancedMode} onChange={handleAdvancedChange} />} label=\"Advanced mode\" />\n        <FormControlLabel sx={{marginBottom:2}}  control={<Switch value={hiddenNsPrefixMode} onChange={handleHiddenNsPrefixModeChange} defaultChecked />} label=\"Hidden NS Prefix mode\" />\n        <Box>\n        <FormControl sx={{width:500,marginBottom:2}} >\n          <InputLabel id=\"graphSelectorLabel\">Graph to query</InputLabel>\n            <Select\n              labelId=\"graphSelectorLabel\"\n              id=\"graphSelector\"\n              value={graphName}\n              label=\"Graph to query\"\n              size='small'\n              onChange={handleGraphChange}\n            >\n              <MenuItem value=\"source\" >Source graph </MenuItem>\n              <MenuItem value=\"solution\" >Solution graph </MenuItem>\n            </Select>\n        </FormControl>\n        </Box>\n        {advancedMode && (\n        <React.Fragment>\n        <FormControl sx={{width:\"80vw\"}}>\n          <InputLabel id=\"queryTemplateSelectorLabel\">Query template</InputLabel>\n          <Select\n            labelId=\"queryTemplateSelectorLabel\"\n            id=\"queryTemplateSelector\"\n            value={query}\n            size='small'\n            label=\"Query template\"\n            onChange={handleTemplateChange}\n          >\n          {\n            data && data.map((item,i) => (\n              <MenuItem value={item.query} key={i}>{item.name} </MenuItem>\n            ))\n          }\n          </Select>\n        </FormControl>\n        <div style={{margin:\"10px\"}}> </div>\n        <Box>\n        <TextareaAutosize  aria-label=\"SPARQL query\" minRows={2} value = {query} placeholder=\"SPARQL query\" style={{width:\"80vw\"}}  onChange={handleQueryChange} />\n        <Button sx={{ margin: \"5px\" }} variant=\"contained\" onClick={()=>{ props.selectedHandler(query,\"query\") }}> Run query </Button>\n        </Box>\n        <Box>\n         <TextField id=\"rule\" label=\"Rule\" value = {rule} size='small' sx={{width:\"80vw\"}} variant=\"outlined\" onChange={handleRuleChange}  />\n         <Button sx={{ margin: \"5px\" }} variant=\"contained\" onClick={()=>{ props.selectedHandler(rule,\"rule\") }}> Execute rule </Button>\n         </Box>\n        </React.Fragment>\n)}\n        <Box>\n\n        </Box>\n      </Box>\n    );\n  }\n\nexport function SearchBar(props:{searchButtonHandler:Function}) {\n    const [searchStr, setSearchStr] = useState('');\n    const [searchType,setSearchType] = useState(\"value_exact_match\");\n\n    const handleSearchTypeChange = (event: SelectChangeEvent) => {\n      setSearchType(event.target.value);\n    };\n    const handleSearchStrChange = (event: React.ChangeEvent<HTMLTextAreaElement>) => {\n      setSearchStr(event.target.value);\n    };\n\n\n    return (\n        <Box sx={{marginBottom:1,marginTop:1}}>\n         <TextField id=\"search\" label=\"Search\" value={searchStr} size='small' sx={{width:500}} variant=\"outlined\" onChange={handleSearchStrChange}  />\n         <FormControl sx={{width:180 , marginLeft:2}} >\n          <InputLabel id=\"graphSearchTypeLabel\">type</InputLabel>\n            <Select\n              labelId=\"graphSearcTypehLabel\"\n              id=\"graphSearchType\"\n              value={searchType}\n              label=\"type\"\n              size='small'\n              onChange={handleSearchTypeChange}\n            >\n              <MenuItem value=\"value_exact_match\" > Exact match </MenuItem>\n              <MenuItem value=\"value_regexp\" > Free search </MenuItem>\n              <MenuItem value=\"reference\" > Object reference </MenuItem>\n            </Select>\n        </FormControl>\n         <Button sx={{ marginLeft: 2 }} variant=\"contained\" onClick={()=>{props.searchButtonHandler(searchStr,searchType)}}> Search </Button>\n        </Box>\n    );\n  }\n\nconst ITEM_HEIGHT = 48;\nconst ITEM_PADDING_TOP = 8;\nconst MenuProps = {\n    PaperProps: {\n      style: {\n        maxHeight: ITEM_HEIGHT * 4.5 + ITEM_PADDING_TOP,\n        width: 250,\n      },\n    },\n};\n\nfunction getStyles(name: string, personName: readonly string[], theme: Theme) {\n  return {\n    fontWeight:\n      personName.indexOf(name) === -1\n        ? theme.typography.fontWeightRegular\n        : theme.typography.fontWeightMedium,\n  };\n}\n\nexport function FilterBar(props:{filterChangeHandler:Function}) {\n    const neatApiRootUrl = getNeatApiRootUrl();\n    const [filters, setFilters] = React.useState<string[]>([]);\n    const theme = useTheme();\n    const {hiddenNsPrefixModeCtx, graphNameCtx} = React.useContext(ExplorerContext);\n    const [graphName, setGraphName] = graphNameCtx;\n    const [hiddenNsPrefixMode, setHiddenNsPrefixMode ] = hiddenNsPrefixModeCtx;\n\n    const [filterOptions, setFilterOptions] = React.useState([]);\n    const [alertMsg, setAlertMsg] = useState(\"\");\n\n    useEffect(() => {\n      loadClassSummary();\n    }, [graphName]);\n\n    const handleChange = (event: SelectChangeEvent<typeof filters>) => {\n      const { target: { value }, } = event;\n      setFilters(\n        // On autofill we get a stringified value.\n        typeof value === 'string' ? value.split(',') : value,\n      );\n      props.filterChangeHandler(filters)\n    };\n\n    function sortArrayOfObjectsByName(arr) {\n      return\n    }\n\n    const loadClassSummary = () => {\n      const workflowName = getSelectedWorkflowName();\n      const url = neatApiRootUrl+\"/api/get-classes?\"+new URLSearchParams({\"graph_name\":graphName,\"cache\":\"false\",\"workflow_name\":workflowName}).toString();\n\n      fetch(url).then((response) => response.json()).then((data) => {\n        if (data.error) {\n          setAlertMsg(\"The workflow is missing or has uninitialized graph stores. Please ensure that you add a graph store and/or run the workflow before proceeding. Error msg: \"+data.error);\n          return;\n        }\n        let options = [];\n        data.rows.forEach((row) => {\n          let vClass = \"\";\n          if (hiddenNsPrefixMode) {\n            vClass = RemoveNsPrefix(row.class);\n          }else {\n            vClass = row.class;\n          }\n\n          // vClass = row.class;\n          setAlertMsg(\"\");\n          options.push({class:vClass,ns_class:row.class});\n        });\n        options = options.sort((a, b) => a.class.localeCompare(b.class));\n        setFilterOptions(options);\n      }).catch((error) => {\n        console.error('Error:', error);\n        setAlertMsg(\"The workflow is missing or has uninitialized graph stores. Please ensure that you add a graph store and/or run the workflow before proceeding. Error msg: \"+error);\n      }).finally(() => {\n       });\n    }\n\n    return (\n      <div>\n    {alertMsg != \"\" && (<Alert severity=\"warning\">\n          <AlertTitle>Warning</AlertTitle>\n          {alertMsg}\n    </Alert> )}\n      <FormControl sx={{ m: 0, width: \"94vw\" }}>\n        <InputLabel id=\"demo-multiple-chip-label\">Filter</InputLabel>\n        <Select\n          labelId=\"demo-multiple-chip-label\"\n          id=\"demo-multiple-chip\"\n          multiple\n          value={filters}\n          size='small'\n          onChange={handleChange}\n          input={<OutlinedInput id=\"select-multiple-chip\" label=\"Chip\" />}\n          renderValue={(selected) => (\n            <Box sx={{ display: 'flex', flexWrap: 'wrap', gap: 0.5 }}>\n              {selected.map((value) => (\n                <Chip key={value} label={value} />\n              ))}\n            </Box>\n          )}\n          MenuProps={MenuProps}\n        >\n          {filterOptions.map((item) => (\n            <MenuItem\n              key={item.ns_class}\n              value={item.ns_class}\n              style={getStyles(item.ns_class, filters, theme)}\n            >\n              {item.class}\n            </MenuItem>\n          ))}\n        </Select>\n      </FormControl>\n    </div>\n    );\n}\n\nfunction reshapeData(data) {\n    data.rows.map((item,i) => {\n      item[\"id\"] = i;\n    });\n    return;\n  }\n\nfunction a11yProps(index: number) {\n    return {\n      id: `simple-tab-${index}`,\n      'aria-controls': `simple-tabpanel-${index}`,\n    };\n}\n\n\nexport default function QDataTable() {\n  const neatApiRootUrl = getNeatApiRootUrl();\n  const [loading, setLoading] = React.useState(false);\n  const [data, setData] = useState({\"fields\": [], \"rows\": [] , \"query\": \"\" ,\"elapsed_time_sec\":0, \"error\": \"\"});\n  const [columns, setColumns] = useState([]);\n  const [openAlert, setOpenAlert] = React.useState(false);\n  const [alertMsg, setAlertMsg] = useState(\"\");\n\n  const [graphName, setGraphName] = React.useState(\"source\");\n  const [hiddenNsPrefixMode, setHiddenNsPrefixMode] = useState(true);\n\n  const [bhistory, setBhistory] = useState(Array<string>);\n  const [tabValue, setTabValue] = React.useState(0);\n  const [filters , setFilters] = React.useState(Array<string>);\n  const [sparqlQuery, setSparqlQuery] = React.useState(\"\");\n\n  // const {hiddenNsPrefixModeCtx, graphNameCtx} = React.useContext(ExplorerContext);\n  // const [graphName, setGraphName] = graphNameCtx;\n  // const [hiddenNsPrefixMode, setHiddenNsPrefixMode ] = hiddenNsPrefixModeCtx;\n  let nodeNameProperty = \"\"\n\n\n  const getColumnDefs = (fields:[string]) => {\n    const columns: GridColDef[] = [];\n    columns.push({field: 'id', headerName: 'ID', width: 70});\n    fields.map((field) => {\n      columns.push({field: field, headerName: field,renderCell: renderCellExpand , flex:0.5});\n    });\n    return columns;\n  }\n\n  const loadObjectAsGraph = (reference:string) => {\n    setTabValue(2);\n    nodeNameProperty = localStorage.getItem('nodeNameProperty')\n    let query = ``\n    if (!nodeNameProperty) {\n      query = `SELECT (?inst AS ?node_name) ?node_class (?inst AS ?node_id) WHERE {\n        BIND( <`+reference+`> AS ?inst)\n        ?inst rdf:type ?node_class .\n        } `\n    } else {\n      query = `SELECT ?node_name ?node_class (?inst AS ?node_id) WHERE {\n        BIND( <`+reference+`> AS ?inst)\n        ?inst `+nodeNameProperty+` ?node_name .\n        ?inst rdf:type ?node_class .\n        } `\n    }\n\n    setSparqlQuery(query);\n    // loadDataset(sparqlQuery,\"query\");\n  }\n\n  const loadObjectProperties = (reference:string) => {\n    const newHistory  = bhistory.slice();\n    let deleteFlag = false;\n    for (const [index, value] of newHistory.entries()) {\n      if (value == reference) {\n         deleteFlag = true;\n         bhistory.splice(index);\n         break;\n      }\n      console.log(\"somethiong here\");\n    }\n    bhistory.push(reference);\n    const workflowName = getSelectedWorkflowName();\n    fetch(neatApiRootUrl+`/api/object-properties?`+new URLSearchParams({\"reference\":reference,\"graph_name\":graphName,\"workflow_name\":workflowName}).toString())\n     .then((response) => response.json())\n      .then((rdata) => {\n        reshapeData(rdata);\n        const cm = getColumnDefs(rdata.fields)\n        setColumns(cm);\n        setData(rdata)\n        setLoading(false);\n        setOpenAlert(true);\n      }).catch((error) => {\n        console.error('Error:', error);\n        setData({\"fields\": [], \"rows\": [] , \"query\": \"\" ,\"elapsed_time_sec\":0, \"error\": error.message})\n        setLoading(false);\n        setOpenAlert(true);\n      });\n   }\n\n   const searchObjects = (searchStr:string,searchType:string) => {\n      setTabValue(1);\n      setLoading(true);\n      const workflowName = getSelectedWorkflowName();\n      fetch(neatApiRootUrl+`/api/search?`+new URLSearchParams({\"search_str\":searchStr,\"graph_name\":graphName,\"search_type\":searchType,\"workflow_name\":workflowName}).toString())\n      .then((response) => response.json())\n        .then((rdata) => {\n          reshapeData(rdata);\n          const cm = getColumnDefs(rdata.fields)\n          setColumns(cm);\n          setData(rdata)\n          setLoading(false);\n          setOpenAlert(true);\n        }).catch((error) => {\n          console.error('Error:', error);\n          setData({\"fields\": [], \"rows\": [] , \"query\": \"\" ,\"elapsed_time_sec\":0, \"error\": error.message})\n          setLoading(false);\n          setOpenAlert(true);\n        });\n   }\n\n   const handleFilterChange = (filters:string[]) => {\n    console.log(\"handleFilterChange\",filters);\n    setFilters(filters);\n   }\n  const renderCellExpand = (params) => {\n    console.log(hiddenNsPrefixMode);\n    if (params.value?.includes(\"#_\")) {\n      return <Box>{getShortenedString(params.value,10)} <Button onClick={(e)=> {loadObjectProperties(params.value)}}>Table </Button> <Button onClick={(e)=> {loadObjectAsGraph(params.value)}}>Graph </Button></Box>\n\n      } else if (params.value?.includes(\"#\") && hiddenNsPrefixMode) {\n      const value = RemoveNsPrefix(params.value);\n\n      return <Box sx={{ display: 'flex' }}> {value}</Box>\n    } else\n    return (\n       <Box sx={{ display: 'flex' }}> {params.value}</Box>\n    );\n  }\n\n  const settingsUpdateHandler = (settings:any) => {\n    console.log(\"settingsUpdateHandler\",settings);\n    if (settings) {\n      setGraphName(settings.graphName);\n      setHiddenNsPrefixMode(settings.hiddenNsPrefixMode);\n    }\n  }\n\n  const handleRunQueryCommand = (q:string,qtype:string) => {\n    setSparqlQuery(q);\n    if (tabValue == 0) {\n      // switching from Overview tab to Table tab\n      setTabValue(1);\n    }\n    if (tabValue != 2) {\n      // non-graph tab\n      loadDataset(q,qtype);\n    }\n\n  };\n\n  const loadDataset = (q:string,qtype:string) => {\n    let query = {}\n    let url = \"\"\n\n    console.log('reseting history');\n    setLoading(true);\n    const workflowName = getSelectedWorkflowName();\n    if (qtype == \"query\") {\n      query = {\"query\":q,\"graph_name\":graphName,\"workflow_name\":workflowName}\n      url = neatApiRootUrl+\"/api/query\"\n    } else if (qtype == \"rule\") {\n      query = {\"rule\":q,\"rule_type\":\"rdfpath\",\"graph_name\":graphName,\"workflow_name\":workflowName}\n      url = neatApiRootUrl+\"/api/execute-rule\"\n    }\n\n    fetch(url,{ method:\"post\",body:JSON.stringify(query),headers: {\n      'Content-Type': 'application/json;charset=utf-8'\n    }})\n    .then((response) => response.json()).then((rdata) => {\n      console.dir(rdata)\n      reshapeData(rdata);\n      const cm = getColumnDefs(rdata.fields)\n      setColumns(cm);\n      setData(rdata)\n      setLoading(false);\n      setOpenAlert(true);\n    }).catch((error) => {\n      console.error('Error:', error);\n      setData({\"fields\": [], \"rows\": [] , \"query\": \"\" ,\"elapsed_time_sec\":0, \"error\": error.message})\n      setLoading(false);\n      setOpenAlert(true);\n    });\n  }\n\n  const handleTabChange = (event: React.SyntheticEvent, newValue: number) => {\n    console.log(\"handleTabChange\",newValue);\n    setTabValue(newValue);\n  };\n\n  const activateTable= (className:string) => {\n    setTabValue(1);\n    let sparqlQuery = `SELECT ?instance ?property ?value  WHERE {\n      ?instance rdf:type <`+className+`> .\n      ?instance ?property ?value\n     } LIMIT 10000`\n    loadDataset(sparqlQuery,\"query\");\n  }\n\n  return (\n    <div>\n\n    <ExplorerContext.Provider value={{hiddenNsPrefixModeCtx:[hiddenNsPrefixMode, setHiddenNsPrefixMode],graphNameCtx:[graphName, setGraphName]}}>\n    {alertMsg != \"\" && (<Alert severity=\"warning\">\n          <AlertTitle>Warning</AlertTitle>\n            {alertMsg}\n    </Alert> )}\n    <QuerySelector selectedHandler={handleRunQueryCommand} settingsUpdateHandler={settingsUpdateHandler}/>\n    <SearchBar searchButtonHandler={searchObjects} />\n    <FilterBar filterChangeHandler={handleFilterChange}/>\n    { loading &&( <LinearProgress />) }\n    <Box sx={{ width: '100%' }}>\n      <Tabs value={tabValue} onChange={handleTabChange} aria-label=\"Explorer tabls\">\n        <Tab label=\"Overview\" {...a11yProps(0)} />\n        <Tab label=\"Table\" {...a11yProps(1)} />\n        <Tab label=\"Graph\" {...a11yProps(2)} />\n      </Tabs>\n      <TabPanel value={tabValue} index={0}>\n       <OverviewTable onItemClick={activateTable}/>\n      </TabPanel>\n      <TabPanel value={tabValue} index={1} >\n        <NavBreadcrumbs bhistory={bhistory} selectedHandler={loadObjectProperties}/>\n        <div style={{ height: '70vh', width: '100%' }}>\n          <DataGrid\n              rows={data.rows}\n              columns={columns}\n              pageSize={100}\n              rowsPerPageOptions={[5]}\n            />\n        </div>\n      </TabPanel>\n      <TabPanel value={tabValue} index={2}>\n        <GraphExplorer filters={filters} sparqlQuery={sparqlQuery}/>\n      </TabPanel>\n      <Collapse in={openAlert}>\n            <Alert\n              action={\n                <IconButton aria-label=\"close\" color=\"inherit\" size=\"small\" onClick={() => { setOpenAlert(false); }} >\n                  <CloseIcon fontSize=\"inherit\" />\n                </IconButton>\n              } sx={{ mb: 2 }}>\n              Elapsed time: {data.elapsed_time_sec*1000} ms. Number of rows: {data.rows.length} . <Box> SPARQL query : {data.query } </Box>\n              {data.error &&(<Box> Error: {data.error} </Box>) }\n            </Alert>\n        </Collapse>\n    </Box>\n\n    </ExplorerContext.Provider>\n    </div>\n  );\n}\n",
         "function _defineProperty(obj, key, value) {\n  if (key in obj) {\n    Object.defineProperty(obj, key, {\n      value: value,\n      enumerable: true,\n      configurable: true,\n      writable: true\n    });\n  } else {\n    obj[key] = value;\n  }\n\n  return obj;\n}\n\nfunction ownKeys(object, enumerableOnly) {\n  var keys = Object.keys(object);\n\n  if (Object.getOwnPropertySymbols) {\n    var symbols = Object.getOwnPropertySymbols(object);\n    if (enumerableOnly) symbols = symbols.filter(function (sym) {\n      return Object.getOwnPropertyDescriptor(object, sym).enumerable;\n    });\n    keys.push.apply(keys, symbols);\n  }\n\n  return keys;\n}\n\nfunction _objectSpread2(target) {\n  for (var i = 1; i < arguments.length; i++) {\n    var source = arguments[i] != null ? arguments[i] : {};\n\n    if (i % 2) {\n      ownKeys(Object(source), true).forEach(function (key) {\n        _defineProperty(target, key, source[key]);\n      });\n    } else if (Object.getOwnPropertyDescriptors) {\n      Object.defineProperties(target, Object.getOwnPropertyDescriptors(source));\n    } else {\n      ownKeys(Object(source)).forEach(function (key) {\n        Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key));\n      });\n    }\n  }\n\n  return target;\n}\n\nfunction _objectWithoutPropertiesLoose(source, excluded) {\n  if (source == null) return {};\n  var target = {};\n  var sourceKeys = Object.keys(source);\n  var key, i;\n\n  for (i = 0; i < sourceKeys.length; i++) {\n    key = sourceKeys[i];\n    if (excluded.indexOf(key) >= 0) continue;\n    target[key] = source[key];\n  }\n\n  return target;\n}\n\nfunction _objectWithoutProperties(source, excluded) {\n  if (source == null) return {};\n\n  var target = _objectWithoutPropertiesLoose(source, excluded);\n\n  var key, i;\n\n  if (Object.getOwnPropertySymbols) {\n    var sourceSymbolKeys = Object.getOwnPropertySymbols(source);\n\n    for (i = 0; i < sourceSymbolKeys.length; i++) {\n      key = sourceSymbolKeys[i];\n      if (excluded.indexOf(key) >= 0) continue;\n      if (!Object.prototype.propertyIsEnumerable.call(source, key)) continue;\n      target[key] = source[key];\n    }\n  }\n\n  return target;\n}\n\nfunction _slicedToArray(arr, i) {\n  return _arrayWithHoles(arr) || _iterableToArrayLimit(arr, i) || _unsupportedIterableToArray(arr, i) || _nonIterableRest();\n}\n\nfunction _arrayWithHoles(arr) {\n  if (Array.isArray(arr)) return arr;\n}\n\nfunction _iterableToArrayLimit(arr, i) {\n  if (typeof Symbol === \"undefined\" || !(Symbol.iterator in Object(arr))) return;\n  var _arr = [];\n  var _n = true;\n  var _d = false;\n  var _e = undefined;\n\n  try {\n    for (var _i = arr[Symbol.iterator](), _s; !(_n = (_s = _i.next()).done); _n = true) {\n      _arr.push(_s.value);\n\n      if (i && _arr.length === i) break;\n    }\n  } catch (err) {\n    _d = true;\n    _e = err;\n  } finally {\n    try {\n      if (!_n && _i[\"return\"] != null) _i[\"return\"]();\n    } finally {\n      if (_d) throw _e;\n    }\n  }\n\n  return _arr;\n}\n\nfunction _unsupportedIterableToArray(o, minLen) {\n  if (!o) return;\n  if (typeof o === \"string\") return _arrayLikeToArray(o, minLen);\n  var n = Object.prototype.toString.call(o).slice(8, -1);\n  if (n === \"Object\" && o.constructor) n = o.constructor.name;\n  if (n === \"Map\" || n === \"Set\") return Array.from(o);\n  if (n === \"Arguments\" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return _arrayLikeToArray(o, minLen);\n}\n\nfunction _arrayLikeToArray(arr, len) {\n  if (len == null || len > arr.length) len = arr.length;\n\n  for (var i = 0, arr2 = new Array(len); i < len; i++) arr2[i] = arr[i];\n\n  return arr2;\n}\n\nfunction _nonIterableRest() {\n  throw new TypeError(\"Invalid attempt to destructure non-iterable instance.\\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.\");\n}\n\nexport { _arrayLikeToArray as arrayLikeToArray, _arrayWithHoles as arrayWithHoles, _defineProperty as defineProperty, _iterableToArrayLimit as iterableToArrayLimit, _nonIterableRest as nonIterableRest, _objectSpread2 as objectSpread2, _objectWithoutProperties as objectWithoutProperties, _objectWithoutPropertiesLoose as objectWithoutPropertiesLoose, _slicedToArray as slicedToArray, _unsupportedIterableToArray as unsupportedIterableToArray };\n",
         "function _defineProperty(obj, key, value) {\n  if (key in obj) {\n    Object.defineProperty(obj, key, {\n      value: value,\n      enumerable: true,\n      configurable: true,\n      writable: true\n    });\n  } else {\n    obj[key] = value;\n  }\n\n  return obj;\n}\n\nfunction ownKeys(object, enumerableOnly) {\n  var keys = Object.keys(object);\n\n  if (Object.getOwnPropertySymbols) {\n    var symbols = Object.getOwnPropertySymbols(object);\n    if (enumerableOnly) symbols = symbols.filter(function (sym) {\n      return Object.getOwnPropertyDescriptor(object, sym).enumerable;\n    });\n    keys.push.apply(keys, symbols);\n  }\n\n  return keys;\n}\n\nfunction _objectSpread2(target) {\n  for (var i = 1; i < arguments.length; i++) {\n    var source = arguments[i] != null ? arguments[i] : {};\n\n    if (i % 2) {\n      ownKeys(Object(source), true).forEach(function (key) {\n        _defineProperty(target, key, source[key]);\n      });\n    } else if (Object.getOwnPropertyDescriptors) {\n      Object.defineProperties(target, Object.getOwnPropertyDescriptors(source));\n    } else {\n      ownKeys(Object(source)).forEach(function (key) {\n        Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key));\n      });\n    }\n  }\n\n  return target;\n}\n\nfunction compose() {\n  for (var _len = arguments.length, fns = new Array(_len), _key = 0; _key < _len; _key++) {\n    fns[_key] = arguments[_key];\n  }\n\n  return function (x) {\n    return fns.reduceRight(function (y, f) {\n      return f(y);\n    }, x);\n  };\n}\n\nfunction curry(fn) {\n  return function curried() {\n    var _this = this;\n\n    for (var _len2 = arguments.length, args = new Array(_len2), _key2 = 0; _key2 < _len2; _key2++) {\n      args[_key2] = arguments[_key2];\n    }\n\n    return args.length >= fn.length ? fn.apply(this, args) : function () {\n      for (var _len3 = arguments.length, nextArgs = new Array(_len3), _key3 = 0; _key3 < _len3; _key3++) {\n        nextArgs[_key3] = arguments[_key3];\n      }\n\n      return curried.apply(_this, [].concat(args, nextArgs));\n    };\n  };\n}\n\nfunction isObject(value) {\n  return {}.toString.call(value).includes('Object');\n}\n\nfunction isEmpty(obj) {\n  return !Object.keys(obj).length;\n}\n\nfunction isFunction(value) {\n  return typeof value === 'function';\n}\n\nfunction hasOwnProperty(object, property) {\n  return Object.prototype.hasOwnProperty.call(object, property);\n}\n\nfunction validateChanges(initial, changes) {\n  if (!isObject(changes)) errorHandler('changeType');\n  if (Object.keys(changes).some(function (field) {\n    return !hasOwnProperty(initial, field);\n  })) errorHandler('changeField');\n  return changes;\n}\n\nfunction validateSelector(selector) {\n  if (!isFunction(selector)) errorHandler('selectorType');\n}\n\nfunction validateHandler(handler) {\n  if (!(isFunction(handler) || isObject(handler))) errorHandler('handlerType');\n  if (isObject(handler) && Object.values(handler).some(function (_handler) {\n    return !isFunction(_handler);\n  })) errorHandler('handlersType');\n}\n\nfunction validateInitial(initial) {\n  if (!initial) errorHandler('initialIsRequired');\n  if (!isObject(initial)) errorHandler('initialType');\n  if (isEmpty(initial)) errorHandler('initialContent');\n}\n\nfunction throwError(errorMessages, type) {\n  throw new Error(errorMessages[type] || errorMessages[\"default\"]);\n}\n\nvar errorMessages = {\n  initialIsRequired: 'initial state is required',\n  initialType: 'initial state should be an object',\n  initialContent: 'initial state shouldn\\'t be an empty object',\n  handlerType: 'handler should be an object or a function',\n  handlersType: 'all handlers should be a functions',\n  selectorType: 'selector should be a function',\n  changeType: 'provided value of changes should be an object',\n  changeField: 'it seams you want to change a field in the state which is not specified in the \"initial\" state',\n  \"default\": 'an unknown error accured in `state-local` package'\n};\nvar errorHandler = curry(throwError)(errorMessages);\nvar validators = {\n  changes: validateChanges,\n  selector: validateSelector,\n  handler: validateHandler,\n  initial: validateInitial\n};\n\nfunction create(initial) {\n  var handler = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};\n  validators.initial(initial);\n  validators.handler(handler);\n  var state = {\n    current: initial\n  };\n  var didUpdate = curry(didStateUpdate)(state, handler);\n  var update = curry(updateState)(state);\n  var validate = curry(validators.changes)(initial);\n  var getChanges = curry(extractChanges)(state);\n\n  function getState() {\n    var selector = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : function (state) {\n      return state;\n    };\n    validators.selector(selector);\n    return selector(state.current);\n  }\n\n  function setState(causedChanges) {\n    compose(didUpdate, update, validate, getChanges)(causedChanges);\n  }\n\n  return [getState, setState];\n}\n\nfunction extractChanges(state, causedChanges) {\n  return isFunction(causedChanges) ? causedChanges(state.current) : causedChanges;\n}\n\nfunction updateState(state, changes) {\n  state.current = _objectSpread2(_objectSpread2({}, state.current), changes);\n  return changes;\n}\n\nfunction didStateUpdate(state, handler, changes) {\n  isFunction(handler) ? handler(state.current) : Object.keys(changes).forEach(function (field) {\n    var _handler$field;\n\n    return (_handler$field = handler[field]) === null || _handler$field === void 0 ? void 0 : _handler$field.call(handler, state.current[field]);\n  });\n  return changes;\n}\n\nvar index = {\n  create: create\n};\n\nexport default index;\n",
         "var config = {\n  paths: {\n    vs: 'https://cdn.jsdelivr.net/npm/monaco-editor@0.36.1/min/vs'\n  }\n};\n\nexport default config;\n",
         "function curry(fn) {\n  return function curried() {\n    var _this = this;\n\n    for (var _len = arguments.length, args = new Array(_len), _key = 0; _key < _len; _key++) {\n      args[_key] = arguments[_key];\n    }\n\n    return args.length >= fn.length ? fn.apply(this, args) : function () {\n      for (var _len2 = arguments.length, nextArgs = new Array(_len2), _key2 = 0; _key2 < _len2; _key2++) {\n        nextArgs[_key2] = arguments[_key2];\n      }\n\n      return curried.apply(_this, [].concat(args, nextArgs));\n    };\n  };\n}\n\nexport default curry;\n",
         "function isObject(value) {\n  return {}.toString.call(value).includes('Object');\n}\n\nexport default isObject;\n",
         "import curry from '../utils/curry.js';\nimport isObject from '../utils/isObject.js';\n\n/**\n * validates the configuration object and informs about deprecation\n * @param {Object} config - the configuration object \n * @return {Object} config - the validated configuration object\n */\n\nfunction validateConfig(config) {\n  if (!config) errorHandler('configIsRequired');\n  if (!isObject(config)) errorHandler('configType');\n\n  if (config.urls) {\n    informAboutDeprecation();\n    return {\n      paths: {\n        vs: config.urls.monacoBase\n      }\n    };\n  }\n\n  return config;\n}\n/**\n * logs deprecation message\n */\n\n\nfunction informAboutDeprecation() {\n  console.warn(errorMessages.deprecation);\n}\n\nfunction throwError(errorMessages, type) {\n  throw new Error(errorMessages[type] || errorMessages[\"default\"]);\n}\n\nvar errorMessages = {\n  configIsRequired: 'the configuration object is required',\n  configType: 'the configuration object should be an object',\n  \"default\": 'an unknown error accured in `@monaco-editor/loader` package',\n  deprecation: \"Deprecation warning!\\n    You are using deprecated way of configuration.\\n\\n    Instead of using\\n      monaco.config({ urls: { monacoBase: '...' } })\\n    use\\n      monaco.config({ paths: { vs: '...' } })\\n\\n    For more please check the link https://github.com/suren-atoyan/monaco-loader#config\\n  \"\n};\nvar errorHandler = curry(throwError)(errorMessages);\nvar validators = {\n  config: validateConfig\n};\n\nexport default validators;\nexport { errorHandler, errorMessages };\n",
         "var compose = function compose() {\n  for (var _len = arguments.length, fns = new Array(_len), _key = 0; _key < _len; _key++) {\n    fns[_key] = arguments[_key];\n  }\n\n  return function (x) {\n    return fns.reduceRight(function (y, f) {\n      return f(y);\n    }, x);\n  };\n};\n\nexport default compose;\n",
@@ -12656,15 +12656,15 @@
         "import React, { useState, useRef, useCallback, useEffect } from 'react';\nimport loader from '@monaco-editor/loader';\n\nimport MonacoContainer from '../MonacoContainer';\nimport useMount from '../hooks/useMount';\nimport useUpdate from '../hooks/useUpdate';\nimport { noop, getOrCreateModel } from '../utils';\nimport { type DiffEditorProps, type MonacoDiffEditor } from './types';\nimport { type Monaco } from '..';\n\nfunction DiffEditor({\n  original,\n  modified,\n  language,\n  originalLanguage,\n  modifiedLanguage,\n  originalModelPath,\n  modifiedModelPath,\n  keepCurrentOriginalModel = false,\n  keepCurrentModifiedModel = false,\n  theme = 'light',\n  loading = 'Loading...',\n  options = {},\n  height = '100%',\n  width = '100%',\n  className,\n  wrapperProps = {},\n  beforeMount = noop,\n  onMount = noop,\n}: DiffEditorProps) {\n  const [isEditorReady, setIsEditorReady] = useState(false);\n  const [isMonacoMounting, setIsMonacoMounting] = useState(true);\n  const editorRef = useRef<MonacoDiffEditor | null>(null);\n  const monacoRef = useRef<Monaco | null>(null);\n  const containerRef = useRef<HTMLDivElement>(null);\n  const onMountRef = useRef(onMount);\n  const beforeMountRef = useRef(beforeMount);\n  const preventCreation = useRef(false);\n\n  useMount(() => {\n    const cancelable = loader.init();\n\n    cancelable\n      .then((monaco) => (monacoRef.current = monaco) && setIsMonacoMounting(false))\n      .catch(\n        (error) =>\n          error?.type !== 'cancelation' && console.error('Monaco initialization: error:', error),\n      );\n\n    return () => (editorRef.current ? disposeEditor() : cancelable.cancel());\n  });\n\n  useUpdate(\n    () => {\n      const modifiedEditor = editorRef.current!.getModifiedEditor();\n      if (modifiedEditor.getOption(monacoRef.current!.editor.EditorOption.readOnly)) {\n        modifiedEditor.setValue(modified || '');\n      } else {\n        if (modified !== modifiedEditor.getValue()) {\n          modifiedEditor.executeEdits('', [\n            {\n              range: modifiedEditor.getModel()!.getFullModelRange(),\n              text: modified || '',\n              forceMoveMarkers: true,\n            },\n          ]);\n\n          modifiedEditor.pushUndoStop();\n        }\n      }\n    },\n    [modified],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      editorRef.current?.getModel()?.original.setValue(original || '');\n    },\n    [original],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      const { original, modified } = editorRef.current!.getModel()!;\n\n      monacoRef.current!.editor.setModelLanguage(original, originalLanguage || language || 'text');\n      monacoRef.current!.editor.setModelLanguage(modified, modifiedLanguage || language || 'text');\n    },\n    [language, originalLanguage, modifiedLanguage],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      monacoRef.current?.editor.setTheme(theme);\n    },\n    [theme],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      editorRef.current?.updateOptions(options);\n    },\n    [options],\n    isEditorReady,\n  );\n\n  const setModels = useCallback(() => {\n    if (!monacoRef.current) return;\n    beforeMountRef.current(monacoRef.current);\n    const originalModel = getOrCreateModel(\n      monacoRef.current,\n      original || '',\n      originalLanguage || language || 'text',\n      originalModelPath || '',\n    );\n\n    const modifiedModel = getOrCreateModel(\n      monacoRef.current,\n      modified || '',\n      modifiedLanguage || language || 'text',\n      modifiedModelPath || '',\n    );\n\n    editorRef.current?.setModel({\n      original: originalModel,\n      modified: modifiedModel,\n    });\n  }, [\n    language,\n    modified,\n    modifiedLanguage,\n    original,\n    originalLanguage,\n    originalModelPath,\n    modifiedModelPath,\n  ]);\n\n  const createEditor = useCallback(() => {\n    if (!preventCreation.current && containerRef.current) {\n      editorRef.current = monacoRef.current!.editor.createDiffEditor(containerRef.current, {\n        automaticLayout: true,\n        ...options,\n      });\n\n      setModels();\n\n      monacoRef.current?.editor.setTheme(theme);\n\n      setIsEditorReady(true);\n      preventCreation.current = true;\n    }\n  }, [options, theme, setModels]);\n\n  useEffect(() => {\n    if (isEditorReady) {\n      onMountRef.current(editorRef.current!, monacoRef.current!);\n    }\n  }, [isEditorReady]);\n\n  useEffect(() => {\n    !isMonacoMounting && !isEditorReady && createEditor();\n  }, [isMonacoMounting, isEditorReady, createEditor]);\n\n  useUpdate(\n    () => {\n      if (editorRef.current && monacoRef.current) {\n        const originalEditor = editorRef.current.getOriginalEditor();\n        const model = getOrCreateModel(\n          monacoRef.current,\n          original || '',\n          originalLanguage || language || 'text',\n          originalModelPath || '',\n        );\n\n        if (model !== originalEditor.getModel()) {\n          originalEditor.setModel(model);\n        }\n      }\n    },\n    [originalModelPath],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      if (editorRef.current && monacoRef.current) {\n        const modifiedEditor = editorRef.current.getModifiedEditor();\n        const model = getOrCreateModel(\n          monacoRef.current,\n          modified || '',\n          modifiedLanguage || language || 'text',\n          modifiedModelPath || '',\n        );\n\n        if (model !== modifiedEditor.getModel()) {\n          modifiedEditor.setModel(model);\n        }\n      }\n    },\n    [modifiedModelPath],\n    isEditorReady,\n  );\n\n  function disposeEditor() {\n    const models = editorRef.current?.getModel();\n\n    if (!keepCurrentOriginalModel) {\n      models?.original?.dispose();\n    }\n\n    if (!keepCurrentModifiedModel) {\n      models?.modified?.dispose();\n    }\n\n    editorRef.current?.dispose();\n  }\n\n  return (\n    <MonacoContainer\n      width={width}\n      height={height}\n      isEditorReady={isEditorReady}\n      loading={loading}\n      _ref={containerRef}\n      className={className}\n      wrapperProps={wrapperProps}\n    />\n  );\n}\n\nexport default DiffEditor;\n",
         "import { memo } from 'react';\n\nimport DiffEditor from './DiffEditor';\n\nexport * from './types';\n\nexport default memo(DiffEditor);\n",
         "import { useEffect, useRef } from 'react';\n\nfunction usePrevious<T>(value: T) {\n  const ref = useRef<T>();\n\n  useEffect(() => {\n    ref.current = value;\n  }, [value]);\n\n  return ref.current;\n}\n\nexport default usePrevious;\n",
         "import React, { useState, useEffect, useRef, useCallback } from 'react';\nimport loader from '@monaco-editor/loader';\nimport useMount from '../hooks/useMount';\nimport useUpdate from '../hooks/useUpdate';\nimport usePrevious from '../hooks/usePrevious';\nimport { type IDisposable, type editor } from 'monaco-editor';\nimport { noop, getOrCreateModel } from '../utils';\nimport { type EditorProps } from './types';\nimport { type Monaco } from '..';\nimport MonacoContainer from '../MonacoContainer';\n\nconst viewStates = new Map();\n\nfunction Editor({\n  defaultValue,\n  defaultLanguage,\n  defaultPath,\n  value,\n  language,\n  path,\n  /* === */\n  theme = 'light',\n  line,\n  loading = 'Loading...',\n  options = {},\n  overrideServices = {},\n  saveViewState = true,\n  keepCurrentModel = false,\n  /* === */\n  width = '100%',\n  height = '100%',\n  className,\n  wrapperProps = {},\n  /* === */\n  beforeMount = noop,\n  onMount = noop,\n  onChange,\n  onValidate = noop,\n}: EditorProps) {\n  const [isEditorReady, setIsEditorReady] = useState(false);\n  const [isMonacoMounting, setIsMonacoMounting] = useState(true);\n  const monacoRef = useRef<Monaco | null>(null);\n  const editorRef = useRef<editor.IStandaloneCodeEditor | null>(null);\n  const containerRef = useRef<HTMLDivElement>(null);\n  const onMountRef = useRef(onMount);\n  const beforeMountRef = useRef(beforeMount);\n  const subscriptionRef = useRef<IDisposable>();\n  const valueRef = useRef(value);\n  const previousPath = usePrevious(path);\n  const preventCreation = useRef(false);\n  const preventTriggerChangeEvent = useRef<boolean>(false);\n\n  useMount(() => {\n    const cancelable = loader.init();\n\n    cancelable\n      .then((monaco) => (monacoRef.current = monaco) && setIsMonacoMounting(false))\n      .catch(\n        (error) =>\n          error?.type !== 'cancelation' && console.error('Monaco initialization: error:', error),\n      );\n\n    return () => (editorRef.current ? disposeEditor() : cancelable.cancel());\n  });\n\n  useUpdate(\n    () => {\n      const model = getOrCreateModel(\n        monacoRef.current!,\n        defaultValue || value || '',\n        defaultLanguage || language || '',\n        path || defaultPath || '',\n      );\n\n      if (model !== editorRef.current?.getModel()) {\n        if (saveViewState) viewStates.set(previousPath, editorRef.current?.saveViewState());\n        editorRef.current?.setModel(model);\n        if (saveViewState) editorRef.current?.restoreViewState(viewStates.get(path));\n      }\n    },\n    [path],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      editorRef.current?.updateOptions(options);\n    },\n    [options],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      if (!editorRef.current || value === undefined) return;\n      if (editorRef.current.getOption(monacoRef.current!.editor.EditorOption.readOnly)) {\n        editorRef.current.setValue(value);\n      } else if (value !== editorRef.current.getValue()) {\n        preventTriggerChangeEvent.current = true;\n        editorRef.current.executeEdits('', [\n          {\n            range: editorRef.current.getModel()!.getFullModelRange(),\n            text: value,\n            forceMoveMarkers: true,\n          },\n        ]);\n\n        editorRef.current.pushUndoStop();\n        preventTriggerChangeEvent.current = false;\n      }\n    },\n    [value],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      const model = editorRef.current?.getModel();\n      if (model && language) monacoRef.current?.editor.setModelLanguage(model, language);\n    },\n    [language],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      // reason for undefined check: https://github.com/suren-atoyan/monaco-react/pull/188\n      if (line !== undefined) {\n        editorRef.current?.revealLine(line);\n      }\n    },\n    [line],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      monacoRef.current?.editor.setTheme(theme);\n    },\n    [theme],\n    isEditorReady,\n  );\n\n  const createEditor = useCallback(() => {\n    if (!containerRef.current || !monacoRef.current) return;\n    if (!preventCreation.current) {\n      beforeMountRef.current(monacoRef.current);\n      const autoCreatedModelPath = path || defaultPath;\n\n      const defaultModel = getOrCreateModel(\n        monacoRef.current,\n        value || defaultValue || '',\n        defaultLanguage || language || '',\n        autoCreatedModelPath || '',\n      );\n\n      editorRef.current = monacoRef.current?.editor.create(\n        containerRef.current,\n        {\n          model: defaultModel,\n          automaticLayout: true,\n          ...options,\n        },\n        overrideServices,\n      );\n\n      saveViewState && editorRef.current.restoreViewState(viewStates.get(autoCreatedModelPath));\n\n      monacoRef.current.editor.setTheme(theme);\n\n      setIsEditorReady(true);\n      preventCreation.current = true;\n    }\n  }, [\n    defaultValue,\n    defaultLanguage,\n    defaultPath,\n    value,\n    language,\n    path,\n    options,\n    overrideServices,\n    saveViewState,\n    theme,\n  ]);\n\n  useEffect(() => {\n    if (isEditorReady) {\n      onMountRef.current(editorRef.current!, monacoRef.current!);\n    }\n  }, [isEditorReady]);\n\n  useEffect(() => {\n    !isMonacoMounting && !isEditorReady && createEditor();\n  }, [isMonacoMounting, isEditorReady, createEditor]);\n\n  // subscription\n  // to avoid unnecessary updates (attach - dispose listener) in subscription\n  valueRef.current = value;\n\n  // onChange\n  useEffect(() => {\n    if (isEditorReady && onChange) {\n      subscriptionRef.current?.dispose();\n      subscriptionRef.current = editorRef.current?.onDidChangeModelContent((event) => {\n        if (!preventTriggerChangeEvent.current) {\n          onChange(editorRef.current!.getValue(), event);\n        }\n      });\n    }\n  }, [isEditorReady, onChange]);\n\n  // onValidate\n  useEffect(() => {\n    if (isEditorReady) {\n      const changeMarkersListener = monacoRef.current!.editor.onDidChangeMarkers((uris) => {\n        const editorUri = editorRef.current!.getModel()?.uri;\n\n        if (editorUri) {\n          const currentEditorHasMarkerChanges = uris.find((uri) => uri.path === editorUri.path);\n          if (currentEditorHasMarkerChanges) {\n            const markers = monacoRef.current!.editor.getModelMarkers({\n              resource: editorUri,\n            });\n            onValidate?.(markers);\n          }\n        }\n      });\n\n      return () => {\n        changeMarkersListener?.dispose();\n      };\n    }\n    return () => {\n      // eslint happy\n    };\n  }, [isEditorReady, onValidate]);\n\n  function disposeEditor() {\n    subscriptionRef.current?.dispose();\n\n    if (keepCurrentModel) {\n      saveViewState && viewStates.set(path, editorRef.current!.saveViewState());\n    } else {\n      editorRef.current!.getModel()?.dispose();\n    }\n\n    editorRef.current!.dispose();\n  }\n\n  return (\n    <MonacoContainer\n      width={width}\n      height={height}\n      isEditorReady={isEditorReady}\n      loading={loading}\n      _ref={containerRef}\n      className={className}\n      wrapperProps={wrapperProps}\n    />\n  );\n}\n\nexport default Editor;\n",
         "import loader from '@monaco-editor/loader';\nexport { loader };\n\nimport DiffEditor from './DiffEditor';\nexport * from './DiffEditor/types';\nexport { DiffEditor };\n\nimport useMonaco from './hooks/useMonaco';\nexport { useMonaco };\n\nimport Editor from './Editor';\nexport * from './Editor/types';\nexport { Editor };\nexport default Editor;\n\n// Monaco\nimport type * as monaco from 'monaco-editor/esm/vs/editor/editor.api';\nexport type Monaco = typeof monaco;\n\n// Default themes\nexport type Theme = 'vs-dark' | 'light';\n",
         "import { memo } from 'react';\n\nimport Editor from './Editor';\n\nexport * from './types';\n\nexport default memo(Editor);\n",
         "import Button from \"@mui/material/Button\"\nimport Dialog from \"@mui/material/Dialog\"\nimport DialogActions from \"@mui/material/DialogActions\"\nimport DialogContent from \"@mui/material/DialogContent\"\nimport DialogTitle from \"@mui/material/DialogTitle\"\nimport FormControl from \"@mui/material/FormControl\"\nimport TextField from \"@mui/material/TextField\"\nimport { useEffect, useState } from \"react\"\nimport { WorkflowSystemComponent } from \"types/WorkflowTypes\"\n\nexport default function OverviewComponentEditorDialog(props: any)\n{\n    const [dialogOpen, setDialogOpen] = useState(false);\n    const [component, setComponent] = useState<WorkflowSystemComponent>(null);\n    const handleDialogSave = () => {\n        setDialogOpen(false);\n        props.onClose(component,\"save\");\n    };\n    const handleDialogCancel = () => {\n        setDialogOpen(false);\n        props.onClose(component,\"cancel\");\n    };\n    const handleDelete = () => {\n        setDialogOpen(false);\n        props.onClose(component,\"delete\");\n    };\n    const handleStepConfigChange = (name: string, value: any) => {\n        console.log('handleComponentConfigChange')\n        console.dir(component);\n        let updComponent = Object.assign({},component);\n        updComponent[name] = value;\n        console.log(\"Updateed component\")\n        console.dir(updComponent);\n        setComponent(updComponent);\n    }\n    useEffect(() => {\n        if (props.open){\n            setDialogOpen(true);\n            setComponent(props.component);\n            console.dir(props.component);\n        }\n      }, [props.open]);\n\n\n\nreturn (\n<Dialog open={dialogOpen} onClose={handleDialogCancel}>\n<DialogTitle>Component editor</DialogTitle>\n<DialogContent>\n  <FormControl sx={{ width: 300 }} >\n    <TextField sx={{ marginTop: 1 }} id=\"step-config-id\" fullWidth label=\"Component id\" size='small' variant=\"outlined\" value={component?.id} onChange={(event) => { handleStepConfigChange(\"id\", event.target.value) }} />\n    <TextField sx={{ marginTop: 1 }} id=\"step-config-label\" fullWidth label=\"Label\" size='small' variant=\"outlined\" value={component?.label} onChange={(event) => { handleStepConfigChange(\"label\", event.target.value) }} />\n    <TextField sx={{ marginTop: 1 }} id=\"step-config-descr\" fullWidth label=\"Description\" size='small' variant=\"outlined\" value={component?.description} onChange={(event) => { handleStepConfigChange(\"description\", event.target.value) }} />\n  </FormControl>\n</DialogContent>\n<DialogActions>\n  <Button variant=\"outlined\" size=\"small\" onClick={handleDialogSave}>Save</Button>\n  <Button variant=\"outlined\" size=\"small\" onClick={handleDialogCancel}>Cancel</Button>\n  <Button variant=\"outlined\" size=\"small\" color=\"error\" onClick={handleDelete}>Delete</Button>\n</DialogActions>\n</Dialog>\n)\n}\n",
-        "import Button from \"@mui/material/Button\"\nimport Checkbox from \"@mui/material/Checkbox\"\nimport { red } from \"@mui/material/colors\"\nimport Dialog from \"@mui/material/Dialog\"\nimport DialogActions from \"@mui/material/DialogActions\"\nimport DialogContent from \"@mui/material/DialogContent\"\nimport DialogTitle from \"@mui/material/DialogTitle\"\nimport FormControl from \"@mui/material/FormControl\"\nimport FormControlLabel from \"@mui/material/FormControlLabel\"\nimport MenuItem from \"@mui/material/MenuItem\"\nimport Select from \"@mui/material/Select\"\nimport TextField from \"@mui/material/TextField\"\nimport React, { useEffect, useState } from \"react\"\nimport { WorkflowStepDefinition, WorkflowSystemComponent } from \"types/WorkflowTypes\"\nimport { getNeatApiRootUrl } from \"./Utils\"\nimport LocalUploader from \"./LocalUploader\"\nimport { InputLabel, Typography } from \"@mui/material\"\n\nexport default function StepEditorDialog(props: any)\n{\n    const [dialogOpen, setDialogOpen] = useState(false);\n    const [selectedStep, setSelectedStep] = useState<WorkflowStepDefinition>();\n    const neatApiRootUrl = getNeatApiRootUrl();\n    const [runPayload,setRunPayload] = useState<string>(JSON.stringify({\"action\":\"approve\"}))\n    const [statusText,setStatusText] = useState<string>(\"\")\n\n    const handleDialogSave = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"save\");\n    };\n    const handleDialogCancel = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"cancel\");\n    };\n    const handleDelete = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"delete\");\n    };\n\n    const handleRunCommand = () => {\n        setDialogOpen(false);\n        // send POST request to run the step\n        fetch(neatApiRootUrl +'/api/workflow/'+props.workflowName+'/http_trigger/'+selectedStep.id, { method: 'POST', body: runPayload })\n        .then(response => response.json())\n        .then(data => {\n            console.log('Success:', data);\n        }).catch((error) => {\n            console.error('Error:', error);\n        })\n        props.onClose(selectedStep,\"run\");\n    };\n\n    const handleResumeCommand = () => {\n      setDialogOpen(false);\n      // send POST request to run the step\n      fetch(neatApiRootUrl +'/api/workflow/'+props.workflowName+'/resume/'+selectedStep.id+'/default', { method: 'POST', body: runPayload })\n      .then(response => response.json())\n      .then(data => {\n          console.log('Success:', data);\n      }).catch((error) => {\n          console.error('Error:', error);\n      })\n      props.onClose(selectedStep,\"run\");\n  };\n\n    const onUpload = (fileName:string , hash: string) => {\n      console.log(\"onUpload\",fileName,hash)\n      setStatusText(\"File uplloaded \"+fileName)\n    }\n\n    useEffect(() => {\n        if (props.open){\n            setDialogOpen(true);\n            setSelectedStep(props.step);\n            console.dir(props.step);\n        }\n      }, [props.open]);\n\n      const handleStepConfigChange = (name: string, value: any) => {\n        console.log('handleStepConfigChange')\n        console.dir(selectedStep);\n        let updStep= Object.assign({},selectedStep);\n\n        if (selectedStep) {\n          if (!selectedStep.params) {\n            selectedStep.params = {}\n          }\n          if (name == \"stype\") {\n            switch (value) {\n              case \"time_trigger\":\n                updStep.params = { \"interval\": \"every 60 minutes\" }\n                break;\n              case \"start_workflow_task_step\":\n                updStep.params = { \"workflow_name\": \"\", \"sync\": \"false\" }\n                break;\n            }\n            updStep[\"stype\"] = value;\n          } else {\n            switch (name) {\n              case \"time-interval\":\n                updStep.params[\"interval\"] = value;\n                break;\n              case \"workflow_name\":\n                updStep.params[\"workflow_name\"] = value;\n                break;\n              case \"workflow_sync_run_flag\":\n                value = \"false\"\n                if (value) {\n                  value = \"true\"\n                }\n                updStep.params[\"sync\"] = value;\n                break;\n              case \"workflow_start_method\":\n                updStep.params[\"workflow_start_method\"] = value;\n                break;\n              case \"max_wait_time\":\n                updStep.params[\"max_wait_time\"] = value;\n                break;\n              default:\n                updStep[name] = value;\n            }\n          }\n          console.log(\"rendering view\")\n        }\n        setSelectedStep(updStep);\n      }\n\n\nreturn (\n  <Dialog open={dialogOpen} onClose={handleDialogCancel}>\n        <DialogTitle>Step configurator</DialogTitle>\n        <DialogContent >\n          <FormControl  fullWidth>\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-id\" fullWidth label=\"Step id\" size='small' variant=\"outlined\" value={selectedStep?.id} onChange={(event) => { handleStepConfigChange(\"id\", event.target.value) }} />\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-label\" fullWidth label=\"Label\" size='small' variant=\"outlined\" value={selectedStep?.label} onChange={(event) => { handleStepConfigChange(\"label\", event.target.value) }} />\n          </FormControl>\n          <FormControl sx={{ marginTop: 2 }} fullWidth >\n            <InputLabel id=\"step_type_label\">Step type</InputLabel>\n            <Select sx={{ marginTop: 1 }}\n              id=\"step-config-stype\"\n              labelId=\"step_type_label\"\n              value={selectedStep?.stype}\n              label=\"Step type\"\n              size='small'\n              variant=\"outlined\"\n              onChange={(event) => { handleStepConfigChange(\"stype\", event.target.value) }}\n            >\n              <MenuItem value=\"pystep\">Python function</MenuItem>\n              <MenuItem value=\"http_trigger\">HTTP trigger</MenuItem>\n              <MenuItem value=\"time_trigger\">Time trigger</MenuItem>\n              <MenuItem value=\"wait_for_event\">Wait for event</MenuItem>\n              <MenuItem value=\"start_workflow_task_step\">Start workflow</MenuItem>\n              <MenuItem value=\"file_uploader\">File uploader</MenuItem>\n            </Select>\n          </FormControl>\n          <FormControl sx={{ marginTop: 1 }} fullWidth >\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-descr\" fullWidth label=\"Description\" size='small' variant=\"outlined\" value={selectedStep?.description} onChange={(event) => { handleStepConfigChange(\"description\", event.target.value) }} />\n            {(selectedStep?.stype == \"time_trigger\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-config-time-config\" fullWidth label=\"Time interval\" size='small' variant=\"outlined\" value={selectedStep?.params[\"interval\"]} onChange={(event) => { handleStepConfigChange(\"time-interval\", event.target.value) }} />\n            )}\n             {(selectedStep?.stype == \"pystep\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-pystep-method\" fullWidth label=\"Override function name (optional)\" size='small' variant=\"outlined\" value={selectedStep?.method} onChange={(event) => { handleStepConfigChange(\"method\", event.target.value) }} />\n            )}\n            {(selectedStep?.stype == \"start_workflow_task_step\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-start_workflow_task_step\" fullWidth label=\"Name of the workflow\" size='small' variant=\"outlined\" value={selectedStep?.params[\"workflow_name\"]} onChange={(event) => { handleStepConfigChange(\"workflow_name\", event.target.value) }} />\n            )}\n            {(selectedStep?.stype == \"start_workflow_task_step\" || selectedStep?.stype == \"http_trigger\") && (\n              <FormControlLabel control={<Checkbox checked={selectedStep?.params[\"sync\"] == \"true\"} onChange={(event) => { handleStepConfigChange(\"workflow_sync_run_flag\", event.target.checked) }} />} label=\"Synchronous execution\" />\n            )}\n            {(selectedStep?.stype == \"file_uploader\") && (\n               <LocalUploader fileType=\"staging\" action=\"start_workflow\" onUpload={onUpload} stepId={selectedStep.id} workflowName={props.workflowName} />\n            )}\n\n            <FormControlLabel control={<Checkbox checked={selectedStep?.enabled} onChange={(event) => { handleStepConfigChange(\"enabled\", event.target.checked) }} />} label=\"Is step enabled\" />\n            <FormControlLabel control={<Checkbox checked={selectedStep?.trigger} onChange={(event) => { handleStepConfigChange(\"trigger\", event.target.checked) }} />} label=\"Is trigger step\" />\n            {(selectedStep?.trigger == false) && (\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-max-retries\" fullWidth label=\"Max retries on failure\" size='small' type=\"number\" variant=\"outlined\" value={selectedStep?.max_retries} onChange={(event) => { handleStepConfigChange(\"max_retries\", event.target.value) }} />\n            )}\n             {(selectedStep?.trigger == false) && (\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-retry-delay\" fullWidth label=\"Retry delay\" size='small' variant=\"outlined\" type=\"number\" value={selectedStep?.retry_delay} onChange={(event) => { handleStepConfigChange(\"retry_delay\", event.target.value) }} />\n             )}\n            </FormControl>\n            {(selectedStep?.stype == \"http_trigger\") && (\n\n                      <FormControl fullWidth sx={{ marginTop: 2 }}>\n                          <InputLabel id=\"workflow_start_method_label\">Workflow instance start method</InputLabel>\n                          <Select sx={{ marginTop: 1 }}\n                          labelId=\"workflow_start_method_label\"\n                          id=\"workflow_start_method\"\n                          value={selectedStep?.params[\"workflow_start_method\"]}\n                          label=\"Workflow instance start method\"\n                          size='small'\n                          variant=\"outlined\"\n                          onChange={(event) => { handleStepConfigChange(\"workflow_start_method\", event.target.value) }}\n                        >\n                          <MenuItem value=\"persistent_blocking\">Start single global workflow instance in blocking mode (default)</MenuItem>\n                          <MenuItem value=\"persistent_non_blocking\">Start single global workflow instance in non-blocking mode</MenuItem>\n                          <MenuItem value=\"ephemeral_instance\">Start ephemeral workflow instance per request</MenuItem>\n                        </Select>\n                       </FormControl>\n            )}\n            <FormControl fullWidth sx={{ marginTop: 2 }}>\n            {(selectedStep?.stype == \"http_trigger\" || selectedStep?.stype == \"wait_for_event\") && (\n              <TextField sx={{ marginTop: 1 }} value={runPayload} label=\"Run payload\"  size='small' variant=\"outlined\"  onChange={(event)=>setRunPayload(event.target.value)} id=\"run_payload\"> </TextField>\n            )}\n            {(selectedStep?.stype == \"http_trigger\" && selectedStep?.params[\"workflow_start_method\"]==\"persistent_blocking\") && (\n              <TextField sx={{ marginTop: 1 }} value={selectedStep?.params[\"max_wait_time\"]}  size='small' variant=\"outlined\"  label=\"Max blocking wait time\" onChange={(event) => { handleStepConfigChange(\"max_wait_time\", event.target.value) }} id=\"max_wait_time\"> </TextField>\n            )}\n            </FormControl>\n\n          <Typography> {statusText} </Typography>\n\n        </DialogContent>\n        <DialogActions>\n          <Button variant=\"outlined\" size=\"small\" onClick={handleDialogSave}>Save</Button>\n          <Button variant=\"outlined\" size=\"small\" onClick={handleDialogCancel}>Cancel</Button>\n          <Button variant=\"outlined\" size=\"small\" color=\"error\" onClick={handleDelete} >Delete</Button>\n          {(selectedStep?.stype == \"http_trigger\") && (\n              <Button variant=\"outlined\" size=\"small\" color=\"success\" onClick={handleRunCommand}>Run</Button>\n          )}\n          {(selectedStep?.stype == \"wait_for_event\") && (\n              <Button variant=\"outlined\" size=\"small\" color=\"success\" onClick={handleResumeCommand}>Resume execution</Button>\n          )}\n\n        </DialogActions>\n      </Dialog>\n)\n}\n",
+        "import Button from \"@mui/material/Button\"\nimport Checkbox from \"@mui/material/Checkbox\"\nimport { red } from \"@mui/material/colors\"\nimport Dialog from \"@mui/material/Dialog\"\nimport DialogActions from \"@mui/material/DialogActions\"\nimport DialogContent from \"@mui/material/DialogContent\"\nimport DialogTitle from \"@mui/material/DialogTitle\"\nimport FormControl from \"@mui/material/FormControl\"\nimport FormControlLabel from \"@mui/material/FormControlLabel\"\nimport MenuItem from \"@mui/material/MenuItem\"\nimport Select from \"@mui/material/Select\"\nimport TextField from \"@mui/material/TextField\"\nimport React, { useEffect, useState } from \"react\"\nimport { WorkflowStepDefinition, WorkflowSystemComponent } from \"types/WorkflowTypes\"\nimport { getNeatApiRootUrl } from \"./Utils\"\nimport LocalUploader from \"./LocalUploader\"\nimport { InputLabel, Typography } from \"@mui/material\"\n\nexport default function StepEditorDialog(props: any)\n{\n    const [dialogOpen, setDialogOpen] = useState(false);\n    const [selectedStep, setSelectedStep] = useState<WorkflowStepDefinition>();\n    const neatApiRootUrl = getNeatApiRootUrl();\n    const [runPayload,setRunPayload] = useState<string>(JSON.stringify({\"action\":\"approve\"}))\n    const [statusText,setStatusText] = useState<string>(\"\")\n\n    const handleDialogSave = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"save\");\n    };\n    const handleDialogCancel = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"cancel\");\n    };\n    const handleDelete = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"delete\");\n    };\n\n    const handleRunCommand = () => {\n        setDialogOpen(false);\n        // send POST request to run the step\n        fetch(neatApiRootUrl +'/api/workflow/'+props.workflowName+'/http_trigger/'+selectedStep.id, { method: 'POST', body: runPayload })\n        .then(response => response.json())\n        .then(data => {\n            console.log('Success:', data);\n        }).catch((error) => {\n            console.error('Error:', error);\n        })\n        props.onClose(selectedStep,\"run\");\n    };\n\n    const handleResumeCommand = () => {\n      setDialogOpen(false);\n      // send POST request to run the step\n      fetch(neatApiRootUrl +'/api/workflow/'+props.workflowName+'/resume/'+selectedStep.id+'/default', { method: 'POST', body: runPayload })\n      .then(response => response.json())\n      .then(data => {\n          console.log('Success:', data);\n      }).catch((error) => {\n          console.error('Error:', error);\n      })\n      props.onClose(selectedStep,\"run\");\n  };\n\n    const onUpload = (fileName:string , hash: string) => {\n      console.log(\"onUpload\",fileName,hash)\n      setStatusText(\"File uplloaded \"+fileName)\n    }\n\n    useEffect(() => {\n        if (props.open){\n            setDialogOpen(true);\n            setSelectedStep(props.step);\n            console.dir(props.step);\n        }\n      }, [props.open]);\n\n      const handleStepConfigChange = (name: string, value: any) => {\n        console.log('handleStepConfigChange')\n        console.dir(selectedStep);\n        let updStep= Object.assign({},selectedStep);\n\n        if (selectedStep) {\n          if (!selectedStep.params) {\n            selectedStep.params = {}\n          }\n          if (name == \"stype\") {\n            switch (value) {\n              case \"time_trigger\":\n                updStep.params = { \"interval\": \"every 60 minutes\" }\n                break;\n              case \"start_workflow_task_step\":\n                updStep.params = { \"workflow_name\": \"\", \"sync\": \"false\" }\n                break;\n            }\n            updStep[\"stype\"] = value;\n          } else {\n            switch (name) {\n              case \"time-interval\":\n                updStep.params[\"interval\"] = value;\n                break;\n              case \"workflow_name\":\n                updStep.params[\"workflow_name\"] = value;\n                break;\n              case \"workflow_sync_run_flag\":\n                value = \"false\"\n                if (value) {\n                  value = \"true\"\n                }\n                updStep.params[\"sync\"] = value;\n                break;\n              case \"workflow_start_method\":\n                updStep.params[\"workflow_start_method\"] = value;\n                break;\n              case \"max_wait_time\":\n                updStep.params[\"max_wait_time\"] = value;\n                break;\n              default:\n                updStep[name] = value;\n            }\n          }\n          console.log(\"rendering view\")\n        }\n        setSelectedStep(updStep);\n      }\n\n\nreturn (\n  <Dialog open={dialogOpen} onClose={handleDialogCancel}>\n        <DialogTitle>Step configurator</DialogTitle>\n        <DialogContent >\n          <FormControl  fullWidth>\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-id\" fullWidth label=\"Step id\" size='small' variant=\"outlined\" value={selectedStep?.id} onChange={(event) => { handleStepConfigChange(\"id\", event.target.value) }} />\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-label\" fullWidth label=\"Label\" size='small' variant=\"outlined\" value={selectedStep?.label} onChange={(event) => { handleStepConfigChange(\"label\", event.target.value) }} />\n          </FormControl>\n          <FormControl sx={{ marginTop: 2 }} fullWidth >\n            <InputLabel id=\"step_type_label\">Step type</InputLabel>\n            <Select sx={{ marginTop: 1 }}\n              id=\"step-config-stype\"\n              labelId=\"step_type_label\"\n              value={selectedStep?.stype}\n              label=\"Step type\"\n              size='small'\n              variant=\"outlined\"\n              onChange={(event) => { handleStepConfigChange(\"stype\", event.target.value) }}\n            >\n              <MenuItem value=\"stdstep\">Step from standard library</MenuItem>\n              <MenuItem value=\"pystep\">Python function</MenuItem>\n              <MenuItem value=\"http_trigger\">HTTP trigger</MenuItem>\n              <MenuItem value=\"time_trigger\">Time trigger</MenuItem>\n              <MenuItem value=\"wait_for_event\">Wait for event</MenuItem>\n              <MenuItem value=\"start_workflow_task_step\">Start workflow</MenuItem>\n              <MenuItem value=\"file_uploader\">File uploader</MenuItem>\n            </Select>\n          </FormControl>\n          <FormControl sx={{ marginTop: 1 }} fullWidth >\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-descr\" fullWidth label=\"Description\" size='small' variant=\"outlined\" value={selectedStep?.description} onChange={(event) => { handleStepConfigChange(\"description\", event.target.value) }} />\n            {(selectedStep?.stype == \"time_trigger\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-config-time-config\" fullWidth label=\"Time interval\" size='small' variant=\"outlined\" value={selectedStep?.params[\"interval\"]} onChange={(event) => { handleStepConfigChange(\"time-interval\", event.target.value) }} />\n            )}\n            {(selectedStep?.stype == \"stdstep\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-stdstep-method\" fullWidth label=\"Name of the step\" size='small' variant=\"outlined\" value={selectedStep?.method} onChange={(event) => { handleStepConfigChange(\"method\", event.target.value) }} />\n            )}\n             {(selectedStep?.stype == \"pystep\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-pystep-method\" fullWidth label=\"Override function name (optional)\" size='small' variant=\"outlined\" value={selectedStep?.method} onChange={(event) => { handleStepConfigChange(\"method\", event.target.value) }} />\n            )}\n            {(selectedStep?.stype == \"start_workflow_task_step\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-start_workflow_task_step\" fullWidth label=\"Name of the workflow\" size='small' variant=\"outlined\" value={selectedStep?.params[\"workflow_name\"]} onChange={(event) => { handleStepConfigChange(\"workflow_name\", event.target.value) }} />\n            )}\n            {(selectedStep?.stype == \"start_workflow_task_step\" || selectedStep?.stype == \"http_trigger\") && (\n              <FormControlLabel control={<Checkbox checked={selectedStep?.params[\"sync\"] == \"true\"} onChange={(event) => { handleStepConfigChange(\"workflow_sync_run_flag\", event.target.checked) }} />} label=\"Synchronous execution\" />\n            )}\n            {(selectedStep?.stype == \"file_uploader\") && (\n               <LocalUploader fileType=\"staging\" action=\"start_workflow\" onUpload={onUpload} stepId={selectedStep.id} workflowName={props.workflowName} />\n            )}\n\n            <FormControlLabel control={<Checkbox checked={selectedStep?.enabled} onChange={(event) => { handleStepConfigChange(\"enabled\", event.target.checked) }} />} label=\"Is step enabled\" />\n            <FormControlLabel control={<Checkbox checked={selectedStep?.trigger} onChange={(event) => { handleStepConfigChange(\"trigger\", event.target.checked) }} />} label=\"Is trigger step\" />\n            {(selectedStep?.trigger == false) && (\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-max-retries\" fullWidth label=\"Max retries on failure\" size='small' type=\"number\" variant=\"outlined\" value={selectedStep?.max_retries} onChange={(event) => { handleStepConfigChange(\"max_retries\", event.target.value) }} />\n            )}\n             {(selectedStep?.trigger == false) && (\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-retry-delay\" fullWidth label=\"Retry delay\" size='small' variant=\"outlined\" type=\"number\" value={selectedStep?.retry_delay} onChange={(event) => { handleStepConfigChange(\"retry_delay\", event.target.value) }} />\n             )}\n            </FormControl>\n            {(selectedStep?.stype == \"http_trigger\") && (\n\n                      <FormControl fullWidth sx={{ marginTop: 2 }}>\n                          <InputLabel id=\"workflow_start_method_label\">Workflow instance start method</InputLabel>\n                          <Select sx={{ marginTop: 1 }}\n                          labelId=\"workflow_start_method_label\"\n                          id=\"workflow_start_method\"\n                          value={selectedStep?.params[\"workflow_start_method\"]}\n                          label=\"Workflow instance start method\"\n                          size='small'\n                          variant=\"outlined\"\n                          onChange={(event) => { handleStepConfigChange(\"workflow_start_method\", event.target.value) }}\n                        >\n                          <MenuItem value=\"persistent_blocking\">Start single global workflow instance in blocking mode (default)</MenuItem>\n                          <MenuItem value=\"persistent_non_blocking\">Start single global workflow instance in non-blocking mode</MenuItem>\n                          <MenuItem value=\"ephemeral_instance\">Start ephemeral workflow instance per request</MenuItem>\n                        </Select>\n                       </FormControl>\n            )}\n            <FormControl fullWidth sx={{ marginTop: 2 }}>\n            {(selectedStep?.stype == \"http_trigger\" || selectedStep?.stype == \"wait_for_event\") && (\n              <TextField sx={{ marginTop: 1 }} value={runPayload} label=\"Run payload\"  size='small' variant=\"outlined\"  onChange={(event)=>setRunPayload(event.target.value)} id=\"run_payload\"> </TextField>\n            )}\n            {(selectedStep?.stype == \"http_trigger\" && selectedStep?.params[\"workflow_start_method\"]==\"persistent_blocking\") && (\n              <TextField sx={{ marginTop: 1 }} value={selectedStep?.params[\"max_wait_time\"]}  size='small' variant=\"outlined\"  label=\"Max blocking wait time\" onChange={(event) => { handleStepConfigChange(\"max_wait_time\", event.target.value) }} id=\"max_wait_time\"> </TextField>\n            )}\n            </FormControl>\n\n          <Typography> {statusText} </Typography>\n\n        </DialogContent>\n        <DialogActions>\n          <Button variant=\"outlined\" size=\"small\" onClick={handleDialogSave}>Save</Button>\n          <Button variant=\"outlined\" size=\"small\" onClick={handleDialogCancel}>Cancel</Button>\n          <Button variant=\"outlined\" size=\"small\" color=\"error\" onClick={handleDelete} >Delete</Button>\n          {(selectedStep?.stype == \"http_trigger\") && (\n              <Button variant=\"outlined\" size=\"small\" color=\"success\" onClick={handleRunCommand}>Run</Button>\n          )}\n          {(selectedStep?.stype == \"wait_for_event\") && (\n              <Button variant=\"outlined\" size=\"small\" color=\"success\" onClick={handleResumeCommand}>Resume execution</Button>\n          )}\n\n        </DialogActions>\n      </Dialog>\n)\n}\n",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getListItemUtilityClass(slot) {\n  return generateUtilityClass('MuiListItem', slot);\n}\nconst listItemClasses = generateUtilityClasses('MuiListItem', ['root', 'container', 'focusVisible', 'dense', 'alignItemsFlexStart', 'disabled', 'divider', 'gutters', 'padding', 'button', 'secondaryAction', 'selected']);\nexport default listItemClasses;",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getListItemButtonUtilityClass(slot) {\n  return generateUtilityClass('MuiListItemButton', slot);\n}\nconst listItemButtonClasses = generateUtilityClasses('MuiListItemButton', ['root', 'focusVisible', 'dense', 'alignItemsFlexStart', 'disabled', 'divider', 'gutters', 'selected']);\nexport default listItemButtonClasses;",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getListItemSecondaryActionClassesUtilityClass(slot) {\n  return generateUtilityClass('MuiListItemSecondaryAction', slot);\n}\nconst listItemSecondaryActionClasses = generateUtilityClasses('MuiListItemSecondaryAction', ['root', 'disableGutters']);\nexport default listItemSecondaryActionClasses;",
```

### Comparing `cognite_neat-0.17.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.17.3/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/cognite/neat/migration/wf_manifests.py` & `cognite_neat-0.17.3/cognite/neat/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.17.2/pyproject.toml` & `cognite_neat-0.17.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.17.2"
+version = "0.17.3"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 documentation = "https://cognite-neat.readthedocs-hosted.com/"
```

### Comparing `cognite_neat-0.17.2/PKG-INFO` & `cognite_neat-0.17.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
```
