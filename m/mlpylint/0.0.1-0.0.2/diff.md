# Comparing `tmp/mlpylint-0.0.1.tar.gz` & `tmp/mlpylint-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpylint-0.0.1.tar", last modified: Tue Jul 18 19:49:07 2023, max compression
+gzip compressed data, was "mlpylint-0.0.2.tar", last modified: Mon Jul 24 07:43:46 2023, max compression
```

## Comparing `mlpylint-0.0.1.tar` & `mlpylint-0.0.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 19:49:07.824793 mlpylint-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-07-17 17:13:05.000000 mlpylint-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4365 2023-07-18 19:49:07.824793 mlpylint-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3037 2023-07-18 12:17:35.000000 mlpylint-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 19:49:07.724941 mlpylint-0.0.1/mlpylint.egg-info/
--rw-rw-rw-   0        0        0     4365 2023-07-18 19:49:07.000000 mlpylint-0.0.1/mlpylint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4655 2023-07-18 19:49:07.000000 mlpylint-0.0.1/mlpylint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 19:49:07.000000 mlpylint-0.0.1/mlpylint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-18 19:49:07.000000 mlpylint-0.0.1/mlpylint.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 11:54:16.000000 mlpylint-0.0.1/mlpylint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-07-18 19:49:07.000000 mlpylint-0.0.1/mlpylint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 19:49:07.000000 mlpylint-0.0.1/mlpylint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-07-18 11:00:37.000000 mlpylint-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1495 2023-07-18 19:49:07.824793 mlpylint-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 19:49:07.740558 mlpylint-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-07-18 09:26:23.000000 mlpylint-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 19:49:07.740558 mlpylint-0.0.1/src/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-01 22:11:59.000000 mlpylint-0.0.1/src/analysis/__init__.py
--rw-rw-rw-   0        0        0     6936 2023-07-18 09:30:36.000000 mlpylint-0.0.1/src/analysis/argument.py
--rw-rw-rw-   0        0        0      348 2023-06-22 14:08:30.000000 mlpylint-0.0.1/src/analysis/config.py
--rw-rw-rw-   0        0        0     3482 2023-07-18 09:30:36.000000 mlpylint-0.0.1/src/analysis/result.py
--rw-rw-rw-   0        0        0     5415 2023-07-18 10:50:49.000000 mlpylint-0.0.1/src/analysis/runner.py
-drwxrwxrwx   0        0        0        0 2023-07-18 19:49:07.771875 mlpylint-0.0.1/src/checkers/
--rw-rw-rw-   0        0        0        0 2023-04-01 22:14:02.000000 mlpylint-0.0.1/src/checkers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 19:49:07.777907 mlpylint-0.0.1/src/checkers/advice/
--rw-rw-rw-   0        0        0        0 2023-05-07 15:22:41.000000 mlpylint-0.0.1/src/checkers/advice/__init__.py
--rw-rw-rw-   0        0        0     2329 2023-07-18 14:56:02.000000 mlpylint-0.0.1/src/checkers/advice/advice_checker_4_12_memory_not_freed.py
--rw-rw-rw-   0        0        0     2411 2023-07-18 14:56:34.000000 mlpylint-0.0.1/src/checkers/advice/advice_checker_4_16_broadcasting_feature_not_used.py
--rw-rw-rw-   0        0        0     3612 2023-07-18 14:57:06.000000 mlpylint-0.0.1/src/checkers/advice/advice_checker_4_18_training_evaluation_mode_improper_toggling.py
--rw-rw-rw-   0        0        0     3699 2023-07-18 14:55:02.000000 mlpylint-0.0.1/src/checkers/advice/advice_checker_4_1_unnecessary_iteration.py
--rw-rw-rw-   0        0        0     3248 2023-07-18 14:57:31.000000 mlpylint-0.0.1/src/checkers/advice/advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py
--rw-rw-rw-   0        0        0     4286 2023-07-18 14:58:00.000000 mlpylint-0.0.1/src/checkers/advice/advice_checker_4_21_data_leakage.py
--rw-rw-rw-   0        0        0      558 2023-04-28 15:37:23.000000 mlpylint-0.0.1/src/checkers/base_checker.py
--rw-rw-rw-   0        0        0     3682 2023-07-18 15:02:34.000000 mlpylint-0.0.1/src/checkers/checker_4_11_hyperparameter_not_explicitly_set.py
--rw-rw-rw-   0        0        0     3749 2023-07-18 15:03:16.000000 mlpylint-0.0.1/src/checkers/checker_4_13_deterministic_algorithm_option_not_used.py
--rw-rw-rw-   0        0        0    13736 2023-07-18 15:03:55.000000 mlpylint-0.0.1/src/checkers/checker_4_14_randomness_uncontrolled.py
--rw-rw-rw-   0        0        0     5564 2023-07-18 15:04:37.000000 mlpylint-0.0.1/src/checkers/checker_4_15_missing_the_mask_of_invalid_value.py
--rw-rw-rw-   0        0        0     3585 2023-07-18 15:04:59.000000 mlpylint-0.0.1/src/checkers/checker_4_17_tensorarray_not_used.py
--rw-rw-rw-   0        0        0     2526 2023-07-18 15:07:05.000000 mlpylint-0.0.1/src/checkers/checker_4_19_pytorch_call_method_misused.py
--rw-rw-rw-   0        0        0     5162 2023-07-18 14:58:23.000000 mlpylint-0.0.1/src/checkers/checker_4_2_nan_equivalence_comparison_misused.py
--rw-rw-rw-   0        0        0     3341 2023-07-18 14:58:44.000000 mlpylint-0.0.1/src/checkers/checker_4_3_chain_indexing.py
--rw-rw-rw-   0        0        0     3275 2023-07-18 14:59:10.000000 mlpylint-0.0.1/src/checkers/checker_4_4_columns_and_data_type_not_explicitly_set.py
--rw-rw-rw-   0        0        0    11187 2023-07-18 15:00:03.000000 mlpylint-0.0.1/src/checkers/checker_4_5_empty_column_misinitialization.py
--rw-rw-rw-   0        0        0     3677 2023-07-18 15:00:30.000000 mlpylint-0.0.1/src/checkers/checker_4_6_merge_api_parameter_not_explicitly_set.py
--rw-rw-rw-   0        0        0     4202 2023-07-18 15:00:55.000000 mlpylint-0.0.1/src/checkers/checker_4_7_in_place_apis_misused.py
--rw-rw-rw-   0        0        0     2703 2023-07-18 15:01:39.000000 mlpylint-0.0.1/src/checkers/checker_4_8_dataframe_conversion_api_misused.py
--rw-rw-rw-   0        0        0     5903 2023-07-18 15:02:17.000000 mlpylint-0.0.1/src/checkers/checker_4_9_matrix_multiplication_api_misused.py
-drwxrwxrwx   0        0        0        0 2023-07-18 19:49:07.777907 mlpylint-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-04-01 23:33:14.000000 mlpylint-0.0.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 19:49:07.809169 mlpylint-0.0.1/tests/test_checkers/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:23:11.000000 mlpylint-0.0.1/tests/test_checkers/__init__.py
--rw-rw-rw-   0        0        0      780 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_advice_checker_4_16_broadcasting_feature_not_used.py
--rw-rw-rw-   0        0        0      856 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_advice_checker_4_18_training_evaluation_mode_improper_toggling.py
--rw-rw-rw-   0        0        0      741 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_advice_checker_4_1_unnecessary_iteration.py
--rw-rw-rw-   0        0        0      883 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py
--rw-rw-rw-   0        0        0      633 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_advice_checker_4_21_data_leakage.py
--rw-rw-rw-   0        0        0      720 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_11_hyperparameter_not_explicitly_set.py
--rw-rw-rw-   0        0        0      658 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_12_memory_not_freed.py
--rw-rw-rw-   0        0        0      748 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_13_deterministic_algorithm_option_not_used.py
--rw-rw-rw-   0        0        0      674 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_14_randomness_uncontrolled.py
--rw-rw-rw-   0        0        0      716 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_15_missing_the_mask_of_invalid_value.py
--rw-rw-rw-   0        0        0      657 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_17_tensorarray_not_used.py
--rw-rw-rw-   0        0        0      690 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_19_pytorch_call_method_misused.py
--rw-rw-rw-   0        0        0      736 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_2_nan_equivalence_comparison_misused.py
--rw-rw-rw-   0        0        0      626 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_3_chain_indexing.py
--rw-rw-rw-   0        0        0      741 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_4_columns_and_datatype_not_explicitly_set.py
--rw-rw-rw-   0        0        0      704 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_5_empty_column_misinitialization.py
--rw-rw-rw-   0        0        0      738 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_6_merge_api_parameter_not_explicitly_set.py
--rw-rw-rw-   0        0        0      657 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_7_in_place_apis_misused.py
--rw-rw-rw-   0        0        0      712 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_8_dataframe_conversion_api_misused.py
--rw-rw-rw-   0        0        0      717 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_checkers/test_checker_4_9_matrix_multiplication_api_misused.py
-drwxrwxrwx   0        0        0        0 2023-07-18 19:49:07.824793 mlpylint-0.0.1/tests/test_files/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:23:30.000000 mlpylint-0.0.1/tests/test_files/__init__.py
--rw-rw-rw-   0        0        0      291 2023-07-17 12:38:57.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_11_hyperparameter_not_explicitly_set.py
--rw-rw-rw-   0        0        0      682 2023-05-01 21:52:29.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_12_memory_not_freed.py
--rw-rw-rw-   0        0        0     2016 2023-06-15 00:02:04.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_13_deterministic_algorithm_option_not_used.py
--rw-rw-rw-   0        0        0     2454 2023-06-11 19:11:44.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_14_randomness_uncontrolled.py
--rw-rw-rw-   0        0        0      637 2023-06-11 20:09:44.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_15_missing_the_mask_of_invalid_value.py
--rw-rw-rw-   0        0        0       95 2023-06-05 12:12:32.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_16_broadcasting_feature_not_used.py
--rw-rw-rw-   0        0        0      918 2023-05-08 08:32:09.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_17_tensorarray_not_used.py
--rw-rw-rw-   0        0        0     1001 2023-06-05 12:37:31.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_18_training_evaluation_mode_improper_toggling.py
--rw-rw-rw-   0        0        0      603 2023-05-08 09:54:37.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_19_pytorch_call_method_misused.py
--rw-rw-rw-   0        0        0     2274 2023-06-15 00:05:10.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_1_unnecessary_iteration.py
--rw-rw-rw-   0        0        0     1180 2023-06-05 13:23:18.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_20_gradients_not_cleared_before_backward_propagation.py
--rw-rw-rw-   0        0        0     1520 2023-06-11 22:51:06.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_21_data_leakage.py
--rw-rw-rw-   0        0        0      587 2023-06-06 07:43:34.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_2_nan_equivalence_comparison_misused.py
--rw-rw-rw-   0        0        0     1114 2023-06-06 15:36:23.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_3_chain_indexing.py
--rw-rw-rw-   0        0        0     2099 2023-04-29 14:13:44.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_4_columns_and_datatype_not_explicitly_set.py
--rw-rw-rw-   0        0        0     1145 2023-06-14 21:59:24.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_5_empty_column_misinitialization.py
--rw-rw-rw-   0        0        0      956 2023-04-29 18:45:40.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_6_merge_api_parameter_not_explicitly_set.py
--rw-rw-rw-   0        0        0      854 2023-06-11 10:28:02.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_7_in_place_apis_misused.py
--rw-rw-rw-   0        0        0      660 2023-06-11 12:07:03.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_8_dataframe_conversion_api_misused.py
--rw-rw-rw-   0        0        0     2173 2023-06-14 22:51:51.000000 mlpylint-0.0.1/tests/test_files/file_checker_4_9_matrix_multiplication_api_misused.py
--rw-rw-rw-   0        0        0        2 2023-07-18 09:37:54.000000 mlpylint-0.0.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.121135 mlpylint-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-07-17 17:13:05.000000 mlpylint-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4368 2023-07-24 07:43:46.121135 mlpylint-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3040 2023-07-24 07:29:37.000000 mlpylint-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.071458 mlpylint-0.0.2/mlpylint.egg-info/
+-rw-rw-rw-   0        0        0     4368 2023-07-24 07:43:46.000000 mlpylint-0.0.2/mlpylint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4662 2023-07-24 07:43:46.000000 mlpylint-0.0.2/mlpylint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 07:43:46.000000 mlpylint-0.0.2/mlpylint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-24 07:43:46.000000 mlpylint-0.0.2/mlpylint.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 18:52:34.000000 mlpylint-0.0.2/mlpylint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       89 2023-07-24 07:43:46.000000 mlpylint-0.0.2/mlpylint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-24 07:43:46.000000 mlpylint-0.0.2/mlpylint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-07-18 11:00:37.000000 mlpylint-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1548 2023-07-24 07:43:46.122136 mlpylint-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.072458 mlpylint-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-07-18 09:26:23.000000 mlpylint-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.075460 mlpylint-0.0.2/src/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-01 22:11:59.000000 mlpylint-0.0.2/src/analysis/__init__.py
+-rw-rw-rw-   0        0        0     6936 2023-07-18 09:30:36.000000 mlpylint-0.0.2/src/analysis/argument.py
+-rw-rw-rw-   0        0        0      348 2023-06-22 14:08:30.000000 mlpylint-0.0.2/src/analysis/config.py
+-rw-rw-rw-   0        0        0     3482 2023-07-18 09:30:36.000000 mlpylint-0.0.2/src/analysis/result.py
+-rw-rw-rw-   0        0        0     5462 2023-07-22 13:10:28.000000 mlpylint-0.0.2/src/analysis/runner.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.088460 mlpylint-0.0.2/src/checkers/
+-rw-rw-rw-   0        0        0        0 2023-04-01 22:14:02.000000 mlpylint-0.0.2/src/checkers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.092459 mlpylint-0.0.2/src/checkers/advice/
+-rw-rw-rw-   0        0        0        0 2023-05-07 15:22:41.000000 mlpylint-0.0.2/src/checkers/advice/__init__.py
+-rw-rw-rw-   0        0        0     5023 2023-07-22 13:13:35.000000 mlpylint-0.0.2/src/checkers/advice/advice_checker_4_12_memory_not_freed.py
+-rw-rw-rw-   0        0        0     3025 2023-07-21 16:41:28.000000 mlpylint-0.0.2/src/checkers/advice/advice_checker_4_16_broadcasting_feature_not_used.py
+-rw-rw-rw-   0        0        0     3628 2023-07-23 07:45:25.000000 mlpylint-0.0.2/src/checkers/advice/advice_checker_4_18_training_evaluation_mode_improper_toggling.py
+-rw-rw-rw-   0        0        0     3694 2023-07-21 20:07:07.000000 mlpylint-0.0.2/src/checkers/advice/advice_checker_4_1_unnecessary_iteration.py
+-rw-rw-rw-   0        0        0     3430 2023-07-23 08:09:22.000000 mlpylint-0.0.2/src/checkers/advice/advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py
+-rw-rw-rw-   0        0        0     4780 2023-07-23 08:34:13.000000 mlpylint-0.0.2/src/checkers/advice/advice_checker_4_21_data_leakage.py
+-rw-rw-rw-   0        0        0      558 2023-04-28 15:37:23.000000 mlpylint-0.0.2/src/checkers/base_checker.py
+-rw-rw-rw-   0        0        0     3682 2023-07-18 15:02:34.000000 mlpylint-0.0.2/src/checkers/checker_4_11_hyperparameter_not_explicitly_set.py
+-rw-rw-rw-   0        0        0     3749 2023-07-18 15:03:16.000000 mlpylint-0.0.2/src/checkers/checker_4_13_deterministic_algorithm_option_not_used.py
+-rw-rw-rw-   0        0        0    13736 2023-07-18 15:03:55.000000 mlpylint-0.0.2/src/checkers/checker_4_14_randomness_uncontrolled.py
+-rw-rw-rw-   0        0        0     5564 2023-07-18 15:04:37.000000 mlpylint-0.0.2/src/checkers/checker_4_15_missing_the_mask_of_invalid_value.py
+-rw-rw-rw-   0        0        0     3585 2023-07-18 15:04:59.000000 mlpylint-0.0.2/src/checkers/checker_4_17_tensorarray_not_used.py
+-rw-rw-rw-   0        0        0     3010 2023-07-23 12:30:18.000000 mlpylint-0.0.2/src/checkers/checker_4_19_pytorch_call_method_misused.py
+-rw-rw-rw-   0        0        0     5162 2023-07-18 14:58:23.000000 mlpylint-0.0.2/src/checkers/checker_4_2_nan_equivalence_comparison_misused.py
+-rw-rw-rw-   0        0        0     3341 2023-07-18 14:58:44.000000 mlpylint-0.0.2/src/checkers/checker_4_3_chain_indexing.py
+-rw-rw-rw-   0        0        0     3275 2023-07-18 14:59:10.000000 mlpylint-0.0.2/src/checkers/checker_4_4_columns_and_data_type_not_explicitly_set.py
+-rw-rw-rw-   0        0        0    11187 2023-07-18 15:00:03.000000 mlpylint-0.0.2/src/checkers/checker_4_5_empty_column_misinitialization.py
+-rw-rw-rw-   0        0        0     3677 2023-07-18 15:00:30.000000 mlpylint-0.0.2/src/checkers/checker_4_6_merge_api_parameter_not_explicitly_set.py
+-rw-rw-rw-   0        0        0     4202 2023-07-18 15:00:55.000000 mlpylint-0.0.2/src/checkers/checker_4_7_in_place_apis_misused.py
+-rw-rw-rw-   0        0        0     2703 2023-07-18 15:01:39.000000 mlpylint-0.0.2/src/checkers/checker_4_8_dataframe_conversion_api_misused.py
+-rw-rw-rw-   0        0        0     5829 2023-07-23 18:48:38.000000 mlpylint-0.0.2/src/checkers/checker_4_9_matrix_multiplication_api_misused.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.093460 mlpylint-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:33:14.000000 mlpylint-0.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.107351 mlpylint-0.0.2/tests/test_checkers/
+-rw-rw-rw-   0        0        0        0 2023-04-02 16:23:11.000000 mlpylint-0.0.2/tests/test_checkers/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-07-22 12:56:13.000000 mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_12_memory_not_freed.py
+-rw-rw-rw-   0        0        0      780 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_16_broadcasting_feature_not_used.py
+-rw-rw-rw-   0        0        0      856 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_18_training_evaluation_mode_improper_toggling.py
+-rw-rw-rw-   0        0        0      741 2023-07-21 20:05:10.000000 mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_1_unnecessary_iteration.py
+-rw-rw-rw-   0        0        0      883 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py
+-rw-rw-rw-   0        0        0      633 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_21_data_leakage.py
+-rw-rw-rw-   0        0        0      720 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_11_hyperparameter_not_explicitly_set.py
+-rw-rw-rw-   0        0        0      748 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_13_deterministic_algorithm_option_not_used.py
+-rw-rw-rw-   0        0        0      674 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_14_randomness_uncontrolled.py
+-rw-rw-rw-   0        0        0      716 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_15_missing_the_mask_of_invalid_value.py
+-rw-rw-rw-   0        0        0      657 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_17_tensorarray_not_used.py
+-rw-rw-rw-   0        0        0      690 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_19_pytorch_call_method_misused.py
+-rw-rw-rw-   0        0        0      736 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_2_nan_equivalence_comparison_misused.py
+-rw-rw-rw-   0        0        0      626 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_3_chain_indexing.py
+-rw-rw-rw-   0        0        0      741 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_4_columns_and_datatype_not_explicitly_set.py
+-rw-rw-rw-   0        0        0      704 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_5_empty_column_misinitialization.py
+-rw-rw-rw-   0        0        0      738 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_6_merge_api_parameter_not_explicitly_set.py
+-rw-rw-rw-   0        0        0      657 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_7_in_place_apis_misused.py
+-rw-rw-rw-   0        0        0      712 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_8_dataframe_conversion_api_misused.py
+-rw-rw-rw-   0        0        0      717 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_9_matrix_multiplication_api_misused.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.120135 mlpylint-0.0.2/tests/test_files/
+-rw-rw-rw-   0        0        0        0 2023-04-02 16:23:30.000000 mlpylint-0.0.2/tests/test_files/__init__.py
+-rw-rw-rw-   0        0        0      291 2023-07-17 12:38:57.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_11_hyperparameter_not_explicitly_set.py
+-rw-rw-rw-   0        0        0      941 2023-07-22 12:57:56.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_12_memory_not_freed.py
+-rw-rw-rw-   0        0        0     2016 2023-06-15 00:02:04.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_13_deterministic_algorithm_option_not_used.py
+-rw-rw-rw-   0        0        0     2454 2023-06-11 19:11:44.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_14_randomness_uncontrolled.py
+-rw-rw-rw-   0        0        0      637 2023-06-11 20:09:44.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_15_missing_the_mask_of_invalid_value.py
+-rw-rw-rw-   0        0        0      538 2023-07-21 16:12:07.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_16_broadcasting_feature_not_used.py
+-rw-rw-rw-   0        0        0      918 2023-05-08 08:32:09.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_17_tensorarray_not_used.py
+-rw-rw-rw-   0        0        0     1001 2023-06-05 12:37:31.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_18_training_evaluation_mode_improper_toggling.py
+-rw-rw-rw-   0        0        0      603 2023-05-08 09:54:37.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_19_pytorch_call_method_misused.py
+-rw-rw-rw-   0        0        0     2274 2023-07-21 19:39:51.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_1_unnecessary_iteration.py
+-rw-rw-rw-   0        0        0     1202 2023-07-23 08:09:22.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_20_gradients_not_cleared_before_backward_propagation.py
+-rw-rw-rw-   0        0        0     1621 2023-07-23 08:34:26.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_21_data_leakage.py
+-rw-rw-rw-   0        0        0      587 2023-06-06 07:43:34.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_2_nan_equivalence_comparison_misused.py
+-rw-rw-rw-   0        0        0     1114 2023-06-06 15:36:23.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_3_chain_indexing.py
+-rw-rw-rw-   0        0        0     2099 2023-04-29 14:13:44.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_4_columns_and_datatype_not_explicitly_set.py
+-rw-rw-rw-   0        0        0     1145 2023-06-14 21:59:24.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_5_empty_column_misinitialization.py
+-rw-rw-rw-   0        0        0      956 2023-04-29 18:45:40.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_6_merge_api_parameter_not_explicitly_set.py
+-rw-rw-rw-   0        0        0      854 2023-06-11 10:28:02.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_7_in_place_apis_misused.py
+-rw-rw-rw-   0        0        0      660 2023-06-11 12:07:03.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_8_dataframe_conversion_api_misused.py
+-rw-rw-rw-   0        0        0     2173 2023-06-14 22:51:51.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_9_matrix_multiplication_api_misused.py
+-rw-rw-rw-   0        0        0        2 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_utils.py
```

### Comparing `mlpylint-0.0.1/LICENSE` & `mlpylint-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/PKG-INFO` & `mlpylint-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpylint
-Version: 0.0.1
+Version: 0.0.2
 Summary: MLpylint, a static analysis tool for identifying ML-specific code smells
 Author: Peter Hamfelt
 Author-email: peter.hamfelt@gmail.com
 Keywords: linting,static-analysis,python-linting,python-static-analysis,machine-learning,machine-learning-engineering,ML-model-quality,artificial-intelligence,python,software-quality,technical-debt,software-engineering,maintainability,code-smell
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,14 @@
 MLpylint is a static code analyzer designed specifically for Python applications. Drawing from extensive research in the
 field of ML-specific code smells, MLpylint focuses on identifying ML-specific issues in your code. This assists in
 enhancing the readability, maintainability, and efficiency of your ML codebase, ensuring it adheres to best practices in
 the field of artificial intelligence and machine learning software development.
 
 ## Getting started
 
-
 The project structure is organized into three main components:
 
 1. Code Smell Checkers: These are the core of our tool, designed to identify specific code smells in your Python scripts.
 
 2. Test Scripts: Each code smell checker comes with an associated test script. These are used to validate the functionality of each checker, ensuring it correctly identifies its corresponding code smell.
 
 3. Code Smell Test Files: These are Python scripts that contain examples of code smells. They serve as practical test cases for the code smell checkers, helping to ensure that the checkers are accurately identifying the intended code smells.
@@ -51,15 +50,15 @@
 
 ## Installation
 
 ```
 cd mlpylint
 py -m venv venv
 source venv/Scripts/activate
-pip install -e .
+pip install -e .[dev]
 ```
 
 ## Usage
 
 ```
 $ mlpylint --help                          # View tool options
 $ mlpylint <path>                          # Check for code smells (CS)
```

### Comparing `mlpylint-0.0.1/README.md` & `mlpylint-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 MLpylint is a static code analyzer designed specifically for Python applications. Drawing from extensive research in the
 field of ML-specific code smells, MLpylint focuses on identifying ML-specific issues in your code. This assists in
 enhancing the readability, maintainability, and efficiency of your ML codebase, ensuring it adheres to best practices in
 the field of artificial intelligence and machine learning software development.
 
 ## Getting started
 
-
 The project structure is organized into three main components:
 
 1. Code Smell Checkers: These are the core of our tool, designed to identify specific code smells in your Python scripts.
 
 2. Test Scripts: Each code smell checker comes with an associated test script. These are used to validate the functionality of each checker, ensuring it correctly identifies its corresponding code smell.
 
 3. Code Smell Test Files: These are Python scripts that contain examples of code smells. They serve as practical test cases for the code smell checkers, helping to ensure that the checkers are accurately identifying the intended code smells.
@@ -25,15 +24,15 @@
 
 ## Installation
 
 ```
 cd mlpylint
 py -m venv venv
 source venv/Scripts/activate
-pip install -e .
+pip install -e .[dev]
 ```
 
 ## Usage
 
 ```
 $ mlpylint --help                          # View tool options
 $ mlpylint <path>                          # Check for code smells (CS)
```

### Comparing `mlpylint-0.0.1/mlpylint.egg-info/PKG-INFO` & `mlpylint-0.0.2/mlpylint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpylint
-Version: 0.0.1
+Version: 0.0.2
 Summary: MLpylint, a static analysis tool for identifying ML-specific code smells
 Author: Peter Hamfelt
 Author-email: peter.hamfelt@gmail.com
 Keywords: linting,static-analysis,python-linting,python-static-analysis,machine-learning,machine-learning-engineering,ML-model-quality,artificial-intelligence,python,software-quality,technical-debt,software-engineering,maintainability,code-smell
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,14 @@
 MLpylint is a static code analyzer designed specifically for Python applications. Drawing from extensive research in the
 field of ML-specific code smells, MLpylint focuses on identifying ML-specific issues in your code. This assists in
 enhancing the readability, maintainability, and efficiency of your ML codebase, ensuring it adheres to best practices in
 the field of artificial intelligence and machine learning software development.
 
 ## Getting started
 
-
 The project structure is organized into three main components:
 
 1. Code Smell Checkers: These are the core of our tool, designed to identify specific code smells in your Python scripts.
 
 2. Test Scripts: Each code smell checker comes with an associated test script. These are used to validate the functionality of each checker, ensuring it correctly identifies its corresponding code smell.
 
 3. Code Smell Test Files: These are Python scripts that contain examples of code smells. They serve as practical test cases for the code smell checkers, helping to ensure that the checkers are accurately identifying the intended code smells.
@@ -51,15 +50,15 @@
 
 ## Installation
 
 ```
 cd mlpylint
 py -m venv venv
 source venv/Scripts/activate
-pip install -e .
+pip install -e .[dev]
 ```
 
 ## Usage
 
 ```
 $ mlpylint --help                          # View tool options
 $ mlpylint <path>                          # Check for code smells (CS)
```

### Comparing `mlpylint-0.0.1/mlpylint.egg-info/SOURCES.txt` & `mlpylint-0.0.2/mlpylint.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 src/checkers/advice/advice_checker_4_18_training_evaluation_mode_improper_toggling.py
 src/checkers/advice/advice_checker_4_1_unnecessary_iteration.py
 src/checkers/advice/advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py
 src/checkers/advice/advice_checker_4_21_data_leakage.py
 tests/__init__.py
 tests/test_utils.py
 tests/test_checkers/__init__.py
+tests/test_checkers/test_advice_checker_4_12_memory_not_freed.py
 tests/test_checkers/test_advice_checker_4_16_broadcasting_feature_not_used.py
 tests/test_checkers/test_advice_checker_4_18_training_evaluation_mode_improper_toggling.py
 tests/test_checkers/test_advice_checker_4_1_unnecessary_iteration.py
 tests/test_checkers/test_advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py
 tests/test_checkers/test_advice_checker_4_21_data_leakage.py
 tests/test_checkers/test_checker_4_11_hyperparameter_not_explicitly_set.py
-tests/test_checkers/test_checker_4_12_memory_not_freed.py
 tests/test_checkers/test_checker_4_13_deterministic_algorithm_option_not_used.py
 tests/test_checkers/test_checker_4_14_randomness_uncontrolled.py
 tests/test_checkers/test_checker_4_15_missing_the_mask_of_invalid_value.py
 tests/test_checkers/test_checker_4_17_tensorarray_not_used.py
 tests/test_checkers/test_checker_4_19_pytorch_call_method_misused.py
 tests/test_checkers/test_checker_4_2_nan_equivalence_comparison_misused.py
 tests/test_checkers/test_checker_4_3_chain_indexing.py
```

### Comparing `mlpylint-0.0.1/setup.cfg` & `mlpylint-0.0.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6c70 796c 696e 740d 0a76 6572   = mlpylint..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e31 0d0a 6465  sion = 0.0.1..de
+00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 6465  sion = 0.0.2..de
 00000030: 7363 7269 7074 696f 6e20 3d20 4d4c 7079  scription = MLpy
 00000040: 6c69 6e74 2c20 6120 7374 6174 6963 2061  lint, a static a
 00000050: 6e61 6c79 7369 7320 746f 6f6c 2066 6f72  nalysis tool for
 00000060: 2069 6465 6e74 6966 7969 6e67 204d 4c2d   identifying ML-
 00000070: 7370 6563 6966 6963 2063 6f64 6520 736d  specific code sm
 00000080: 656c 6c73 0d0a 6c6f 6e67 5f64 6573 6372  ells..long_descr
 00000090: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
@@ -76,19 +76,22 @@
 000004b0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
 000004c0: 0d0a 7a69 705f 7361 6665 203d 2046 616c  ..zip_safe = Fal
 000004d0: 7365 0d0a 696e 636c 7564 655f 7061 636b  se..include_pack
 000004e0: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
 000004f0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
 00000500: 7320 3d20 0d0a 0961 7374 726f 6964 3e3d  s = ...astroid>=
 00000510: 322e 3135 2e31 0d0a 0963 6f6c 6f72 616d  2.15.1...coloram
-00000520: 610d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  a....[options.en
-00000530: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
-00000540: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
-00000550: 0a09 6d6c 7079 6c69 6e74 203d 2073 7263  ..mlpylint = src
-00000560: 2e61 6e61 6c79 7369 732e 7275 6e6e 6572  .analysis.runner
-00000570: 3a6d 6169 6e0d 0a0d 0a5b 6f70 7469 6f6e  :main....[option
-00000580: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
-00000590: 5d0d 0a64 6576 203d 200d 0a09 7079 7465  ]..dev = ...pyte
-000005a0: 7374 3e3d 372e 322e 320d 0a0d 0a5b 6567  st>=7.2.2....[eg
-000005b0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-000005c0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-000005d0: 3d20 300d 0a0d 0a                        = 0....
+00000520: 610d 0a09 7465 6e73 6f72 666c 6f77 0d0a  a...tensorflow..
+00000530: 0970 616e 6461 730d 0a09 6e75 6d70 790d  .pandas...numpy.
+00000540: 0a09 7363 696b 6974 2d6c 6561 726e 0d0a  ..scikit-learn..
+00000550: 0974 6f72 6368 0d0a 0d0a 5b6f 7074 696f  .torch....[optio
+00000560: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
+00000570: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
+00000580: 7320 3d20 0d0a 096d 6c70 796c 696e 7420  s = ...mlpylint 
+00000590: 3d20 7372 632e 616e 616c 7973 6973 2e72  = src.analysis.r
+000005a0: 756e 6e65 723a 6d61 696e 0d0a 0d0a 5b6f  unner:main....[o
+000005b0: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
+000005c0: 7175 6972 655d 0d0a 6465 7620 3d20 0d0a  quire]..dev = ..
+000005d0: 0970 7974 6573 743e 3d37 2e32 2e32 0d0a  .pytest>=7.2.2..
+000005e0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+000005f0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000600: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `mlpylint-0.0.1/src/analysis/argument.py` & `mlpylint-0.0.2/src/analysis/argument.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/analysis/result.py` & `mlpylint-0.0.2/src/analysis/result.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/analysis/runner.py` & `mlpylint-0.0.2/src/analysis/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
         except SyntaxError as e:
             print(f"Syntax error in file {filename}: {str(e)}")
             self.file_syntax_error_count += 1
 
         except Exception as e:
             print(f"Error analyzing file {filename}: {str(e)}")
+            self.file_syntax_error_count += 1
 
     def analyze_directory(self, directory):
         print(f"Analyzing files in directory: {directory}")
         for root, dirs, files in os.walk(directory):
             for file in files:
                 if file.endswith('.py'):
                     filename = os.path.join(root, file)
```

### Comparing `mlpylint-0.0.1/src/checkers/advice/advice_checker_4_12_memory_not_freed.py` & `mlpylint-0.0.2/src/checkers/advice/advice_checker_4_16_broadcasting_feature_not_used.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,78 @@
 import astroid
+from astroid.helpers import safe_infer
 
 from src.analysis.result import Result, CodeSmell
 from src.checkers.base_checker import BaseChecker
 
 
-class MemoryNotFreed(BaseChecker):
+class BroadcastingFeatureNotUsed(BaseChecker):
     """
-    This class inspects the Python code for import statements related to the "tensorflow" or "pytorch" libraries.
+    This class scrutinizes the Python code for import statements pertaining to the "tensorflow" library and usage of
+    tf.tile() method.
     """
 
-    ID = "CSA12"
-    TITLE = "Free memory in time."
+    ID = "CSA16"
+    TITLE = "Use the broadcasting feature in deep learning code to be more memory efficient."
     DESCRIPTION = """
     Context:
-    Machine learning training is memory-consuming, and
-    the machine’s memory is always limited by budget.
+    Deep learning libraries like PyTorch and TensorFlow supports
+    the element-wise broadcasting operation.
 
     Problem:
-    If the machine runs out of memory while training the
-    model, the training will fail.
+    Without broadcasting, tiling a tensor first to match another
+    tensor consumes more memory due to the creation and storage
+    of a middle tiling operation result.
 
     Solution:
-    Some APIs are provided to alleviate the run-out-ofmemory
-    issue in deep learning libraries. TensorFlow’s documentation
-    notes that if the model is created in a loop, it is suggested to use
-    clear_session() in the loop. Meanwhile, the GitHub repository
-    pytorch-styleguide recommends using .detach() to free the tensor
-    from the graph whenever possible. The .detach() API can prevent
-    unnecessary operations from being recorded and therefore can save
-    memory. Developers should check whether they use this kind
-    of APIs to free the memory whenever possible in their code.
+    With broadcasting, it is more memory efficient. However,
+    there is a trade-off in debugging since the tiling process is not
+    explicitly stated.
     """
 
     def __init__(self, filename):
         super().__init__(filename)
+        self.code_smell_found = False
+        self.has_import = False
+
+        self.tensorflow_alias = set()
 
     def visit_import(self, node: astroid.Import) -> None:
+        if self.has_import or self.code_smell_found:
+            return
+
         for name, alias in node.names:
             if name == "tensorflow":
-                self.record_finding(node=node)
-
-            if name == "torch":
-                self.record_finding(node=node)
+                if node.names[0][1] is not None:
+                    self.tensorflow_alias.add(node.names[0][1])
+                else:
+                    self.tensorflow_alias.add(node.names[0][0])
+
+                self.has_import = True
+
+    def visit_call(self, node: astroid.Call) -> None:
+        if self.code_smell_found or not self.has_import:
+            return
+
+        # Check usage of tf.tile()
+        if (
+                isinstance(node.func, astroid.Attribute)
+                and node.func.attrname == "tile"
+                and isinstance(node.func.expr, astroid.Name)
+                and node.func.expr.name in self.tensorflow_alias
+        ):
+            self.record_finding(node)
+            self.code_smell_found = True
 
-    def record_finding(self, node: astroid.Import) -> None:
+    def record_finding(self, node: astroid.NodeNG) -> None:
         Result.add(CodeSmell(code_smell_id=self.ID,
-                             code_smell_title="Memory Not Freed",
+                             code_smell_title="Broadcasting Feature Not Used",
                              file_path=self.filename,
                              line=node.lineno,
                              col_offset=node.col_offset,
                              smell_type="Generic",
-                             description="Free memory in time.",
+                             description="Use the broadcasting feature in deep learning code to be more memory "
+                                         "efficient.",
                              pipeline_stage="Model Training",
-                             effect="Memory Issue",
+                             effect="Efficiency",
                              source_code=node.as_string(),
                              source_astroid_node=f"Astroid AST: {node} \n Code: {node.as_string()}"))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mlpylint-0.0.1/src/checkers/advice/advice_checker_4_18_training_evaluation_mode_improper_toggling.py` & `mlpylint-0.0.2/src/checkers/advice/advice_checker_4_18_training_evaluation_mode_improper_toggling.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import astroid
+from astroid.helpers import safe_infer
 
 from src.analysis.result import Result, CodeSmell
 from src.checkers.base_checker import BaseChecker
 
 
 class TrainingAndEvaluationModeImproperToggling(BaseChecker):
     """
     This class is designed to validate and keep track of the import of "torch" along with its alias, scrutinize
     'importfrom' statements related to "torch" to see if "eval" is being imported, and, provided that "torch" is
     imported, assess function calls for instances of 'torch.eval' usage.
     """
 
     ID = "CSA18"
-    TITLE = "Call the training mode in the appropriate place in deep learning code to avoid forgetting to toggle back " \
-            "the training mode after the inference step. "
+    TITLE = "Call the training mode in the appropriate place in deep learning code to avoid forgetting to toggle " \
+            "back the training mode after the inference step. "
     DESCRIPTION = """
     Context:
     In PyTorch, calling .eval() means we are going into the
     evaluation mode and the Dropout layer will be deactivated.
 
     Problem:
     If the training mode did not toggle back in time, the
@@ -60,22 +61,21 @@
                 self.code_smell_found = True
 
     def visit_call(self, node: astroid.Call) -> None:
         if self.code_smell_found:
             return
 
         if (
-                self.has_torch_import and
                 isinstance(node.func, astroid.Attribute) and
                 node.func.attrname == "eval"
         ):
-            for infer in node.func.inferred():
-                if "torch" in str(infer):
-                    self.record_finding(node=node)
-                    self.code_smell_found = True
+            inferred_node = safe_infer(node)
+            if inferred_node and "torch" in inferred_node.root().name:
+                self.record_finding(node=node)
+                self.code_smell_found = True
 
     def record_finding(self, node: astroid.NodeNG) -> None:
         Result.add(CodeSmell(code_smell_id=self.ID,
                              code_smell_title="Training / Evaluation Mode Improper Toggling",
                              file_path=self.filename,
                              line=node.lineno,
                              col_offset=node.col_offset,
```

### Comparing `mlpylint-0.0.1/src/checkers/advice/advice_checker_4_1_unnecessary_iteration.py` & `mlpylint-0.0.2/src/checkers/advice/advice_checker_4_1_unnecessary_iteration.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             return
 
         for name, alias in node.names:
             if name == ("pandas" or "tensor"):
                 self.has_import = True
 
     def visit_for(self, node: astroid.For) -> None:
-        if self.code_smell_found or self.has_import is False:
+        if self.code_smell_found or not self.has_import:
             return
 
         if self.dfs(node=node.iter):
             # Code smell
             self.record_finding(node=node)
             self.code_smell_found = True
```

### Comparing `mlpylint-0.0.1/src/checkers/advice/advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py` & `mlpylint-0.0.2/src/checkers/advice/advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import astroid
+from astroid.helpers import safe_infer
 
 from src.analysis.result import Result, CodeSmell
 from src.checkers.base_checker import BaseChecker
 
 
 class GradientsNotClearedBeforeBackwardPropagation(BaseChecker):
     """
@@ -35,29 +36,33 @@
     def __init__(self, filename):
         super().__init__(filename)
         self.has_torch_import = False
         self.code_smell_found = False
 
     def visit_import(self, node: astroid.Import) -> None:
         for name, alias in node.names:
-            if name == "torch":
+            if "torch" in name:
+                self.has_torch_import = True
+
+    def visit_importfrom(self, node: astroid.ImportFrom) -> None:
+        if node.modname == "torch":
+            if any(name in {"nn", "optim"} for name in node.names[0]):
                 self.has_torch_import = True
 
     def visit_call(self, node: astroid.Call):
         if self.code_smell_found:
             return
 
         if (
                 self.has_torch_import
                 and isinstance(node.func, astroid.Attribute)
                 and node.func.attrname in {"zero_grad", "backward", "step"}
-                and any("torch" in str(infer) for infer in node.func.inferred())
         ):
-            self.code_smell_found = True
             self.record_finding(node=node)
+            self.code_smell_found = True
 
     def record_finding(self, node: astroid.Call) -> None:
         Result.add(CodeSmell(code_smell_id=self.ID,
                              code_smell_title="Gradients Not Cleared before Backward Propagation",
                              file_path=self.filename,
                              line=node.lineno,
                              col_offset=node.col_offset,
```

### Comparing `mlpylint-0.0.1/src/checkers/advice/advice_checker_4_21_data_leakage.py` & `mlpylint-0.0.2/src/checkers/advice/advice_checker_4_21_data_leakage.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,42 +38,53 @@
     def __init__(self, filename):
         super().__init__(filename)
         self.has_sklearn_import = False
         self.has_sklearn_pipeline = False
         self.sklearn_node = None
 
     def visit_nodes(self, node: astroid.NodeNG) -> None:
+        if self.has_sklearn_pipeline:
+            return
+
         if isinstance(node, astroid.Import):
             for name, alias in node.names:
                 if "sklearn" in name:
                     self.sklearn_node = node
                     self.has_sklearn_import = True
         elif (
                 isinstance(node, astroid.ImportFrom)
                 and "sklearn" in node.modname
         ):
+            self.has_sklearn_pipeline = True if node.modname in {"sklearn.pipeline"} else False
             self.has_sklearn_import = True
             self.sklearn_node = node
 
             if "Pipeline" in node.names[0]:
                 # Checks if Pipeline is imported directly "from sklearn.pipeline import Pipeline"
                 # Assuming that it is being used
                 self.has_sklearn_pipeline = True
         elif (
                 isinstance(node, astroid.Call)
         ):
             if (
-                    isinstance(node.func, astroid.Attribute)
-                    and node.func.attrname == "Pipeline"
-                    and isinstance(node.func.expr, astroid.Attribute)
-                    and node.func.expr.attrname == "pipeline"
+                    (self.has_sklearn_import
+                     and isinstance(node.func, astroid.Name)
+                     and node.func.name == "make_pipeline")
+                    or
+                    (self.has_sklearn_import
+                     and isinstance(node.func, astroid.Attribute)
+                     and node.func.attrname == "make_pipeline")
+                    or
+                    (self.has_sklearn_import
+                     and isinstance(node.func, astroid.Attribute)
+                     and node.func.attrname == "Pipeline"
+                     and isinstance(node.func.expr, astroid.Attribute)
+                     and node.func.expr.attrname == "pipeline")
             ):
-                for infer in node.func.expr.inferred():
-                    if "sklearn" in str(infer):
-                        self.has_sklearn_pipeline = True
+                self.has_sklearn_pipeline = True
 
         for child in node.get_children():
             self.visit_nodes(child)
 
     def visit_module(self, module_node: astroid.Module) -> None:
         # Iterate module and search for indicators
         for node in module_node.body:
```

### Comparing `mlpylint-0.0.1/src/checkers/base_checker.py` & `mlpylint-0.0.2/src/checkers/base_checker.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_11_hyperparameter_not_explicitly_set.py` & `mlpylint-0.0.2/src/checkers/checker_4_11_hyperparameter_not_explicitly_set.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_13_deterministic_algorithm_option_not_used.py` & `mlpylint-0.0.2/src/checkers/checker_4_13_deterministic_algorithm_option_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_14_randomness_uncontrolled.py` & `mlpylint-0.0.2/src/checkers/checker_4_14_randomness_uncontrolled.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_15_missing_the_mask_of_invalid_value.py` & `mlpylint-0.0.2/src/checkers/checker_4_15_missing_the_mask_of_invalid_value.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_17_tensorarray_not_used.py` & `mlpylint-0.0.2/src/checkers/checker_4_17_tensorarray_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_19_pytorch_call_method_misused.py` & `mlpylint-0.0.2/src/checkers/checker_4_19_pytorch_call_method_misused.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,19 +26,31 @@
     Solution:
     It is recommended to use self.net() rather than
     self.net.forward().
     """
 
     def __init__(self, filename):
         super().__init__(filename)
+        self.has_torch_import = False
+
+    def visit_import(self, node: astroid.Import) -> None:
+        for name, alias in node.names:
+            if "torch.nn" in name:
+                self.has_torch_import = True
+
+    def visit_importfrom(self, node: astroid.ImportFrom) -> None:
+        if node.modname == "torch":
+            if any(name in {"nn"} for name in node.names[0]):
+                self.has_torch_import = True
 
     def visit_attribute(self, node: astroid.Attribute):
         # Check if the attribute is 'forward' and its parent is a call to 'self.net'
         if node.attrname == 'forward' and isinstance(node.expr, astroid.Attribute):
             if (
+                    self.has_torch_import and
                     node.expr.attrname == 'net' and
                     isinstance(node.expr.expr, astroid.Name) and
                     node.expr.expr.name == 'self'
             ):
                 self.record_finding(node=node)
 
     def record_finding(self, node: astroid.Attribute) -> None:
```

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_2_nan_equivalence_comparison_misused.py` & `mlpylint-0.0.2/src/checkers/checker_4_2_nan_equivalence_comparison_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_3_chain_indexing.py` & `mlpylint-0.0.2/src/checkers/checker_4_3_chain_indexing.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_4_columns_and_data_type_not_explicitly_set.py` & `mlpylint-0.0.2/src/checkers/checker_4_4_columns_and_data_type_not_explicitly_set.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_5_empty_column_misinitialization.py` & `mlpylint-0.0.2/src/checkers/checker_4_5_empty_column_misinitialization.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_6_merge_api_parameter_not_explicitly_set.py` & `mlpylint-0.0.2/src/checkers/checker_4_6_merge_api_parameter_not_explicitly_set.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_7_in_place_apis_misused.py` & `mlpylint-0.0.2/src/checkers/checker_4_7_in_place_apis_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_8_dataframe_conversion_api_misused.py` & `mlpylint-0.0.2/src/checkers/checker_4_8_dataframe_conversion_api_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/src/checkers/checker_4_9_matrix_multiplication_api_misused.py` & `mlpylint-0.0.2/src/checkers/checker_4_9_matrix_multiplication_api_misused.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
     """
     This class performs several checks involving the usage of the "numpy" library:
     - It verifies the import of "numpy", storing its alias for subsequent checks.
     - It checks for assignments of two-dimensional numpy arrays, storing the associated variable names.
     - It scrutinizes function calls for the invocation of the 'dot()' function:
         - If the 'dot()' function is invoked on the numpy alias and its arguments are variables storing two-dimensional
         numpy arrays, this is flagged as a code smell.
-    - If any of these checks pass, it records the code smell instance.
-
     """
 
     ID = "CS9"
     TITLE = "When the multiply operation is performed on two-dimensional matrixes, use np.matmul() instead of " \
             "np.dot() in NumPy for better semantics."
     DESCRIPTION = """
     Context:
```

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_advice_checker_4_16_broadcasting_feature_not_used.py` & `mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_16_broadcasting_feature_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_advice_checker_4_18_training_evaluation_mode_improper_toggling.py` & `mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_18_training_evaluation_mode_improper_toggling.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_advice_checker_4_1_unnecessary_iteration.py` & `mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_1_unnecessary_iteration.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py` & `mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_advice_checker_4_21_data_leakage.py` & `mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_21_data_leakage.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_11_hyperparameter_not_explicitly_set.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_11_hyperparameter_not_explicitly_set.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_12_memory_not_freed.py` & `mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_12_memory_not_freed.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 
     file_path = 'file_checker_4_12_memory_not_freed.py'
     absolute_file_path = os.path.join(ROOT_DIR, 'test_files', file_path)
 
     runner = Runner(path=absolute_file_path, registered_checkers=REGISTERED_CHECKERS)
     runner.run()
 
-    assert len(Result.code_smells) == 2
+    assert len(Result.code_smells) == 1  # Advice should stop after single detection of code smell
```

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_13_deterministic_algorithm_option_not_used.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_13_deterministic_algorithm_option_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_14_randomness_uncontrolled.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_14_randomness_uncontrolled.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_15_missing_the_mask_of_invalid_value.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_15_missing_the_mask_of_invalid_value.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_17_tensorarray_not_used.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_17_tensorarray_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_19_pytorch_call_method_misused.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_19_pytorch_call_method_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_2_nan_equivalence_comparison_misused.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_2_nan_equivalence_comparison_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_3_chain_indexing.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_3_chain_indexing.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_4_columns_and_datatype_not_explicitly_set.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_4_columns_and_datatype_not_explicitly_set.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_5_empty_column_misinitialization.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_5_empty_column_misinitialization.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_6_merge_api_parameter_not_explicitly_set.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_6_merge_api_parameter_not_explicitly_set.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_7_in_place_apis_misused.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_7_in_place_apis_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_8_dataframe_conversion_api_misused.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_8_dataframe_conversion_api_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_checkers/test_checker_4_9_matrix_multiplication_api_misused.py` & `mlpylint-0.0.2/tests/test_checkers/test_checker_4_9_matrix_multiplication_api_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_13_deterministic_algorithm_option_not_used.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_13_deterministic_algorithm_option_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_14_randomness_uncontrolled.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_14_randomness_uncontrolled.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_15_missing_the_mask_of_invalid_value.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_15_missing_the_mask_of_invalid_value.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_17_tensorarray_not_used.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_17_tensorarray_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_18_training_evaluation_mode_improper_toggling.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_18_training_evaluation_mode_improper_toggling.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_19_pytorch_call_method_misused.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_19_pytorch_call_method_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_1_unnecessary_iteration.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_1_unnecessary_iteration.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_20_gradients_not_cleared_before_backward_propagation.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_20_gradients_not_cleared_before_backward_propagation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
 import torch.optim as optim
-
+# from torch import nn
 
 class Model(nn.Module):
     def __init__(self):
         super(Model, self).__init__()
         self.layer = nn.Linear(10, 1)
 
     def forward(self, x):
```

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_21_data_leakage.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_21_data_leakage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import sklearn
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import StandardScaler
 from sklearn.linear_model import LogisticRegression
 # from sklearn.pipeline import Pipeline   # No data leakage issue (using Pipeline, comment-out to trigger code smell)
 from sklearn.datasets import load_iris
+# from sklearn.pipeline import make_pipeline
 
+# make_pipeline()
+# sklearn.pipeline.make_pipeline()
 
 def data_leakage_example():
     iris = load_iris()
     X, y = iris.data, iris.target
 
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
```

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_2_nan_equivalence_comparison_misused.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_2_nan_equivalence_comparison_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_3_chain_indexing.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_3_chain_indexing.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_4_columns_and_datatype_not_explicitly_set.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_4_columns_and_datatype_not_explicitly_set.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_5_empty_column_misinitialization.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_5_empty_column_misinitialization.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_6_merge_api_parameter_not_explicitly_set.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_6_merge_api_parameter_not_explicitly_set.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_7_in_place_apis_misused.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_7_in_place_apis_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_8_dataframe_conversion_api_misused.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_8_dataframe_conversion_api_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.1/tests/test_files/file_checker_4_9_matrix_multiplication_api_misused.py` & `mlpylint-0.0.2/tests/test_files/file_checker_4_9_matrix_multiplication_api_misused.py`

 * *Files identical despite different names*

