# Comparing `tmp/quickstats-0.6.8.9.tar.gz` & `tmp/quickstats-0.6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.6.8.9.tar", last modified: Fri Jul 14 09:26:18 2023, max compression
+gzip compressed data, was "quickstats-0.6.9.0.tar", last modified: Mon Jul 24 14:35:13 2023, max compression
```

## Comparing `quickstats-0.6.8.9.tar` & `quickstats-0.6.9.0.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:18.000000 quickstats-0.6.8.9/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-07-14 09:26:18.000000 quickstats-0.6.8.9/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.8.9/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:12.000000 quickstats-0.6.8.9/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.8.9/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:12.000000 quickstats-0.6.8.9/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-05-31 15:23:38.000000 quickstats-0.6.8.9/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-07-13 23:45:35.000000 quickstats-0.6.8.9/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:12.000000 quickstats-0.6.8.9/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.8.9/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.8.9/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.8.9/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.8.9/quickstats/analysis/config_format_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.8.9/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.8.9/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.8.9/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.8.9/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.8.9/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    32121 2023-07-07 22:03:31.000000 quickstats-0.6.8.9/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8897 2023-06-07 14:20:37.000000 quickstats-0.6.8.9/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:12.000000 quickstats-0.6.8.9/quickstats/analysis/systematics/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.8.9/quickstats/analysis/systematics/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29560 2023-07-07 22:04:35.000000 quickstats-0.6.8.9/quickstats/analysis/systematics/base_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.8.9/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.8.9/quickstats/analysis/systematics/normalization_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11869 2023-07-07 22:04:22.000000 quickstats-0.6.8.9/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:13.000000 quickstats-0.6.8.9/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.8.9/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    35538 2023-07-13 11:58:34.000000 quickstats-0.6.8.9/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.8.9/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.8.9/quickstats/clis/inspect_ws.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-06-05 09:37:42.000000 quickstats-0.6.8.9/quickstats/clis/likelihood_fit.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7980 2023-06-26 09:38:29.000000 quickstats-0.6.8.9/quickstats/clis/likelihood_scan.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.8.9/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1512 2023-06-13 21:11:53.000000 quickstats-0.6.8.9/quickstats/clis/processor_cli.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15259 2023-06-13 03:13:49.000000 quickstats-0.6.8.9/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:13.000000 quickstats-0.6.8.9/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      849 2023-05-30 19:49:31.000000 quickstats-0.6.8.9/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-27 07:22:07.000000 quickstats-0.6.8.9/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13357 2023-07-07 21:51:04.000000 quickstats-0.6.8.9/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7333 2023-06-08 10:12:47.000000 quickstats-0.6.8.9/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    30804 2023-05-20 02:55:29.000000 quickstats-0.6.8.9/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.8.9/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31916 2023-06-07 11:32:50.000000 quickstats-0.6.8.9/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)   102824 2023-07-08 04:44:50.000000 quickstats-0.6.8.9/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5542 2023-07-07 21:58:36.000000 quickstats-0.6.8.9/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13996 2023-07-12 12:32:58.000000 quickstats-0.6.8.9/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:13.000000 quickstats-0.6.8.9/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.8.9/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.8.9/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.8.9/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.8.9/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.8.9/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.8.9/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.8.9/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10888 2023-07-03 21:42:51.000000 quickstats-0.6.8.9/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17463 2023-07-07 22:11:31.000000 quickstats-0.6.8.9/quickstats/components/nuisance_parameter_pull.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12396 2023-07-07 22:07:20.000000 quickstats-0.6.8.9/quickstats/components/nuisance_parameter_ranking.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:13.000000 quickstats-0.6.8.9/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.8.9/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:14.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2666 2023-07-07 21:51:37.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      870 2023-05-23 18:53:54.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1154 2023-06-03 14:06:41.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1250 2023-06-13 21:07:45.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_load_macro.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1677 2023-05-22 21:51:19.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2129 2023-06-03 16:04:25.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      645 2023-06-03 14:13:00.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9969 2023-06-05 23:09:50.000000 quickstats-0.6.8.9/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.8.9/quickstats/components/processors/roo_config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6792 2023-07-12 23:26:18.000000 quickstats-0.6.8.9/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.8.9/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3551 2023-07-07 21:53:49.000000 quickstats-0.6.8.9/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.8.9/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.8.9/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:14.000000 quickstats-0.6.8.9/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.8.9/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.8.9/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.8.9/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.8.9/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.8.9/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.8.9/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.8.9/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53162 2023-06-06 14:20:25.000000 quickstats-0.6.8.9/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.8.9/quickstats/components/workspaces/ws_decomposer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.8.9/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    45869 2023-07-07 21:58:59.000000 quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    49268 2023-07-08 04:44:49.000000 quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:15.000000 quickstats-0.6.8.9/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      306 2023-05-31 15:27:50.000000 quickstats-0.6.8.9/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3379 2023-06-26 09:41:33.000000 quickstats-0.6.8.9/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.8.9/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5239 2023-05-31 16:02:49.000000 quickstats-0.6.8.9/quickstats/concurrent/nuisance_parameter_ranking_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5891 2023-06-10 22:16:28.000000 quickstats-0.6.8.9/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10758 2023-06-28 16:38:35.000000 quickstats-0.6.8.9/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3963 2023-05-31 15:27:15.000000 quickstats-0.6.8.9/quickstats/concurrent/parameterised_runner.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:15.000000 quickstats-0.6.8.9/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.8.9/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.8.9/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.8.9/quickstats/core/configs.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.8.9/quickstats/core/configurable_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.8.9/quickstats/core/dataclass_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      971 2023-05-20 03:27:42.000000 quickstats-0.6.8.9/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2296 2023-05-23 21:10:32.000000 quickstats-0.6.8.9/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.8.9/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.8.9/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.8.9/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:15.000000 quickstats-0.6.8.9/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2023-05-31 15:27:05.000000 quickstats-0.6.8.9/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:15.000000 quickstats-0.6.8.9/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.6.8.9/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.8.9/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2023-07-12 23:07:57.000000 quickstats-0.6.8.9/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.8.9/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:15.000000 quickstats-0.6.8.9/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.8.9/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.8.9/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.8.9/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.8.9/quickstats/interface/root/RooCategory.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.8.9/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.8.9/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.8.9/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.8.9/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.8.9/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.8.9/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.8.9/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.8.9/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.8.9/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.8.9/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.8.9/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.8.9/quickstats/interface/root/inspection.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.8.9/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.8.9/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5637 2023-05-27 06:13:47.000000 quickstats-0.6.8.9/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:12.000000 quickstats-0.6.8.9/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:15.000000 quickstats-0.6.8.9/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.8.9/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.8.9/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:16.000000 quickstats-0.6.8.9/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.8.9/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.8.9/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:16.000000 quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:16.000000 quickstats-0.6.8.9/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.8.9/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.8.9/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:16.000000 quickstats-0.6.8.9/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.8.9/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.8.9/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:16.000000 quickstats-0.6.8.9/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.8.9/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2093 2023-06-21 12:10:05.000000 quickstats-0.6.8.9/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.8.9/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    28267 2023-07-08 04:40:34.000000 quickstats-0.6.8.9/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.8.9/quickstats/maths/statistics_jitted.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.8.9/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:16.000000 quickstats-0.6.8.9/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.8.9/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.8.9/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15974 2023-07-13 23:36:20.000000 quickstats-0.6.8.9/quickstats/parsers/param_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:17.000000 quickstats-0.6.8.9/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.8.9/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14389 2023-06-21 01:49:40.000000 quickstats-0.6.8.9/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.8.9/quickstats/plots/bidirectional_bar_chart.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.8.9/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.8.9/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.8.9/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.8.9/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6018 2023-07-03 18:31:57.000000 quickstats-0.6.8.9/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.8.9/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.8.9/quickstats/plots/histo_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.8.9/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8917 2023-07-04 13:41:54.000000 quickstats-0.6.8.9/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15974 2023-07-10 11:46:54.000000 quickstats-0.6.8.9/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.8.9/quickstats/plots/likelihood_scan_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29141 2023-07-13 12:02:23.000000 quickstats-0.6.8.9/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25696 2023-04-18 01:26:39.000000 quickstats-0.6.8.9/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.8.9/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.8.9/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.8.9/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-07-12 22:40:24.000000 quickstats-0.6.8.9/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.8.9/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.8.9/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18278 2023-07-12 22:35:07.000000 quickstats-0.6.8.9/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-06-19 12:52:28.000000 quickstats-0.6.8.9/quickstats/plots/upper_limit_2D_plot_deprecated.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.8.9/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17108 2023-07-10 22:33:48.000000 quickstats-0.6.8.9/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29707 2023-06-27 09:55:20.000000 quickstats-0.6.8.9/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:17.000000 quickstats-0.6.8.9/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.8.9/quickstats/resources/default_workspace_extensions.json
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.8.9/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:17.000000 quickstats-0.6.8.9/quickstats/stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.8.9/quickstats/stylesheets/quick_default.mplstyle
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:18.000000 quickstats-0.6.8.9/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.8.9/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11009 2023-07-07 22:00:44.000000 quickstats-0.6.8.9/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.8.9/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17089 2023-06-04 03:39:00.000000 quickstats-0.6.8.9/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.8.9/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6812 2023-05-31 13:27:25.000000 quickstats-0.6.8.9/quickstats/utils/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.8.9/quickstats/utils/process_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    26262 2023-06-07 15:13:35.000000 quickstats-0.6.8.9/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.8.9/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12379 2023-07-07 22:00:16.000000 quickstats-0.6.8.9/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1448 2023-07-08 03:51:23.000000 quickstats-0.6.8.9/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15023 2023-07-07 22:01:35.000000 quickstats-0.6.8.9/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:12.000000 quickstats-0.6.8.9/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-07-14 09:26:08.000000 quickstats-0.6.8.9/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9130 2023-07-14 09:26:10.000000 quickstats-0.6.8.9/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-07-14 09:26:08.000000 quickstats-0.6.8.9/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-07-14 09:26:08.000000 quickstats-0.6.8.9/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-07-14 09:26:08.000000 quickstats-0.6.8.9/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-07-14 09:26:18.000000 quickstats-0.6.8.9/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.8.9/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:13.000000 quickstats-0.6.9.0/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-07-24 14:35:13.000000 quickstats-0.6.9.0/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.9.0/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:34:51.000000 quickstats-0.6.9.0/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.9.0/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:34:51.000000 quickstats-0.6.9.0/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      581 2023-07-23 19:03:03.000000 quickstats-0.6.9.0/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-07-24 13:33:59.000000 quickstats-0.6.9.0/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:34:55.000000 quickstats-0.6.9.0/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.9.0/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.9.0/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.9.0/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.9.0/quickstats/analysis/config_format_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.9.0/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.9.0/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.9.0/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.9.0/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.9.0/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    32121 2023-07-07 22:03:31.000000 quickstats-0.6.9.0/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8897 2023-06-07 14:20:37.000000 quickstats-0.6.9.0/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:34:56.000000 quickstats-0.6.9.0/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.9.0/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29560 2023-07-07 22:04:35.000000 quickstats-0.6.9.0/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.9.0/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.9.0/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11869 2023-07-07 22:04:22.000000 quickstats-0.6.9.0/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:34:58.000000 quickstats-0.6.9.0/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.9.0/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    35538 2023-07-13 11:58:34.000000 quickstats-0.6.9.0/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.9.0/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.9.0/quickstats/clis/inspect_ws.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-06-05 09:37:42.000000 quickstats-0.6.9.0/quickstats/clis/likelihood_fit.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7980 2023-06-26 09:38:29.000000 quickstats-0.6.9.0/quickstats/clis/likelihood_scan.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.9.0/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1512 2023-06-13 21:11:53.000000 quickstats-0.6.9.0/quickstats/clis/processor_cli.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15259 2023-06-13 03:13:49.000000 quickstats-0.6.9.0/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:01.000000 quickstats-0.6.9.0/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      849 2023-05-30 19:49:31.000000 quickstats-0.6.9.0/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-27 07:22:07.000000 quickstats-0.6.9.0/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13357 2023-07-07 21:51:04.000000 quickstats-0.6.9.0/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7333 2023-06-08 10:12:47.000000 quickstats-0.6.9.0/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    30762 2023-07-23 18:54:18.000000 quickstats-0.6.9.0/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3030 2023-07-19 10:50:53.000000 quickstats-0.6.9.0/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31916 2023-06-07 11:32:50.000000 quickstats-0.6.9.0/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)   103483 2023-07-19 10:51:41.000000 quickstats-0.6.9.0/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5542 2023-07-07 21:58:36.000000 quickstats-0.6.9.0/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13996 2023-07-12 12:32:58.000000 quickstats-0.6.9.0/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:01.000000 quickstats-0.6.9.0/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.9.0/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.9.0/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.9.0/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.9.0/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.9.0/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.9.0/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.9.0/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10888 2023-07-03 21:42:51.000000 quickstats-0.6.9.0/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17591 2023-07-23 18:52:55.000000 quickstats-0.6.9.0/quickstats/components/nuisance_parameter_pull.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12396 2023-07-07 22:07:20.000000 quickstats-0.6.9.0/quickstats/components/nuisance_parameter_ranking.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:01.000000 quickstats-0.6.9.0/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.9.0/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:02.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2666 2023-07-07 21:51:37.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      870 2023-05-23 18:53:54.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1154 2023-06-03 14:06:41.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1250 2023-06-13 21:07:45.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1677 2023-05-22 21:51:19.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2129 2023-06-03 16:04:25.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      645 2023-06-03 14:13:00.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9969 2023-06-05 23:09:50.000000 quickstats-0.6.9.0/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.9.0/quickstats/components/processors/roo_config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6792 2023-07-12 23:26:18.000000 quickstats-0.6.9.0/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5396 2023-07-23 19:24:23.000000 quickstats-0.6.9.0/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3551 2023-07-07 21:53:49.000000 quickstats-0.6.9.0/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.9.0/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.9.0/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:04.000000 quickstats-0.6.9.0/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.9.0/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.9.0/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.9.0/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.9.0/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.9.0/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.9.0/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.9.0/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53162 2023-06-06 14:20:25.000000 quickstats-0.6.9.0/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.9.0/quickstats/components/workspaces/ws_decomposer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.9.0/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.9.0/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.9.0/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.9.0/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    45869 2023-07-07 21:58:59.000000 quickstats-0.6.9.0/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    49268 2023-07-08 04:44:49.000000 quickstats-0.6.9.0/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:05.000000 quickstats-0.6.9.0/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      306 2023-05-31 15:27:50.000000 quickstats-0.6.9.0/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3379 2023-06-26 09:41:33.000000 quickstats-0.6.9.0/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.9.0/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5239 2023-05-31 16:02:49.000000 quickstats-0.6.9.0/quickstats/concurrent/nuisance_parameter_ranking_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5891 2023-06-10 22:16:28.000000 quickstats-0.6.9.0/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10758 2023-06-28 16:38:35.000000 quickstats-0.6.9.0/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3963 2023-05-31 15:27:15.000000 quickstats-0.6.9.0/quickstats/concurrent/parameterised_runner.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:06.000000 quickstats-0.6.9.0/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      438 2023-07-23 19:02:20.000000 quickstats-0.6.9.0/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      783 2023-07-23 19:18:06.000000 quickstats-0.6.9.0/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.9.0/quickstats/core/configs.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.9.0/quickstats/core/configurable_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.9.0/quickstats/core/dataclass_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4276 2023-07-23 02:09:11.000000 quickstats-0.6.9.0/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7528 2023-07-23 19:04:39.000000 quickstats-0.6.9.0/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7082 2023-07-23 19:01:51.000000 quickstats-0.6.9.0/quickstats/core/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6641 2023-07-23 19:25:33.000000 quickstats-0.6.9.0/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.9.0/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.9.0/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:06.000000 quickstats-0.6.9.0/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2023-05-31 15:27:05.000000 quickstats-0.6.9.0/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:06.000000 quickstats-0.6.9.0/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.6.9.0/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.9.0/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2023-07-12 23:07:57.000000 quickstats-0.6.9.0/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.9.0/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:07.000000 quickstats-0.6.9.0/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.9.0/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.9.0/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.9.0/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.9.0/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.9.0/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.9.0/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.9.0/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.9.0/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.9.0/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.9.0/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.9.0/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.9.0/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.9.0/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.9.0/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.9.0/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.9.0/quickstats/interface/root/inspection.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.9.0/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.9.0/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5634 2023-07-23 19:23:46.000000 quickstats-0.6.9.0/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:34:51.000000 quickstats-0.6.9.0/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:08.000000 quickstats-0.6.9.0/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.9.0/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.9.0/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:08.000000 quickstats-0.6.9.0/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.9.0/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.9.0/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:08.000000 quickstats-0.6.9.0/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3133 2023-07-23 01:48:41.000000 quickstats-0.6.9.0/quickstats/macros/QuickStatsCore/QStringUtils.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1259 2023-07-23 01:29:12.000000 quickstats-0.6.9.0/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.9.0/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.9.0/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:08.000000 quickstats-0.6.9.0/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.9.0/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.9.0/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:08.000000 quickstats-0.6.9.0/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.9.0/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.9.0/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:09.000000 quickstats-0.6.9.0/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.9.0/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2421 2023-07-17 00:45:10.000000 quickstats-0.6.9.0/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6026 2023-07-14 16:35:45.000000 quickstats-0.6.9.0/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    28267 2023-07-08 04:40:34.000000 quickstats-0.6.9.0/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.9.0/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.9.0/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:09.000000 quickstats-0.6.9.0/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.9.0/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.9.0/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15974 2023-07-13 23:36:20.000000 quickstats-0.6.9.0/quickstats/parsers/param_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:11.000000 quickstats-0.6.9.0/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1445 2023-07-17 13:33:28.000000 quickstats-0.6.9.0/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14389 2023-06-21 01:49:40.000000 quickstats-0.6.9.0/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.9.0/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.9.0/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.9.0/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.9.0/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.9.0/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6018 2023-07-03 18:31:57.000000 quickstats-0.6.9.0/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3542 2023-07-24 12:28:32.000000 quickstats-0.6.9.0/quickstats/plots/general_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.9.0/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.9.0/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8917 2023-07-04 13:41:54.000000 quickstats-0.6.9.0/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16009 2023-07-17 00:34:30.000000 quickstats-0.6.9.0/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.9.0/quickstats/plots/likelihood_scan_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29140 2023-07-23 01:38:20.000000 quickstats-0.6.9.0/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25851 2023-07-24 11:57:52.000000 quickstats-0.6.9.0/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.9.0/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.9.0/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.9.0/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22526 2023-07-24 11:07:45.000000 quickstats-0.6.9.0/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.9.0/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-07-21 13:27:32.000000 quickstats-0.6.9.0/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18278 2023-07-23 22:06:59.000000 quickstats-0.6.9.0/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-06-19 12:52:28.000000 quickstats-0.6.9.0/quickstats/plots/upper_limit_2D_plot_deprecated.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.9.0/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    23255 2023-07-21 14:08:44.000000 quickstats-0.6.9.0/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29933 2023-07-21 09:28:38.000000 quickstats-0.6.9.0/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:11.000000 quickstats-0.6.9.0/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.9.0/quickstats/resources/default_workspace_extensions.json
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.9.0/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:11.000000 quickstats-0.6.9.0/quickstats/stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.9.0/quickstats/stylesheets/quick_default.mplstyle
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:35:12.000000 quickstats-0.6.9.0/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.9.0/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11668 2023-07-23 01:58:52.000000 quickstats-0.6.9.0/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.9.0/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17121 2023-07-21 12:03:57.000000 quickstats-0.6.9.0/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.9.0/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    26262 2023-06-07 15:13:35.000000 quickstats-0.6.9.0/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.9.0/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12370 2023-07-23 18:55:25.000000 quickstats-0.6.9.0/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4968 2023-07-23 00:52:38.000000 quickstats-0.6.9.0/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15023 2023-07-07 22:01:35.000000 quickstats-0.6.9.0/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-24 14:34:51.000000 quickstats-0.6.9.0/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-07-24 14:34:46.000000 quickstats-0.6.9.0/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9147 2023-07-24 14:34:47.000000 quickstats-0.6.9.0/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-07-24 14:34:46.000000 quickstats-0.6.9.0/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-07-24 14:34:46.000000 quickstats-0.6.9.0/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-07-24 14:34:46.000000 quickstats-0.6.9.0/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-07-24 14:35:13.000000 quickstats-0.6.9.0/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.9.0/setup.py
```

### Comparing `quickstats-0.6.8.9/PKG-INFO` & `quickstats-0.6.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.8.9
+Version: 0.6.9.0
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.8.9/README.md` & `quickstats-0.6.9.0/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/bin/quickstats` & `quickstats-0.6.9.0/bin/quickstats`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/__init__.py` & `quickstats-0.6.9.0/quickstats/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 stylesheet_path = os.path.join(module_path, 'stylesheets')
 resource_path = os.path.join(module_path, 'resources')
 
 # ROOT.gInterpreter.AddIncludePath(os.path.join(macro_path, "macros"))
 
 MAX_WORKERS = 8
 
-from quickstats.utils.io import VerbosePrint
-_PRINT_ = VerbosePrint("INFO")
-
 corelib_loaded = False
 
 from quickstats.core import *
 
+stdout = AbstractObject.stdout
+
 root_version = get_root_version()
```

### Comparing `quickstats-0.6.8.9/quickstats/analysis/analysis_base.py` & `quickstats-0.6.9.0/quickstats/analysis/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.6.9.0/quickstats/analysis/analysis_path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/config_format_templates.py` & `quickstats-0.6.9.0/quickstats/analysis/config_format_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/data_loading.py` & `quickstats-0.6.9.0/quickstats/analysis/data_loading.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/data_preprocessing.py` & `quickstats-0.6.9.0/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/event_categorization.py` & `quickstats-0.6.9.0/quickstats/analysis/event_categorization.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.6.9.0/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.6.9.0/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.6.9.0/quickstats/analysis/ntuple_process_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.6.9.0/quickstats/analysis/sample_poly_param_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.6.9.0/quickstats/analysis/systematics/base_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.6.9.0/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.6.9.0/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.6.9.0/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/clis/core.py` & `quickstats-0.6.9.0/quickstats/clis/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/clis/inspect_rfile.py` & `quickstats-0.6.9.0/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/clis/inspect_ws.py` & `quickstats-0.6.9.0/quickstats/clis/inspect_ws.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/clis/likelihood_fit.py` & `quickstats-0.6.9.0/quickstats/clis/likelihood_fit.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/clis/likelihood_scan.py` & `quickstats-0.6.9.0/quickstats/clis/likelihood_scan.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/clis/limit_setting.py` & `quickstats-0.6.9.0/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/clis/processor_cli.py` & `quickstats-0.6.9.0/quickstats/clis/processor_cli.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/clis/workspace_tools.py` & `quickstats-0.6.9.0/quickstats/clis/workspace_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/__init__.py` & `quickstats-0.6.9.0/quickstats/components/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/analysis_base.py` & `quickstats-0.6.9.0/quickstats/components/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/analysis_object.py` & `quickstats-0.6.9.0/quickstats/components/analysis_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/asimov_generator.py` & `quickstats-0.6.9.0/quickstats/components/asimov_generator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/asymptotic_cls.py` & `quickstats-0.6.9.0/quickstats/components/asymptotic_cls.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 import math
 import json
 
 import numpy as np
 
 import ROOT
 
-from quickstats import semistaticmethod
+from quickstats import semistaticmethod, cls_method_timer
 from quickstats.components import AnalysisObject
 from quickstats.utils.root_utils import load_macro
 from quickstats.utils import common_utils
-from quickstats.utils.io import Verbosity
 from quickstats.maths.numerics import pretty_value
 from quickstats.components.basics import WSArgument
 
 class AsymptoticCLs(AnalysisObject):
     
     _SIGMA_LABEL_ = {
             2: '+2sigma',
@@ -183,22 +182,22 @@
 
     def get_nll_val(self, nll:"ROOT.RooNLLVar"):
         snapshot_name = self.nll_maps[nll].get('snapshot', None)
         if snapshot_name:
             self.load_snapshot(snapshot_name)
         else:
             raise RuntimeError(f'Failed to load snapshot for nll "{nll.GetName()}"')
-        if Verbosity.DEBUG >= self.stdout.verbosity:
+        if self.stdout.verbosity <= "DEBUG":
             self.stdout.debug("Before Fit ----------------------------------------------")
             self.model.print_summary(items=['poi', 'nuisance_parameter', 'global_observable'])
         self.last_fit_status = self.minimizer.minimize(nll) 
         self.global_status += self.last_fit_status
         self.minimizer_calls += 1
         nll_val = nll.getVal()
-        if Verbosity.DEBUG >= self.stdout.verbosity:
+        if self.stdout.verbosity <= "DEBUG":
             self.stdout.debug("After Fit ----------------------------------------------")
             self.model.print_summary(items=['poi', 'nuisance_parameter', 'global_observable'])          
         self.load_snapshot(self.nom_glob_name)
         return nll_val
     
     def create_nll(self, dataset:"ROOT.RooDataSet"):
         return self.minimizer._create_nll(dataset=dataset)
@@ -514,15 +513,15 @@
         self.LimitTool.setTargetCLs(init_target_cls)
         self.direction = 1
         self.LimitTool.setDirection(1)
         mu_guess = self.LimitTool.findCrossing(sigma, sigma, n_times_sigma)
         limit = self.get_limit(asimov_n_nll, mu_guess, n)
         return limit    
     
-    @common_utils.timer
+    @cls_method_timer
     def evaluate_limits(self):
         # TODO: maybe load nominal snapshot first
         self.reset()
         obs_nll = self.create_nll(self.data)
         self.nll_maps[obs_nll] = {"dataset": self.data, "snapshot": self.nom_glob_name}
         self.dataset_maps[self.data] = obs_nll
         self.save_snapshot(self.nom_glob_name, variables=WSArgument.GLOBAL_OBSERVABLE)
```

### Comparing `quickstats-0.6.8.9/quickstats/components/extended_minimizer.py` & `quickstats-0.6.9.0/quickstats/components/extended_minimizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/extended_model.py` & `quickstats-0.6.9.0/quickstats/components/extended_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,23 @@
 
 import ROOT
 from ROOT.RooPrintable import (kName, kClassName, kValue, kArgs, kExtras, kAddress,
                                kTitle, kCollectionHeader, kSingleLine)
 
 import quickstats
 from quickstats import semistaticmethod, AbstractObject
-from quickstats.maths.numerics import is_integer, pretty_value, get_bins_given_edges, array_issubset
+from quickstats.maths.numerics import is_integer, pretty_value, get_bins_given_edges, array_issubset, get_rmin_rmax
 from quickstats.utils.root_utils import load_macro
 from quickstats.utils.common_utils import str_list_filter, combine_dict
-from quickstats.utils.roofit_utils import (get_variable_attributes, variable_collection_to_dataframe,
-                                           get_relevant_components)
+from quickstats.utils import roofit_utils
 from quickstats.utils.string_utils import split_str, remove_whitespace
 from quickstats.interface.root import TH1, RooDataSet, RooArgSet, RooMsgService, RooAbsPdf
 from quickstats.interface.root import roofit_extension as rf_ext
 from quickstats.interface.root.roofit_extension import get_str_data
-from quickstats.components.basics import WSArgument, SetValueMode
+from quickstats.components.basics import WSArgument, SetValueMode, ConstraintType
 from .extended_minimizer import ExtendedMinimizer
 
 class ExtendedModel(AbstractObject):
     
     _DEFAULT_CONSTR_CLS_ = ["RooGaussian", "RooLognormal", "RooGamma", "RooPoisson", "RooBifurGauss"]
     
     _DEFAULT_NAMES_ = {
@@ -184,23 +183,15 @@
     def deactivate_lv2_const_optimization(self, ws, condition):
         self.stdout.info('Deactivating level 2 constant term optimization for specified pdfs')
         for component in ws.components():
             name = component.GetName()
             if (component.InheritsFrom(ROOT.RooAbsPdf.Class()) and condition(name)):
                 component.setAttribute("NOCacheAndTrack")
                 self.stdout.info(f'Deactivated level 2 constant term optimization for {name}')
-                
-    def load_snapshots(self, snapshot_names:List[str]):
-        for snapshot_name in snapshot_names:
-            if self.workspace.getSnapshot(snapshot_name):
-                self.workspace.loadSnapshot(snapshot_name)
-                self.stdout.info(f'Loaded snapshot "{snapshot_name}"')
-            else:
-                self.stdout.warning(f'Failed to load snapshot "{snapshot_name}"')
-            
+     
     def initialize(self):
         if isinstance(self.filename, str):
             if not os.path.exists(self.filename):
                 raise FileNotFoundError(f'workspace file "{self.filename}" does not exist')
             self.stdout.info(f'Opening file "{self.filename}"')
             file = ROOT.TFile(self.filename) 
             if (not file):
@@ -580,29 +571,35 @@
         constraints = self.get_all_constraints()
         unfolded_constraints = rf_ext.unfold_constraints(constraints, self.observables, self.nuisance_parameters,
                                                          constraint_cls=constr_cls,
                                                          recursion_limit=recursion_limit,
                                                          strip_disconnected=strip_disconnected)
         return unfolded_constraints
     
-    def pair_constraints(self, fmt:str="list", to_str=False, sort:bool=True, base_component:bool=False):
+    def pair_constraints(self, fmt:str="list", to_str=False, sort:bool=True, base_component:bool=False,
+                         constraint_type:Optional[ConstraintType]=None):
         constraint_pdfs = self.unfold_constraints()
+        if constraint_type is not None:
+            constraint_type = ConstraintType.parse(constraint_type)
+            constraint_pdfs = [pdf for pdf in constraint_pdfs if pdf.ClassName() == constraint_type.classname]
+            constraint_pdfs = ROOT.RooArgSet(*constraint_pdfs)
         if base_component:
             # for glob value matching
             return rf_ext.pair_constraints_base_component(constraint_pdfs, self.nuisance_parameters,
                                                           self.global_observables, fmt=fmt,
                                                           sort=sort, to_str=to_str)
         return rf_ext.pair_constraints(constraint_pdfs, self.nuisance_parameters,
                                        self.global_observables, fmt=fmt,
                                        sort=sort, to_str=to_str)
     
-    def get_constrained_nuisance_parameters(self, fmt:str='list'):
+    def get_constrained_nuisance_parameters(self, fmt:str='list',
+                                            constraint_type:Optional[ConstraintType]=None):
         """Get the list of constrained nuisance parameters instances
         """
-        _, constrained_nuis, _ = self.pair_constraints(fmt=fmt)
+        _, constrained_nuis, _ = self.pair_constraints(fmt=fmt, constraint_type=constraint_type)
         return constrained_nuis
     
     def get_unconstrained_nuisance_parameters(self, constrained_nuis=None):
         """Get the list of unconstrained nuisance parameters instances
         """
         # do not re-isolate constrained nuisance parameters
         if constrained_nuis is None:
@@ -1800,14 +1797,18 @@
             variables = ROOT.RooArgSet(self.pois)
         elif resolved_vtype == WSArgument.GLOBAL_OBSERVABLE:
             variables = ROOT.RooArgSet(self.global_observables)
         elif resolved_vtype == WSArgument.NUISANCE_PARAMETER:
             variables = ROOT.RooArgSet(self.nuisance_parameters)
         elif resolved_vtype == WSArgument.CONSTRAINED_NUISANCE_PARAMETER:
             variables = RooArgSet.from_list(self.get_constrained_nuisance_parameters())
+        elif resolved_vtype == WSArgument.GAUSSIAN_CONSTRAINT_NP:
+            variables = RooArgSet.from_list(self.get_constrained_nuisance_parameters(constraint_type=ConstraintType.GAUSSIAN))
+        elif resolved_vtype == WSArgument.POISSON_CONSTRAINT_NP:
+            variables = RooArgSet.from_list(self.get_constrained_nuisance_parameters(constraint_type=ConstraintType.POISSON))
         elif resolved_vtype == WSArgument.UNCONSTRAINED_NUISANCE_PARAMETER:
             variables = RooArgSet.from_list(self.get_unconstrained_nuisance_parameters())
         elif resolved_vtype == WSArgument.CONSTRAINT:
             nuis_list, glob_list, pdf_list = self.pair_constraints(sort=sort)
             return RooArgSet.from_list(nuis_list), RooArgSet.from_list(glob_list), RooArgSet.from_list(pdf_list)
         elif resolved_vtype == WSArgument.AUXILIARY:
             variables           = self.get_variables(WSArgument.VARIABLE)
@@ -1865,41 +1866,42 @@
                         content = self._DEFAULT_CONTENT_[WSArgument.FUNCTION]
                     collection = self.workspace.allFunctions()
                 else:
                     raise RuntimeError("unexpected error")
                 df_1 = get_str_data(collection, fill_classes=True,
                                     fill_definitions=True, content=content,
                                     style=kSingleLine, fmt="dataframe")
-                df_2 = variable_collection_to_dataframe(collection)
+                df_2 = roofit_utils.variable_collection_to_dataframe(collection)
                 df = df_1.merge(df_2, on="name", how='outer', sort=True, validate="one_to_one")
                 return df
             else:
                 raise ValueError(f"unsupported workspace attribute: {attribute}")
-        df = variable_collection_to_dataframe(collection, asym_error=asym_error)
+        df = roofit_utils.variable_collection_to_dataframe(collection, asym_error=asym_error)
         return df
     
     def rename_dataset(self, rename_map:Dict):
         for old_name, new_name in rename_map.items():
             if old_name == new_name:
                 continue
             dataset = self.workspace.data(old_name)
             if not dataset:
-                raise RuntimeError(f"dataset \"{old_name}\" not found in the workspace")
+                raise RuntimeError(f'dataset "{old_name}" not found in the workspace')
             check_dataset = self.workspace.data(new_name)
             if check_dataset:
-                raise RuntimeError(f"cannot rename dataset from \"{old_name}\" to \"{new_name}\": "
-                                   f"the dataset \"{new_name}\" already exists in the workspace")
+                raise RuntimeError(f'cannot rename dataset from "{old_name}" to "{new_name}": '
+                                   f'dataset "{new_name}" already exists in the workspace')
             dataset.SetName(new_name)
     
     @staticmethod
     def _format_category_summary(category_name:str, category_map:Dict):
         observable = category_map['observable']
-        bin_range = category_map['bin_range']
+        bin_range  = category_map['bin_range']
+        rmin, rmax = get_rmin_rmax(bin_range)
         bins = category_map['bins']
-        summary_str = f"{category_name} (observable = {observable}, range = [{bin_range[0]}, {bin_range[1]}], bins = {bins})"
+        summary_str = f"{category_name} (observable = {observable}, range = [{rmin}, {rmax}], bins = {bins})"
         return summary_str
         
     def print_summary(self, items:Optional[List]=None, suppress_print:bool=False, detailed:bool=True,
                       include_patterns:Optional[List]=None, exclude_patterns:Optional[List]=None,
                       save_as:Optional[str]=None):
         if items is None:
             items = ['workspace', 'dataset', 'snapshot', 'category',
@@ -1957,15 +1959,15 @@
             param_names_to_include = param_names.copy()
             if include_patterns is not None:
                 param_names_to_include = str_list_filter(param_names_to_include, include_patterns, inclusive=True)
             if exclude_patterns is not None:
                 param_names_to_include = str_list_filter(param_names_to_include, exclude_patterns, inclusive=False)
             param_index = np.in1d(param_names, param_names_to_include).nonzero()
             pset = np.array(pset)[param_index]
-            data = [get_variable_attributes(p) for p in pset]
+            data = [roofit_utils.get_variable_attributes(p) for p in pset]
             data = sorted(data, key=lambda d: d['name'])
             if detailed:
                 for d in data:
                     name   = d['name']
                     value  = d['value']
                     vmin   = d['min']
                     vmax   = d['max']
@@ -1976,22 +1978,15 @@
                     name = d['name']
                     summary_str += f"\t{name}\n"
         if not suppress_print:
             self.stdout.info(summary_str, bare=True)
         if save_as is not None:
             with open(save_as, "w") as f:
                 f.write(summary_str)
-                
-    def get_systematics_variations(self, filter_name:Optional[str]=None,
-                                   filter_client:Optional[str]=None, fmt:str="pandas"):
-        from quickstats.utils.roofit_utils import get_systematics_variations
-        constr_pdfs, constr_nuis, _ = self.pair_constraints()
-        return get_systematics_variations(constr_nuis, constr_pdfs, filter_name=filter_name,
-                                          filter_client=filter_client, fmt=fmt)
-    
+
     def compare_snapshots(self, ss1:Union[str, ROOT.RooArgSet], ss2:Union[str, ROOT.RooArgSet]):
         snapshots = {}
         for label, ss in [("left", ss1), ("right", ss2)]:
             if isinstance(ss, str):
                 if not self.workspace.getSnapshot(ss):
                     raise ValueError(f'workspace does not contain a snapshot named "{ss}"')
                 ss = self.workspace.getSnapshot(ss)
@@ -2009,43 +2004,56 @@
         data_2 = get_str_data(snapshots["right"], fill_classes=False,
                               fill_definitions=True,
                               content=content, style=style, fmt="dataframe")
         data.add(data_1, data_2)
         data.process()
         summary_str = data.get_summary_str(visibility=0b01011, indent="    ")
         self.stdout.info(summary_str, bare=True)
+        
+    def get_systematics_variations(self, filter_name:Optional[str]=None,
+                                   filter_client:Optional[str]=None, fmt:str="pandas"):
+        constr_pdfs, constr_nuis, _ = self.pair_constraints()
+        syst_variations = roofit_utils. get_systematics_variations(constr_nuis, constr_pdfs,
+                                                                   filter_name=filter_name,
+                                                                   filter_client=filter_client, fmt=fmt)
+        return syst_variations
     
     def get_gaussian_constraint_attributes(self, fmt:str="pandas"):
         constr_pdfs, _, _ = self.pair_constraints()
-        from quickstats.utils.roofit_utils import get_gaussian_pdf_attributes
-        return get_gaussian_pdf_attributes(constr_pdfs, fmt=fmt)
+        constr_attributes = roofit_utils.get_gaussian_pdf_attributes(constr_pdfs, fmt=fmt)
+        return constr_attributes
    
     def get_poisson_constraint_attributes(self, fmt:str="pandas"):
         constr_pdfs, _, _ = self.pair_constraints()
-        from quickstats.utils.roofit_utils import get_poisson_pdf_attributes
-        return get_poisson_pdf_attributes(constr_pdfs, fmt=fmt)
-    
+        constr_attributes = roofit_utils.get_poisson_pdf_attributes(constr_pdfs, fmt=fmt)
+        return constr_attributes
     
-    def get_category_expected_events_over_range(self, category:str, range:List[float],
-                                                normalize:bool=False):
-        assert len(range) == 2
+    def get_category_pdf(self, category:str):
         pdf_cat = self.pdf.getPdf(category)
         if not pdf_cat:
             raise RuntimeError(f'{category} is not a valid category in the workspace')
+        return pdf_cat
+        
+    def get_category_expected_events_over_range(self, category:str, range:List[float],
+                                                normalize:bool=False):
+        pdf_cat = self.get_category_pdf(category)
+        rmin, rmax = get_rmin_rmax(range)
         expected_events = RooAbsPdf.get_expected_events_over_range(pdf_cat, self.observables,
-                                                                   range[0], range[1],
-                                                                   normalize=normalize)
+                                                                   rmin, rmax, normalize=normalize)
         return expected_events
     
-    
+    def load_snapshots(self, snapshot_names:List[str]):
+        for snapshot_name in snapshot_names:
+            self.load_snapshot(snapshot_name)
+
     def load_snapshot(self, snapshot_name:Optional[str]=None):
         if snapshot_name is not None:
             snapshot = self.workspace.getSnapshot(snapshot_name)
             if (not snapshot) and ('0x(nil)' in snapshot.__repr__()):
-                self.stdout.warning(f'Snapshot "{snapshot_name}" does not exist.')
+                self.stdout.warning(f'Failed to load snapshot "{snapshot_name}" (snapshot does not exist)')
             else:
                 self.workspace.loadSnapshot(snapshot_name)
                 self.stdout.info(f'Loaded snapshot "{snapshot_name}"')
                 
     def save_snapshot(self, snapshot_name:Optional[str]=None, 
                       variables:Optional[Union[ROOT.RooArgSet, str, WSArgument]]=None):
         if snapshot_name is not None:
```

### Comparing `quickstats-0.6.8.9/quickstats/components/extended_rfile.py` & `quickstats-0.6.9.0/quickstats/components/extended_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/likelihood.py` & `quickstats-0.6.9.0/quickstats/components/likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/modelling/component_source.py` & `quickstats-0.6.9.0/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/modelling/data_modelling.py` & `quickstats-0.6.9.0/quickstats/components/modelling/data_modelling.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/modelling/model_source.py` & `quickstats-0.6.9.0/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.6.9.0/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.6.9.0/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.6.9.0/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.6.9.0/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.6.9.0/quickstats/components/nuisance_parameter_pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 ##################################################################################################
 import os
 import sys
 import time
 import json
 import fnmatch
 from itertools import repeat
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import numpy as np
 
+from quickstats import AbstractObject, cls_method_timer, VerbosePrint
 from quickstats.components import ExtendedModel, ExtendedMinimizer
 from quickstats.utils import root_utils, common_utils, string_utils
-from quickstats.utils.io import VerbosePrint
 
 import ROOT
 
-class NuisanceParameterPull(object):
+class NuisanceParameterPull(AbstractObject):
     @property
     def model(self):
         return self._model
     
     @property
     def workspace(self):
         return self._workspace
@@ -45,15 +45,16 @@
     @property
     def pois(self):
         return self._pois
     @property
     def observables(self):
         return self._observables  
     
-    def __init__(self):
+    def __init__(self, verbosity:Optional[Union[int, str]]="INFO"):
+        super().__init__(verbosity=verbosity)
         self._model               = None
         self._workspace           = None
         self._model_config        = None
         self._pdf                 = None
         self._data                = None
         self._nuisance_parameters = None
         self._global_observables  = None
@@ -274,15 +275,15 @@
         stdout.info('Saved output to {}'.format(outname_root))
         outname_json = os.path.join(outdir, nuis_name + '.json')
         json.dump(result, open(outname_json, 'w'), indent=2)
         
         if logfile_path is not None:
             common_utils.restore_stdout()
 
-    @common_utils.timer
+    @cls_method_timer
     def run_pulls(self, filename:str, data_name:str='combData', poi_name:str='', 
                   snapshot_name:Optional[str]=None, outdir:str='output', profile_param:Optional[str]=None,
                   fix_param:Optional[str]=None, ws_name:Optional[str]=None, mc_name:Optional[str]=None,
                   minimizer_type:str='Minuit2', minimizer_algo:str='Migrad', num_cpu:int=1, save_log:bool=True,
                   binned_likelihood:bool=True, precision:float=0.001, eps:float=1.0, retry:int=0, verbosity:str='INFO',
                   eigen:bool=False, strategy:int=0, print_level:int=1, fix_cache:bool=True, fix_multi:bool=True,
                   offset:bool=True, optimize:int=2, filter_expr:Optional[str]=None, max_calls:int=-1, max_iters:int=-1,
```

### Comparing `quickstats-0.6.8.9/quickstats/components/nuisance_parameter_ranking.py` & `quickstats-0.6.9.0/quickstats/components/nuisance_parameter_ranking.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/__init__.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_export.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_load_macro.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_load_macro.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_report.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_save.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.6.9.0/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/builtin_methods.py` & `quickstats-0.6.9.0/quickstats/components/processors/builtin_methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/roo_config_parser.py` & `quickstats-0.6.9.0/quickstats/components/processors/roo_config_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/processors/roo_processor.py` & `quickstats-0.6.9.0/quickstats/components/processors/roo_processor.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/pvalue_toys.py` & `quickstats-0.6.9.0/quickstats/components/pvalue_toys.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             batch_indices = np.delete(batch_indices, cached_indices)
         else:
             batch_save_as = [None]*len(batches)
             
         arguments = (batches, repeat(seed), batch_indices, batch_save_as)
         
         
-        tmp_verbosity = quickstats._PRINT_.verbosity
+        tmp_verbosity = quickstats.stdout.verbosity
 
         batch_results = execute_multi_tasks(self._get_toy_results, *arguments, parallel=parallel)
         
         quickstats.set_verbosity(tmp_verbosity)
         
         for batch_result in batch_results:
             results += batch_result
```

### Comparing `quickstats-0.6.8.9/quickstats/components/roo_inspector.py` & `quickstats-0.6.9.0/quickstats/components/roo_inspector.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/root_object.py` & `quickstats-0.6.9.0/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/toy_limit_calculator.py` & `quickstats-0.6.9.0/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/__init__.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/sample.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/settings.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/systematic.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/systematic.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/ws_comparer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/ws_decomposer.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/ws_decomposer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.6.9.0/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/concurrent/abstract_runner.py` & `quickstats-0.6.9.0/quickstats/concurrent/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/concurrent/logging.py` & `quickstats-0.6.9.0/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/concurrent/nuisance_parameter_ranking_runner.py` & `quickstats-0.6.9.0/quickstats/concurrent/nuisance_parameter_ranking_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.6.9.0/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.6.9.0/quickstats/concurrent/parameterised_likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.6.9.0/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/core/abstract_object.py` & `quickstats-0.6.9.0/quickstats/core/abstract_object.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from typing import Optional, Union, List, Dict
 
-import quickstats
-
-from quickstats.utils.io import VerbosePrint
+from .io import VerbosePrint
 
 class AbstractObject(object):
     
-    stdout = quickstats._PRINT_
+    stdout = VerbosePrint("INFO")
     
     @property
     def debug_mode(self):
         return self.stdout._verbosity._name_ == "DEBUG"
     
-    def __init__(self, verbosity:Optional[Union[int, str]]=None, **kwargs):
+    def __init__(self, verbosity:Optional[Union[int, str]]="INFO", **kwargs):
         
         if verbosity is None:
-            self.stdout = quickstats._PRINT_
+            self.stdout = AbstractObject.stdout
         else:
             self.stdout = VerbosePrint(verbosity)
         
     def set_verbosity(self, verbosity:Optional[Union[int, str]]):
         """
             Change the verbosity of the current class. This will detach the class's standard output 
             from the centrally-managed standard output.
```

### Comparing `quickstats-0.6.8.9/quickstats/core/configs.py` & `quickstats-0.6.9.0/quickstats/core/configs.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/core/configurable_object.py` & `quickstats-0.6.9.0/quickstats/core/configurable_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/core/dataclass_object.py` & `quickstats-0.6.9.0/quickstats/core/dataclass_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/core/methods.py` & `quickstats-0.6.9.0/quickstats/core/methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         custom_list = False
     elif isinstance(macros, str):
         from quickstats.utils.string_utils import split_str
         macros = split_str(macros, sep=',', remove_empty=True)
     from quickstats.utils.root_utils import compile_macro
     for macro in macros:
         if ((macro == "FlexibleInterpVarMkII") and (quickstats.root_version >= (6, 26, 0))) and (not custom_list):
-            quickstats._PRINT_.info("INFO: Skip compiling macro \"FlexibleInterpVarMkII\" which is "
+            quickstats.stdout.info("INFO: Skip compiling macro \"FlexibleInterpVarMkII\" which is "
                                     "deprecated since ROOT 6.26/00")
             continue
         compile_macro(macro)
         
 def get_all_macros():
     """
     Get the list of macros names
@@ -43,15 +43,15 @@
         macro_name = os.path.basename(macro_subdir)
         macro_path = os.path.join(macro_subdir, f"{macro_name}.cxx")
         if os.path.exists(macro_path):
             macro_names.append(macro_name)
     return macro_names
 
 def set_verbosity(verbosity:Union[str, int]="INFO"):
-    quickstats._PRINT_.verbosity = verbosity
+    quickstats.stdout.verbosity = verbosity
     
 def get_root_version():
     from quickstats.root_checker import ROOTChecker, ROOTVersion
     try:
         root_config_cmd = ROOTChecker.get_root_config_cmd()
         root_version = ROOTChecker.get_installed_root_version(root_config_cmd)
     except:
@@ -88,49 +88,49 @@
     macro_path = quickstats.macro_path
     if copy_files:
         dest_path = os.path.join(macro_path, name)
         if os.path.exists(dest_path):
             if force or input(f'WARNING: The macro already exists in {dest_path}, overwrite? [Y/N]') == "Y":
                 shutil.rmtree(dest_path)
                 shutil.copytree(path, dest_path)
-                quickstats._PRINT_.info(f'INFO: Overwritten contents for the macro "{name}" from {path} to {dest_path}.')
+                quickstats.stdout.info(f'INFO: Overwritten contents for the macro "{name}" from {path} to {dest_path}.')
             else:
-                quickstats._PRINT_.info(f'INFO: Overwrite cancelled.')
+                quickstats.stdout.info(f'INFO: Overwrite cancelled.')
         else:
             shutil.copytree(path, dest_path)
-            quickstats._PRINT_.info(f'INFO: Copied contents for the macro "{name}" from {path} to {dest_path}.')
+            quickstats.stdout.info(f'INFO: Copied contents for the macro "{name}" from {path} to {dest_path}.')
     if workspace_extension:
         resource_path = quickstats.resource_path
         extension_config_file = os.path.join(resource_path, "workspace_extensions.json")
         extension_config = get_workspace_extension_config()
         if name not in extension_config['required']:
             extension_config['required'].append(name)
             with open(extension_config_file, "w") as file:
                 json.dump(extension_config, file, indent=2)
-        quickstats._PRINT_.info(f'INFO: The macro "{name}" has been added to the workspace extension list.')
+        quickstats.stdout.info(f'INFO: The macro "{name}" has been added to the workspace extension list.')
         
 def remove_macro(name:str, remove_files:bool=True, force:bool=False):
     resource_path = quickstats.resource_path
     extension_config_file = os.path.join(resource_path, "workspace_extensions.json")
     extension_config = get_workspace_extension_config()
     if (name not in extension_config):
-        quickstats._PRINT_.info(f'WARNING: Extension "{name}" not found in the workspace extension list. Skipped.')
+        quickstats.stdout.info(f'WARNING: Extension "{name}" not found in the workspace extension list. Skipped.')
     else:
         extension_config.remove(name)
         with open(extension_config_file, "w") as file:
             json.dump(extension_config, file, indent=2)
-        quickstats._PRINT_.info(f'INFO: The extension "{name}" has been removed from the workspace extension list.')
+        quickstats.stdout.info(f'INFO: The extension "{name}" has been removed from the workspace extension list.')
     if remove_files:
         macro_path = quickstats.macro_path
         extension_path = os.path.abspath(os.path.join(macro_path, name))
         if force or input(f'WARNING: Attempting to remove files from {extension_path}, confirm? [Y/N]') == "Y":
-            quickstats._PRINT_.info(f'INFO: Files for the macro "{name}" has been removed from {extension_path}.')
+            quickstats.stdout.info(f'INFO: Files for the macro "{name}" has been removed from {extension_path}.')
             shutil.rmtree(extension_path)
         else:
-            quickstats._PRINT_.info(f'INFO: Macro files removal cancelled.')
+            quickstats.stdout.info(f'INFO: Macro files removal cancelled.')
 
 def load_corelib():
     if not quickstats.corelib_loaded:
         from quickstats.utils.root_utils import load_macro
         load_macro("QuickStatsCore")
         quickstats.corelib_loaded = True
```

### Comparing `quickstats-0.6.8.9/quickstats/core/path_manager.py` & `quickstats-0.6.9.0/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/core/virtual_trees.py` & `quickstats-0.6.9.0/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/cppyy/core.py` & `quickstats-0.6.9.0/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/cppyy/macros.py` & `quickstats-0.6.9.0/quickstats/interface/cppyy/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.6.9.0/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/RooAbsData.py` & `quickstats-0.6.9.0/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/RooAbsPdf.py` & `quickstats-0.6.9.0/quickstats/interface/root/RooAbsPdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/RooCategory.py` & `quickstats-0.6.9.0/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/RooDataSet.py` & `quickstats-0.6.9.0/quickstats/interface/root/RooDataSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/RooMsgService.py` & `quickstats-0.6.9.0/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/RooRealVar.py` & `quickstats-0.6.9.0/quickstats/interface/root/RooRealVar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/TF1.py` & `quickstats-0.6.9.0/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/TFile.py` & `quickstats-0.6.9.0/quickstats/interface/root/TFile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/TH1.py` & `quickstats-0.6.9.0/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/TH2.py` & `quickstats-0.6.9.0/quickstats/interface/root/TH2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/TObject.py` & `quickstats-0.6.9.0/quickstats/interface/root/TObject.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/__init__.py` & `quickstats-0.6.9.0/quickstats/interface/root/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/helper.py` & `quickstats-0.6.9.0/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/inspection.py` & `quickstats-0.6.9.0/quickstats/interface/root/inspection.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/macros.py` & `quickstats-0.6.9.0/quickstats/interface/root/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/interface/root/roofit_extension.py` & `quickstats-0.6.9.0/quickstats/interface/root/roofit_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Dict, List, Union
 
 import numpy as np
 
 from quickstats.interface.cppyy.vectorize import list2vec, as_np_array
-from quickstats import _PRINT_
+from quickstats import stdout
 
 def unfold_constraints(constraint_pdfs:"ROOT.RooArgSet", observables:"ROOT.RooArgSet",
                        nuisance_parameters:"ROOT.RooArgSet", constraint_cls:Optional[List[str]]=None,
                        recursion_limit:int=50, strip_disconnected:bool=False):
     import ROOT
     result = ROOT.RooArgSet()
     if constraint_cls is None:
@@ -95,22 +95,22 @@
                 target_component = components.first()
         else:
             for nuis in nuisance_parameters:
                 if pdf.dependsOn(nuis):
                     target_component = nuis
                     break
         if not target_component:
-            _PRINT_.warning(f'WARNING: Could not find base component for the constraint: {pdf_name}')
+            stdout.warning(f'WARNING: Could not find base component for the constraint: {pdf_name}')
             continue
         for glob in global_observables:
             if pdf.dependsOn(glob):
                 target_glob = glob
                 break
         if not target_glob:
-            _PRINT_.warning(f'WARNING: Could not find global observable for the constraint: {pdf_name}')
+            stdout.warning(f'WARNING: Could not find global observable for the constraint: {pdf_name}')
             continue
         paired_pdfs.add(pdf)
         paired_component.add(target_component)
         paired_globs.add(target_glob)
         
     return convert_argsets(paired_pdfs, paired_component, paired_globs, fmt=fmt, to_str=to_str)
```

### Comparing `quickstats-0.6.8.9/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.6.9.0/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.6.9.0/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.6.9.0/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.6.9.0/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.6.9.0/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #include <map>
 #include <string>
 
 #include "RooDataSet.h"
 #include "RooAbsPdf.h"
 
 #include "RooFitExt.cxx"
+#include "QStringUtils.cxx"
 
 #ifdef __CINT__
 
 #pragma link off all functions;
 #pragma link off all globals;
 #pragma link off all classes;
```

### Comparing `quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.6.9.0/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.6.9.0/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.6.9.0/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.6.9.0/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.6.9.0/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.6.9.0/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/maths/interpolation.py` & `quickstats-0.6.9.0/quickstats/maths/interpolation.py`

 * *Files 26% similar despite different names*

```diff
@@ -48,8 +48,16 @@
     diff = interp_y1 - y2 
     # determines what index intersection points are at 
     idx = np.argwhere(np.diff(np.sign(diff))).flatten()
 
     #linear interpolation to get exact intercepts: x = x1 + (x2-x1)/(y2-y1) * (y-y1)
     #y = 0 -> x = x1 - (x2-x1)/(y2-y1) * y1
     intersections = [x2[i] - (x2[i + 1] - x2[i])/(diff[i + 1] - diff[i]) * diff[i] for i in idx]
-    return intersections
+    return intersections
+
+def interpolate_2d(x:np.ndarray, y:np.ndarray, z:np.ndarray, method:str='cubic', n:int=500):
+    from scipy import interpolate
+    mask = ~np.isnan(z)
+    x, y, z = x[mask], y[mask], z[mask]
+    X, Y = get_regular_meshgrid(x, y, n=n)
+    Z = interpolate.griddata(np.stack((x, y), axis=1), z, (X, Y), method)
+    return X, Y, Z
```

### Comparing `quickstats-0.6.8.9/quickstats/maths/numerics.py` & `quickstats-0.6.9.0/quickstats/maths/numerics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Any, List, Dict, Optional
+from typing import Union, Any, List, Dict, Optional, Tuple
 from fractions import Fraction
 
 import numpy as np
 
 def pretty_float(val:Union[str, float])->Union[int, float]:
     if float(val).is_integer():
         return int(float(val))
@@ -158,14 +158,25 @@
         if not np.all(ranges[:, 1] >= reference_value):
             raise ValueError("maximum range is smaller than the nominal value")
     if no_overlap:
         if not np.all(np.diff(ranges.flatten()) >= 0):
             raise ValueError("found overlap ranges")
     return ranges
 
+def get_rmin_rmax(range:Tuple[float], require_finite:bool=True):
+    try:
+        rmin, rmax = range
+    except:
+        raise RuntimeError('range must be convertible to a 2-tuple of the form (rmin, rmax)')
+    if rmin > rmax:
+        raise ValueError('max range must be larger than min range')
+    if require_finite and (not (np.isfinite(rmin) and np.isfinite(rmax))):
+        raise ValueError(f'supplied range of [{rmin}, {rmax}] is not finite')
+    return rmin, rmax
+
 def get_batch_slice_indices(totalsize:int, batchsize:int):
     assert (totalsize > 0) and (batchsize > 0)
     for i in range(0, totalsize, batchsize):
         yield (i, min(i + batchsize, totalsize))
         
 def safe_div(dividend, divisor, usenan:bool=False):
     out = np.full(dividend.shape, np.nan) if usenan else np.zeros_like(dividend)
```

### Comparing `quickstats-0.6.8.9/quickstats/maths/statistics.py` & `quickstats-0.6.9.0/quickstats/maths/statistics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/maths/statistics_jitted.py` & `quickstats-0.6.9.0/quickstats/maths/statistics_jitted.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/maths/symbolics.py` & `quickstats-0.6.9.0/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/parsers/param_parser.py` & `quickstats-0.6.9.0/quickstats/parsers/param_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/__init__.py` & `quickstats-0.6.9.0/quickstats/plots/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from .collective_data_plot import CollectiveDataPlot
 from .stat_plot_config import *
 from .hypotest_inverter_plot import HypoTestInverterPlot
 from .variable_distribution_plot import VariableDistributionPlot
 from .score_distribution_plot import score_distribution_plot, score_distribution_plot_2D, ScoreDistributionPlot
 from .test_statistic_distribution_plot import TestStatisticDistributionPlot
 from .general_1D_plot import General1DPlot
+from .general_2D_plot import General2DPlot
 from .upper_limit_1D_plot import UpperLimit1DPlot
 from .upper_limit_2D_plot import UpperLimit2DPlot
 from .upper_limit_3D_plot import UpperLimit3DPlot
 from .upper_limit_benchmark_plot import UpperLimitBenchmarkPlot
 from .likelihood_1D_plot import Likelihood1DPlot
 from .likelihood_2D_plot import Likelihood2DPlot
 from .pdf_distribution_plot import PdfDistributionPlot
 from .correlation_plot import CorrelationPlot
-from .histo_1D_plot import Histo1DPlot
 from .sample_purity_plot import SamplePurityPlot
 from .bidirectional_bar_chart import BidirectionalBarChart
 
 from matplotlib import style, colors
 
 # Reference from https://github.com/beojan/atlas-mpl
```

### Comparing `quickstats-0.6.8.9/quickstats/plots/abstract_plot.py` & `quickstats-0.6.9.0/quickstats/plots/abstract_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.6.9.0/quickstats/plots/bidirectional_bar_chart.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/collective_data_plot.py` & `quickstats-0.6.9.0/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/color_schemes.py` & `quickstats-0.6.9.0/quickstats/plots/color_schemes.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/core.py` & `quickstats-0.6.9.0/quickstats/plots/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/correlation_plot.py` & `quickstats-0.6.9.0/quickstats/plots/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/general_1D_plot.py` & `quickstats-0.6.9.0/quickstats/plots/general_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/general_distribution_plot.py` & `quickstats-0.6.9.0/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.6.9.0/quickstats/plots/hypotest_inverter_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.6.9.0/quickstats/plots/likelihood_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.6.9.0/quickstats/plots/likelihood_2D_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 from quickstats.utils.string_utils import remove_neg_zero
 from quickstats.maths.interpolation import get_regular_meshgrid
 from matplotlib.lines import Line2D
 from matplotlib.patches import Polygon
 
 
 class Likelihood2DPlot(AbstractPlot):
+    
+    STYLES = {
+        'contour': {
+            'linestyles': 'solid',
+            'linewidths': 3            
+        }
+    }
 
     CONFIG = {
         # intervals to include in the plot
         "interval_formats": {
             "68_95"               : ('0.68', '0.95'),
             "one_two_sigma"       : ('1sigma', '2sigma'),
             "68_95_99"            : ('0.68', '0.95', '0.99'),
@@ -32,18 +39,14 @@
             'markeredgecolor': 'black'
         },
         'bestfit_styles':{
             'marker': 'P',
             'linewidth': 0,
             'markersize': 15
         },
-        'contour_styles': {
-            'linestyles': 'solid',
-            'linewidths': 3
-        },
         'legend_label': '{sigma_label}',
         'bestfit_label': 'Best fit ({x:.2f}, {y:.2f})',
         'polygon_label': "Nan NLL region",
         'cmap': 'GnBu',
         'interpolation': 'cubic',
         'num_grid_points': 500,
         'alphashape_alpha': 2,
@@ -169,14 +172,15 @@
             Z = interpolate.griddata(np.stack((x, y), axis=1), z, (X, Y), interpolate_method)
         else:
             X_unique = np.sort(data[xattrib].unique())
             Y_unique = np.sort(data[yattrib].unique())
             X, Y = np.meshgrid(X_unique, Y_unique)
             Z = (data.pivot_table(index=xattrib, columns=yattrib, values=zattrib).T.values
                  - data[zattrib].min())
+            
         if (remove_nan_points_within_distance is not None) or (shade_nan_points):
             nan_shapes = self.get_nan_shapes(data, xattrib, yattrib, zattrib)
         else:
             nan_shapes = None
         if (remove_nan_points_within_distance is not None) and (len(nan_shapes) > 0):
             if len(nan_shapes) > 0:
                 from shapely import Point
@@ -205,23 +209,23 @@
             cmap = config['cmap']
             im = ax.pcolormesh(X, Y, Z, cmap=cmap, shading='auto')
             import matplotlib.pyplot as plt
             self.cbar = plt.colorbar(im, ax=ax, **config['colorbar'])
             self.cbar.set_label(**config['colorbar_label'])
             
         if sigma_values:
-            if 'colors' not in config['contour_styles']:
+            if 'colors' not in self.styles['contour']:
                 cp = ax.contour(X, Y, Z, levels=sigma_values, colors=sigma_colors,
-                                **config['contour_styles'])
+                                **self.styles['contour'])
             else:
-                cp = ax.contour(X, Y, Z, levels=sigma_values, **config['contour_styles'])
+                cp = ax.contour(X, Y, Z, levels=sigma_values, **self.styles['contour'])
             if clabel_size is not None:
                 ax.clabel(cp, inline=True, fontsize=clabel_size)
                 
-        contour_styles = self._get_contour_styles(config['contour_styles'])
+        contour_styles = self._get_contour_styles(self.styles['contour'])
         labels = [config['legend_label'].format(sigma_label=sigma_label) for sigma_label in sigma_labels]
         def line2d_kwargs(color, styles):
             kwargs = combine_dict(styles)
             if 'color' not in kwargs:
                 kwargs['color'] = color
             return kwargs
         custom_handles = [Line2D([0], [0], label=label,
```

### Comparing `quickstats-0.6.8.9/quickstats/plots/np_ranking_plot.py` & `quickstats-0.6.9.0/quickstats/plots/np_ranking_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import matplotlib.transforms as transforms
 from matplotlib.patches import Rectangle
 from matplotlib.backends.backend_pdf import PdfPages
 from quickstats import AbstractObject, semistaticmethod
-from quickstats.utils.process_tools import parallel_run
+from quickstats.utils.common_utils import parallel_run
 from quickstats.plots.template import draw_analysis_label, format_axis_ticks, parse_transform, draw_hatches, \
                                       draw_sigma_bands, draw_sigma_lines, get_box_dimension, draw_text, centralize_axis
 from quickstats.maths.numerics import ceildiv
 from quickstats.utils.common_utils import json_load
 
 BASE_STYLE = {
     'pull': {
```

### Comparing `quickstats-0.6.8.9/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.6.9.0/quickstats/plots/pdf_distribution_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,14 @@
             self.label_map = label_map
         self.colors = {}
         
         self.annotation = None
         
     def set_data(self, collective_data:Dict):
         self.collective_data = collective_data
-        self.legend_order = list(collective_data.keys())
         for name in self.collective_data:
             if name not in self.error_options:
                 self.set_error_options(name)
 
     def get_error_data(self, data):
         xerr = data.get('xerr', None)
         yerr = data.get('yerr', None)
@@ -347,20 +346,20 @@
             ylim[1] = np.max(y)
         ax.set_ylim(ylim)
         
         if vmode == 0:
             centralize_axis(ax, which="y", ref_value=1)
             if draw_ratio_line:
                 ratio_linestyles = self.config['ratio_line_styles']
-                ax.axhline(1, zorder=0, **ratio_linestyles)
+                ax.axhline(1, **ratio_linestyles)
         elif vmode == 1:
             centralize_axis(ax, which="y", ref_value=0)
             if draw_ratio_line:
                 ratio_linestyles = self.config['ratio_line_styles']
-                ax.axhline(0, zorder=0, **ratio_linestyles)
+                ax.axhline(0, **ratio_linestyles)
         if not ylabel:
             if vmode == 0:
                 ylabel = "Fit / Data"
             elif vmode == 1:
                 ylabel = "Fit - Data"
             else:
                 ylabel = ""
@@ -410,51 +409,55 @@
              ypad:Optional[float]=None):
         
         if comparison_options is not None:
             ax, ax_ratio = self.draw_frame(ratio_frames, logx=logx, logy=logy,
                                            **self.styles["ratio_frames"])
         else:
             ax = self.draw_frame(logx=logx, logy=logy)
-
-        for name in self.collective_data:
-            if (targets is not None) and(name not in targets):
-                continue
-            data = self.collective_data[name]
-            label = self.label_map.get(name, name)
-            label_blind = self.label_map.get(f"{name}_blind", None)
-            plot_options = self.plot_options.get(name, {})
-            if (name not in self.error_options) or \
-               (self.error_options[name]["display_format"] is None):
+        
+        if targets is None:
+            targets = list(self.collective_data)
+        if not self.legend_order:
+            self.legend_order = list(targets)
+        for target in targets:
+            if target not in self.collective_data:
+                raise RuntimeError(f'no input found for the target: {target}')
+            data = self.collective_data[target]
+            label = self.label_map.get(target, target)
+            label_blind = self.label_map.get(f"{target}_blind", None)
+            plot_options = self.plot_options.get(target, {})
+            if (target not in self.error_options) or \
+               (self.error_options[target]["display_format"] is None):
                 error_format = None
                 error_styles = None
             else:
-                error_format = self.error_options[name]["display_format"]
-                error_styles = self.error_options[name]["styles"]
+                error_format = self.error_options[target]["display_format"]
+                error_styles = self.error_options[target]["styles"]
             handle = self.draw_single_data(ax, data, label,
                                            label_blind=label_blind,
                                            blind_range=blind_range,
                                            plot_options=plot_options,
                                            show_error=show_error,
                                            error_format=error_format,
                                            error_styles=error_styles,
                                            plot_type=plot_type)
             if not handle.get_children():
-                    self.colors[name] = handle.get_color()
+                    self.colors[target] = handle.get_color()
             else:
                 if plot_type == 'errorbar':
-                    self.colors[name] = handle[0].get_color()
+                    self.colors[target] = handle[0].get_color()
                 elif plot_type == 'hist':
-                    self.colors[name] = handle[0].get_edgecolor()
+                    self.colors[target] = handle[0].get_edgecolor()
             # case draw blind
             if isinstance(handle, list) and len(handle) == 2:
-                blind_name = f"{name}_blind"
-                self.legend_order.append(blind_name)
-                self.update_legend_handles({name: handle[0], blind_name: handle[1]})
+                blind_target = f"{target}_blind"
+                self.legend_order.append(blind_target)
+                self.update_legend_handles({target: handle[0], blind_target: handle[1]})
             else:
-                self.update_legend_handles({name: handle})
+                self.update_legend_handles({target: handle})
 
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
         self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax, ypad=ypad)  
         handles, labels = self.get_legend_handles_labels()
         ax.legend(handles, labels, **self.styles['legend'])
         
         if comparison_options is not None:
```

### Comparing `quickstats-0.6.8.9/quickstats/plots/sample_purity_plot.py` & `quickstats-0.6.9.0/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/score_distribution_plot.py` & `quickstats-0.6.9.0/quickstats/plots/score_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/stat_plot_config.py` & `quickstats-0.6.9.0/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/template.py` & `quickstats-0.6.9.0/quickstats/plots/template.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import re
 from cycler import cycler
 from contextlib import contextmanager
 
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.transforms as transforms
-from matplotlib.patches import Rectangle
+from matplotlib.patches import Rectangle, Polygon
+from matplotlib.collections import PolyCollection
 from matplotlib.lines import Line2D
 from matplotlib.ticker import (MultipleLocator, FormatStrFormatter,
                                AutoMinorLocator, ScalarFormatter,
                                Locator, Formatter, AutoLocator,
                                MaxNLocator)
 
 from quickstats.utils.common_utils import update_nested_dict
@@ -60,14 +61,24 @@
             'major_width': 2,
             'minor_width': 1,
             'spine_width': 2,
             'labelsize': 20,
             'offsetlabelsize': 20,
             'tick_bothsides': True
         },
+        'cbar_axis': {
+            'labelsize': 20,
+            'y_axis_styles': {
+                'labelleft': False,
+                'labelright': True,
+                'left': False,
+                'right': True,
+                'direction': 'out'
+            }
+        },
         'xtick':{
             'format': 'numeric',
             'locator': 'auto',
             'steps': None,
             'prune': None,
             'integer': False
         },
@@ -116,14 +127,18 @@
             'height_ratios': (3, 1),
             'hspace': 0.07            
         },
         'barh': {
             'height': 0.5
         },
         'bar': {
+        },
+        'colorbar': {
+            'fraction': 0.15, 
+            'shrink': 1.
         }
     }
 }
 
 ANALYSIS_OPTIONS = {
     'default': {
         'status': 'int',
@@ -405,34 +420,64 @@
     x_max    = axis.get_xlim()[1]
     x_range  = x_max - x_min
     y_values = np.arange(0, height*ymax, 2*height) - height/2
     transform = create_transform(transform_x='axis', transform_y='data')
     for y in y_values:
         axis.add_patch(Rectangle((0, y), 1, 1, **styles, zorder=-1, transform=transform))
 
+special_text_fontstyles = {
+    re.compile(r'\\bolditalic\{(.*?)\}'): {
+        "weight":"bold", "style":"italic"
+    },
+    re.compile(r'\\italic\{(.*?)\}'): {
+        "style":"italic"
+    },
+    re.compile(r'\\bold\{(.*?)\}'): {
+        "weight":"bold"
+    }    
+}
+special_text_regex = re.compile("|".join([f"({regex.pattern.replace('(', '').replace(')', '')})" 
+                                          for regex in special_text_fontstyles.keys()]))
+
 def draw_text(axis, x:float, y:float, s:str,
               transform_x:str='axis',
               transform_y:str='axis',
               **styles):
     with change_axis(axis):
         transform = create_transform(transform_x, transform_y)
-        text = axis.text(x, y, s, transform=transform, **styles)
-        xmin, xmax, ymin, ymax = get_box_dimension(text)
+        components = special_text_regex.split(s)
+        components = [component for component in components if component]
+        xmax = x
+        xmin = None
+        for component in components:
+            if special_text_regex.match(component):
+                for regex, fontstyles in special_text_fontstyles.items():
+                    match = regex.match(component)
+                    if match:
+                        text = axis.text(xmax, y, match.group(1), transform=transform,
+                                         **styles, **fontstyles)
+                        break
+            else:
+                text = axis.text(xmax, y, component, transform=transform, **styles)
+            xmin_, xmax, ymin, ymax = get_box_dimension(text)
+            if xmin is None:
+                xmin = xmin_
     return xmin, xmax, ymin, ymax
 
 @contextmanager
 def change_axis(axis):
     current_axis = plt.gca()
     plt.sca(axis)
     yield
     plt.sca(current_axis)
 
 def draw_analysis_label(axis, loc=(0.05, 0.95), fontsize:float=25, status:str='int',
                         energy:Optional[str]=None, lumi:Optional[str]=None,
-                        colab:str='ATLAS', extra_text:Optional[str]=None, dy:float=0.05,
+                        colab:Optional[str]='ATLAS', main_text:Optional[str]=None,
+                        extra_text:Optional[str]=None, dy:float=0.05, dy_main:float=0.02,
                         transform_x:str='axis', transform_y:str='axis',
                         vertical_align:str='top', horizontal_align:str='left',
                         text_options:Optional[Dict]=None):
     """
     Draw analysis label and additional texts on a given axis.
     
         Parameters
@@ -448,22 +493,29 @@
             automatically to the corresponding built-in status texts
             (see `ResultStatus`).
         energy: (optional) str
             Display text for the Center-of-mass energy. A prefix of "\sqrt{s} = " will be
             automatically appended to the front of the text.
         lumi: (optional) str
             Display text for the luminosity. It will be displayed as is.
-        colab: str
+        colab: (optional) str
             Display text for the collaboration involved in the analysis. It will be
             bolded and italised.
+        main_text: (optional) str
+            Main text to be displayed before the colab text. A new line
+            can be added by adding a double-slash, i.e. "//". Use the "\bolditalic{<text>}"
+            keyword for bold-italic styled text.            
         extra_text: (optional) str
             Extra text to be displayed after energy and luminosity texts. A new line
-            can be added by adding a double-slash, i.e. "//".
+            can be added by adding a double-slash, i.e. "//". Use the "\bolditalic{<text>}"
+            keyword for bold-italic styled text.
         dy: float, default = 0.05
-            Vertical separation between each line of text in the axis coordinates.
+            Vertical separation between each line of the sub-texts in the axis coordinates.
+        dy_main: float, default = 0.02
+            Vertical separation between each line of the main-texts in the axis coordinates.
         transform_x: str, default = 'axis'
             Coordinate transform for the x location of the analysis label.
         transform_y: str, default = 'axis'
             Coordinate transform for the y location of the analysis label.
         vertical_align: str, default = 'top'
             Vertical alignment of the analysis label.
         horizontal_align: str, default = 'top'
@@ -473,29 +525,45 @@
     """
     try:
         status_text = ResultStatus.parse(status).display_text
     except:
         status_text = status
     
     with change_axis(axis):
-        transform = create_transform(transform_x, transform_y)
-        x, y = loc
-        # draw collaboration label
+        xmin, ymin = loc
+        main_texts = []
+        if main_text is not None:
+            main_texts.extend(main_text.split("//"))
+        if colab is not None:
+            # add collaboration and status text
+            colab_text = r"\bolditalic{" + colab + "} " + status_text
+            main_texts.append(colab_text)
+        for text in main_texts:
+            _, _, ymin, _ = draw_text(axis, xmin, ymin, text,
+                                      fontsize=fontsize,
+                                      transform_x=transform_x,
+                                      transform_y=transform_y,
+                                      horizontalalignment=horizontal_align,
+                                      verticalalignment=vertical_align)
+            ymin -= dy_main
+            transform_x, transform_y = 'axis', 'axis'
+        """
         text_colab = axis.text(x, y, colab, fontsize=fontsize, transform=transform,
                                horizontalalignment=horizontal_align,
                                verticalalignment=vertical_align,
                                fontproperties={"weight":"bold", "style":"italic"})
         xmin, xmax, ymin, _ = get_box_dimension(text_colab)
         text_width = xmax - xmin
         dx = text_width / 15
         # draw status label
         text_status = axis.text(xmax + dx, ymin, status_text, fontsize=fontsize,
                                 transform=axis.transAxes,
                                 horizontalalignment='left',
                                 verticalalignment='bottom')
+        """
         
     # draw energy and luminosity labels as well as additional texts
     elumi_text = []
     if energy is not None:
         elumi_text.append(r"$\sqrt{s} = $" + energy )
     if lumi is not None:
         elumi_text.append(lumi)
@@ -508,8 +576,31 @@
     if extra_text is not None:
         all_texts.extend(extra_text.split("//"))
 
     if text_options is None:
         text_options = {}
 
     for text in all_texts:
-        _, _, ymin, _ = draw_text(axis, xmin, ymin - dy, text, **text_options)
+        _, _, ymin, _ = draw_text(axis, xmin, ymin - dy, text, **text_options)
+        
+def remake_handles(handles:List, polygon_to_line:bool=True, fill_border:bool=True):
+    new_handles = []
+    for handle in handles:
+        new_subhandles = []
+        if isinstance(handle, (list, tuple)):
+            subhandles = handle
+        else:
+            subhandles = [handle]
+        for subhandle in subhandles:
+            if (polygon_to_line) and isinstance(subhandle, Polygon):
+                subhandle = Line2D([], [], c=subhandle.get_edgecolor())
+            new_subhandles.append(subhandle)
+            if fill_border and isinstance(subhandle, PolyCollection):
+                border_handle = Rectangle((0, 0), 1, 1, facecolor='none',
+                                          edgecolor='black', linewidth=1)
+                new_subhandles.append(border_handle)
+        if len(new_subhandles) == 1:
+            new_subhandles = new_subhandles[0]
+        else:
+            new_subhandles = tuple(new_subhandles)
+        new_handles.append(new_subhandles)
+    return new_handles
```

### Comparing `quickstats-0.6.8.9/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.6.9.0/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.6.9.0/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.6.9.0/quickstats/plots/upper_limit_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/upper_limit_2D_plot_deprecated.py` & `quickstats-0.6.9.0/quickstats/plots/upper_limit_2D_plot_deprecated.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.6.9.0/quickstats/plots/upper_limit_3D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.6.9.0/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Optional, Union, Dict, List, Callable, Sequence
 
 from matplotlib.lines import Line2D
 from matplotlib.container import ErrorbarContainer
 from matplotlib.legend_handler import HandlerErrorbar
+from matplotlib.patches import Polygon
 import numpy as np
 import pandas as pd
 
-from quickstats.plots.template import single_frame, ratio_frames
+from quickstats.plots.template import single_frame, ratio_frames, create_transform, remake_handles
 from quickstats.plots import AbstractPlot
 from quickstats.utils.common_utils import combine_dict
 from quickstats.maths.statistics import HistComparisonMode
 
 class UpperLimitBenchmarkPlot(AbstractPlot):
     
     STYLES = {
@@ -27,44 +28,50 @@
             'marker': 'o',
             'capsize': 0.0,
             'markersize': 8
         }
     }
     
     COLOR_PALLETE = {
-        '2sigma': 'hh:darkyellow',
-        '1sigma': 'hh:lightturquoise',
-        'expected': 'k',
-        'observed': 'k',
+        '2sigma'     : 'hh:darkyellow',
+        '1sigma'     : 'hh:lightturquoise',
+        'expected'   : 'k',
+        'observed'   : 'k',
+        'theory'     : 'darkred',
+        'theory_unc' : 'hh:darkpink'
     }
     
     COLOR_PALLETE_EXTRA = {
         '2sigma': '#ffcc00',
         '1sigma': '#00cc00',
         'expected': 'r',
         'observed': 'r',
     }
     
     LABELS = {
         '2sigma': r'Expected limit $\pm 2\sigma$',
         '1sigma': r'Expected limit $\pm 1\sigma$',
         'expected': r'Expected limit (95% CL)',
         'observed': r'Observed limit (95% CL)',
+        'theory'  : r'Theory prediction'
     }
     
     LABELS_EXTRA = {
         '2sigma': r'Alt. Expected limit $\pm 2\sigma$',
         '1sigma': r'Alt. Expected limit $\pm 1\sigma$',
         'expected': r'Alt. Expected limit (95% CL)',
         'observed': r'Alt. Observed limit (95% CL)',
     }
 
     CONFIG = {     
         'xmargin': 0.3,
         'sigma_width': 0.6,
+        'hide_shaded_data': True,
+        'shade_main_panel': True,
+        'shade_comparison_panel': False        
     }
     
     CUSTOM_STYLES = {
         '2sigma': {
             'alpha': 1
         },
         '1sigma': {
@@ -76,14 +83,27 @@
             'markerfacecolor': 'None',
             'marker': 'o'
         },
         'observed': {
             'elinestyle': 'None',
             'elinewidth': 1,
             'marker': 'o'
+        },
+        'theory': {
+            'elinestyle': 'None',
+            'elinewidth': 1,            
+            'marker': 'P'
+        },
+        'theory_unc': {
+            'alpha': 1
+        },
+        'shade': {
+            'hatch': '/',
+            'alpha': 0.5,
+            'color': 'gray'
         }
     }
         
     CUSTOM_STYLES_EXTRA = {
         '2sigma': {
             'alpha': 1
         },
@@ -96,14 +116,19 @@
             'markerfacecolor': 'None',
             'marker': '^'
         },
         'observed': {
             'elinestyle': 'None',
             'elinewidth': 1,
             'marker': '^'
+        },
+        'shade': {
+            'hatch': '\\',
+            'alpha': 0.5,
+            'color': 'gray'
         }
     }
     
     @property
     def theory_func(self):
         return self._theory_func    
     
@@ -143,15 +168,15 @@
             raise RuntimeError('key can not be None')
         self.alt_data[key] = data
         self.alt_color_pallete[key] = combine_dict(self.COLOR_PALLETE_EXTRA, color_pallete)
         self.alt_labels[key] = combine_dict(self.LABELS_EXTRA, labels)
         self.alt_custom_styles[key] = combine_dict(self.CUSTOM_STYLES_EXTRA, custom_styles)
         
     def get_default_legend_order(self):
-        return ['observed', 'expected', '1sigma', '2sigma']
+        return ['observed', 'expected', '1sigma', '2sigma', 'theory']
     
     def set_theory_function(self, func:Optional[Callable]=None):
         if func is None:
             self._theory_func = None
             return
         if not isinstance(func, Callable):
             raise TypeError('theory function must be callable')
@@ -185,60 +210,76 @@
             h = ax.axhline(data['y'], label=data['label'], **data['styles'])
             self.update_legend_handles({data['label']: h})
             
     def draw_single_data(self, ax, data:pd.DataFrame,
                          color_pallete:Dict,
                          labels:Dict,
                          custom_styles:Dict,
+                         shade_index:Optional[List[int]]=None,
                          data_key:Optional[str]=None,
                          draw_expected:bool=True,
                          draw_observed:bool=True,
                          draw_errorband:bool=True,
                          update_handle:bool=True):
+        if shade_index is None:
+            shade_index = []
+        hide_shaded = self.config['hide_shaded_data']
         df = data
         nbenchmark = len(df.index)
         eps = self.config['sigma_width'] / 2
         handle_keys = {}
         for handle_type in ['expected', 'observed', '1sigma', '2sigma']:
             handle_keys[handle_type] = handle_type if data_key is None else f"{handle_type}_{data_key}"
         for index, (benchmark, limit) in enumerate(df.iterrows()):
+            if (index in shade_index) and (hide_shaded):
+                continue
             if draw_errorband:
                 h_2sigma = ax.fill_between([index - eps, index + eps], limit['-2'] , limit['2'],
                                            facecolor=color_pallete['2sigma'],
                                            label=labels['2sigma'],
                                            **custom_styles['2sigma'])
                 h_1sigma = ax.fill_between([index - eps, index + eps], limit['-1'], limit['1'],
                                            facecolor=color_pallete['1sigma'],
                                            label=labels['1sigma'],
                                            **custom_styles['1sigma'])
                 if update_handle:
                     self.update_legend_handles({handle_keys['2sigma']: h_2sigma,
                                                 handle_keys['1sigma']: h_1sigma})
         x = np.arange(nbenchmark)
+        if hide_shaded:
+            x = np.delete(x, shade_index)
         for flag, column, key in [(draw_expected, '0', 'expected'),
                                   (draw_observed, 'obs', 'observed')]:
             if not flag:
                 continue
             styles = combine_dict(self.styles['errorbar'], custom_styles[key])
             # overwrite marker and errorbar colors
             for color_key in ['markerfacecolor', 'markeredgecolor', 'ecolor']:
                 if color_key not in styles:
                     styles[color_key] = color_pallete[key]
             # overwrite the errorbar linestyle
             elinestyle = styles.pop('elinestyle', None)
+            y = df[column].values[x]
             if elinestyle in ['None', 'none', None]:
-                handle = ax.errorbar(x=x, y=df[column],
+                handle = ax.errorbar(x=x, y=y,
                                      label=labels[key], **styles)
             else:
-                handle = ax.errorbar(x=x, y=df[column], xerr=eps,
+                handle = ax.errorbar(x=x, y=y, xerr=eps,
                                      label=labels[key], **styles)
                 if elinestyle is not None:
                     handle[-1][0].set_linestyle(elinestyle)
             if update_handle:
                 self.update_legend_handles({handle_keys[key]: handle})
+        shade_main_panel = self.config['shade_main_panel']
+        if (shade_index is not None) and (shade_main_panel):
+            for index, (benchmark, limit) in enumerate(df.iterrows()):
+                if index not in shade_index:
+                    continue        
+                ax.fill_between([index - eps, index + eps], limit['-2'] , limit['2'],
+                                **custom_styles['shade'])
             
     def draw_comparison_data(self, ax,
                              reference_data:pd.DataFrame,
                              target_data:pd.DataFrame,
                              color_pallete:Dict,
                              labels:Dict,
                              custom_styles:Dict,
@@ -287,57 +328,124 @@
                          iloc:Optional[List[int]]=None, target:Optional[str]=None):
         if df is None:
             df = self.get_target_df(iloc=iloc, target=target)
         nbenchmark = len(df.index)
         nlevel = df.index.nlevels 
         values = np.array(sum(df.index.values, ())).reshape(nbenchmark, nlevel).T
         theory_scale = self.get_theory_prediction(*values)[-3]
+        theory_errlo = self.get_theory_prediction(*values)[-2]
+        theory_errhi = self.get_theory_prediction(*values)[-1]
         df_theory = df.drop(columns=df.columns)
         df_theory['theory_scale'] = theory_scale
+        df_theory['theory_errlo'] = theory_errlo
+        df_theory['theory_errhi'] = theory_errhi
         return df_theory
     
     def get_target_df(self, iloc:Optional[List[int]]=None, target:Optional[str]=None):
         if target is None:
             df = self.data.copy()
         else:
             df = self.alt_data[target].copy()
         if iloc is not None:
-            df = df[iloc]
+            df = df.iloc[iloc]
         return df
     
-    def draw(self, iloc:Optional[List[int]]=None, xticklabels:Optional[List[str]]=None,
+    def draw_theory_points(self, ax, df:Optional[pd.DataFrame]=None,
+                           iloc:Optional[List[int]]=None,
+                           target:Optional[str]=None,
+                           shade_index:Optional[List[int]]=None,
+                           styles:Optional[Dict]=None,
+                           color:Optional[str]=None,
+                           unc_styles:Optional[Dict]=None,
+                           unc_color:Optional[str]=None,
+                           label:Optional[str]=None):
+        if styles is None:
+            styles = combine_dict(self.CUSTOM_STYLES['theory'])
+        if color is None:
+            color = self.COLOR_PALLETE['theory']
+        if unc_styles is None:
+            unc_styles = combine_dict(self.CUSTOM_STYLES['theory_unc'])
+        if unc_color is None:
+            unc_color = self.COLOR_PALLETE['theory_unc']
+        if label is None:
+            label = self.LABELS['theory']
+        if shade_index is None:
+            shade_index = []
+        df_theory = self.get_theory_scale(df=df, iloc=iloc, target=target)
+        nbenchmark = len(df_theory.index)
+        eps = self.config['sigma_width'] / 2
+        x = np.arange(nbenchmark)
+        hide_shaded = self.config['hide_shaded_data']
+        if hide_shaded:
+            x = np.delete(x, shade_index)
+        styles = combine_dict(self.styles['errorbar'], styles)
+        unc_styles = combine_dict(unc_styles)
+        # overwrite marker and errorbar colors
+        for color_key in ['markerfacecolor', 'markeredgecolor', 'ecolor']:
+            if color_key not in styles:
+                styles[color_key] = color
+        # overwrite the errorbar linestyle
+        elinestyle = styles.pop('elinestyle', None)
+        y = df_theory['theory_scale'].values[x]
+        yerrlo = df_theory['theory_errlo'].values[x]
+        yerrhi = df_theory['theory_errhi'].values[x]
+        # draw errorbands
+        handle_fill = None
+        if (yerrlo[0] is not None) or (yerrhi[0] is not None):
+            unc_styles['color'] = unc_color
+            for x_i, yerrlo_i, yerrhi_i in zip(x, yerrlo, yerrhi):
+                handle_fill = ax.fill_between([x_i - eps, x_i + eps], yerrlo_i , yerrhi_i,
+                                              label=label, **unc_styles)
+        # draw values
+        if elinestyle in ['None', 'none', None]:
+            handle_line = ax.errorbar(x=x, y=y, label=label, **styles)
+        else:
+            handle_line = ax.errorbar(x=x, y=y, xerr=eps,
+                                      label=label, **styles)
+            if elinestyle is not None:
+                handle_line[-1][0].set_linestyle(elinestyle)
+        if handle_fill is None:
+            handle = handle_line
+        else:
+            handle = (handle_fill, handle_line)
+        self.update_legend_handles({'theory': handle})
+    
+    def draw(self, iloc:Optional[List[int]]=None,
+             shade_index:Optional[List[int]]=None,
+             xticklabels:Optional[List[str]]=None,
              logy:bool=False, xlabel:str="", ylabel:str="", ylim=None,
              scale_theory:bool=False, draw_expected:bool=True,
              draw_observed:bool=True, draw_errorband:bool=True,
+             draw_theory:bool=False,
              alt_draw_options:Optional[Dict]=None,
              comparison_options:Optional[Dict]=None):
         # setup input data
         targets = [None]
         if alt_draw_options is not None:
             targets.extend(list(alt_draw_options.keys()))
         target_kwargs = {}
         nbenchmark = None
         for target in targets:
             target_kwargs[target] = {}
             df = self.get_target_df(iloc=iloc, target=target)
             if target is None:
-                target_kwargs[target]['color_pallete'] = self.color_pallete
-                target_kwargs[target]['labels'] = self.labels
-                target_kwargs[target]['custom_styles'] = self.custom_styles
-                target_kwargs[target]['draw_expected'] = draw_expected
-                target_kwargs[target]['draw_observed'] = draw_observed
+                target_kwargs[target]['color_pallete']  = self.color_pallete
+                target_kwargs[target]['labels']         = self.labels
+                target_kwargs[target]['custom_styles']  = self.custom_styles
+                target_kwargs[target]['draw_expected']  = draw_expected
+                target_kwargs[target]['draw_observed']  = draw_observed
                 target_kwargs[target]['draw_errorband'] = draw_errorband
                 target_scale_theory = scale_theory
             else:
                 draw_options = alt_draw_options[target]
-                target_kwargs[target]['color_pallete'] = self.alt_color_pallete[target]
-                target_kwargs[target]['labels'] = self.alt_labels[target]
-                target_kwargs[target]['custom_styles'] = self.alt_custom_styles[target] 
-                target_kwargs[target]['draw_expected'] = draw_options.get('draw_expected', draw_expected)
-                target_kwargs[target]['draw_observed'] = draw_options.get('draw_observed', draw_observed)
+                target_kwargs[target]['color_pallete']  = self.alt_color_pallete[target]
+                target_kwargs[target]['labels']         = self.alt_labels[target]
+                target_kwargs[target]['custom_styles']  = self.alt_custom_styles[target] 
+                target_kwargs[target]['draw_expected']  = draw_options.get('draw_expected', draw_expected)
+                target_kwargs[target]['draw_observed']  = draw_options.get('draw_observed', draw_observed)
                 target_kwargs[target]['draw_errorband'] = draw_options.get('draw_errorband', draw_errorband)
                 target_scale_theory = draw_options.get('scale_theory', scale_theory)
             if nbenchmark is None:
                 nbenchmark = len(df.index)
             elif len(df.index) != nbenchmark:
                 RuntimeError(f'main and alternative data ("{target}") have different number of benchmark points')
             if target_scale_theory:
@@ -362,15 +470,16 @@
             
         eps = self.config['sigma_width'] / 2
         xmargin = self.config['xmargin']
         xlim = (0 - eps - xmargin, nbenchmark - 1 + eps + xmargin)
         self.draw_axis_components(ax, ylabel=ylabel, xlabel=xlabel, ylim=ylim, xlim=xlim)
         
         for data_key, kwargs in target_kwargs.items():
-            self.draw_single_data(ax, **kwargs, data_key=data_key)
+            self.draw_single_data(ax, **kwargs, data_key=data_key,
+                                  shade_index=shade_index)
 
         self.draw_hlines(ax)
         
         if comparison_options is not None:
             components = comparison_options.pop('components')
             for component in components:
                 reference = component.pop('reference')
@@ -383,20 +492,41 @@
                 self.draw_comparison_data(ax_ratio,
                                           target_kwargs[reference]['data'],
                                           target_kwargs[target]['data'],
                                           **kwargs)
             comparison_options['xlabel'] = ax.get_xlabel()
             self.decorate_comparison_axis(ax_ratio, **comparison_options)
             ax.set(xlabel=None)
-            ax.tick_params(axis="x", labelbottom=False)        
-        
+            ax.tick_params(axis="x", labelbottom=False)
+            
+            shade_comparison_panel = self.config['shade_comparison_panel']
+            if (shade_index is not None) and shade_comparison_panel:
+                transform = create_transform(transform_x='data', transform_y='axis')
+                fill_styles = target_kwargs[None]['custom_styles']['shade']
+                for index in shade_index:
+                    ax_ratio.fill_between([index - eps, index + eps], 0, 1,
+                                          **fill_styles,
+                                          transform=transform)
+        if draw_theory:
+            theory_styles = target_kwargs[None]['custom_styles']['theory']
+            theory_label  = target_kwargs[None]['labels']['theory']
+            theory_color  = target_kwargs[None]['color_pallete']['theory']
+            theory_unc_styles = target_kwargs[None]['custom_styles']['theory_unc']
+            theory_unc_color = target_kwargs[None]['color_pallete']['theory_unc']
+            self.draw_theory_points(ax, shade_index=shade_index,
+                                    styles=theory_styles,
+                                    color=theory_color,
+                                    label=theory_label,
+                                    unc_styles=theory_unc_styles,
+                                    unc_color=theory_unc_color)
         ax.set_xticks(np.arange(nbenchmark))
         ax.set_xticklabels(xticklabels)
         
         handles, labels = self.get_legend_handles_labels()
+        handles = remake_handles(handles, polygon_to_line=False, fill_border=True)
         handler_map = {ErrorbarContainer: HandlerErrorbar(xerr_size=1)}
         ax.legend(handles, labels, **self.styles['legend'], handler_map=handler_map)
         
         if comparison_options is not None:
             return ax, ax_ratio
         
         return ax
```

### Comparing `quickstats-0.6.8.9/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.6.9.0/quickstats/plots/variable_distribution_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from matplotlib import colors
 from matplotlib.ticker import MaxNLocator
 from matplotlib.lines import Line2D
 from matplotlib.patches import Polygon
 
 from quickstats.plots import AbstractPlot, get_color_cycle
-from quickstats.plots.template import ratio_frames, centralize_axis
+from quickstats.plots.template import ratio_frames, centralize_axis, remake_handles
 from quickstats.utils.common_utils import combine_dict
 from quickstats.maths.numerics import safe_div
 from quickstats.maths.statistics import (HistComparisonMode,
                                          min_max_to_range, get_hist_data,
                                          get_stacked_hist_data,
                                          get_hist_comparison_data,
                                          get_clipped_data)
@@ -56,15 +56,16 @@
             'linestyle': '--',
             'zorder': 0
         },
         'plot_format': 'hist',
         'error_format': 'shade',
         'error_label_format': r'{label} $\pm \sigma$',
         'show_xerr': True,
-        'stacked_label': ':stacked_{index}:'
+        'stacked_label': ':stacked_{index}:',
+        'box_legend_handle': True
     }
     
     def __init__(self, data_map:Union["pandas.DataFrame", Dict[str, "pandas.DataFrame"]],
                  plot_options:Optional[Dict]=None,
                  label_map:Optional[Dict]=None,
                  color_cycle:Optional[Union[List, str, "ListedColorMap"]]=None,
                  styles:Optional[Union[Dict, str]]=None,
@@ -555,14 +556,17 @@
         
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
         self.set_axis_range(ax, xmin=xmin, xmax=xmax,
                             ymin=ymin, ymax=ymax, ypad=ypad)
                 
         if not self.is_single_data():
             handles, labels = self.get_legend_handles_labels()
+            box_legend_handle = self.config['box_legend_handle']
+            if not box_legend_handle:
+                handles = remake_handles(handles, polygon_to_line=True)
             ax.legend(handles=handles, labels=labels, **self.styles['legend'])
         
         if comparison_options is not None:
             components = comparison_options.pop('components')
             for component in components:
                 reference = component.pop('reference')
                 target    = component.pop('target')
```

### Comparing `quickstats-0.6.8.9/quickstats/root_checker.py` & `quickstats-0.6.9.0/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/utils/common_utils.py` & `quickstats-0.6.9.0/quickstats/utils/common_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,27 +37,14 @@
     else:
         if parallel == -1:
             max_workers = get_cpu_count()
         else:
             max_workers = parallel
         return parallel_run(func, *iterables, max_workers=max_workers)
 
-
-def timer(func):
-    """Print the runtime of the decorated function"""
-    @functools.wraps(func)
-    def wrapper_timer(*args, **kwargs):
-        start_time = time.perf_counter()    # 1
-        value = func(*args, **kwargs)
-        end_time = time.perf_counter()      # 2
-        run_time = end_time - start_time    # 3
-        print('INFO: All jobs have finished. Total time taken: {:.3f} s'.format(run_time))
-        return value
-    return wrapper_timer
-
 def stdout_print(msg):
     sys.__stdout__.write(msg + '\n')
     
 def redirect_stdout(logfile_path):
     import ROOT
     sys.stdout = open(logfile_path, 'w')
     ROOT.gSystem.RedirectOutput(logfile_path)
@@ -103,22 +90,55 @@
         return config
     elif isinstance(source, dict):
         return source
     else:
         raise ValueError("invalid config input")
         
 class NpEncoder(json.JSONEncoder):
+    """
+    Custom JSON Encoder for handling NumPy data types in JSON serialization.
+
+    This custom JSONEncoder subclass is designed to handle NumPy data types 
+    (such as np.integer, np.floating, and np.ndarray) during JSON serialization. 
+    
+    Note:
+        To use this custom encoder, you can pass it as the 'cls' argument when 
+        calling the json.dumps() function or json.dump() method.
+
+    Example:
+        import json
+        import numpy as np
+
+        # Create a dictionary with NumPy data types
+        data = {
+            'integer': np.int64(42),
+            'floating': np.float64(3.14),
+            'array': np.array([1, 2, 3])
+        }
+
+        # Serialize the dictionary using the NpEncoder
+        json_string = json.dumps(data, cls=NpEncoder)
+
+        # Deserialize the JSON string
+        decoded_data = json.loads(json_string)
+
+        # The NumPy data types are now properly serialized and deserialized
+        print(decoded_data['integer'])  # outputs: 42
+        print(decoded_data['floating'])  # outputs: 3.14
+        print(decoded_data['array'])  # outputs: [1, 2, 3]
+    """
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.floating):
             return float(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         return super(NpEncoder, self).default(obj)
+
     
 def update_nested_dict(d:Dict, u:Dict):
     for k, v in u.items():
         if isinstance(d.get(k, None), collections.Mapping) and isinstance(v, collections.Mapping):
             d[k] = update_nested_dict(d[k], v)
         else:
             d[k] = v
```

### Comparing `quickstats-0.6.8.9/quickstats/utils/data_conversion.py` & `quickstats-0.6.9.0/quickstats/utils/data_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
                 for column in batch:
                     if column not in result:
                         result[column] = batch[column]
                     else:
                         result[column] = np.concatenate([result[column], batch[column]])
             return result
         else:
+            import pandas as pd
             result = None
             for batch in results:
                 if downcast:
                     downcast_dataframe(batch)
                 if result is None:
                     result = batch
                 else:
```

### Comparing `quickstats-0.6.8.9/quickstats/utils/hep_utils.py` & `quickstats-0.6.9.0/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/utils/io.py` & `quickstats-0.6.9.0/quickstats/core/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,25 @@
     'bright magenta': '\033[35;1m',
     'bright cyan': '\033[36;1m',
     'bright white': '\033[37;1m',    
     'darkred': '\033[91m',
     'reset': '\033[0m'
 }
 
-def get_colored_text(text:str, color:str):
+def get_colored_text(text: str, color: str) -> str:
+    """
+    Returns the text formatted with the specified color.
+
+    Args:
+        text (str): The text to be colored.
+        color (str): The color to apply to the text. 
+
+    Returns:
+        str: The input text with the specified color formatting.
+    """
     return f"{text_color_map[color]}{text}{text_color_map['reset']}"
 
 def format_comparison_text(text_left:str, text_right:str,
                            equal_color=None, delete_color:str="red", insert_color:str="green"):
     codes = difflib.SequenceMatcher(a=text_left, b=text_right).get_opcodes()
     s_left  = ""
     s_right = ""
```

### Comparing `quickstats-0.6.8.9/quickstats/utils/roofit_utils.py` & `quickstats-0.6.9.0/quickstats/utils/roofit_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/utils/roostats_utils.py` & `quickstats-0.6.9.0/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats/utils/root_utils.py` & `quickstats-0.6.9.0/quickstats/utils/root_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         if isinstance(obj, ROOT.TTree):
             tree_names.append(obj.GetName())
     return tree_names
 
 def merge_root_files(source_files:Union[str, List[str]], target_file:str, treename:str=None,
                      multithread:bool=True, keep_order:bool=False, use_template:bool=True,
                      ignore_missing_columns:bool=True, verbosity:str="INFO"):
-    from quickstats.utils.io import VerbosePrint
+    from quickstats import VerbosePrint
     stdout = VerbosePrint(verbosity)
     
     if isinstance(source_files, str):
         source_files = [source_files]
     rfiles = []
     for source_file in source_files:
         files = glob.glob(source_file)
```

### Comparing `quickstats-0.6.8.9/quickstats/utils/xml_tools.py` & `quickstats-0.6.9.0/quickstats/utils/xml_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.9/quickstats.egg-info/PKG-INFO` & `quickstats-0.6.9.0/quickstats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.8.9
+Version: 0.6.9.0
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.8.9/quickstats.egg-info/SOURCES.txt` & `quickstats-0.6.9.0/quickstats.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 quickstats/core/__init__.py
 quickstats/core/abstract_object.py
 quickstats/core/configs.py
 quickstats/core/configurable_object.py
 quickstats/core/dataclass_object.py
 quickstats/core/decorators.py
 quickstats/core/enums.py
+quickstats/core/io.py
 quickstats/core/methods.py
 quickstats/core/path_manager.py
 quickstats/core/virtual_trees.py
 quickstats/interface/__init__.py
 quickstats/interface/cppyy/__init__.py
 quickstats/interface/cppyy/core.py
 quickstats/interface/cppyy/macros.py
@@ -148,14 +149,15 @@
 quickstats/interface/root/io.py
 quickstats/interface/root/macros.py
 quickstats/interface/root/roofit_extension.py
 quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
 quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
 quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
 quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+quickstats/macros/QuickStatsCore/QStringUtils.cxx
 quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
 quickstats/macros/QuickStatsCore/RooFitExt.cxx
 quickstats/macros/QuickStatsCore/RooFitExt.h
 quickstats/macros/ResponseFunction/ResponseFunction.cxx
 quickstats/macros/ResponseFunction/ResponseFunction.h
 quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
 quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
@@ -172,16 +174,16 @@
 quickstats/plots/abstract_plot.py
 quickstats/plots/bidirectional_bar_chart.py
 quickstats/plots/collective_data_plot.py
 quickstats/plots/color_schemes.py
 quickstats/plots/core.py
 quickstats/plots/correlation_plot.py
 quickstats/plots/general_1D_plot.py
+quickstats/plots/general_2D_plot.py
 quickstats/plots/general_distribution_plot.py
-quickstats/plots/histo_1D_plot.py
 quickstats/plots/hypotest_inverter_plot.py
 quickstats/plots/likelihood_1D_plot.py
 quickstats/plots/likelihood_2D_plot.py
 quickstats/plots/likelihood_scan_plot.py
 quickstats/plots/np_ranking_plot.py
 quickstats/plots/pdf_distribution_plot.py
 quickstats/plots/sample_purity_plot.py
@@ -198,14 +200,12 @@
 quickstats/resources/default_workspace_extensions.json
 quickstats/stylesheets/quick_default.mplstyle
 quickstats/utils/__init__.py
 quickstats/utils/common_utils.py
 quickstats/utils/condor_tasks.py
 quickstats/utils/data_conversion.py
 quickstats/utils/hep_utils.py
-quickstats/utils/io.py
-quickstats/utils/process_tools.py
 quickstats/utils/roofit_utils.py
 quickstats/utils/roostats_utils.py
 quickstats/utils/root_utils.py
 quickstats/utils/string_utils.py
 quickstats/utils/xml_tools.py
```

### Comparing `quickstats-0.6.8.9/setup.py` & `quickstats-0.6.9.0/setup.py`

 * *Files identical despite different names*

