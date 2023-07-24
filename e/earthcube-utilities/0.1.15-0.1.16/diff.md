# Comparing `tmp/earthcube_utilities-0.1.15.tar.gz` & `tmp/earthcube_utilities-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthcube_utilities-0.1.15.tar", last modified: Mon Jun 26 16:38:59 2023, max compression
+gzip compressed data, was "earthcube_utilities-0.1.16.tar", last modified: Mon Jul 24 19:04:20 2023, max compression
```

## Comparing `earthcube_utilities-0.1.15.tar` & `earthcube_utilities-0.1.16.tar`

### file list

```diff
@@ -1,112 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.496760 earthcube_utilities-0.1.15/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-26 16:38:59.496760 earthcube_utilities-0.1.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:38:59.496760 earthcube_utilities-0.1.15/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.480760 earthcube_utilities-0.1.15/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.484760 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-26 16:38:59.000000 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-26 16:38:59.000000 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:38:59.000000 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-26 16:38:59.000000 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-26 16:38:59.000000 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-26 16:38:59.000000 earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.484760 earthcube_utilities-0.1.15/src/ec/
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/check_sitemap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.484760 earthcube_utilities-0.1.15/src/ec/collection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/collection/rocrate_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/collection/rocrate_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.484760 earthcube_utilities-0.1.15/src/ec/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/datastore/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/ec_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/generate_graph_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.484760 earthcube_utilities-0.1.15/src/ec/gleanerio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/gleanerio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/gleanerio/gleaner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.484760 earthcube_utilities-0.1.15/src/ec/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/manageGraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_keywords.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_multiple_versioned_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_triples.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_types.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_types_top_level.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_count_variablename.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_graph_sizes.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_count_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_count_graphs.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_count_keywords.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_count_types.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_count_versioned_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_with_keywords.sparql
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_select_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_select_graphs.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_summary_query.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_urn_w_types_toplevel.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/org_all_org_triples.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/org_all_returns_properties.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/org_all_returns_urns.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/q_n_o_exact_query__returns_properties.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/q_n_o_query_returns_urn.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_graphs.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_keywords.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_multi_versioned_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_triples.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_triples_by_graph.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_types.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_types_top_level.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_count_variablename.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_graph_sizes.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_graphs_startwith.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_select_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_select_graphs.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_summary_query.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_urn_w_types_toplevel.sparql
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/select_one.sparql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/sparql_static/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/sparql_static/repo_graphs_opentopo.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/subj_construct_w_blanknodes.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_files/urn_triples_for_a_graph.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/graph/sparql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/logger/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/missing_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/notebook/geocodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/notebook/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/datacatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/ec_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/ecobjectmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/objects/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/query_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/reporting/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/sitemap/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/sitemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/sitemap/sitemap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/sos_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/sos_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/sos_json/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.492761 earthcube_utilities-0.1.15/src/ec/sos_json/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/sos_json/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/sos_json/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:38:59.496760 earthcube_utilities-0.1.15/src/ec/summarize/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/summarize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/summarize/summarize_materializedview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-26 16:38:49.000000 earthcube_utilities-0.1.15/src/ec/summarize_identifier_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.025465 earthcube_utilities-0.1.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-24 19:04:20.025465 earthcube_utilities-0.1.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:04:20.025465 earthcube_utilities-0.1.16/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.009464 earthcube_utilities-0.1.16/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.013464 earthcube_utilities-0.1.16/src/earthcube_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-24 19:04:19.000000 earthcube_utilities-0.1.16/src/earthcube_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-24 19:04:20.000000 earthcube_utilities-0.1.16/src/earthcube_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:04:19.000000 earthcube_utilities-0.1.16/src/earthcube_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-24 19:04:19.000000 earthcube_utilities-0.1.16/src/earthcube_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 19:04:19.000000 earthcube_utilities-0.1.16/src/earthcube_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-24 19:04:19.000000 earthcube_utilities-0.1.16/src/earthcube_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.013464 earthcube_utilities-0.1.16/src/ec/
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/bucketutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/check_sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.017464 earthcube_utilities-0.1.16/src/ec/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/collection/rocrate_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/collection/rocrate_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.017464 earthcube_utilities-0.1.16/src/ec/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/datastore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11582 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/ec_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/generate_graph_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.017464 earthcube_utilities-0.1.16/src/ec/gleanerio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/gleanerio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/gleanerio/gleaner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.017464 earthcube_utilities-0.1.16/src/ec/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/manageGraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.021465 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_count_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_count_keywords.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_count_multiple_versioned_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_count_triples.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_count_types.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_count_types_top_level.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_count_variablename.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_graph_sizes.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_repo_count_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_repo_count_graphs.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_repo_count_keywords.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_repo_count_types.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_repo_count_versioned_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_repo_with_keywords.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_select_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_select_graphs.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_summary_query.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_urn_w_types_toplevel.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/org_all_org_triples.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/org_all_returns_properties.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/org_all_returns_urns.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/q_n_o_exact_query__returns_properties.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/q_n_o_query_returns_urn.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_count_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_count_graphs.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_count_keywords.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_count_multi_versioned_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_count_triples.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_count_triples_by_graph.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_count_types.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_count_types_top_level.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_count_variablename.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_graph_sizes.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_graphs_startwith.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_select_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_select_graphs.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_summary_query.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_urn_w_types_toplevel.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/select_one.sparql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.025465 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/sparql_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/sparql_static/repo_graphs_opentopo.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/subj_construct_w_blanknodes.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_files/urn_triples_for_a_graph.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/graph/sparql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.025465 earthcube_utilities-0.1.16/src/ec/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/logger/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/missing_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.025465 earthcube_utilities-0.1.16/src/ec/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/notebook/geocodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/notebook/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.025465 earthcube_utilities-0.1.16/src/ec/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/objects/datacatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/objects/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/objects/ec_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/objects/ecobjectmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/objects/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/objects/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/query_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.025465 earthcube_utilities-0.1.16/src/ec/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13595 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/reporting/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.025465 earthcube_utilities-0.1.16/src/ec/sitemap/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/sitemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/sitemap/sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.025465 earthcube_utilities-0.1.16/src/ec/sos_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/sos_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/sos_json/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.025465 earthcube_utilities-0.1.16/src/ec/sos_json/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/sos_json/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/sos_json/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:04:20.025465 earthcube_utilities-0.1.16/src/ec/summarize/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/summarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/summarize/summarize_materializedview.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3804 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/summarize_from_graph_namespace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5270 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/summarize_from_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/summarize_identifier_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4666 2023-07-24 19:04:05.000000 earthcube_utilities-0.1.16/src/ec/summarize_repo.py
```

### Comparing `earthcube_utilities-0.1.15/PKG-INFO` & `earthcube_utilities-0.1.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthcube_utilities
-Version: 0.1.15
+Version: 0.1.16
 Summary: A package of utilities for NSF Earthcube Geocodes Project
 Author-email: Mike Bobak <mbobak@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>, Ya-Lan Yang <ylyang@illinois.edu>
 Maintainer-email: Ya-Lan Yang <ylyang@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>
 Project-URL: Homepage, https://www.earthcube.org/
 Project-URL: Bug Tracker, https://github.com/earthcube/earthcube_utilities/issues
 Project-URL: Geocodes Documentation, https://earthcube.github.io/geocodes_documentation/
 Project-URL: Source, https://github.com/earthcube/earthcube_utilities
```

### Comparing `earthcube_utilities-0.1.15/README.md` & `earthcube_utilities-0.1.16/README.md`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/pyproject.toml` & `earthcube_utilities-0.1.16/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "earthcube_utilities"
-version = "0.1.15"
+version = "0.1.16"
 dynamic = ["dependencies"]
 description = "A package of utilities for NSF Earthcube Geocodes Project"
 readme =  "README.md"
 
 authors = [
     {name = "Mike Bobak", email = "mbobak@illinois.edu"},
     {name= "David Valentine", email="dwvalentine@ucsd.edu"},
@@ -35,14 +35,16 @@
 #    'module' object is not callable
 [project.scripts]
 generategraphstats = "ec.generate_graph_stats:start"
 check_sitemap = "ec.check_sitemap:start"
 query_graph = "ec.query_graph:start"
 missing_report = "ec.missing_report:start"
 summarize_identifier_metadata = "ec.summarize_identifier_metadata:start"
+ec_reports = "ec.ec_reports:start"
+bucketutil = "ec.bucketutil:start"
 
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 [tool.setuptools.packages.find]
 where = ["src"]
 [tool.setuptools.package-data]
```

### Comparing `earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/PKG-INFO` & `earthcube_utilities-0.1.16/src/earthcube_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthcube-utilities
-Version: 0.1.15
+Version: 0.1.16
 Summary: A package of utilities for NSF Earthcube Geocodes Project
 Author-email: Mike Bobak <mbobak@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>, Ya-Lan Yang <ylyang@illinois.edu>
 Maintainer-email: Ya-Lan Yang <ylyang@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>
 Project-URL: Homepage, https://www.earthcube.org/
 Project-URL: Bug Tracker, https://github.com/earthcube/earthcube_utilities/issues
 Project-URL: Geocodes Documentation, https://earthcube.github.io/geocodes_documentation/
 Project-URL: Source, https://github.com/earthcube/earthcube_utilities
```

### Comparing `earthcube_utilities-0.1.15/src/earthcube_utilities.egg-info/SOURCES.txt` & `earthcube_utilities-0.1.16/src/earthcube_utilities.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 requirements.txt
 src/earthcube_utilities.egg-info/PKG-INFO
 src/earthcube_utilities.egg-info/SOURCES.txt
 src/earthcube_utilities.egg-info/dependency_links.txt
 src/earthcube_utilities.egg-info/entry_points.txt
 src/earthcube_utilities.egg-info/requires.txt
 src/earthcube_utilities.egg-info/top_level.txt
+src/ec/bucketutil.py
 src/ec/check_sitemap.py
 src/ec/ec_reports.py
 src/ec/generate_graph_stats.py
 src/ec/missing_report.py
 src/ec/query_graph.py
+src/ec/summarize_from_graph_namespace.py
+src/ec/summarize_from_release.py
 src/ec/summarize_identifier_metadata.py
+src/ec/summarize_repo.py
 src/ec/collection/__init__.py
 src/ec/collection/rocrate_archive.py
 src/ec/collection/rocrate_collection.py
 src/ec/datastore/__init__.py
 src/ec/datastore/s3.py
 src/ec/gleanerio/__init__.py
 src/ec/gleanerio/gleaner.py
```

### Comparing `earthcube_utilities-0.1.15/src/ec/check_sitemap.py` & `earthcube_utilities-0.1.16/src/ec/check_sitemap.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/collection/rocrate_collection.py` & `earthcube_utilities-0.1.16/src/ec/collection/rocrate_collection.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/datastore/s3.py` & `earthcube_utilities-0.1.16/src/ec/datastore/s3.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
+import logging
 from datetime import datetime
 from io import BytesIO
 
 import minio
 import pandas
 import pydash
 from minio.commonconfig import CopySource, REPLACE
+from pydash import is_empty
 from pydash.collections import find
 
 def shaFroms3Path(path, extension=None):
     split = path.split("/")
     sha = split[len(split)-1]
     if extension is not None:
         sha = pydash.strings.replace_end(sha, extension, '')
@@ -38,14 +40,15 @@
         self.options = options
         self.default_bucket = default_bucket
 
     def listPath(self, bucket, path, include_user_meta=False):
         pass
     def countPath(self, bucket, path):
         count = len(list(self.listPath(bucket,path)))
+        return count
 
     def DataframeFromPath(self, bucket, path, include_user_meta=False):
         pass
 # who knows, we might implement on disk, or in a database. This just separates the data from the annotated metadata
     def getFileFromStore(self, s3ObjectInfo):
         pass
     def getFileMetadataFromStore(self, s3ObjectInfo):
@@ -65,15 +68,15 @@
            # metadata=metadata,
             metadata_directive=REPLACE,
         )
 
     #### Methods for a getting information using infrastructure information
 
     """ Method for gleaner store"""
-    def listJsonld(self,bucket, repo,include_user_meta=False):
+    def listJsonld(self,bucket, repo, include_user_meta=False):
         """ urllist returns list of urn;s with urls"""
         # include user meta not working.
         path = f"{self.paths['summon']}/{repo}/"
         return self.listPath(bucket, path,include_user_meta=include_user_meta)
 
     def countJsonld(self,bucket, repo) -> int:
         count = len(list(self.listJsonld(bucket,repo)))
@@ -81,22 +84,22 @@
 
     def getJsonLD(self, bucket, repo, sha):
         path = f"{self.paths['summon']}/{repo}/{sha}.jsonld"
         s3ObjectInfo = {"bucket_name": bucket, "object_name": path}
         resp = self.getFileFromStore(s3ObjectInfo)
         return resp
 
+
     def listSummonedUrls(self,bucket, repo):
         """  returns list of urns with urls"""
         jsonlds = self.listJsonld(bucket, repo, include_user_meta=True)
         objs = map(lambda f: self.s3client.stat_object(f.bucket_name, f.object_name), jsonlds)
-        # for ob in objs:
-        #     print(ob)
         o_list = list(map(lambda f: {"sha": shaFroms3Path(f.object_name), "url": f.metadata["X-Amz-Meta-Url"]}, objs))
         return o_list
+
     def listSummonedSha(self,bucket, repo):
         """  returns list of urns with urls"""
         jsonlds = self.listJsonld(bucket, repo, include_user_meta=False)
         objs = map(lambda f: shaFroms3Path( f.object_name, extension=".jsonld"), jsonlds)
         # for ob in objs:
         #     print(ob)
         o_list = list(objs)
@@ -194,22 +197,51 @@
             """
         self.endpoint = s3endpoint
         self.options = options
         self.default_bucket= default_bucket
         self.s3client  =minio.Minio(s3endpoint) # this will neeed to be fixed with authentication
 
 
-    def listPath(self, bucket, path, include_user_meta=False):
+    def listPath(self, bucket, path, include_user_meta=False, recursive=True):
         """ returns the filelist for a path with the starting path removed from the list"""
-        resp = self.s3client.list_objects(bucket, path, include_user_meta=include_user_meta)
+        resp = self.s3client.list_objects(bucket, path, include_user_meta=include_user_meta, recursive=recursive)
         # the returned list includes the path
-        #o_list = list(resp)
         o_list = filter(lambda f: f.object_name != path, resp)
         return o_list
 
+    def listDuplicateUrls(self, bucket, sources, include_user_meta=False, recursive=False):
+        if is_empty(sources):
+            raise Exception("must provide sources")
+
+        sources_to_run = sources
+        dfs = pandas.DataFrame()
+        paths = list(self.listPath(bucket, "summoned/", include_user_meta=include_user_meta, recursive=recursive))
+        for p in paths:
+            if not find(sources_to_run, lambda x: f"{self.paths.get('summon')}/{x}/" == p.object_name):
+                continue
+            try:
+                jsonlds = self.listPath(bucket, p.object_name)
+                objs = map(lambda f: self.s3client.stat_object(f.bucket_name, f.object_name), jsonlds)
+                o_list = list(map(lambda f: {'Source': p.object_name,
+                                             'Url': f.metadata.get('X-Amz-Meta-Url'),
+                                             'Name': f.object_name,
+                                             'Date': f.last_modified,
+                                             }, objs))
+            except Exception as e:
+                logging.error(e)
+            df = pandas.DataFrame(o_list)
+            df['Url Duplicates'] = df.groupby(['Source', 'Url'])['Name'].transform('count')
+            dfs = pandas.concat([dfs, df])
+        return dfs
+
+
+    def countPath(self, bucket, path):
+        count = len(list(self.listPath(bucket, path)))
+        return count
+
     def getFileFromStore(self, s3ObjectInfo):
         """ get an s3 file from teh store
         Parameters:
           s3ObjectInfo: {"bucket_name":obj.bucket_name, "object_name":obj.object_name }
 
         """
         resp = self.s3client.get_object(s3ObjectInfo["bucket_name"], s3ObjectInfo["object_name"])
@@ -229,17 +261,20 @@
 
     def getFileMetadataFromStore(self, s3ObjectInfo):
         """ get metadata s3 file from teh store
                Parameters:
                  s3ObjectInfo: {"bucket_name":obj.bucket_name, "object_name":obj.object_name }
 
                """
-        s3obj = self.s3client.stat_object(s3ObjectInfo.bucket_name, s3ObjectInfo.object_name)
-        for o in s3obj:
-            user_meta = pydash.collections.filter_(o,lambda m: m.startswith("X-Amz-Meta") )
+        s3obj = self.s3client.stat_object(s3ObjectInfo.get('bucket_name'), s3ObjectInfo.get('object_name'))
+        md = s3obj.metadata
+        user_meta = list()
+        for o in md:
+            if o.startswith("X-Amz-Meta"):
+               user_meta.append({"name": o, "value": md[o]})
         # this needs to return the metadata
         return user_meta
 
     def putReportFile(self, bucket, repo, filename, json_str, date="latest", copy_to_date=True):
         path = f"{self.paths['report']}/{repo}/{date}/{filename}"
         f = BytesIO()
         length = f.write(bytes(json_str, 'utf-8'))
@@ -270,7 +305,10 @@
         return paths
 
     def getRoCrateFile(self, filename, bucket="gleaner", user="public"):
         path = f"/{self.paths['collection']}/{user}/{filename}"
         crate = self.s3client.get_object(bucket, path)
         return crate
 
+    def removeObject(self, bucket, path):
+        self.s3client.remove_object(bucket, path)
+        return
```

### Comparing `earthcube_utilities-0.1.15/src/ec/ec_reports.py` & `earthcube_utilities-0.1.16/src/ec/ec_reports.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import functools
 import click
 import logging
 import json
 import sys
 from pydash.collections import find
 from pydash import is_empty
-import pandas as pd
 from ec.gleanerio.gleaner import getSitemapSourcesFromGleaner, getGleaner
-from ec.reporting.report import missingReport
-from ec.reporting.report import  generateGraphReportsRepo, reportTypes
+from ec.reporting.report import generateGraphReportsRepo, reportTypes, missingReport, generateIdentifierRepo
 from ec.datastore import s3
 from ec.logger import config_app
 
 log = config_app()
 class EcConfig(object):
     """ Parameters that might be common to commands"""
     def __init__(self, cfgfile=None, s3server=None, s3bucket=None, graphendpoint=None, upload=None, output=None,debug=False):
@@ -124,27 +122,33 @@
 
     ctx.hasS3Upload()
     ctx.hasGraphendpoint(message=" must provide graphendpoint")
     if upload:
         s3Minio = s3.MinioDatastore(s3server, None)
     """query an endpoint, store results as a json file in an s3 store"""
     log.info(f"Querying {graphendpoint} for graph statisitcs  ")
+    if source:
+        sources = source
+    else:
+        sources = getSitemapSourcesFromGleaner(cfgfile)
+        sources = list(filter(lambda source: source.get('active'), sources))
+        sources = list(map(lambda r: r.get('name'), sources))
 ### more work needed before detailed works
     if "all" in source:
         if detailed:
             report_json = generateGraphReportsRepo("all", graphendpoint, reportList=reportTypes["all_detailed"])
         else:
             report_json = generateGraphReportsRepo("all", graphendpoint,reportList=reportTypes["all"])
-            if output:  # just append the json files to one filem, for now.
-                log.info(f" report for ALL appended to file")
-                output.write(report_json)
-            if upload:
-                bucketname, objectname = s3Minio.putReportFile(s3bucket, "all", "graph_report.json", report_json)
+        if output:  # just append the json files to one filem, for now.
+            log.info(f" report for ALL appended to file")
+            output.write(report_json)
+        if upload:
+            bucketname, objectname = s3Minio.putReportFile(s3bucket, "all", "graph_report.json", report_json)
     else:
-        for s in source:
+        for s in sources:
             if detailed:
                 report_json = generateGraphReportsRepo(s, graphendpoint, reportList=reportTypes["repo_detailed"])
             else:
                 report_json = generateGraphReportsRepo(s, graphendpoint, reportList=reportTypes["repo"])
             if output:  # just append the json files to one filem, for now.
                 log.info(f" report for {s} appended to file")
                 output.write(bytes(report_json, 'utf-8'))
@@ -184,27 +188,16 @@
     if source:
         sources = source
     else:
         sources = getSitemapSourcesFromGleaner(cfgfile)
         sources = list(filter(lambda source: source.get('active'), sources))
         sources = list(map(lambda r: r.get('name'), sources))
     for repo in sources:
-        jsonlds = s3Minio.listJsonld(bucket, repo, include_user_meta=True)
-        objs = map(lambda f: s3Minio.s3client.stat_object(f.bucket_name, f.object_name), jsonlds)
-        o_list = list(map(lambda f: {'Source': repo,
-                                     'Identifiertype': f.metadata.get('X-Amz-Meta-Identifiertype'),
-                                     'Matchedpath': f.metadata.get('X-Amz-Meta-Matchedpath'),
-                                     'Uniqueid': f.metadata.get('X-Amz-Meta-Uniqueid'),
-                                     'Example': f.metadata.get('X-Amz-Meta-Uniqueid')
-                                     }, objs))
-
-        df = pd.DataFrame(o_list)
         try:
-            identifier_stats = df.groupby(['Source', 'Identifiertype', 'Matchedpath'], group_keys=True, dropna=False)\
-                .agg({'Uniqueid': 'count', 'Example': lambda x: x.iloc[0:5].tolist()}).reset_index()
+            identifier_stats = generateIdentifierRepo(repo, bucket, s3Minio)
             if json:
                 o = identifier_stats.to_json(orient='records', indent=2)
             else:
                 o = identifier_stats.to_csv(index=False)
 
             if output:
                 logging.info(f" report for {repo} appended to file")
```

### Comparing `earthcube_utilities-0.1.15/src/ec/generate_graph_stats.py` & `earthcube_utilities-0.1.16/src/ec/generate_graph_stats.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/gleanerio/gleaner.py` & `earthcube_utilities-0.1.16/src/ec/gleanerio/gleaner.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/graph/manageGraph.py` & `earthcube_utilities-0.1.16/src/ec/graph/manageGraph.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_repo_count_graphs.sparql` & `earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_repo_count_graphs.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_summary_query.sparql` & `earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_summary_query.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql` & `earthcube_utilities-0.1.16/src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/org_all_returns_properties.sparql` & `earthcube_utilities-0.1.16/src/ec/graph/sparql_files/org_all_returns_properties.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/q_n_o_exact_query__returns_properties.sparql` & `earthcube_utilities-0.1.16/src/ec/graph/sparql_files/q_n_o_exact_query__returns_properties.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/q_n_o_query_returns_urn.sparql` & `earthcube_utilities-0.1.16/src/ec/graph/sparql_files/q_n_o_query_returns_urn.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/repo_summary_query.sparql` & `earthcube_utilities-0.1.16/src/ec/graph/sparql_files/repo_summary_query.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql` & `earthcube_utilities-0.1.16/src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/graph/sparql_files/subj_construct_w_blanknodes.sparql` & `earthcube_utilities-0.1.16/src/ec/graph/sparql_files/subj_construct_w_blanknodes.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/graph/sparql_query.py` & `earthcube_utilities-0.1.16/src/ec/graph/sparql_query.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/logger/log.py` & `earthcube_utilities-0.1.16/src/ec/logger/log.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/missing_report.py` & `earthcube_utilities-0.1.16/src/ec/missing_report.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/notebook/utils.py` & `earthcube_utilities-0.1.16/src/ec/notebook/utils.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/objects/ecobjectmanager.py` & `earthcube_utilities-0.1.16/src/ec/objects/ecobjectmanager.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/query_graph.py` & `earthcube_utilities-0.1.16/src/ec/query_graph.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/reporting/report.py` & `earthcube_utilities-0.1.16/src/ec/reporting/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,9 +262,24 @@
 
 def listGraphReportDates4Repo(repo,  datastore: bucketDatastore):
     """get the latest for a dashboard"""
     path = f"{datastore.paths['reports']}/{repo}/"
     filelist = datastore.listPath(path)
     return filelist
 
+def generateIdentifierRepo(repo, bucket, datastore: bucketDatastore):
+    jsonlds = datastore.listJsonld(bucket, repo, include_user_meta=True)
+    objs = map(lambda f: datastore.s3client.stat_object(f.bucket_name, f.object_name), jsonlds)
+    o_list = list(map(lambda f: {'Source': repo,
+                                 'Identifiertype': f.metadata.get('X-Amz-Meta-Identifiertype'),
+                                 'Matchedpath': f.metadata.get('X-Amz-Meta-Matchedpath'),
+                                 'Uniqueid': f.metadata.get('X-Amz-Meta-Uniqueid'),
+                                 'Example': f.metadata.get('X-Amz-Meta-Uniqueid')
+                                 }, objs))
+    df = pandas.DataFrame(o_list)
+    identifier_stats = df.groupby(['Source', 'Identifiertype', 'Matchedpath'], group_keys=True, dropna=False) \
+        .agg({'Uniqueid': 'count', 'Example': lambda x: x.iloc[0:5].tolist()}).reset_index()
+    return identifier_stats
+
+
```

### Comparing `earthcube_utilities-0.1.15/src/ec/sitemap/sitemap.py` & `earthcube_utilities-0.1.16/src/ec/sitemap/sitemap.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from numpy import ndarray
 from pandarallel import pandarallel
 from pandas import DataFrame
 
 import requests, sys, os
 import yaml
 from pandas.core.arrays import ExtensionArray
-from tqdm import tqdm
 
 def _urlExists(sitemapurl):
     try:
         r = requests.get(sitemapurl)
         if r.status_code == 404:
             logging.error("Sitemap URL is 404")
             return False
```

### Comparing `earthcube_utilities-0.1.15/src/ec/sos_json/rdf.py` & `earthcube_utilities-0.1.16/src/ec/sos_json/rdf.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/sos_json/utils.py` & `earthcube_utilities-0.1.16/src/ec/sos_json/utils.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.15/src/ec/summarize/summarize_materializedview.py` & `earthcube_utilities-0.1.16/src/ec/summarize/summarize_materializedview.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,37 +14,37 @@
 HTTP_SCHEMA_ORG = "http://schema.org/"
 BASE_SHCEMA_ORG = HTTPS_SCHEMA_ORG
 context = f"@prefix : <{BASE_SHCEMA_ORG}> ."
 
 ### BLAZEGRAPH
 '''original fetch all from temporary namespace'''
 def get_summary4repo(endpoint: str) -> pandas.DataFrame:
-    logging.INFO("Running Summary Query to Get all records")
+    logging.info("Running Summary Query to Get all records")
     df = queryWithSparql("all_summary_query", endpoint)
     return df
     # file = '../resources/sparql/summary_query.txt'
     # with open(file, 'r') as f:
     #     lines = f.read()
     # df = sparqldataframe.query(endpoint,lines)
     # return df
 
 ''' fetch all from graph namespace'''
 def get_summary4graph(endpoint : str) -> pandas.DataFrame:
-    logging.INFO("Running Summary Query to Get all records")
+    logging.info("Running Summary Query to Get all records")
     df= queryWithSparql("all_summary_query",endpoint)
     return df
     # file = '../resources/sparql/all_summary_query.sparql'
     # with open(file, 'r') as f:
     #     lines = f.read()
     # df = sparqldataframe.query(endpoint,lines)
     # return df
 
 ''' fetch subset  from graph namespace'''
 def get_summary4repoSubset(endpoint: str, repo : str) -> pandas.DataFrame:
-    logging.INFO(f"Running Summary Query to Get {repo} records")
+    logging.info(f"Running Summary Query to Get {repo} records")
     df = queryWithSparql("repo_summary_query",endpoint, parameters={"repo":repo})
     return df
     # file = '../resources/sparql/repo_summary_query.sparql'
     # with open(file, 'r') as f:
     #     lines = f.read()
     # #query = getFileFromResources(f"{template_name}")
     # #q_template = Template(query)
```

