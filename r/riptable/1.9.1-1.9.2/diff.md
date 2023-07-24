# Comparing `tmp/riptable-1.9.1.tar.gz` & `tmp/riptable-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riptable-1.9.1.tar", last modified: Thu Jun 22 15:25:04 2023, max compression
+gzip compressed data, was "riptable-1.9.2.tar", last modified: Wed Jul 12 14:48:47 2023, max compression
```

## Comparing `riptable-1.9.1.tar` & `riptable-1.9.2.tar`

### file list

```diff
@@ -1,263 +1,263 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:04.146228 riptable-1.9.1/
--rw-rw-rw-   0        0        0      291 2023-06-22 15:11:21.000000 riptable-1.9.1/.editorconfig
--rw-rw-rw-   0        0        0      196 2023-06-22 15:11:21.000000 riptable-1.9.1/.gitattributes
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:03.864973 riptable-1.9.1/.github/
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:03.896224 riptable-1.9.1/.github/workflows/
--rw-rw-rw-   0        0        0     7753 2023-06-22 15:11:21.000000 riptable-1.9.1/.github/workflows/python-package.yml
--rw-rw-rw-   0        0        0     2110 2023-06-22 15:11:21.000000 riptable-1.9.1/.gitignore
--rw-rw-rw-   0        0        0      309 2023-06-22 15:11:21.000000 riptable-1.9.1/BUILDNOTES.txt
--rw-rw-rw-   0        0        0     2634 2023-06-22 15:11:21.000000 riptable-1.9.1/LICENSE
--rw-rw-rw-   0        0        0     3464 2023-06-22 15:11:21.000000 riptable-1.9.1/LICENSES-thirdparty.md
--rw-rw-rw-   0        0        0      196 2023-06-22 15:11:21.000000 riptable-1.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0      660 2023-06-22 15:25:04.146228 riptable-1.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     6083 2023-06-22 15:11:21.000000 riptable-1.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:03.896224 riptable-1.9.1/conda_recipe/
--rw-rw-rw-   0        0        0       19 2023-06-22 15:11:21.000000 riptable-1.9.1/conda_recipe/conda_build_config.yaml
--rw-rw-rw-   0        0        0     1804 2023-06-22 15:11:21.000000 riptable-1.9.1/conda_recipe/meta.yaml
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:03.896224 riptable-1.9.1/dev_tools/
--rw-rw-rw-   0        0        0     3965 2023-06-22 15:11:21.000000 riptable-1.9.1/dev_tools/gen_requirements.py
--rw-rw-rw-   0        0        0    25367 2023-06-22 15:11:21.000000 riptable-1.9.1/dev_tools/validate_docstrings.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:03.896224 riptable-1.9.1/docs/
--rw-rw-rw-   0        0        0      901 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0      658 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/Makefile
--rw-rw-rw-   0        0        0     2979 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/THREADING.md
--rwxrwxrwx   0        0        0      799 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/make.bat
--rw-rw-rw-   0        0        0     1085 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/riptable_logo.PNG
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:03.911849 riptable-1.9.1/docs/source/
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:03.911849 riptable-1.9.1/docs/source/_static/
--rw-rw-rw-   0        0        0        0 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/_static/.keep
--rw-rw-rw-   0        0        0    14482 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/benchmarking.rst
--rw-rw-rw-   0        0        0     4478 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/conf.py
--rw-rw-rw-   0        0        0      487 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/index.rst
--rw-rw-rw-   0        0        0       68 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/modules.rst
--rw-rw-rw-   0        0        0     6795 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/riptable.rst
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:03.943097 riptable-1.9.1/docs/source/tutorial/
--rw-rw-rw-   0        0        0    23344 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/RiptableExercises.ipynb
--rw-rw-rw-   0        0        0    95601 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/RiptableSolutions.ipynb
--rw-rw-rw-   0        0        0    35605 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/output_11_0.png
--rw-rw-rw-   0        0        0     5827 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/output_13_0.png
--rw-rw-rw-   0        0        0    60197 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/output_15_0.png
--rw-rw-rw-   0        0        0   148394 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/output_25_0.png
--rw-rw-rw-   0        0        0   100101 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/output_27_0.png
--rw-rw-rw-   0        0        0    16998 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/perf-may-suffer.png
--rw-rw-rw-   0        0        0    45876 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/rt_autocomplete.png
--rw-rw-rw-   0        0        0    24063 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/rt_autocomplete_internal.png
--rw-rw-rw-   0        0        0    12995 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/rt_dataset.svg
--rw-rw-rw-   0        0        0    21979 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/rt_dataset_indices.svg
--rw-rw-rw-   0        0        0     6885 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/rt_fastarray.svg
--rw-rw-rw-   0        0        0    83328 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/split-apply-combine-gray.svg
--rw-rw-rw-   0        0        0      770 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial.rst
--rw-rw-rw-   0        0        0    13974 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_accums.rst
--rw-rw-rw-   0        0        0     3913 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_cat_adv_instantiation.rst
--rw-rw-rw-   0        0        0     2914 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_cat_reduce.rst
--rw-rw-rw-   0        0        0    49655 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_categoricals.rst
--rw-rw-rw-   0        0        0     7129 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_concat.rst
--rw-rw-rw-   0        0        0    35411 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_datasets.rst
--rw-rw-rw-   0        0        0    32677 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_datetimes.rst
--rw-rw-rw-   0        0        0    15663 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_filters.rst
--rw-rw-rw-   0        0        0    13353 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_intro.rst
--rw-rw-rw-   0        0        0    13589 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_io.rst
--rw-rw-rw-   0        0        0    19446 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_merge.rst
--rw-rw-rw-   0        0        0    13997 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_missing_data.rst
--rw-rw-rw-   0        0        0      820 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_numpy_rt.rst
--rw-rw-rw-   0        0        0     2173 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_performance.rst
--rw-rw-rw-   0        0        0     4168 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_reshape.rst
--rw-rw-rw-   0        0        0     5501 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_sample_data.rst
--rw-rw-rw-   0        0        0    12285 2023-06-22 15:11:21.000000 riptable-1.9.1/docs/source/tutorial/tutorial_visualize.rst
--rw-rw-rw-   0        0        0      236 2023-06-22 15:11:21.000000 riptable-1.9.1/environment.yml
--rw-rw-rw-   0        0        0     3372 2023-06-22 15:11:21.000000 riptable-1.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       47 2023-06-22 15:11:21.000000 riptable-1.9.1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:03.989993 riptable-1.9.1/riptable/
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:04.021239 riptable-1.9.1/riptable/Utils/
--rw-rw-rw-   0        0        0        2 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/__init__.py
--rw-rw-rw-   0        0        0    25494 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/appdirs.py
--rw-rw-rw-   0        0        0     9278 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/common.py
--rw-rw-rw-   0        0        0     8728 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/conversion_utils.py
--rw-rw-rw-   0        0        0    21765 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/display_options.py
--rw-rw-rw-   0        0        0    13165 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/ipython_utils.py
--rw-rw-rw-   0        0        0     2250 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/pandas_utils.py
--rw-rw-rw-   0        0        0    18069 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/rt_display_nested.py
--rw-rw-rw-   0        0        0    14095 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/rt_display_properties.py
--rw-rw-rw-   0        0        0     3762 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/rt_metadata.py
--rw-rw-rw-   0        0        0    18357 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/rt_testdata.py
--rw-rw-rw-   0        0        0    11396 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/rt_testing.py
--rw-rw-rw-   0        0        0      501 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/teamcity_helper.py
--rw-rw-rw-   0        0        0     3056 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/Utils/terminalsize.py
--rw-rw-rw-   0        0        0     6318 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/__init__.py
--rw-rw-rw-   0        0        0       21 2023-06-22 15:25:03.000000 riptable-1.9.1/riptable/_version.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:04.036859 riptable-1.9.1/riptable/benchmarks/
--rw-rw-rw-   0        0        0     3959 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/__init__.py
--rw-rw-rw-   0        0        0      109 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/__main__.py
--rw-rw-rw-   0        0        0     8894 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/analysis.py
--rw-rw-rw-   0        0        0      725 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/bench_categorical.py
--rw-rw-rw-   0        0        0    11417 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/bench_grouping.py
--rw-rw-rw-   0        0        0    20287 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/bench_merge.py
--rw-rw-rw-   0        0        0    24713 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/bench_numpy.py
--rw-rw-rw-   0        0        0     1079 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/bench_operators.py
--rw-rw-rw-   0        0        0    46363 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/bench_primops.py
--rw-rw-rw-   0        0        0     6962 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/benchmark.py
--rw-rw-rw-   0        0        0    15951 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/main.py
--rw-rw-rw-   0        0        0     9889 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/rand_data.py
--rw-rw-rw-   0        0        0    19555 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/rand_keydata.py
--rw-rw-rw-   0        0        0      914 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/results.py
--rw-rw-rw-   0        0        0    13247 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/benchmarks/runner.py
--rw-rw-rw-   0        0        0     1475 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/config.py
--rw-rw-rw-   0        0        0     2685 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/conftest.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:04.036859 riptable-1.9.1/riptable/hypothesis_tests/
--rw-rw-rw-   0        0        0        9 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/hypothesis_tests/__init__.py
--rw-rw-rw-   0        0        0     2938 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/hypothesis_tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:04.036859 riptable-1.9.1/riptable/hypothesis_tests/strategies/
--rw-rw-rw-   0        0        0        0 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/hypothesis_tests/strategies/__init__.py
--rw-rw-rw-   0        0        0    19383 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/hypothesis_tests/strategies/categorical_strategy.py
--rw-rw-rw-   0        0        0    21811 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/hypothesis_tests/strategies/helper_strategies.py
--rw-rw-rw-   0        0        0    11783 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/hypothesis_tests/test_categorical_property.py
--rw-rw-rw-   0        0        0    86304 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/hypothesis_tests/test_riptide_numpy_equivalency.py
--rw-rw-rw-   0        0        0     3108 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/hypothesis_tests/test_rt_numpy_property.py
--rw-rw-rw-   0        0        0    10986 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/hypothesis_tests/test_sds_property.py
--rw-rw-rw-   0        0        0    12991 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/hypothesis_tests/test_ufunc_unary.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:04.052475 riptable-1.9.1/riptable/numba/
--rw-rw-rw-   0        0        0      224 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/numba/__init__.py
--rw-rw-rw-   0        0        0     2909 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/numba/indexing.py
--rw-rw-rw-   0        0        0     9430 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/numba/invalid_values.py
--rw-rw-rw-   0        0        0    50008 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_accum2.py
--rw-rw-rw-   0        0        0    19869 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_accumtable.py
--rw-rw-rw-   0        0        0     3812 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_algos.py
--rw-rw-rw-   0        0        0    24445 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_bin.py
--rw-rw-rw-   0        0        0   265096 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_categorical.py
--rw-rw-rw-   0        0        0     1076 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_compressedarray.py
--rw-rw-rw-   0        0        0     5758 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_csv.py
--rw-rw-rw-   0        0        0   299671 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_dataset.py
--rw-rw-rw-   0        0        0   275045 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_datetime.py
--rw-rw-rw-   0        0        0   106187 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_display.py
--rw-rw-rw-   0        0        0     2116 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_ema.py
--rw-rw-rw-   0        0        0    32335 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_enum.py
--rw-rw-rw-   0        0        0   250055 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_fastarray.py
--rw-rw-rw-   0        0        0    24106 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_fastarraynumba.py
--rw-rw-rw-   0        0        0    29848 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_groupby.py
--rw-rw-rw-   0        0        0    18239 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_groupbykeys.py
--rw-rw-rw-   0        0        0    27752 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_groupbynumba.py
--rw-rw-rw-   0        0        0   141314 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_groupbyops.py
--rw-rw-rw-   0        0        0   162009 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_grouping.py
--rw-rw-rw-   0        0        0    29765 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_hstack.py
--rw-rw-rw-   0        0        0     3345 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_imatrix.py
--rw-rw-rw-   0        0        0     4797 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_io.py
--rw-rw-rw-   0        0        0    23024 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_itemcontainer.py
--rw-rw-rw-   0        0        0    12137 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_ledger.py
--rw-rw-rw-   0        0        0    24920 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_matplotlib.py
--rw-rw-rw-   0        0        0   213710 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_merge.py
--rw-rw-rw-   0        0        0    93114 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_merge_asof.py
--rw-rw-rw-   0        0        0    11689 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_meta.py
--rw-rw-rw-   0        0        0    32617 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_misc.py
--rw-rw-rw-   0        0        0     1059 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_mlutils.py
--rw-rw-rw-   0        0        0    34329 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_multiset.py
--rw-rw-rw-   0        0        0   195890 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_numpy.py
--rw-rw-rw-   0        0        0    26902 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_pdataset.py
--rw-rw-rw-   0        0        0     1204 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_pgroupby.py
--rw-rw-rw-   0        0        0   135842 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_sds.py
--rw-rw-rw-   0        0        0     4463 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_sharedmemory.py
--rw-rw-rw-   0        0        0     2979 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_sort_cache.py
--rw-rw-rw-   0        0        0     7060 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_stats.py
--rw-rw-rw-   0        0        0    54138 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_str.py
--rw-rw-rw-   0        0        0   196456 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_struct.py
--rw-rw-rw-   0        0        0    17614 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_timers.py
--rw-rw-rw-   0        0        0    42160 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_timezone.py
--rw-rw-rw-   0        0        0    39281 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/rt_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:04.052475 riptable-1.9.1/riptable/test_tooling_integration/
--rw-rw-rw-   0        0        0       71 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/test_tooling_integration/__init__.py
--rw-rw-rw-   0        0        0    11006 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/test_tooling_integration/ipykernel_integration_test.py
--rw-rw-rw-   0        0        0    38590 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/test_tooling_integration/ipython_compatibility_test.py
--rw-rw-rw-   0        0        0    14870 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/test_tooling_integration/ipython_integration_test.py
--rw-rw-rw-   0        0        0      742 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/test_tooling_integration/run.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:04.052475 riptable-1.9.1/riptable/test_tooling_integration/test_display/
--rw-rw-rw-   0        0        0        9 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/test_tooling_integration/test_display/__init__.py
--rw-rw-rw-   0        0        0     1604 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/test_tooling_integration/test_display/test_display.py
--rw-rw-rw-   0        0        0     4668 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/test_tooling_integration/test_display/vnu_checker.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:04.052475 riptable-1.9.1/riptable/testing/
--rw-rw-rw-   0        0        0    14911 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/testing/array_assert.py
--rw-rw-rw-   0        0        0     5788 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/testing/randgen.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:04.130633 riptable-1.9.1/riptable/tests/
--rw-rw-rw-   0        0        0       27 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/__init__.py
--rw-rw-rw-   0        0        0     6646 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/generator_categorical_unit_test.py
--rw-rw-rw-   0        0        0     6456 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/generator_groupby_unit_test.py
--rw-rw-rw-   0        0        0     3933 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/groupby_categorical_unit_test_parameters.py
--rw-rw-rw-   0        0        0     5076 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/groupby_unit_test_parameters.py
--rw-rw-rw-   0        0        0      593 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/run.py
--rw-rw-rw-   0        0        0     1387 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/runall.py
--rw-rw-rw-   0        0        0    27730 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_accum2.py
--rw-rw-rw-   0        0        0     5075 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_accumtable.py
--rw-rw-rw-   0        0        0    20462 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_apply.py
--rw-rw-rw-   0        0        0     8459 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_base_function.py
--rw-rw-rw-   0        0        0     2553 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_bitcount.py
--rw-rw-rw-   0        0        0   140662 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical.py
--rw-rw-rw-   0        0        0    19605 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical_autotest_aggregated_functions.py
--rw-rw-rw-   0        0        0     1141 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical_base_index.py
--rw-rw-rw-   0        0        0     3312 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical_dtype.py
--rw-rw-rw-   0        0        0    16622 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical_filter_invalid.py
--rw-rw-rw-   0        0        0     4124 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical_functions.py
--rw-rw-rw-   0        0        0    38234 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical_groupby.py
--rw-rw-rw-   0        0        0     3430 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical_keywords.py
--rw-rw-rw-   0        0        0     3544 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical_modify.py
--rw-rw-rw-   0        0        0    11480 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical_ordered.py
--rw-rw-rw-   0        0        0     5883 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical_setitem.py
--rw-rw-rw-   0        0        0     7248 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical_sort_order.py
--rw-rw-rw-   0        0        0    19221 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_categorical_values.py
--rw-rw-rw-   0        0        0     7283 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_conversion_utils.py
--rw-rw-rw-   0        0        0     4894 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_csv.py
--rw-rw-rw-   0        0        0     7141 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_cut.py
--rw-rw-rw-   0        0        0    99757 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_dataset.py
--rw-rw-rw-   0        0        0    20216 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_dataset_slicing.py
--rw-rw-rw-   0        0        0    17508 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_date.py
--rw-rw-rw-   0        0        0   114419 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_datetime.py
--rw-rw-rw-   0        0        0    15276 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_datetime_math.py
--rw-rw-rw-   0        0        0    69259 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_fastarray.py
--rw-rw-rw-   0        0        0     6396 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_fastarray_bn.py
--rw-rw-rw-   0        0        0     3120 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_fastarray_constructor.py
--rw-rw-rw-   0        0        0    25031 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_fastarray_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:04.146228 riptable-1.9.1/riptable/tests/test_files/
--rw-rw-rw-   0        0        0      739 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_files/groupby1_ex3.pickle
--rw-rw-rw-   0        0        0     2328 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_files/unicode_ex1.csv
--rw-rw-rw-   0        0        0     2334 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_files/unicode_ex2.csv
--rw-rw-rw-   0        0        0     2474 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_files/unicode_ex3.csv
--rw-rw-rw-   0        0        0     6831 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_flatten.py
--rw-rw-rw-   0        0        0    35665 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_groupby.py
--rw-rw-rw-   0        0        0   161516 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_groupby_autotest_aggregated_functions.py
--rw-rw-rw-   0        0        0     5882 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_groupby_functions.py
--rw-rw-rw-   0        0        0     3443 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_groupby_simple_multikey.py
--rw-rw-rw-   0        0        0    56796 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_groupbyops.py
--rw-rw-rw-   0        0        0    25055 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_grouping.py
--rw-rw-rw-   0        0        0      105 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_hstack.py
--rw-rw-rw-   0        0        0    20277 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_interop_pyarrow.py
--rw-rw-rw-   0        0        0    23500 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_ismember.py
--rw-rw-rw-   0        0        0    12621 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_lexsort.py
--rw-rw-rw-   0        0        0   252691 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_merge.py
--rw-rw-rw-   0        0        0    24228 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_merge_asof.py
--rw-rw-rw-   0        0        0     7247 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_meta.py
--rw-rw-rw-   0        0        0    11644 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_multiset.py
--rw-rw-rw-   0        0        0     1086 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_pandas_utils.py
--rw-rw-rw-   0        0        0    11833 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_pdataset.py
--rw-rw-rw-   0        0        0     3664 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_pgroupby.py
--rw-rw-rw-   0        0        0     5296 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_restore_subclass.py
--rw-rw-rw-   0        0        0     7000 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_riptide_cpp.py
--rw-rw-rw-   0        0        0    21887 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_rtnumpy.py
--rw-rw-rw-   0        0        0     5435 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_rtutils.py
--rw-rw-rw-   0        0        0    80879 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_saveload.py
--rw-rw-rw-   0        0        0     1504 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_scalar.py
--rw-rw-rw-   0        0        0     3528 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_sds.py
--rw-rw-rw-   0        0        0    40713 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_sprint_fastarray.py
--rw-rw-rw-   0        0        0    26324 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_str.py
--rw-rw-rw-   0        0        0    33302 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_struct.py
--rw-rw-rw-   0        0        0      791 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_timewindow.py
--rw-rw-rw-   0        0        0    92861 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_ufunc2.py
--rw-rw-rw-   0        0        0     4828 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_unique.py
--rw-rw-rw-   0        0        0     5654 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/test_utils.py
--rw-rw-rw-   0        0        0     3380 2023-06-22 15:11:21.000000 riptable-1.9.1/riptable/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:25:04.005647 riptable-1.9.1/riptable.egg-info/
--rw-rw-rw-   0        0        0      660 2023-06-22 15:25:03.000000 riptable-1.9.1/riptable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7978 2023-06-22 15:25:03.000000 riptable-1.9.1/riptable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 15:25:03.000000 riptable-1.9.1/riptable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-22 15:25:03.000000 riptable-1.9.1/riptable.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       99 2023-06-22 15:25:03.000000 riptable-1.9.1/riptable.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 15:25:03.000000 riptable-1.9.1/riptable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-06-22 15:11:21.000000 riptable-1.9.1/runtest.py
--rw-rw-rw-   0        0        0       42 2023-06-22 15:25:04.146228 riptable-1.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1507 2023-06-22 15:11:21.000000 riptable-1.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:47.102224 riptable-1.9.2/
+-rw-rw-rw-   0        0        0      291 2023-07-12 14:30:39.000000 riptable-1.9.2/.editorconfig
+-rw-rw-rw-   0        0        0      196 2023-07-12 14:30:39.000000 riptable-1.9.2/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:46.836595 riptable-1.9.2/.github/
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:46.852221 riptable-1.9.2/.github/workflows/
+-rw-rw-rw-   0        0        0     8370 2023-07-12 14:30:39.000000 riptable-1.9.2/.github/workflows/python-package.yml
+-rw-rw-rw-   0        0        0     2110 2023-07-12 14:30:39.000000 riptable-1.9.2/.gitignore
+-rw-rw-rw-   0        0        0      309 2023-07-12 14:30:39.000000 riptable-1.9.2/BUILDNOTES.txt
+-rw-rw-rw-   0        0        0     2634 2023-07-12 14:30:39.000000 riptable-1.9.2/LICENSE
+-rw-rw-rw-   0        0        0     3464 2023-07-12 14:30:39.000000 riptable-1.9.2/LICENSES-thirdparty.md
+-rw-rw-rw-   0        0        0      196 2023-07-12 14:30:39.000000 riptable-1.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      660 2023-07-12 14:48:47.102224 riptable-1.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6110 2023-07-12 14:30:39.000000 riptable-1.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:46.852221 riptable-1.9.2/conda_recipe/
+-rw-rw-rw-   0        0        0       19 2023-07-12 14:30:39.000000 riptable-1.9.2/conda_recipe/conda_build_config.yaml
+-rw-rw-rw-   0        0        0     1804 2023-07-12 14:30:39.000000 riptable-1.9.2/conda_recipe/meta.yaml
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:46.852221 riptable-1.9.2/dev_tools/
+-rw-rw-rw-   0        0        0     4110 2023-07-12 14:30:39.000000 riptable-1.9.2/dev_tools/gen_requirements.py
+-rw-rw-rw-   0        0        0    25367 2023-07-12 14:30:39.000000 riptable-1.9.2/dev_tools/validate_docstrings.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:46.867847 riptable-1.9.2/docs/
+-rw-rw-rw-   0        0        0      901 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0      658 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/Makefile
+-rw-rw-rw-   0        0        0     2979 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/THREADING.md
+-rwxrwxrwx   0        0        0      799 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/make.bat
+-rw-rw-rw-   0        0        0     1085 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/riptable_logo.PNG
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:46.867847 riptable-1.9.2/docs/source/
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:46.867847 riptable-1.9.2/docs/source/_static/
+-rw-rw-rw-   0        0        0        0 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/_static/.keep
+-rw-rw-rw-   0        0        0    14482 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/benchmarking.rst
+-rw-rw-rw-   0        0        0     4478 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/conf.py
+-rw-rw-rw-   0        0        0      487 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/index.rst
+-rw-rw-rw-   0        0        0       68 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/modules.rst
+-rw-rw-rw-   0        0        0     6795 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/riptable.rst
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:46.899097 riptable-1.9.2/docs/source/tutorial/
+-rw-rw-rw-   0        0        0    23344 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/RiptableExercises.ipynb
+-rw-rw-rw-   0        0        0    95601 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/RiptableSolutions.ipynb
+-rw-rw-rw-   0        0        0    35605 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/output_11_0.png
+-rw-rw-rw-   0        0        0     5827 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/output_13_0.png
+-rw-rw-rw-   0        0        0    60197 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/output_15_0.png
+-rw-rw-rw-   0        0        0   148394 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/output_25_0.png
+-rw-rw-rw-   0        0        0   100101 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/output_27_0.png
+-rw-rw-rw-   0        0        0    16998 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/perf-may-suffer.png
+-rw-rw-rw-   0        0        0    45876 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/rt_autocomplete.png
+-rw-rw-rw-   0        0        0    24063 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/rt_autocomplete_internal.png
+-rw-rw-rw-   0        0        0    12995 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/rt_dataset.svg
+-rw-rw-rw-   0        0        0    21979 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/rt_dataset_indices.svg
+-rw-rw-rw-   0        0        0     6885 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/rt_fastarray.svg
+-rw-rw-rw-   0        0        0    83328 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/split-apply-combine-gray.svg
+-rw-rw-rw-   0        0        0      770 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial.rst
+-rw-rw-rw-   0        0        0    13974 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_accums.rst
+-rw-rw-rw-   0        0        0     3913 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_cat_adv_instantiation.rst
+-rw-rw-rw-   0        0        0     2914 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_cat_reduce.rst
+-rw-rw-rw-   0        0        0    49655 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_categoricals.rst
+-rw-rw-rw-   0        0        0     7129 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_concat.rst
+-rw-rw-rw-   0        0        0    35411 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_datasets.rst
+-rw-rw-rw-   0        0        0    32677 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_datetimes.rst
+-rw-rw-rw-   0        0        0    15663 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_filters.rst
+-rw-rw-rw-   0        0        0    13353 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_intro.rst
+-rw-rw-rw-   0        0        0    13589 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_io.rst
+-rw-rw-rw-   0        0        0    19446 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_merge.rst
+-rw-rw-rw-   0        0        0    13997 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_missing_data.rst
+-rw-rw-rw-   0        0        0      820 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_numpy_rt.rst
+-rw-rw-rw-   0        0        0     2173 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_performance.rst
+-rw-rw-rw-   0        0        0     4168 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_reshape.rst
+-rw-rw-rw-   0        0        0     5501 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_sample_data.rst
+-rw-rw-rw-   0        0        0    12285 2023-07-12 14:30:39.000000 riptable-1.9.2/docs/source/tutorial/tutorial_visualize.rst
+-rw-rw-rw-   0        0        0      236 2023-07-12 14:30:39.000000 riptable-1.9.2/environment.yml
+-rw-rw-rw-   0        0        0     3372 2023-07-12 14:30:39.000000 riptable-1.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       47 2023-07-12 14:30:39.000000 riptable-1.9.2/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:46.945969 riptable-1.9.2/riptable/
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:46.977223 riptable-1.9.2/riptable/Utils/
+-rw-rw-rw-   0        0        0        2 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/__init__.py
+-rw-rw-rw-   0        0        0    25494 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/appdirs.py
+-rw-rw-rw-   0        0        0     9278 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/common.py
+-rw-rw-rw-   0        0        0     8728 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/conversion_utils.py
+-rw-rw-rw-   0        0        0    21765 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/display_options.py
+-rw-rw-rw-   0        0        0    13165 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/ipython_utils.py
+-rw-rw-rw-   0        0        0     2250 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/pandas_utils.py
+-rw-rw-rw-   0        0        0    18069 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/rt_display_nested.py
+-rw-rw-rw-   0        0        0    14095 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/rt_display_properties.py
+-rw-rw-rw-   0        0        0     3762 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/rt_metadata.py
+-rw-rw-rw-   0        0        0    18357 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/rt_testdata.py
+-rw-rw-rw-   0        0        0    11396 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/rt_testing.py
+-rw-rw-rw-   0        0        0      501 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/teamcity_helper.py
+-rw-rw-rw-   0        0        0     3056 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/Utils/terminalsize.py
+-rw-rw-rw-   0        0        0     6318 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-07-12 14:48:46.000000 riptable-1.9.2/riptable/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:46.992848 riptable-1.9.2/riptable/benchmarks/
+-rw-rw-rw-   0        0        0     3959 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/__init__.py
+-rw-rw-rw-   0        0        0      109 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/__main__.py
+-rw-rw-rw-   0        0        0     8894 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/analysis.py
+-rw-rw-rw-   0        0        0      725 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/bench_categorical.py
+-rw-rw-rw-   0        0        0    11417 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/bench_grouping.py
+-rw-rw-rw-   0        0        0    20287 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/bench_merge.py
+-rw-rw-rw-   0        0        0    24713 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/bench_numpy.py
+-rw-rw-rw-   0        0        0     1079 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/bench_operators.py
+-rw-rw-rw-   0        0        0    46363 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/bench_primops.py
+-rw-rw-rw-   0        0        0     6962 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/benchmark.py
+-rw-rw-rw-   0        0        0    15951 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/main.py
+-rw-rw-rw-   0        0        0     9889 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/rand_data.py
+-rw-rw-rw-   0        0        0    19555 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/rand_keydata.py
+-rw-rw-rw-   0        0        0      914 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/results.py
+-rw-rw-rw-   0        0        0    13247 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/benchmarks/runner.py
+-rw-rw-rw-   0        0        0     1475 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/config.py
+-rw-rw-rw-   0        0        0     2685 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:47.008471 riptable-1.9.2/riptable/hypothesis_tests/
+-rw-rw-rw-   0        0        0        9 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/hypothesis_tests/__init__.py
+-rw-rw-rw-   0        0        0     2938 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/hypothesis_tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:47.008471 riptable-1.9.2/riptable/hypothesis_tests/strategies/
+-rw-rw-rw-   0        0        0        0 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/hypothesis_tests/strategies/__init__.py
+-rw-rw-rw-   0        0        0    19383 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/hypothesis_tests/strategies/categorical_strategy.py
+-rw-rw-rw-   0        0        0    21811 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/hypothesis_tests/strategies/helper_strategies.py
+-rw-rw-rw-   0        0        0    11783 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/hypothesis_tests/test_categorical_property.py
+-rw-rw-rw-   0        0        0    86304 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/hypothesis_tests/test_riptide_numpy_equivalency.py
+-rw-rw-rw-   0        0        0     3108 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/hypothesis_tests/test_rt_numpy_property.py
+-rw-rw-rw-   0        0        0    10986 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/hypothesis_tests/test_sds_property.py
+-rw-rw-rw-   0        0        0    12991 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/hypothesis_tests/test_ufunc_unary.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:47.008471 riptable-1.9.2/riptable/numba/
+-rw-rw-rw-   0        0        0      224 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/numba/__init__.py
+-rw-rw-rw-   0        0        0     2909 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/numba/indexing.py
+-rw-rw-rw-   0        0        0     9430 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/numba/invalid_values.py
+-rw-rw-rw-   0        0        0    50008 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_accum2.py
+-rw-rw-rw-   0        0        0    19869 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_accumtable.py
+-rw-rw-rw-   0        0        0     3812 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_algos.py
+-rw-rw-rw-   0        0        0    24445 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_bin.py
+-rw-rw-rw-   0        0        0   265096 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_categorical.py
+-rw-rw-rw-   0        0        0     1076 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_compressedarray.py
+-rw-rw-rw-   0        0        0     5758 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_csv.py
+-rw-rw-rw-   0        0        0   299671 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_dataset.py
+-rw-rw-rw-   0        0        0   275341 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_datetime.py
+-rw-rw-rw-   0        0        0   106187 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_display.py
+-rw-rw-rw-   0        0        0     2116 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_ema.py
+-rw-rw-rw-   0        0        0    32335 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_enum.py
+-rw-rw-rw-   0        0        0   250056 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_fastarray.py
+-rw-rw-rw-   0        0        0    24106 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_fastarraynumba.py
+-rw-rw-rw-   0        0        0    29848 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_groupby.py
+-rw-rw-rw-   0        0        0    18239 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_groupbykeys.py
+-rw-rw-rw-   0        0        0    27752 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_groupbynumba.py
+-rw-rw-rw-   0        0        0   141314 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_groupbyops.py
+-rw-rw-rw-   0        0        0   162009 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_grouping.py
+-rw-rw-rw-   0        0        0    29765 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_hstack.py
+-rw-rw-rw-   0        0        0     3345 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_imatrix.py
+-rw-rw-rw-   0        0        0     4797 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_io.py
+-rw-rw-rw-   0        0        0    23024 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_itemcontainer.py
+-rw-rw-rw-   0        0        0    12137 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_ledger.py
+-rw-rw-rw-   0        0        0    24920 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_matplotlib.py
+-rw-rw-rw-   0        0        0   213710 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_merge.py
+-rw-rw-rw-   0        0        0    93114 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_merge_asof.py
+-rw-rw-rw-   0        0        0    11689 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_meta.py
+-rw-rw-rw-   0        0        0    32617 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_misc.py
+-rw-rw-rw-   0        0        0     1059 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_mlutils.py
+-rw-rw-rw-   0        0        0    34329 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_multiset.py
+-rw-rw-rw-   0        0        0   195891 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_numpy.py
+-rw-rw-rw-   0        0        0    26902 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_pdataset.py
+-rw-rw-rw-   0        0        0     1204 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_pgroupby.py
+-rw-rw-rw-   0        0        0   135842 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_sds.py
+-rw-rw-rw-   0        0        0     4463 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_sharedmemory.py
+-rw-rw-rw-   0        0        0     2979 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_sort_cache.py
+-rw-rw-rw-   0        0        0     7060 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_stats.py
+-rw-rw-rw-   0        0        0    54138 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_str.py
+-rw-rw-rw-   0        0        0   196456 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_struct.py
+-rw-rw-rw-   0        0        0    17614 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_timers.py
+-rw-rw-rw-   0        0        0    42160 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_timezone.py
+-rw-rw-rw-   0        0        0    39281 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/rt_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:47.008471 riptable-1.9.2/riptable/test_tooling_integration/
+-rw-rw-rw-   0        0        0       71 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/test_tooling_integration/__init__.py
+-rw-rw-rw-   0        0        0    11006 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/test_tooling_integration/ipykernel_integration_test.py
+-rw-rw-rw-   0        0        0    38590 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/test_tooling_integration/ipython_compatibility_test.py
+-rw-rw-rw-   0        0        0    14870 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/test_tooling_integration/ipython_integration_test.py
+-rw-rw-rw-   0        0        0      742 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/test_tooling_integration/run.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:47.008471 riptable-1.9.2/riptable/test_tooling_integration/test_display/
+-rw-rw-rw-   0        0        0        9 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/test_tooling_integration/test_display/__init__.py
+-rw-rw-rw-   0        0        0     1604 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/test_tooling_integration/test_display/test_display.py
+-rw-rw-rw-   0        0        0     4668 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/test_tooling_integration/test_display/vnu_checker.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:47.024097 riptable-1.9.2/riptable/testing/
+-rw-rw-rw-   0        0        0    14911 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/testing/array_assert.py
+-rw-rw-rw-   0        0        0     5788 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/testing/randgen.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:47.086600 riptable-1.9.2/riptable/tests/
+-rw-rw-rw-   0        0        0       27 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/__init__.py
+-rw-rw-rw-   0        0        0     6646 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/generator_categorical_unit_test.py
+-rw-rw-rw-   0        0        0     6456 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/generator_groupby_unit_test.py
+-rw-rw-rw-   0        0        0     3933 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/groupby_categorical_unit_test_parameters.py
+-rw-rw-rw-   0        0        0     5076 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/groupby_unit_test_parameters.py
+-rw-rw-rw-   0        0        0      593 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/run.py
+-rw-rw-rw-   0        0        0     1387 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/runall.py
+-rw-rw-rw-   0        0        0    27730 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_accum2.py
+-rw-rw-rw-   0        0        0     5075 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_accumtable.py
+-rw-rw-rw-   0        0        0    20462 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_apply.py
+-rw-rw-rw-   0        0        0     8459 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_base_function.py
+-rw-rw-rw-   0        0        0     2553 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_bitcount.py
+-rw-rw-rw-   0        0        0   140662 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical.py
+-rw-rw-rw-   0        0        0    19605 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical_autotest_aggregated_functions.py
+-rw-rw-rw-   0        0        0     1141 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical_base_index.py
+-rw-rw-rw-   0        0        0     3312 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical_dtype.py
+-rw-rw-rw-   0        0        0    16622 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical_filter_invalid.py
+-rw-rw-rw-   0        0        0     4124 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical_functions.py
+-rw-rw-rw-   0        0        0    38234 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical_groupby.py
+-rw-rw-rw-   0        0        0     3430 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical_keywords.py
+-rw-rw-rw-   0        0        0     3544 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical_modify.py
+-rw-rw-rw-   0        0        0    11480 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical_ordered.py
+-rw-rw-rw-   0        0        0     5883 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical_setitem.py
+-rw-rw-rw-   0        0        0     7248 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical_sort_order.py
+-rw-rw-rw-   0        0        0    19221 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_categorical_values.py
+-rw-rw-rw-   0        0        0     7283 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_conversion_utils.py
+-rw-rw-rw-   0        0        0     4894 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_csv.py
+-rw-rw-rw-   0        0        0     7141 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_cut.py
+-rw-rw-rw-   0        0        0    99757 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_dataset.py
+-rw-rw-rw-   0        0        0    20216 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_dataset_slicing.py
+-rw-rw-rw-   0        0        0    17508 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_date.py
+-rw-rw-rw-   0        0        0   115627 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_datetime.py
+-rw-rw-rw-   0        0        0    15276 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_datetime_math.py
+-rw-rw-rw-   0        0        0    69259 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_fastarray.py
+-rw-rw-rw-   0        0        0     6396 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_fastarray_bn.py
+-rw-rw-rw-   0        0        0     3120 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_fastarray_constructor.py
+-rw-rw-rw-   0        0        0    25031 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_fastarray_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:47.102224 riptable-1.9.2/riptable/tests/test_files/
+-rw-rw-rw-   0        0        0      739 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_files/groupby1_ex3.pickle
+-rw-rw-rw-   0        0        0     2328 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_files/unicode_ex1.csv
+-rw-rw-rw-   0        0        0     2334 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_files/unicode_ex2.csv
+-rw-rw-rw-   0        0        0     2474 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_files/unicode_ex3.csv
+-rw-rw-rw-   0        0        0     6831 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_flatten.py
+-rw-rw-rw-   0        0        0    35665 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_groupby.py
+-rw-rw-rw-   0        0        0   161516 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_groupby_autotest_aggregated_functions.py
+-rw-rw-rw-   0        0        0     5882 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_groupby_functions.py
+-rw-rw-rw-   0        0        0     3443 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_groupby_simple_multikey.py
+-rw-rw-rw-   0        0        0    56796 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_groupbyops.py
+-rw-rw-rw-   0        0        0    25055 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_grouping.py
+-rw-rw-rw-   0        0        0      105 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_hstack.py
+-rw-rw-rw-   0        0        0    20277 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_interop_pyarrow.py
+-rw-rw-rw-   0        0        0    23500 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_ismember.py
+-rw-rw-rw-   0        0        0    12621 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_lexsort.py
+-rw-rw-rw-   0        0        0   252691 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_merge.py
+-rw-rw-rw-   0        0        0    24228 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_merge_asof.py
+-rw-rw-rw-   0        0        0     7247 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_meta.py
+-rw-rw-rw-   0        0        0    11644 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_multiset.py
+-rw-rw-rw-   0        0        0     1086 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_pandas_utils.py
+-rw-rw-rw-   0        0        0    11833 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_pdataset.py
+-rw-rw-rw-   0        0        0     3664 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_pgroupby.py
+-rw-rw-rw-   0        0        0     5296 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_restore_subclass.py
+-rw-rw-rw-   0        0        0     7000 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_riptide_cpp.py
+-rw-rw-rw-   0        0        0    21887 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_rtnumpy.py
+-rw-rw-rw-   0        0        0     5435 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_rtutils.py
+-rw-rw-rw-   0        0        0    80879 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_saveload.py
+-rw-rw-rw-   0        0        0     1504 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_scalar.py
+-rw-rw-rw-   0        0        0     3528 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_sds.py
+-rw-rw-rw-   0        0        0    40713 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_sprint_fastarray.py
+-rw-rw-rw-   0        0        0    26324 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_str.py
+-rw-rw-rw-   0        0        0    33302 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_struct.py
+-rw-rw-rw-   0        0        0      791 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_timewindow.py
+-rw-rw-rw-   0        0        0    92861 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_ufunc2.py
+-rw-rw-rw-   0        0        0     4828 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_unique.py
+-rw-rw-rw-   0        0        0     5654 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/test_utils.py
+-rw-rw-rw-   0        0        0     3380 2023-07-12 14:30:39.000000 riptable-1.9.2/riptable/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:48:46.961597 riptable-1.9.2/riptable.egg-info/
+-rw-rw-rw-   0        0        0      660 2023-07-12 14:48:46.000000 riptable-1.9.2/riptable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7978 2023-07-12 14:48:46.000000 riptable-1.9.2/riptable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 14:48:46.000000 riptable-1.9.2/riptable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-12 14:48:46.000000 riptable-1.9.2/riptable.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       99 2023-07-12 14:48:46.000000 riptable-1.9.2/riptable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 14:48:46.000000 riptable-1.9.2/riptable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-07-12 14:30:39.000000 riptable-1.9.2/runtest.py
+-rw-rw-rw-   0        0        0       42 2023-07-12 14:48:47.102224 riptable-1.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1507 2023-07-12 14:30:39.000000 riptable-1.9.2/setup.py
```

### Comparing `riptable-1.9.1/.github/workflows/python-package.yml` & `riptable-1.9.2/.github/workflows/python-package.yml`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 jobs:
   pypi_build:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 30
     defaults:
       run:
         shell: bash -l {0}
-        #working-directory: ./
     strategy:
       matrix:
         os: [ubuntu-latest, windows-2019]
         python-version: [3.9, "3.10", "3.11"]
         numpy-version: [1.23]
     steps:
       - name: Checkout repo
@@ -33,25 +32,26 @@
       - name: Setup Miniconda
         env:
           ACTIONS_ALLOW_UNSECURE_COMMANDS: "true"
         uses: conda-incubator/setup-miniconda@v2
         with:
           activate-environment: "pypi_build"
           python-version: ${{ matrix.python-version }}
+          mamba-version: "*"
           auto-update-conda: true
           channels: conda-forge
           channel-priority: flexible
           show-channel-urls: true
       - name: Configure Conda
         run: |
           conda config --set unsatisfiable_hints_check_depth 0 # setting unsatisfiable_hints=False is broken
       - name: Install dependencies
         run: |
           python dev_tools/gen_requirements.py --out pypi_reqs.txt pypi
-          conda create -q -y -n pypi_build python=${{ matrix.python-version }} --file pypi_reqs.txt
+          mamba create -q -y -n pypi_build python=${{ matrix.python-version }} --file pypi_reqs.txt
       - name: Install core dependencies
         # Needed for pip install of riptide_cpp from sdist
         run: |
           python -m pip install --upgrade pip
           pip install numpy==${{ matrix.numpy-version }}.*
           # Pin build-constraints for numpy (see https://github.com/pypa/pip/issues/9542#issuecomment-1242347397)
           echo "numpy==${{ matrix.numpy-version }}.*" > constraints.txt
@@ -87,15 +87,15 @@
         uses: actions/upload-artifact@v3
         with:
           name: build-artifacts
           path: dist/
           if-no-files-found: error
 
   pypi_deploy:
-    if: ${{ github.event_name == 'workflow_dispatch' && github.ref == 'refs/heads/master' }}
+    if: ${{ github.event_name == 'workflow_dispatch' && github.ref_type == 'tag' }}
     # since riptable is all python source code, only a source build is required from one os
     needs: [pypi_build, conda_build]
     runs-on: ubuntu-latest
     steps:
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
@@ -115,14 +115,17 @@
           TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
         run: |
           set -ex
           twine upload dist/* --verbose
 
   conda_build:
     runs-on: ${{ matrix.os }}
+    defaults:
+      run:
+        shell: bash -l {0}
     strategy:
       matrix:
         os: ["ubuntu-latest", "windows-2019"]
         python-version: [3.9, "3.10", "3.11"]
     env:
       python_version: 3.9
       ANACONDA_USER: rtosholdings
@@ -134,61 +137,71 @@
       - name: Setup Miniconda
         uses: conda-incubator/setup-miniconda@v2
         env:
           ACTIONS_ALLOW_UNSECURE_COMMANDS: "true"
         with:
           activate-environment: "conda_build"
           python-version: ${{ env.python_version }}
+          mamba-version: "*"
           auto-update-conda: true
           channels: conda-forge
           channel-priority: flexible
           show-channel-urls: true
-      - name: Install dependencies
-        shell: bash -l {0}
+      - name: Install dependencies (Windows)
+        if: ${{ matrix.os == 'windows-2019' }}
         run: |
           set -ex
           python dev_tools/gen_requirements.py --out conda_reqs.txt conda
-          conda create -q -y -n conda_build python=${{ env.python-version }} --file conda_reqs.txt
-      - name: Build Package
-        shell: bash -l {0}
+          # boa-0.15 broken for Windows (see https://github.com/conda-forge/conda-forge.github.io/issues/1960)
+          mamba install -q -y --override-channels -c conda-forge -c defaults boa=0.14 --file conda_reqs.txt
+          mamba list
+      - name: Install dependencies (Linux)
+        if: ${{ matrix.os == 'ubuntu-latest' }}
+        run: |
+          set -ex
+          python dev_tools/gen_requirements.py --out conda_reqs.txt conda
+          mamba install -q -y --override-channels -c conda-forge -c defaults --file conda_reqs.txt
+          mamba list
+      - name: Build package
         run: |
           set -ex
           export BUILD_VERSION=$(python -c "from setuptools_scm import get_version; print(get_version(version_scheme='post-release'))")
           mkdir conda_pkgs_output
           echo "python: " ${{ matrix.python-version }} > ./conda_variant.yaml
-          conda build conda_recipe -c ${ANACONDA_USER} --output-folder ./conda_pkgs_output --variant-config-files ./conda_variant.yaml
+          conda mambabuild conda_recipe --override-channels -c ${ANACONDA_USER} -c conda-forge -c defaults --output-folder ./conda_pkgs_output --variant-config-files ./conda_variant.yaml
       - name: Publish artifacts
         uses: actions/upload-artifact@v3
         with:
           name: conda-build-artifacts
           path: conda_pkgs_output/*/riptable-*.tar.bz2
           if-no-files-found: "error"
 
   conda_deploy:
-    if: ${{ github.event_name == 'workflow_dispatch' && github.ref == 'refs/heads/master' }}
+    if: ${{ github.event_name == 'workflow_dispatch' && github.ref_type == 'tag' }}
     needs: [pypi_build, conda_build]
     runs-on: ubuntu-latest
     env:
       ANACONDA_USER: rtosholdings
       ANACONDA_TOKEN: ${{ secrets.anaconda_token }}
     steps:
       - name: Setup Miniconda
         uses: conda-incubator/setup-miniconda@v2
         env:
           ACTIONS_ALLOW_UNSECURE_COMMANDS: "true"
         with:
           activate-environment: "conda_deploy"
+          mamba-version: "*"
           auto-update-conda: true
           channels: conda-forge
           channel-priority: flexible
           show-channel-urls: true
       - name: Install dependencies
         shell: bash -l {0}
         run: |
-          conda install anaconda-client -q -y
+          mamba install anaconda-client -q -y
       - name: Download build artifacts
         uses: actions/download-artifact@v3
         with:
           name: conda-build-artifacts
           path: conda_pkgs_output/
       - name: Upload to Anaconda
         shell: bash -l {0}
```

### Comparing `riptable-1.9.1/.gitignore` & `riptable-1.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/LICENSE` & `riptable-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/LICENSES-thirdparty.md` & `riptable-1.9.2/LICENSES-thirdparty.md`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/PKG-INFO` & `riptable-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riptable
-Version: 1.9.1
+Version: 1.9.2
 Summary: Python Package for riptable studies framework
 Home-page: https://github.com/rtosholdings/riptable
 Author: RTOS Holdings
 Author-email: rtosholdings-bot@sig.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `riptable-1.9.1/README.md` & `riptable-1.9.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # RipTable
+
 ![](docs/riptable_logo.PNG)
 
 All in one, high performance 64 bit python analytics engine for numpy arrays with multithreaded support.
 
-Support for Python 3.6, 3.7, 3.8 on 64 bit Linux, Windows, and Mac OS.
+Support for Python 3.9 thru 3.11 on 64 bit Linux, Windows, and Mac OS.
 
 Enhances or replaces numpy, pandas, and includes high speed cross platform SDS file format.
-RipTable can often crunch numbers at 1.5x to 10x the speed of numpy or pandas.  
+RipTable can often crunch numbers at 1.5x to 10x the speed of numpy or pandas.
 
 Maximum speed is achieved through the use of **[vector instrinsics](https://software.intel.com/sites/landingpage/IntrinsicsGuide/)**: hand rolled loops, using [AVX-256](https://en.wikipedia.org/wiki/Advanced_Vector_Extensions#CPUs_with_AVX2)  with [AVX-512](https://en.wikipedia.org/wiki/AVX-512) support coming; **[parallel computing](https://www.drdobbs.com/go-parallel/article/print?articleId=212903586)**: for large arrays, multiple threads are deployed; **[recycling](https://en.wikipedia.org/wiki/Garbage_collection_(computer_science))**: built in array garbage collection; **[hashing](https://en.wikipedia.org/wiki/Hash_function)** and **parallel sorts** for core algorithms.
 
-Install 
+Install
 -------
+
 ```
 pip install riptable
 ```
 
 Documentation: [readthedocs](https://riptable.readthedocs.io/en/latest/py-modindex.html)
 
 Basic Concepts and Classes
 --------------------------
+
 **[FastArray](https://riptable.readthedocs.io/en/latest/riptable.html#riptable.rt_fastarray.FastArray)**: subclasses from a numpy array with builtin multithreaded number crunching.  All scikit routines that expect a numpy array will also accept a FastArray since it is subclassed.  isinstance(fastarray, np.ndarray) will return True.
 
 **[Dataset](https://riptable.readthedocs.io/en/latest/riptable.html#module-riptable.rt_dataset)**: replaces the pandas DataFrame class and holds equal row length numpy arrays (including > 1 dimension).
 
 **Struct**: replaces the pandas Series class.  A **Struct** is a grab bag collection class that **Dataset** subclasses from.
 
 **[Categorical](https://riptable.readthedocs.io/en/latest/riptable.html#module-riptable.rt_categorical)**: replaces both pandas groupby and Categorical class.  RipTable **Categoricals** are multikey, filterable, stackable, archivable, and can chain computations such as apply_reduce loops.  They can do everything groupby can plus more.
@@ -31,68 +34,81 @@
 **Date/Time Classes**: DateTimeNano, Date, TimeSpan, and DateSpan are designed more like Java, C++, or C# classes.  Replaces most numpy and pandas date time classes.
 
 **Accum2/AccumTable**: For cross tabulation.
 
 **[SDS](https://riptable.readthedocs.io/en/latest/riptable.html#riptable.rt_sds.save_sds)**: a new file format which can stack multiple datasets in multiple files with [zstd](https://github.com/facebook/zstd) compression, threads, and no extra memory copies.  SDS also supports loading and writing datasets to shared memory.
 
 Getting Started
-----------------
+---------------
+
 ```
 import riptable as rt
 ds = rt.Dataset({'intarray': rt.arange(1_000_000), 'floatarray': rt.arange(1_000_000.0)})
 ds
 ds.intarray.sum()
 ```
 
 Numpy Users
-------------
+-----------
+
 FastArray is a numpy array, however they can be flipped back and forth with no array copies taking place (it just changes the view).
+
 ```
 import riptable as rt
 import numpy as np
 a = rt.arange(100)
 numpyarray = a._np
 fastarray = rt.FA(numpyarray)
 ```
+
 or directly by changing the view, note how a FastArray is a numpy array
+
 ```
 numpyarray.view(rt.FastArray)
 fastarry.view(np.ndarray)
 ininstance(fastarray, np.ndarray)
 ```
 
 Pandas Users
 ------------
+
 Simply drop a pandas DataFrame class into a riptable Dataset and it will be auto converted.
+
 ```
 import riptable as rt
 import numpy as np
 import pandas as pd
 df = pd.DataFrame({'intarray': np.arange(1_000_000), 'floatarray': np.arange(1_000_000.0)})
 ds = rt.Dataset(df)
 ```
+
 How can I contribute?
 ---------------------
+
 RipTable has been public open sourced because it needs more users and
 contributions to take it to the next level.  The RipTable team is confident
 the engine is the next generation building block for python data analytics
 computing.  We need help from reporting bugs, docs, improved functionality,
 and new functionality.  Please consider a github pull request or email the
 team.
 
 See the [contributing guide](docs/CONTRIBUTING.md) for more information.
 
 How can I trust RipTable calculations?
 --------------------------------------
+
 RipTable has been in development for 3 years and tested by dozens of quants at a large financial firm.  It has a full suite of [testing](riptable/tests).  However just like any project, we still disover bugs and improvements.  Please report them using github issues.
 
 How can RipTable perform the same calculations faster?
 ------------------------------------------------------
+
 RipTable was written from day one to handle large data and mulithreading using the riptide_cpp layer for basic arithmetic functions and algorithms.  Many core algorithms have been painstakingly rewritten for multithreading.
 
 Why doesn't numpy or pandas just pick up the same code?
 -------------------------------------------------------
+
 numpy does not have a multithreaded layer (we are in discussions with the numpy team to add such a layer), nor is it designed to use C++ templates or hashing algorithms.  pandas does not have a C++ layer (it uses cython instead) and is a victim of its own success making early design mistakes difficult to change (such as the block manager and lack of powerful Categoricals).
 
 Small, Medium, and Large array performance
 ------------------------------------------
+
 RipTable is designed for *all* sizes of arrays.  For small arrays (< 100 length), low processing overhead is important.  RipTable's **FastArray** is written in hand coded 'C' and processes simple arithmetic functions faster than numpy arrays.  For medium arrays (< 100,000 length), RipTable has vector instrinic loops.  For large arrays (>= 100,000) RipTable knows how to dynamically scale out threading, waking up threads efficiently using a [futex](https://man7.org/linux/man-pages/man7/futex.7.html).
```

### Comparing `riptable-1.9.1/conda_recipe/meta.yaml` & `riptable-1.9.2/conda_recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/dev_tools/gen_requirements.py` & `riptable-1.9.2/dev_tools/gen_requirements.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         "gxx==8.*",
         "ninja",
     ]
 
 # Conda-build requirements.
 # Most everything else will be specified in meta.yaml.
 conda_reqs = [
+    "boa",
     "conda-build",
     "setuptools_scm",  # Needed to construct BUILD_VERSION for meta.yaml
 ] + toolchain_reqs
 
 # PyPI setup build requirements.
 # Most everything else will be specified in setup.py.
 pypi_reqs = [
@@ -150,20 +151,22 @@
     "toolchain": toolchain_reqs,
     "docstrings": docstrings_reqs,
 }
 
 parser = argparse.ArgumentParser()
 parser.add_argument("targets", help="requirement targets", choices=target_reqs.keys(), nargs="+")
 parser.add_argument("--out", help="output file", type=str)
+parser.add_argument("--quote", "-q", help="quote entries", action="store_true")
 args = parser.parse_args()
 
 reqs = list({r for t in args.targets for r in target_reqs[t]})
 reqs.sort()
 
 # Emit plain list to enable usage like: conda install $(gen_requirements.py developer)
 out = open(args.out, "w") if args.out else sys.stdout
 try:
+    quot = '"' if args.quote else ""
     for req in reqs:
-        print(req, file=out)
+        print(quot + req + quot, file=out)
 finally:
     if args.out:
         out.close()
```

### Comparing `riptable-1.9.1/dev_tools/validate_docstrings.py` & `riptable-1.9.2/dev_tools/validate_docstrings.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/CONTRIBUTING.md` & `riptable-1.9.2/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/Makefile` & `riptable-1.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/THREADING.md` & `riptable-1.9.2/docs/THREADING.md`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/make.bat` & `riptable-1.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/riptable_logo.PNG` & `riptable-1.9.2/docs/riptable_logo.PNG`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/benchmarking.rst` & `riptable-1.9.2/docs/source/benchmarking.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/conf.py` & `riptable-1.9.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/riptable.rst` & `riptable-1.9.2/docs/source/riptable.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/RiptableExercises.ipynb` & `riptable-1.9.2/docs/source/tutorial/RiptableExercises.ipynb`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/RiptableSolutions.ipynb` & `riptable-1.9.2/docs/source/tutorial/RiptableSolutions.ipynb`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/output_11_0.png` & `riptable-1.9.2/docs/source/tutorial/output_11_0.png`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/output_13_0.png` & `riptable-1.9.2/docs/source/tutorial/output_13_0.png`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/output_15_0.png` & `riptable-1.9.2/docs/source/tutorial/output_15_0.png`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/output_25_0.png` & `riptable-1.9.2/docs/source/tutorial/output_25_0.png`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/output_27_0.png` & `riptable-1.9.2/docs/source/tutorial/output_27_0.png`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/perf-may-suffer.png` & `riptable-1.9.2/docs/source/tutorial/perf-may-suffer.png`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/rt_autocomplete.png` & `riptable-1.9.2/docs/source/tutorial/rt_autocomplete.png`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/rt_autocomplete_internal.png` & `riptable-1.9.2/docs/source/tutorial/rt_autocomplete_internal.png`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/rt_dataset.svg` & `riptable-1.9.2/docs/source/tutorial/rt_dataset.svg`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/rt_dataset_indices.svg` & `riptable-1.9.2/docs/source/tutorial/rt_dataset_indices.svg`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/rt_fastarray.svg` & `riptable-1.9.2/docs/source/tutorial/rt_fastarray.svg`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/split-apply-combine-gray.svg` & `riptable-1.9.2/docs/source/tutorial/split-apply-combine-gray.svg`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_accums.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_accums.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_cat_adv_instantiation.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_cat_adv_instantiation.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_cat_reduce.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_cat_reduce.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_categoricals.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_categoricals.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_concat.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_concat.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_datasets.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_datasets.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_datetimes.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_datetimes.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_filters.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_filters.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_intro.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_intro.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_io.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_io.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_merge.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_merge.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_missing_data.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_missing_data.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_numpy_rt.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_numpy_rt.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_performance.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_performance.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_reshape.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_reshape.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_sample_data.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_sample_data.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/docs/source/tutorial/tutorial_visualize.rst` & `riptable-1.9.2/docs/source/tutorial/tutorial_visualize.rst`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/pyproject.toml` & `riptable-1.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/Utils/appdirs.py` & `riptable-1.9.2/riptable/Utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/Utils/common.py` & `riptable-1.9.2/riptable/Utils/common.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/Utils/conversion_utils.py` & `riptable-1.9.2/riptable/Utils/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/Utils/display_options.py` & `riptable-1.9.2/riptable/Utils/display_options.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/Utils/ipython_utils.py` & `riptable-1.9.2/riptable/Utils/ipython_utils.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/Utils/pandas_utils.py` & `riptable-1.9.2/riptable/Utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/Utils/rt_display_nested.py` & `riptable-1.9.2/riptable/Utils/rt_display_nested.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/Utils/rt_display_properties.py` & `riptable-1.9.2/riptable/Utils/rt_display_properties.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/Utils/rt_metadata.py` & `riptable-1.9.2/riptable/Utils/rt_metadata.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/Utils/rt_testdata.py` & `riptable-1.9.2/riptable/Utils/rt_testdata.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/Utils/rt_testing.py` & `riptable-1.9.2/riptable/Utils/rt_testing.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/Utils/terminalsize.py` & `riptable-1.9.2/riptable/Utils/terminalsize.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/__init__.py` & `riptable-1.9.2/riptable/__init__.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/__init__.py` & `riptable-1.9.2/riptable/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/analysis.py` & `riptable-1.9.2/riptable/benchmarks/analysis.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/bench_categorical.py` & `riptable-1.9.2/riptable/benchmarks/bench_categorical.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/bench_grouping.py` & `riptable-1.9.2/riptable/benchmarks/bench_grouping.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/bench_merge.py` & `riptable-1.9.2/riptable/benchmarks/bench_merge.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/bench_numpy.py` & `riptable-1.9.2/riptable/benchmarks/bench_numpy.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/bench_operators.py` & `riptable-1.9.2/riptable/benchmarks/bench_operators.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/bench_primops.py` & `riptable-1.9.2/riptable/benchmarks/bench_primops.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/benchmark.py` & `riptable-1.9.2/riptable/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/main.py` & `riptable-1.9.2/riptable/benchmarks/main.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/rand_data.py` & `riptable-1.9.2/riptable/benchmarks/rand_data.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/rand_keydata.py` & `riptable-1.9.2/riptable/benchmarks/rand_keydata.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/results.py` & `riptable-1.9.2/riptable/benchmarks/results.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/benchmarks/runner.py` & `riptable-1.9.2/riptable/benchmarks/runner.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/config.py` & `riptable-1.9.2/riptable/config.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/conftest.py` & `riptable-1.9.2/riptable/conftest.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/hypothesis_tests/conftest.py` & `riptable-1.9.2/riptable/hypothesis_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/hypothesis_tests/strategies/categorical_strategy.py` & `riptable-1.9.2/riptable/hypothesis_tests/strategies/categorical_strategy.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/hypothesis_tests/strategies/helper_strategies.py` & `riptable-1.9.2/riptable/hypothesis_tests/strategies/helper_strategies.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/hypothesis_tests/test_categorical_property.py` & `riptable-1.9.2/riptable/hypothesis_tests/test_categorical_property.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/hypothesis_tests/test_riptide_numpy_equivalency.py` & `riptable-1.9.2/riptable/hypothesis_tests/test_riptide_numpy_equivalency.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/hypothesis_tests/test_rt_numpy_property.py` & `riptable-1.9.2/riptable/hypothesis_tests/test_rt_numpy_property.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/hypothesis_tests/test_sds_property.py` & `riptable-1.9.2/riptable/hypothesis_tests/test_sds_property.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/hypothesis_tests/test_ufunc_unary.py` & `riptable-1.9.2/riptable/hypothesis_tests/test_ufunc_unary.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/numba/indexing.py` & `riptable-1.9.2/riptable/numba/indexing.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/numba/invalid_values.py` & `riptable-1.9.2/riptable/numba/invalid_values.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_accum2.py` & `riptable-1.9.2/riptable/rt_accum2.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_accumtable.py` & `riptable-1.9.2/riptable/rt_accumtable.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_algos.py` & `riptable-1.9.2/riptable/rt_algos.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_bin.py` & `riptable-1.9.2/riptable/rt_bin.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_categorical.py` & `riptable-1.9.2/riptable/rt_categorical.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_compressedarray.py` & `riptable-1.9.2/riptable/rt_compressedarray.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_csv.py` & `riptable-1.9.2/riptable/rt_csv.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_dataset.py` & `riptable-1.9.2/riptable/rt_dataset.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_datetime.py` & `riptable-1.9.2/riptable/rt_datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -4325,16 +4325,20 @@
                 if isinstance(start_date, (str, bytes)):
                     start_date = FastArray(start_date)
                     start_date = rc.DateStringToNanos(start_date)[0]
                 elif isinstance(start_date, Date):
                     if len(start_date) == len(arr):
                         # user has passed in multiple start dates
                         start_date = start_date._fa * NANOS_PER_DAY
-                    else:
+                    elif len(start_date) == 1:
                         start_date = start_date[0] * NANOS_PER_DAY
+                    else:
+                        raise ValueError(
+                            f"start_date Date array must be either length 1 or the same length as arr. Got arr of length {len(arr)} and start_date of length {len(start_date)}."
+                        )
                 else:
                     raise TypeError(
                         f"Start date must be string in format YYYYMMDD or Date object. Got type {type(start_date)}"
                     )
 
             instance = None
             if isinstance(arr, list) or np.isscalar(arr):
```

### Comparing `riptable-1.9.1/riptable/rt_display.py` & `riptable-1.9.2/riptable/rt_display.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_ema.py` & `riptable-1.9.2/riptable/rt_ema.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_enum.py` & `riptable-1.9.2/riptable/rt_enum.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_fastarray.py` & `riptable-1.9.2/riptable/rt_fastarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -12258,3372 +12258,3372 @@
 0002fe10: 2020 2023 206d 696e 2f6d 6178 2f6e 616e     # min/max/nan
 0002fe20: 6d69 6e2f 6e61 6e6d 6178 202d 2d20 7361  min/nanmax -- sa
 0002fe30: 6d65 2072 6573 756c 740d 0a20 2020 2020  me result..     
 0002fe40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
 0002fe50: 6620 6474 7970 6520 3d3d 206e 702e 626f  f dtype == np.bo
 0002fe60: 6f6c 5f3a 0d0a 2020 2020 2020 2020 2020  ol_:..          
 0002fe70: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0002fe80: 7375 6c74 203d 206e 702e 626f 6f6c 2872  sult = np.bool(r
-0002fe90: 6573 756c 7429 0d0a 2020 2020 2020 2020  esult)..        
-0002fea0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0002feb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0002fec0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002fed0: 7420 3d20 6474 7970 652e 7479 7065 2872  t = dtype.type(r
-0002fee0: 6573 756c 7429 0d0a 0d0a 2020 2020 2020  esult)....      
-0002fef0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0002ff00: 206b 6565 7064 696d 733a 0d0a 2020 2020   keepdims:..    
+0002fe80: 7375 6c74 203d 206e 702e 626f 6f6c 5f28  sult = np.bool_(
+0002fe90: 7265 7375 6c74 290d 0a20 2020 2020 2020  result)..       
+0002fea0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0002feb0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0002fec0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002fed0: 6c74 203d 2064 7479 7065 2e74 7970 6528  lt = dtype.type(
+0002fee0: 7265 7375 6c74 290d 0a0d 0a20 2020 2020  result)....     
+0002fef0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0002ff00: 6620 6b65 6570 6469 6d73 3a0d 0a20 2020  f keepdims:..   
 0002ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ff20: 2020 2020 7265 7375 6c74 203d 2046 6173      result = Fas
-0002ff30: 7441 7272 6179 285b 7265 7375 6c74 5d29  tArray([result])
-0002ff40: 2e61 7374 7970 6528 6474 7970 6529 0d0a  .astype(dtype)..
-0002ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ff60: 656c 6966 206b 6565 7064 696d 733a 0d0a  elif keepdims:..
-0002ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ff80: 2020 2020 2320 666f 7263 6520 6261 636b      # force back
-0002ff90: 2069 6e74 6f20 616e 2061 7272 6179 2066   into an array f
-0002ffa0: 726f 6d20 7363 616c 6172 0d0a 2020 2020  rom scalar..    
+0002ff20: 2020 2020 2072 6573 756c 7420 3d20 4661       result = Fa
+0002ff30: 7374 4172 7261 7928 5b72 6573 756c 745d  stArray([result]
+0002ff40: 292e 6173 7479 7065 2864 7479 7065 290d  ).astype(dtype).
+0002ff50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002ff60: 2065 6c69 6620 6b65 6570 6469 6d73 3a0d   elif keepdims:.
+0002ff70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002ff80: 2020 2020 2023 2066 6f72 6365 2062 6163       # force bac
+0002ff90: 6b20 696e 746f 2061 6e20 6172 7261 7920  k into an array 
+0002ffa0: 6672 6f6d 2073 6361 6c61 720d 0a20 2020  from scalar..   
 0002ffb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ffc0: 7265 7375 6c74 203d 2046 6173 7441 7272  result = FastArr
-0002ffd0: 6179 285b 7265 7375 6c74 5d29 0d0a 0d0a  ay([result])....
-0002ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002fff0: 2320 7765 2064 6964 2074 6865 2072 6564  # we did the red
-00030000: 7563 652c 206e 6f77 2072 6574 7572 6e20  uce, now return 
-00030010: 7468 6520 7265 7375 6c74 0d0a 2020 2020  the result..    
-00030020: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00030030: 726e 2072 6573 756c 740d 0a0d 0a20 2020  rn result....   
-00030040: 2020 2020 2023 2063 6865 636b 2066 6f72       # check for
-00030050: 206e 6f72 6d61 6c20 6361 6c6c 2066 756e   normal call fun
-00030060: 6374 696f 6e0d 0a20 2020 2020 2020 2065  ction..        e
-00030070: 6c69 6620 6661 7374 5f66 756e 6374 696f  lif fast_functio
-00030080: 6e20 6973 206e 6f74 204e 6f6e 653a 0d0a  n is not None:..
-00030090: 2020 2020 2020 2020 2020 2020 2320 4361              # Ca
-000300a0: 6c6c 2074 6865 2046 6173 7441 7272 6179  ll the FastArray
-000300b0: 2041 5049 7320 696e 7374 6561 6420 6f66   APIs instead of
-000300c0: 206e 756d 7079 0d0a 2020 2020 2020 2020   numpy..        
-000300d0: 2020 2020 2320 6361 6c6c 6d6f 6465 203d      # callmode =
-000300e0: 2027 6627 0d0a 2020 2020 2020 2020 2020   'f'..          
-000300f0: 2020 7265 7375 6c74 7320 3d20 4e6f 6e65    results = None
-00030100: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00030110: 2075 6675 6e63 2e6e 696e 203d 3d20 323a   ufunc.nin == 2:
-00030120: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00030130: 2020 6669 6e61 6c5f 6e75 6d20 3d20 2d31    final_num = -1
-00030140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00030150: 2020 6966 2066 696e 616c 5f64 7479 7065    if final_dtype
-00030160: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+0002ffc0: 2072 6573 756c 7420 3d20 4661 7374 4172   result = FastAr
+0002ffd0: 7261 7928 5b72 6573 756c 745d 290d 0a0d  ray([result])...
+0002ffe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002fff0: 2023 2077 6520 6469 6420 7468 6520 7265   # we did the re
+00030000: 6475 6365 2c20 6e6f 7720 7265 7475 726e  duce, now return
+00030010: 2074 6865 2072 6573 756c 740d 0a20 2020   the result..   
+00030020: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00030030: 7572 6e20 7265 7375 6c74 0d0a 0d0a 2020  urn result....  
+00030040: 2020 2020 2020 2320 6368 6563 6b20 666f        # check fo
+00030050: 7220 6e6f 726d 616c 2063 616c 6c20 6675  r normal call fu
+00030060: 6e63 7469 6f6e 0d0a 2020 2020 2020 2020  nction..        
+00030070: 656c 6966 2066 6173 745f 6675 6e63 7469  elif fast_functi
+00030080: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0d  on is not None:.
+00030090: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+000300a0: 616c 6c20 7468 6520 4661 7374 4172 7261  all the FastArra
+000300b0: 7920 4150 4973 2069 6e73 7465 6164 206f  y APIs instead o
+000300c0: 6620 6e75 6d70 790d 0a20 2020 2020 2020  f numpy..       
+000300d0: 2020 2020 2023 2063 616c 6c6d 6f64 6520       # callmode 
+000300e0: 3d20 2766 270d 0a20 2020 2020 2020 2020  = 'f'..         
+000300f0: 2020 2072 6573 756c 7473 203d 204e 6f6e     results = Non
+00030100: 650d 0a20 2020 2020 2020 2020 2020 2069  e..            i
+00030110: 6620 7566 756e 632e 6e69 6e20 3d3d 2032  f ufunc.nin == 2
+00030120: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00030130: 2020 2066 696e 616c 5f6e 756d 203d 202d     final_num = -
+00030140: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+00030150: 2020 2069 6620 6669 6e61 6c5f 6474 7970     if final_dtyp
+00030160: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
 00030170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030180: 2020 2069 6620 6669 6e61 6c5f 6474 7970     if final_dtyp
-00030190: 6520 3d3d 206e 702e 626f 6f6c 5f3a 0d0a  e == np.bool_:..
-000301a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000301b0: 2020 2020 2020 2020 6669 6e61 6c5f 6e75          final_nu
-000301c0: 6d20 3d20 300d 0a20 2020 2020 2020 2020  m = 0..         
-000301d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000301e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000301f0: 2020 2020 2020 2020 2020 6669 6e61 6c5f            final_
-00030200: 6e75 6d20 3d20 6669 6e61 6c5f 6474 7970  num = final_dtyp
-00030210: 652e 6e75 6d0d 0a0d 0a20 2020 2020 2020  e.num....       
-00030220: 2020 2020 2020 2020 2023 2062 6563 6175           # becau
-00030230: 7365 2073 6361 6c61 7273 2063 616e 2062  se scalars can b
-00030240: 6520 7061 7373 6564 2061 7320 6e70 2e69  e passed as np.i
-00030250: 6e74 3634 2838 3634 3030 3029 0d0a 2020  nt64(864000)..  
-00030260: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00030270: 2074 7970 6528 6172 6773 5b30 5d29 2069   type(args[0]) i
-00030280: 6e20 674e 756d 7079 5363 616c 6172 5479  n gNumpyScalarTy
-00030290: 7065 3a0d 0a20 2020 2020 2020 2020 2020  pe:..           
-000302a0: 2020 2020 2020 2020 2023 2070 7269 6e74           # print
-000302b0: 2827 636f 6e76 6572 7469 6e67 2061 7267  ('converting arg
-000302c0: 3127 2c20 6172 6773 5b30 5d29 0d0a 2020  1', args[0])..  
+00030180: 2020 2020 6966 2066 696e 616c 5f64 7479      if final_dty
+00030190: 7065 203d 3d20 6e70 2e62 6f6f 6c5f 3a0d  pe == np.bool_:.
+000301a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000301b0: 2020 2020 2020 2020 2066 696e 616c 5f6e           final_n
+000301c0: 756d 203d 2030 0d0a 2020 2020 2020 2020  um = 0..        
+000301d0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000301e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000301f0: 2020 2020 2020 2020 2020 2066 696e 616c             final
+00030200: 5f6e 756d 203d 2066 696e 616c 5f64 7479  _num = final_dty
+00030210: 7065 2e6e 756d 0d0a 0d0a 2020 2020 2020  pe.num....      
+00030220: 2020 2020 2020 2020 2020 2320 6265 6361            # beca
+00030230: 7573 6520 7363 616c 6172 7320 6361 6e20  use scalars can 
+00030240: 6265 2070 6173 7365 6420 6173 206e 702e  be passed as np.
+00030250: 696e 7436 3428 3836 3430 3030 290d 0a20  int64(864000).. 
+00030260: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00030270: 6620 7479 7065 2861 7267 735b 305d 2920  f type(args[0]) 
+00030280: 696e 2067 4e75 6d70 7953 6361 6c61 7254  in gNumpyScalarT
+00030290: 7970 653a 0d0a 2020 2020 2020 2020 2020  ype:..          
+000302a0: 2020 2020 2020 2020 2020 2320 7072 696e            # prin
+000302b0: 7428 2763 6f6e 7665 7274 696e 6720 6172  t('converting ar
+000302c0: 6731 272c 2061 7267 735b 305d 290d 0a20  g1', args[0]).. 
 000302d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000302e0: 2020 6172 6773 5b30 5d20 3d20 6e70 2e61    args[0] = np.a
-000302f0: 7361 7272 6179 2861 7267 735b 305d 290d  sarray(args[0]).
-00030300: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00030310: 2020 2069 6620 7479 7065 2861 7267 735b     if type(args[
-00030320: 315d 2920 696e 2067 4e75 6d70 7953 6361  1]) in gNumpySca
-00030330: 6c61 7254 7970 653a 0d0a 2020 2020 2020  larType:..      
-00030340: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00030350: 7072 696e 7428 2763 6f6e 7665 7274 696e  print('convertin
-00030360: 6720 6172 6732 272c 2061 7267 735b 315d  g arg2', args[1]
-00030370: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00030380: 2020 2020 2020 2061 7267 735b 315d 203d         args[1] =
-00030390: 206e 702e 6173 6172 7261 7928 6172 6773   np.asarray(args
-000303a0: 5b31 5d29 0d0a 0d0a 2020 2020 2020 2020  [1])....        
-000303b0: 2020 2020 2020 2020 6966 2046 6173 7441          if FastA
-000303c0: 7272 6179 2e56 6572 626f 7365 203e 2032  rray.Verbose > 2
-000303d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000303e0: 2020 2020 2020 2070 7269 6e74 280d 0a20         print(.. 
+000302e0: 2020 2061 7267 735b 305d 203d 206e 702e     args[0] = np.
+000302f0: 6173 6172 7261 7928 6172 6773 5b30 5d29  asarray(args[0])
+00030300: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00030310: 2020 2020 6966 2074 7970 6528 6172 6773      if type(args
+00030320: 5b31 5d29 2069 6e20 674e 756d 7079 5363  [1]) in gNumpySc
+00030330: 616c 6172 5479 7065 3a0d 0a20 2020 2020  alarType:..     
+00030340: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00030350: 2070 7269 6e74 2827 636f 6e76 6572 7469   print('converti
+00030360: 6e67 2061 7267 3227 2c20 6172 6773 5b31  ng arg2', args[1
+00030370: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00030380: 2020 2020 2020 2020 6172 6773 5b31 5d20          args[1] 
+00030390: 3d20 6e70 2e61 7361 7272 6179 2861 7267  = np.asarray(arg
+000303a0: 735b 315d 290d 0a0d 0a20 2020 2020 2020  s[1])....       
+000303b0: 2020 2020 2020 2020 2069 6620 4661 7374           if Fast
+000303c0: 4172 7261 792e 5665 7262 6f73 6520 3e20  Array.Verbose > 
+000303d0: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
+000303e0: 2020 2020 2020 2020 7072 696e 7428 0d0a          print(..
 000303f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030400: 2020 2020 2020 2022 2a2a 2a20 6269 6e61         "*** bina
-00030410: 7279 2074 6869 6e6b 2077 6520 6361 6e20  ry think we can 
-00030420: 6361 6c6c 222c 0d0a 2020 2020 2020 2020  call",..        
+00030400: 2020 2020 2020 2020 222a 2a2a 2062 696e          "*** bin
+00030410: 6172 7920 7468 696e 6b20 7765 2063 616e  ary think we can
+00030420: 2063 616c 6c22 2c0d 0a20 2020 2020 2020   call",..       
 00030430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030440: 6661 7374 5f66 756e 6374 696f 6e2c 0d0a  fast_function,..
-00030450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030460: 2020 2020 2020 2020 7566 756e 632e 6e69          ufunc.ni
-00030470: 6e2c 0d0a 2020 2020 2020 2020 2020 2020  n,..            
-00030480: 2020 2020 2020 2020 2020 2020 7566 756e              ufun
-00030490: 632e 6e6f 7574 2c0d 0a20 2020 2020 2020  c.nout,..       
+00030440: 2066 6173 745f 6675 6e63 7469 6f6e 2c0d   fast_function,.
+00030450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030460: 2020 2020 2020 2020 2075 6675 6e63 2e6e           ufunc.n
+00030470: 696e 2c0d 0a20 2020 2020 2020 2020 2020  in,..           
+00030480: 2020 2020 2020 2020 2020 2020 2075 6675               ufu
+00030490: 6e63 2e6e 6f75 742c 0d0a 2020 2020 2020  nc.nout,..      
 000304a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000304b0: 2022 6172 6731 222c 0d0a 2020 2020 2020   "arg1",..      
+000304b0: 2020 2261 7267 3122 2c0d 0a20 2020 2020    "arg1",..     
 000304c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000304d0: 2020 6172 6773 5b30 5d2c 0d0a 2020 2020    args[0],..    
+000304d0: 2020 2061 7267 735b 305d 2c0d 0a20 2020     args[0],..   
 000304e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000304f0: 2020 2020 2261 7267 3222 2c0d 0a20 2020      "arg2",..   
+000304f0: 2020 2020 2022 6172 6732 222c 0d0a 2020       "arg2",..  
 00030500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030510: 2020 2020 2061 7267 735b 315d 2c0d 0a20       args[1],.. 
+00030510: 2020 2020 2020 6172 6773 5b31 5d2c 0d0a        args[1],..
 00030520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030530: 2020 2020 2020 2022 6f75 7422 2c0d 0a20         "out",.. 
+00030530: 2020 2020 2020 2020 226f 7574 222c 0d0a          "out",..
 00030540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030550: 2020 2020 2020 206f 7574 5f61 7267 732c         out_args,
-00030560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00030570: 2020 2020 2020 2020 2020 2266 696e 616c            "final
-00030580: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00030590: 2020 2020 2020 2020 2020 2020 6669 6e61              fina
-000305a0: 6c5f 6e75 6d2c 0d0a 2020 2020 2020 2020  l_num,..        
-000305b0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-000305c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000305d0: 6620 6c65 6e28 6f75 745f 6172 6773 2920  f len(out_args) 
-000305e0: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
-000305f0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00030600: 7473 203d 2054 7970 6552 6567 6973 7465  ts = TypeRegiste
-00030610: 722e 4d61 7468 4c65 6467 6572 2e5f 4241  r.MathLedger._BA
-00030620: 5349 434d 4154 485f 5457 4f5f 494e 5055  SICMATH_TWO_INPU
-00030630: 5453 280d 0a20 2020 2020 2020 2020 2020  TS(..           
-00030640: 2020 2020 2020 2020 2020 2020 2028 6172               (ar
-00030650: 6773 5b30 5d2c 2061 7267 735b 315d 2c20  gs[0], args[1], 
-00030660: 6f75 745f 6172 6773 5b30 5d29 2c20 6661  out_args[0]), fa
-00030670: 7374 5f66 756e 6374 696f 6e2c 2066 696e  st_function, fin
-00030680: 616c 5f6e 756d 0d0a 2020 2020 2020 2020  al_num..        
-00030690: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-000306a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000306b0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-000306c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000306d0: 7320 3d20 5479 7065 5265 6769 7374 6572  s = TypeRegister
-000306e0: 2e4d 6174 684c 6564 6765 722e 5f42 4153  .MathLedger._BAS
-000306f0: 4943 4d41 5448 5f54 574f 5f49 4e50 5554  ICMATH_TWO_INPUT
-00030700: 5328 0d0a 2020 2020 2020 2020 2020 2020  S(..            
-00030710: 2020 2020 2020 2020 2020 2020 2861 7267              (arg
-00030720: 735b 305d 2c20 6172 6773 5b31 5d29 2c20  s[0], args[1]), 
-00030730: 6661 7374 5f66 756e 6374 696f 6e2c 2066  fast_function, f
-00030740: 696e 616c 5f6e 756d 0d0a 2020 2020 2020  inal_num..      
-00030750: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00030760: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00030770: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00030780: 2020 2020 2320 666f 7220 636f 6e76 6572      # for conver
-00030790: 7369 6f6e 2066 756e 6374 696f 6e73 0d0a  sion functions..
-000307a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000307b0: 2320 6474 7970 653d 6b77 6172 6773 2e67  # dtype=kwargs.g
-000307c0: 6574 2827 6474 7970 6527 2c4e 6f6e 6529  et('dtype',None)
-000307d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000307e0: 2020 6966 2046 6173 7441 7272 6179 2e56    if FastArray.V
-000307f0: 6572 626f 7365 203e 2032 3a0d 0a20 2020  erbose > 2:..   
+00030550: 2020 2020 2020 2020 6f75 745f 6172 6773          out_args
+00030560: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00030570: 2020 2020 2020 2020 2020 2022 6669 6e61             "fina
+00030580: 6c22 2c0d 0a20 2020 2020 2020 2020 2020  l",..           
+00030590: 2020 2020 2020 2020 2020 2020 2066 696e               fin
+000305a0: 616c 5f6e 756d 2c0d 0a20 2020 2020 2020  al_num,..       
+000305b0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+000305c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000305d0: 6966 206c 656e 286f 7574 5f61 7267 7329  if len(out_args)
+000305e0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
+000305f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00030600: 6c74 7320 3d20 5479 7065 5265 6769 7374  lts = TypeRegist
+00030610: 6572 2e4d 6174 684c 6564 6765 722e 5f42  er.MathLedger._B
+00030620: 4153 4943 4d41 5448 5f54 574f 5f49 4e50  ASICMATH_TWO_INP
+00030630: 5554 5328 0d0a 2020 2020 2020 2020 2020  UTS(..          
+00030640: 2020 2020 2020 2020 2020 2020 2020 2861                (a
+00030650: 7267 735b 305d 2c20 6172 6773 5b31 5d2c  rgs[0], args[1],
+00030660: 206f 7574 5f61 7267 735b 305d 292c 2066   out_args[0]), f
+00030670: 6173 745f 6675 6e63 7469 6f6e 2c20 6669  ast_function, fi
+00030680: 6e61 6c5f 6e75 6d0d 0a20 2020 2020 2020  nal_num..       
+00030690: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+000306a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000306b0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000306c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000306d0: 7473 203d 2054 7970 6552 6567 6973 7465  ts = TypeRegiste
+000306e0: 722e 4d61 7468 4c65 6467 6572 2e5f 4241  r.MathLedger._BA
+000306f0: 5349 434d 4154 485f 5457 4f5f 494e 5055  SICMATH_TWO_INPU
+00030700: 5453 280d 0a20 2020 2020 2020 2020 2020  TS(..           
+00030710: 2020 2020 2020 2020 2020 2020 2028 6172               (ar
+00030720: 6773 5b30 5d2c 2061 7267 735b 315d 292c  gs[0], args[1]),
+00030730: 2066 6173 745f 6675 6e63 7469 6f6e 2c20   fast_function, 
+00030740: 6669 6e61 6c5f 6e75 6d0d 0a20 2020 2020  final_num..     
+00030750: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00030760: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00030770: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00030780: 2020 2020 2023 2066 6f72 2063 6f6e 7665       # for conve
+00030790: 7273 696f 6e20 6675 6e63 7469 6f6e 730d  rsion functions.
+000307a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000307b0: 2023 2064 7479 7065 3d6b 7761 7267 732e   # dtype=kwargs.
+000307c0: 6765 7428 2764 7479 7065 272c 4e6f 6e65  get('dtype',None
+000307d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000307e0: 2020 2069 6620 4661 7374 4172 7261 792e     if FastArray.
+000307f0: 5665 7262 6f73 6520 3e20 323a 0d0a 2020  Verbose > 2:..  
 00030800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030810: 2070 7269 6e74 280d 0a20 2020 2020 2020   print(..       
+00030810: 2020 7072 696e 7428 0d0a 2020 2020 2020    print(..      
 00030820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030830: 2022 2a2a 2a20 756e 6172 7920 7468 696e   "*** unary thin
-00030840: 6b20 7765 2063 616e 2063 616c 6c22 2c0d  k we can call",.
-00030850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00030860: 2020 2020 2020 2020 2066 6173 745f 6675           fast_fu
-00030870: 6e63 7469 6f6e 2c0d 0a20 2020 2020 2020  nction,..       
+00030830: 2020 222a 2a2a 2075 6e61 7279 2074 6869    "*** unary thi
+00030840: 6e6b 2077 6520 6361 6e20 6361 6c6c 222c  nk we can call",
+00030850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00030860: 2020 2020 2020 2020 2020 6661 7374 5f66            fast_f
+00030870: 756e 6374 696f 6e2c 0d0a 2020 2020 2020  unction,..      
 00030880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030890: 2075 6675 6e63 2e6e 696e 2c0d 0a20 2020   ufunc.nin,..   
+00030890: 2020 7566 756e 632e 6e69 6e2c 0d0a 2020    ufunc.nin,..  
 000308a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000308b0: 2020 2020 2075 6675 6e63 2e6e 6f75 742c       ufunc.nout,
-000308c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000308d0: 2020 2020 2020 2020 2020 2261 7267 3122            "arg1"
-000308e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000308f0: 2020 2020 2020 2020 2020 2061 7267 735b             args[
-00030900: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
-00030910: 2020 2020 2020 2020 2020 2020 2022 6f75               "ou
-00030920: 7422 2c0d 0a20 2020 2020 2020 2020 2020  t",..           
-00030930: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00030940: 5f61 7267 732c 0d0a 2020 2020 2020 2020  _args,..        
-00030950: 2020 2020 2020 2020 2020 2020 290d 0a0d              )...
-00030960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00030970: 2069 6620 6c65 6e28 6f75 745f 6172 6773   if len(out_args
-00030980: 2920 3d3d 2031 3a0d 0a20 2020 2020 2020  ) == 1:..       
-00030990: 2020 2020 2020 2020 2020 2020 2072 6573               res
-000309a0: 756c 7473 203d 2054 7970 6552 6567 6973  ults = TypeRegis
-000309b0: 7465 722e 4d61 7468 4c65 6467 6572 2e5f  ter.MathLedger._
-000309c0: 4241 5349 434d 4154 485f 4f4e 455f 494e  BASICMATH_ONE_IN
-000309d0: 5055 5428 2861 7267 735b 305d 2c20 6f75  PUT((args[0], ou
-000309e0: 745f 6172 6773 5b30 5d29 2c20 6661 7374  t_args[0]), fast
-000309f0: 5f66 756e 6374 696f 6e2c 2030 290d 0a20  _function, 0).. 
-00030a00: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00030a10: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00030a20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00030a30: 7320 3d20 5479 7065 5265 6769 7374 6572  s = TypeRegister
-00030a40: 2e4d 6174 684c 6564 6765 722e 5f42 4153  .MathLedger._BAS
-00030a50: 4943 4d41 5448 5f4f 4e45 5f49 4e50 5554  ICMATH_ONE_INPUT
-00030a60: 2828 6172 6773 5b30 5d29 2c20 6661 7374  ((args[0]), fast
-00030a70: 5f66 756e 6374 696f 6e2c 2030 290d 0a0d  _function, 0)...
-00030a80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00030a90: 7265 7375 6c74 7320 6973 206e 6f74 204e  results is not N
-00030aa0: 6f6e 6520 616e 6420 6c65 6e28 6f75 745f  one and len(out_
-00030ab0: 6172 6773 2920 3d3d 2031 3a0d 0a20 2020  args) == 1:..   
-00030ac0: 2020 2020 2020 2020 2020 2020 2023 2077               # w
-00030ad0: 6865 6e20 7468 6520 6f75 7470 7574 2061  hen the output a
-00030ae0: 7267 756d 656e 7420 6973 2066 6f72 6365  rgument is force
-00030af0: 6420 6275 7420 7765 2063 616c 6375 6c61  d but we calcula
-00030b00: 7465 2069 7420 696e 746f 2061 6e6f 7468  te it into anoth
-00030b10: 6572 2061 7272 6179 2077 6520 6e65 6564  er array we need
-00030b20: 2074 6f20 636f 7079 2074 6865 2072 6573   to copy the res
-00030b30: 756c 7420 696e 746f 2074 6865 206f 7574  ult into the out
-00030b40: 7075 740d 0a20 2020 2020 2020 2020 2020  put..           
-00030b50: 2020 2020 2069 6620 6e6f 7420 7263 2e43       if not rc.C
-00030b60: 6f6d 7061 7265 4e75 6d70 794d 656d 4164  ompareNumpyMemAd
-00030b70: 6472 6573 7328 6f75 745f 6172 6773 5b30  dress(out_args[0
-00030b80: 5d2c 2072 6573 756c 7473 293a 0d0a 2020  ], results):..  
+000308b0: 2020 2020 2020 7566 756e 632e 6e6f 7574        ufunc.nout
+000308c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000308d0: 2020 2020 2020 2020 2020 2022 6172 6731             "arg1
+000308e0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000308f0: 2020 2020 2020 2020 2020 2020 6172 6773              args
+00030900: 5b30 5d2c 0d0a 2020 2020 2020 2020 2020  [0],..          
+00030910: 2020 2020 2020 2020 2020 2020 2020 226f                "o
+00030920: 7574 222c 0d0a 2020 2020 2020 2020 2020  ut",..          
+00030930: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+00030940: 745f 6172 6773 2c0d 0a20 2020 2020 2020  t_args,..       
+00030950: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+00030960: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00030970: 2020 6966 206c 656e 286f 7574 5f61 7267    if len(out_arg
+00030980: 7329 203d 3d20 313a 0d0a 2020 2020 2020  s) == 1:..      
+00030990: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000309a0: 7375 6c74 7320 3d20 5479 7065 5265 6769  sults = TypeRegi
+000309b0: 7374 6572 2e4d 6174 684c 6564 6765 722e  ster.MathLedger.
+000309c0: 5f42 4153 4943 4d41 5448 5f4f 4e45 5f49  _BASICMATH_ONE_I
+000309d0: 4e50 5554 2828 6172 6773 5b30 5d2c 206f  NPUT((args[0], o
+000309e0: 7574 5f61 7267 735b 305d 292c 2066 6173  ut_args[0]), fas
+000309f0: 745f 6675 6e63 7469 6f6e 2c20 3029 0d0a  t_function, 0)..
+00030a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030a10: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00030a20: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00030a30: 7473 203d 2054 7970 6552 6567 6973 7465  ts = TypeRegiste
+00030a40: 722e 4d61 7468 4c65 6467 6572 2e5f 4241  r.MathLedger._BA
+00030a50: 5349 434d 4154 485f 4f4e 455f 494e 5055  SICMATH_ONE_INPU
+00030a60: 5428 2861 7267 735b 305d 292c 2066 6173  T((args[0]), fas
+00030a70: 745f 6675 6e63 7469 6f6e 2c20 3029 0d0a  t_function, 0)..
+00030a80: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00030a90: 2072 6573 756c 7473 2069 7320 6e6f 7420   results is not 
+00030aa0: 4e6f 6e65 2061 6e64 206c 656e 286f 7574  None and len(out
+00030ab0: 5f61 7267 7329 203d 3d20 313a 0d0a 2020  _args) == 1:..  
+00030ac0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00030ad0: 7768 656e 2074 6865 206f 7574 7075 7420  when the output 
+00030ae0: 6172 6775 6d65 6e74 2069 7320 666f 7263  argument is forc
+00030af0: 6564 2062 7574 2077 6520 6361 6c63 756c  ed but we calcul
+00030b00: 6174 6520 6974 2069 6e74 6f20 616e 6f74  ate it into anot
+00030b10: 6865 7220 6172 7261 7920 7765 206e 6565  her array we nee
+00030b20: 6420 746f 2063 6f70 7920 7468 6520 7265  d to copy the re
+00030b30: 7375 6c74 2069 6e74 6f20 7468 6520 6f75  sult into the ou
+00030b40: 7470 7574 0d0a 2020 2020 2020 2020 2020  tput..          
+00030b50: 2020 2020 2020 6966 206e 6f74 2072 632e        if not rc.
+00030b60: 436f 6d70 6172 654e 756d 7079 4d65 6d41  CompareNumpyMemA
+00030b70: 6464 7265 7373 286f 7574 5f61 7267 735b  ddress(out_args[
+00030b80: 305d 2c20 7265 7375 6c74 7329 3a0d 0a20  0], results):.. 
 00030b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030ba0: 2020 6966 2046 6173 7441 7272 6179 2e56    if FastArray.V
-00030bb0: 6572 626f 7365 203e 2032 3a0d 0a20 2020  erbose > 2:..   
+00030ba0: 2020 2069 6620 4661 7374 4172 7261 792e     if FastArray.
+00030bb0: 5665 7262 6f73 6520 3e20 323a 0d0a 2020  Verbose > 2:..  
 00030bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030bd0: 2020 2020 2070 7269 6e74 280d 0a20 2020       print(..   
+00030bd0: 2020 2020 2020 7072 696e 7428 0d0a 2020        print(..  
 00030be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030bf0: 2020 2020 2020 2020 2022 2a2a 2a20 7065           "*** pe
-00030c00: 7266 6f72 6d69 6e67 2061 6e20 6578 7472  rforming an extr
-00030c10: 6120 636f 7079 2074 6f20 6d61 7463 6820  a copy to match 
-00030c20: 6f75 7470 7574 2072 6571 7565 7374 222c  output request",
-00030c30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00030c40: 2020 2020 2020 2020 2020 2020 2020 6964                id
-00030c50: 286f 7574 5f61 7267 735b 305d 292c 0d0a  (out_args[0]),..
-00030c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030c70: 2020 2020 2020 2020 2020 2020 6964 2872              id(r
-00030c80: 6573 756c 7473 292c 0d0a 2020 2020 2020  esults),..      
+00030bf0: 2020 2020 2020 2020 2020 222a 2a2a 2070            "*** p
+00030c00: 6572 666f 726d 696e 6720 616e 2065 7874  erforming an ext
+00030c10: 7261 2063 6f70 7920 746f 206d 6174 6368  ra copy to match
+00030c20: 206f 7574 7075 7420 7265 7175 6573 7422   output request"
+00030c30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00030c40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00030c50: 6428 6f75 745f 6172 6773 5b30 5d29 2c0d  d(out_args[0]),.
+00030c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030c70: 2020 2020 2020 2020 2020 2020 2069 6428               id(
+00030c80: 7265 7375 6c74 7329 2c0d 0a20 2020 2020  results),..     
 00030c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030ca0: 2020 2020 2020 6f75 745f 6172 6773 5b30        out_args[0
-00030cb0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00030ca0: 2020 2020 2020 206f 7574 5f61 7267 735b         out_args[
+00030cb0: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
 00030cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030cd0: 7265 7375 6c74 732c 0d0a 2020 2020 2020  results,..      
+00030cd0: 2072 6573 756c 7473 2c0d 0a20 2020 2020   results,..     
 00030ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030cf0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00030d00: 2020 2020 2020 2020 206f 7574 5f61 7267           out_arg
-00030d10: 735b 305d 5b2e 2e2e 5d20 3d20 7265 7375  s[0][...] = resu
-00030d20: 6c74 730d 0a20 2020 2020 2020 2020 2020  lts..           
-00030d30: 2020 2020 2020 2020 2072 6573 756c 7473           results
-00030d40: 203d 206f 7574 5f61 7267 735b 305d 0d0a   = out_args[0]..
-00030d50: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00030d60: 2072 6573 756c 7473 2069 7320 4e6f 6e65   results is None
-00030d70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00030d80: 2020 2023 2070 756e 7465 640d 0a20 2020     # punted..   
-00030d90: 2020 2020 2020 2020 2020 2020 2023 2063               # c
-00030da0: 616c 6c6d 6f64 653d 2770 270d 0a20 2020  allmode='p'..   
-00030db0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00030dc0: 4661 7374 4172 7261 792e 5665 7262 6f73  FastArray.Verbos
-00030dd0: 6520 3e20 313a 0d0a 2020 2020 2020 2020  e > 1:..        
-00030de0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00030df0: 7428 222a 2a2a 7075 6e74 6564 2075 6675  t("***punted ufu
-00030e00: 6e63 3a20 222c 2075 6675 6e63 2e6e 696e  nc: ", ufunc.nin
-00030e10: 2c20 7566 756e 632e 6e6f 7574 2c20 7566  , ufunc.nout, uf
-00030e20: 756e 632c 2061 7267 732c 206b 7761 7267  unc, args, kwarg
-00030e30: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00030e40: 2020 2020 6661 7374 5f66 756e 6374 696f      fast_functio
-00030e50: 6e20 3d20 4e6f 6e65 0d0a 2020 2020 2020  n = None..      
-00030e60: 2020 2020 2020 2020 2020 2320 6661 6c6c            # fall
-00030e70: 2074 6f20 2269 6620 6661 7374 5f66 756e   to "if fast_fun
-00030e80: 6374 696f 6e20 6973 204e 6f6e 6522 2061  ction is None" a
-00030e90: 6e64 2072 756e 2074 6872 6f75 6768 206e  nd run through n
-00030ea0: 756d 7079 2e2e 2e0d 0a0d 0a20 2020 2020  umpy.......     
-00030eb0: 2020 2020 2020 2023 2072 6573 7065 6374         # respect
-00030ec0: 2064 7479 7065 0d0a 2020 2020 2020 2020   dtype..        
-00030ed0: 2020 2020 656c 6966 2064 7479 7065 2069      elif dtype i
-00030ee0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2069  s not None and i
-00030ef0: 7369 6e73 7461 6e63 6528 7265 7375 6c74  sinstance(result
-00030f00: 732c 206e 702e 6e64 6172 7261 7929 3a0d  s, np.ndarray):.
-00030f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00030f20: 2069 6620 6474 7970 6520 6973 206e 6f74   if dtype is not
-00030f30: 2072 6573 756c 7473 2e64 7479 7065 3a0d   results.dtype:.
-00030f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00030f50: 2020 2020 2069 6620 4661 7374 4172 7261       if FastArra
-00030f60: 792e 5665 7262 6f73 6520 3e20 313a 0d0a  y.Verbose > 1:..
-00030f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030f80: 2020 2020 2020 2020 7072 696e 7428 222a          print("*
-00030f90: 2a2a 7265 7375 6c74 2066 726f 6d20 7265  **result from re
-00030fa0: 6475 6365 222c 2072 6573 756c 7473 2c20  duce", results, 
-00030fb0: 7265 7375 6c74 732e 6474 7970 652c 2064  results.dtype, d
-00030fc0: 7479 7065 290d 0a20 2020 2020 2020 2020  type)..         
-00030fd0: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
-00030fe0: 7665 7274 0d0a 2020 2020 2020 2020 2020  vert..          
-00030ff0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00031000: 7320 3d20 7265 7375 6c74 732e 6173 7479  s = results.asty
-00031010: 7065 2864 7479 7065 290d 0a0d 0a20 2020  pe(dtype)....   
-00031020: 2020 2020 2069 6620 6661 7374 5f66 756e       if fast_fun
-00031030: 6374 696f 6e20 6973 204e 6f6e 653a 0d0a  ction is None:..
-00031040: 2020 2020 2020 2020 2020 2020 2320 4361              # Ca
-00031050: 6c6c 2074 6865 206e 756d 7079 2041 5049  ll the numpy API
-00031060: 730d 0a20 2020 2020 2020 2020 2020 2023  s..            #
-00031070: 2043 6865 636b 2069 6620 7765 2063 616e   Check if we can
-00031080: 2075 7365 2074 6865 2072 6563 7963 6c65   use the recycle
-00031090: 6420 6172 7261 7973 2074 6f20 6176 6f69  d arrays to avoi
-000310a0: 6420 616e 2061 6c6c 6f63 6174 696f 6e20  d an allocation 
-000310b0: 666f 7220 7468 6520 6f75 7470 7574 2061  for the output a
-000310c0: 7272 6179 0d0a 0d0a 2020 2020 2020 2020  rray....        
-000310d0: 2020 2020 6966 2046 6173 7441 7272 6179      if FastArray
-000310e0: 2e56 6572 626f 7365 203e 2031 3a0d 0a20  .Verbose > 1:.. 
-000310f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00031100: 7269 6e74 2822 2a2a 7075 6e74 6564 206f  rint("**punted o
-00031110: 6e20 6e75 6d70 7921 222c 2075 6675 6e63  n numpy!", ufunc
-00031120: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00031130: 2023 204e 4f54 453a 2057 6520 6172 6520   # NOTE: We are 
-00031140: 676f 696e 6720 746f 206c 6574 206e 756d  going to let num
-00031150: 7079 2070 726f 6365 7373 2069 740d 0a20  py process it.. 
-00031160: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
-00031170: 6d75 7374 2063 6861 6e67 6520 616c 6c20  must change all 
-00031180: 4661 7374 4172 7261 7973 2074 6f20 6e6f  FastArrays to no
-00031190: 726d 616c 206e 756d 7079 2061 7272 6179  rmal numpy array
-000311a0: 730d 0a20 2020 2020 2020 2020 2020 2061  s..            a
-000311b0: 7267 7320 3d20 5b5d 0d0a 2020 2020 2020  rgs = []..      
-000311c0: 2020 2020 2020 666f 7220 696e 7075 7420        for input 
-000311d0: 696e 2069 6e70 7574 733a 0d0a 2020 2020  in inputs:..    
-000311e0: 2020 2020 2020 2020 2020 2020 2320 666c              # fl
-000311f0: 6970 2062 6163 6b20 746f 206e 756d 7079  ip back to numpy
-00031200: 2074 6f20 6176 6f69 6420 6572 726f 7273   to avoid errors
-00031210: 2077 6865 6e20 6e75 6d70 7920 6361 6c63   when numpy calc
-00031220: 756c 6174 6573 0d0a 2020 2020 2020 2020  ulates..        
-00031230: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00031240: 7461 6e63 6528 696e 7075 742c 2046 6173  tance(input, Fas
-00031250: 7441 7272 6179 293a 0d0a 2020 2020 2020  tArray):..      
-00031260: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-00031270: 6773 2e61 7070 656e 6428 696e 7075 742e  gs.append(input.
-00031280: 7669 6577 286e 702e 6e64 6172 7261 7929  view(np.ndarray)
-00031290: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000312a0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000312b0: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-000312c0: 6773 2e61 7070 656e 6428 696e 7075 7429  gs.append(input)
-000312d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000312e0: 6966 2068 6173 5f6f 7574 7075 7473 3a0d  if has_outputs:.
-000312f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00031300: 206f 7574 7075 7473 203d 206b 7761 7267   outputs = kwarg
-00031310: 732e 706f 7028 226f 7574 222c 204e 6f6e  s.pop("out", Non
-00031320: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00031330: 2020 2020 6966 206f 7574 7075 7473 3a0d      if outputs:.
-00031340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00031350: 2020 2020 206f 7574 5f61 7267 7320 3d20       out_args = 
-00031360: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00031370: 2020 2020 2020 2020 666f 7220 6f75 7470          for outp
-00031380: 7574 2069 6e20 6f75 7470 7574 733a 0d0a  ut in outputs:..
-00031390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000313a0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-000313b0: 7461 6e63 6528 6f75 7470 7574 2c20 4661  tance(output, Fa
-000313c0: 7374 4172 7261 7929 3a0d 0a20 2020 2020  stArray):..     
+00030cf0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+00030d00: 2020 2020 2020 2020 2020 6f75 745f 6172            out_ar
+00030d10: 6773 5b30 5d5b 2e2e 2e5d 203d 2072 6573  gs[0][...] = res
+00030d20: 756c 7473 0d0a 2020 2020 2020 2020 2020  ults..          
+00030d30: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00030d40: 7320 3d20 6f75 745f 6172 6773 5b30 5d0d  s = out_args[0].
+00030d50: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+00030d60: 6620 7265 7375 6c74 7320 6973 204e 6f6e  f results is Non
+00030d70: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00030d80: 2020 2020 2320 7075 6e74 6564 0d0a 2020      # punted..  
+00030d90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00030da0: 6361 6c6c 6d6f 6465 3d27 7027 0d0a 2020  callmode='p'..  
+00030db0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00030dc0: 2046 6173 7441 7272 6179 2e56 6572 626f   FastArray.Verbo
+00030dd0: 7365 203e 2031 3a0d 0a20 2020 2020 2020  se > 1:..       
+00030de0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00030df0: 6e74 2822 2a2a 2a70 756e 7465 6420 7566  nt("***punted uf
+00030e00: 756e 633a 2022 2c20 7566 756e 632e 6e69  unc: ", ufunc.ni
+00030e10: 6e2c 2075 6675 6e63 2e6e 6f75 742c 2075  n, ufunc.nout, u
+00030e20: 6675 6e63 2c20 6172 6773 2c20 6b77 6172  func, args, kwar
+00030e30: 6773 290d 0a20 2020 2020 2020 2020 2020  gs)..           
+00030e40: 2020 2020 2066 6173 745f 6675 6e63 7469       fast_functi
+00030e50: 6f6e 203d 204e 6f6e 650d 0a20 2020 2020  on = None..     
+00030e60: 2020 2020 2020 2020 2020 2023 2066 616c             # fal
+00030e70: 6c20 746f 2022 6966 2066 6173 745f 6675  l to "if fast_fu
+00030e80: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2220  nction is None" 
+00030e90: 616e 6420 7275 6e20 7468 726f 7567 6820  and run through 
+00030ea0: 6e75 6d70 792e 2e2e 0d0a 0d0a 2020 2020  numpy.......    
+00030eb0: 2020 2020 2020 2020 2320 7265 7370 6563          # respec
+00030ec0: 7420 6474 7970 650d 0a20 2020 2020 2020  t dtype..       
+00030ed0: 2020 2020 2065 6c69 6620 6474 7970 6520       elif dtype 
+00030ee0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00030ef0: 6973 696e 7374 616e 6365 2872 6573 756c  isinstance(resul
+00030f00: 7473 2c20 6e70 2e6e 6461 7272 6179 293a  ts, np.ndarray):
+00030f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00030f20: 2020 6966 2064 7479 7065 2069 7320 6e6f    if dtype is no
+00030f30: 7420 7265 7375 6c74 732e 6474 7970 653a  t results.dtype:
+00030f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00030f50: 2020 2020 2020 6966 2046 6173 7441 7272        if FastArr
+00030f60: 6179 2e56 6572 626f 7365 203e 2031 3a0d  ay.Verbose > 1:.
+00030f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030f80: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00030f90: 2a2a 2a72 6573 756c 7420 6672 6f6d 2072  ***result from r
+00030fa0: 6564 7563 6522 2c20 7265 7375 6c74 732c  educe", results,
+00030fb0: 2072 6573 756c 7473 2e64 7479 7065 2c20   results.dtype, 
+00030fc0: 6474 7970 6529 0d0a 2020 2020 2020 2020  dtype)..        
+00030fd0: 2020 2020 2020 2020 2020 2020 2320 636f              # co
+00030fe0: 6e76 6572 740d 0a20 2020 2020 2020 2020  nvert..         
+00030ff0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00031000: 7473 203d 2072 6573 756c 7473 2e61 7374  ts = results.ast
+00031010: 7970 6528 6474 7970 6529 0d0a 0d0a 2020  ype(dtype)....  
+00031020: 2020 2020 2020 6966 2066 6173 745f 6675        if fast_fu
+00031030: 6e63 7469 6f6e 2069 7320 4e6f 6e65 3a0d  nction is None:.
+00031040: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+00031050: 616c 6c20 7468 6520 6e75 6d70 7920 4150  all the numpy AP
+00031060: 4973 0d0a 2020 2020 2020 2020 2020 2020  Is..            
+00031070: 2320 4368 6563 6b20 6966 2077 6520 6361  # Check if we ca
+00031080: 6e20 7573 6520 7468 6520 7265 6379 636c  n use the recycl
+00031090: 6564 2061 7272 6179 7320 746f 2061 766f  ed arrays to avo
+000310a0: 6964 2061 6e20 616c 6c6f 6361 7469 6f6e  id an allocation
+000310b0: 2066 6f72 2074 6865 206f 7574 7075 7420   for the output 
+000310c0: 6172 7261 790d 0a0d 0a20 2020 2020 2020  array....       
+000310d0: 2020 2020 2069 6620 4661 7374 4172 7261       if FastArra
+000310e0: 792e 5665 7262 6f73 6520 3e20 313a 0d0a  y.Verbose > 1:..
+000310f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031100: 7072 696e 7428 222a 2a70 756e 7465 6420  print("**punted 
+00031110: 6f6e 206e 756d 7079 2122 2c20 7566 756e  on numpy!", ufun
+00031120: 6329 0d0a 0d0a 2020 2020 2020 2020 2020  c)....          
+00031130: 2020 2320 4e4f 5445 3a20 5765 2061 7265    # NOTE: We are
+00031140: 2067 6f69 6e67 2074 6f20 6c65 7420 6e75   going to let nu
+00031150: 6d70 7920 7072 6f63 6573 7320 6974 0d0a  mpy process it..
+00031160: 2020 2020 2020 2020 2020 2020 2320 5765              # We
+00031170: 206d 7573 7420 6368 616e 6765 2061 6c6c   must change all
+00031180: 2046 6173 7441 7272 6179 7320 746f 206e   FastArrays to n
+00031190: 6f72 6d61 6c20 6e75 6d70 7920 6172 7261  ormal numpy arra
+000311a0: 7973 0d0a 2020 2020 2020 2020 2020 2020  ys..            
+000311b0: 6172 6773 203d 205b 5d0d 0a20 2020 2020  args = []..     
+000311c0: 2020 2020 2020 2066 6f72 2069 6e70 7574         for input
+000311d0: 2069 6e20 696e 7075 7473 3a0d 0a20 2020   in inputs:..   
+000311e0: 2020 2020 2020 2020 2020 2020 2023 2066               # f
+000311f0: 6c69 7020 6261 636b 2074 6f20 6e75 6d70  lip back to nump
+00031200: 7920 746f 2061 766f 6964 2065 7272 6f72  y to avoid error
+00031210: 7320 7768 656e 206e 756d 7079 2063 616c  s when numpy cal
+00031220: 6375 6c61 7465 730d 0a20 2020 2020 2020  culates..       
+00031230: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+00031240: 7374 616e 6365 2869 6e70 7574 2c20 4661  stance(input, Fa
+00031250: 7374 4172 7261 7929 3a0d 0a20 2020 2020  stArray):..     
+00031260: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00031270: 7267 732e 6170 7065 6e64 2869 6e70 7574  rgs.append(input
+00031280: 2e76 6965 7728 6e70 2e6e 6461 7272 6179  .view(np.ndarray
+00031290: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000312a0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000312b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000312c0: 7267 732e 6170 7065 6e64 2869 6e70 7574  rgs.append(input
+000312d0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+000312e0: 2069 6620 6861 735f 6f75 7470 7574 733a   if has_outputs:
+000312f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00031300: 2020 6f75 7470 7574 7320 3d20 6b77 6172    outputs = kwar
+00031310: 6773 2e70 6f70 2822 6f75 7422 2c20 4e6f  gs.pop("out", No
+00031320: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
+00031330: 2020 2020 2069 6620 6f75 7470 7574 733a       if outputs:
+00031340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00031350: 2020 2020 2020 6f75 745f 6172 6773 203d        out_args =
+00031360: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00031370: 2020 2020 2020 2020 2066 6f72 206f 7574           for out
+00031380: 7075 7420 696e 206f 7574 7075 7473 3a0d  put in outputs:.
+00031390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000313a0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+000313b0: 7374 616e 6365 286f 7574 7075 742c 2046  stance(output, F
+000313c0: 6173 7441 7272 6179 293a 0d0a 2020 2020  astArray):..    
 000313d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000313e0: 2020 2020 2020 206f 7574 5f61 7267 732e         out_args.
-000313f0: 6170 7065 6e64 286f 7574 7075 742e 7669  append(output.vi
-00031400: 6577 286e 702e 6e64 6172 7261 7929 290d  ew(np.ndarray)).
-00031410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00031420: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00031430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031440: 2020 2020 2020 2020 2020 2020 6f75 745f              out_
-00031450: 6172 6773 2e61 7070 656e 6428 6f75 7470  args.append(outp
-00031460: 7574 290d 0a20 2020 2020 2020 2020 2020  ut)..           
-00031470: 2020 2020 2020 2020 2023 2072 6570 6c61           # repla
-00031480: 6365 206f 7574 0d0a 2020 2020 2020 2020  ce out..        
-00031490: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-000314a0: 6773 5b22 6f75 7422 5d20 3d20 7475 706c  gs["out"] = tupl
-000314b0: 6528 6f75 745f 6172 6773 290d 0a0d 0a20  e(out_args).... 
-000314c0: 2020 2020 2020 2020 2020 2023 204e 4f54             # NOT
-000314d0: 453a 2049 6620 7468 6520 7370 6563 6966  E: If the specif
-000314e0: 6965 6420 7566 756e 6320 2b20 696e 7075  ied ufunc + inpu
-000314f0: 7473 2063 6f6d 6269 6e61 7469 6f6e 2069  ts combination i
-00031500: 736e 2774 2073 7570 706f 7274 6564 2062  sn't supported b
-00031510: 7920 6e75 6d70 7920 6569 7468 6572 2c0d  y numpy either,.
-00031520: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-00031530: 2020 2020 2061 7320 6f66 206e 756d 7079       as of numpy
-00031540: 2031 2e31 372e 7820 7468 6973 2063 616c   1.17.x this cal
-00031550: 6c20 7769 6c6c 2065 6e64 2075 7020 7261  l will end up ra
-00031560: 6973 696e 6720 6120 5546 756e 6354 7970  ising a UFuncTyp
-00031570: 6545 7272 6f72 2073 6f20 7468 6520 7265  eError so the re
-00031580: 7374 0d0a 2020 2020 2020 2020 2020 2020  st..            
-00031590: 2320 2020 2020 2020 6f66 2074 6865 2046  #       of the F
-000315a0: 6173 7441 7272 6179 2e5f 5f61 7272 6179  astArray.__array
-000315b0: 5f75 6675 6e63 5f5f 2062 6f64 7920 2862  _ufunc__ body (b
-000315c0: 656c 6f77 2920 776f 6e27 7420 656e 6420  elow) won't end 
-000315d0: 7570 2065 7865 6375 7469 6e67 2e0d 0a20  up executing... 
-000315e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000315f0: 7473 203d 2054 7970 6552 6567 6973 7465  ts = TypeRegiste
-00031600: 722e 4d61 7468 4c65 6467 6572 2e5f 4152  r.MathLedger._AR
-00031610: 5241 595f 5546 554e 4328 7375 7065 7228  RAY_UFUNC(super(
-00031620: 4661 7374 4172 7261 792c 2073 656c 6629  FastArray, self)
-00031630: 2c20 7566 756e 632c 206d 6574 686f 642c  , ufunc, method,
-00031640: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-00031650: 290d 0a0d 0a20 2020 2020 2020 2023 2049  )....        # I
-00031660: 6620 7269 7074 6162 6c65 2068 6173 206e  f riptable has n
-00031670: 6f74 2069 6d70 6c65 6d65 6e74 6564 2061  ot implemented a
-00031680: 2063 6572 7461 696e 2075 6675 6e63 2028   certain ufunc (
-00031690: 6f72 2064 6f65 736e 2774 2073 7570 706f  or doesn't suppo
-000316a0: 7274 2069 7420 666f 7220 7468 6520 6769  rt it for the gi
-000316b0: 7665 6e20 6172 6775 6d65 6e74 7329 2c0d  ven arguments),.
-000316c0: 0a20 2020 2020 2020 2023 2065 6d69 7420  .        # emit 
-000316d0: 6120 7761 726e 696e 6720 6162 6f75 7420  a warning about 
-000316e0: 6974 2074 6f20 6c65 7420 7468 6520 7573  it to let the us
-000316f0: 6572 206b 6e6f 772e 0d0a 2020 2020 2020  er know...      
-00031700: 2020 2320 5768 656e 206e 756d 7079 2064    # When numpy d
-00031710: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
-00031720: 7468 6520 7566 756e 632b 696e 7075 7473  the ufunc+inputs
-00031730: 2065 6974 6865 722c 2077 6520 776f 6e27   either, we won'
-00031740: 7420 7265 6163 6820 7468 6973 2070 6f69  t reach this poi
-00031750: 6e74 2028 6173 206f 6620 6e75 6d70 7920  nt (as of numpy 
-00031760: 312e 3137 2e78 292c 0d0a 2020 2020 2020  1.17.x),..      
-00031770: 2020 2320 7369 6e63 6520 6e75 6d70 7920    # since numpy 
-00031780: 7769 6c6c 2072 6169 7365 2061 2055 4675  will raise a UFu
-00031790: 6e63 5479 7065 4572 726f 7220 6561 726c  ncTypeError earl
-000317a0: 6965 7220 2862 6566 6f72 6520 7468 6973  ier (before this
-000317b0: 2070 6f69 6e74 2920 7261 7468 6572 2074   point) rather t
-000317c0: 6861 6e20 6166 7465 7220 7765 2072 6574  han after we ret
-000317d0: 7572 6e20 4e6f 7449 6d70 6c65 6d65 6e74  urn NotImplement
-000317e0: 6564 2e0d 0a20 2020 2020 2020 2069 6620  ed...        if 
-000317f0: 7265 7375 6c74 7320 6973 204e 6f74 496d  results is NotIm
-00031800: 706c 656d 656e 7465 643a 0d0a 2020 2020  plemented:..    
-00031810: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-00031820: 2e77 6172 6e28 6622 2a2a 2a75 6675 6e63  .warn(f"***ufunc
-00031830: 207b 7566 756e 637d 207b 6172 6773 7d20   {ufunc} {args} 
-00031840: 7b6b 7761 7267 737d 2069 7320 6e6f 7420  {kwargs} is not 
-00031850: 696d 706c 656d 656e 7465 6422 290d 0a20  implemented").. 
-00031860: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00031870: 6e20 4e6f 7449 6d70 6c65 6d65 6e74 6564  n NotImplemented
-00031880: 0d0a 0d0a 2020 2020 2020 2020 2320 5566  ....        # Uf
-00031890: 756e 6373 2061 6c73 6f20 6861 7665 2061  uncs also have a
-000318a0: 2066 6966 7468 206d 6574 686f 6420 7468   fifth method th
-000318b0: 6174 2061 6c6c 6f77 7320 696e 2070 6c61  at allows in pla
-000318c0: 6365 206f 7065 7261 7469 6f6e 7320 746f  ce operations to
-000318d0: 2062 6520 7065 7266 6f72 6d65 6420 7573   be performed us
-000318e0: 696e 6720 6661 6e63 7920 696e 6465 7869  ing fancy indexi
-000318f0: 6e67 2e0d 0a20 2020 2020 2020 2023 204e  ng...        # N
-00031900: 6f20 6275 6666 6572 696e 6720 6973 2075  o buffering is u
-00031910: 7365 6420 6f6e 2074 6865 2064 696d 656e  sed on the dimen
-00031920: 7369 6f6e 7320 7768 6572 6520 6661 6e63  sions where fanc
-00031930: 7920 696e 6465 7869 6e67 2069 7320 7573  y indexing is us
-00031940: 6564 2c20 736f 2074 6865 2066 616e 6379  ed, so the fancy
-00031950: 2069 6e64 6578 2063 616e 206c 6973 7420   index can list 
-00031960: 616e 2069 7465 6d20 6d6f 7265 2074 6861  an item more tha
-00031970: 6e20 6f6e 6365 0d0a 2020 2020 2020 2020  n once..        
-00031980: 2320 2020 2020 616e 6420 7468 6520 6f70  #     and the op
-00031990: 6572 6174 696f 6e20 7769 6c6c 2062 6520  eration will be 
-000319a0: 7065 7266 6f72 6d65 6420 6f6e 2074 6865  performed on the
-000319b0: 2072 6573 756c 7420 6f66 2074 6865 2070   result of the p
-000319c0: 7265 7669 6f75 7320 6f70 6572 6174 696f  revious operatio
-000319d0: 6e20 666f 7220 7468 6174 2069 7465 6d2e  n for that item.
-000319e0: 0d0a 2020 2020 2020 2020 2320 7566 756e  ..        # ufun
-000319f0: 632e 7265 6475 6365 2861 5b2c 2061 7869  c.reduce(a[, axi
-00031a00: 732c 2064 7479 7065 2c20 6f75 742c 206b  s, dtype, out, k
-00031a10: 6565 7064 696d 735d 2909 5265 6475 6365  eepdims]).Reduce
-00031a20: 7320 6127 7320 6469 6d65 6e73 696f 6e20  s a's dimension 
-00031a30: 6279 206f 6e65 2c20 6279 2061 7070 6c79  by one, by apply
-00031a40: 696e 6720 7566 756e 6320 616c 6f6e 6720  ing ufunc along 
-00031a50: 6f6e 6520 6178 6973 2e0d 0a20 2020 2020  one axis...     
-00031a60: 2020 2023 2075 6675 6e63 2e61 6363 756d     # ufunc.accum
-00031a70: 756c 6174 6528 6172 7261 795b 2c20 6178  ulate(array[, ax
-00031a80: 6973 2c20 6474 7970 652c 206f 7574 5d29  is, dtype, out])
-00031a90: 0941 6363 756d 756c 6174 6520 7468 6520  .Accumulate the 
-00031aa0: 7265 7375 6c74 206f 6620 6170 706c 7969  result of applyi
-00031ab0: 6e67 2074 6865 206f 7065 7261 746f 7220  ng the operator 
-00031ac0: 746f 2061 6c6c 2065 6c65 6d65 6e74 732e  to all elements.
-00031ad0: 0d0a 2020 2020 2020 2020 2320 7566 756e  ..        # ufun
-00031ae0: 632e 7265 6475 6365 6174 2861 2c20 696e  c.reduceat(a, in
-00031af0: 6469 6365 735b 2c20 6178 6973 2c20 6474  dices[, axis, dt
-00031b00: 7970 652c 206f 7574 5d29 0950 6572 666f  ype, out]).Perfo
-00031b10: 726d 7320 6120 286c 6f63 616c 2920 7265  rms a (local) re
-00031b20: 6475 6365 2077 6974 6820 7370 6563 6966  duce with specif
-00031b30: 6965 6420 736c 6963 6573 206f 7665 7220  ied slices over 
-00031b40: 6120 7369 6e67 6c65 2061 7869 732e 0d0a  a single axis...
-00031b50: 2020 2020 2020 2020 2320 7566 756e 632e          # ufunc.
-00031b60: 6f75 7465 7228 412c 2042 2909 4170 706c  outer(A, B).Appl
-00031b70: 7920 7468 6520 7566 756e 6320 6f70 2074  y the ufunc op t
-00031b80: 6f20 616c 6c20 7061 6972 7320 2861 2c20  o all pairs (a, 
-00031b90: 6229 2077 6974 6820 6120 696e 2041 2061  b) with a in A a
-00031ba0: 6e64 2062 2069 6e20 422e 0d0a 2020 2020  nd b in B...    
-00031bb0: 2020 2020 2320 7566 756e 632e 6174 2861      # ufunc.at(a
-00031bc0: 2c20 696e 6469 6365 735b 2c20 625d 2909  , indices[, b]).
-00031bd0: 5065 7266 6f72 6d73 2075 6e62 7566 6665  Performs unbuffe
-00031be0: 7265 6420 696e 2070 6c61 6365 206f 7065  red in place ope
-00031bf0: 7261 7469 6f6e 206f 6e20 6f70 6572 616e  ration on operan
-00031c00: 6420 2761 2720 666f 7220 656c 656d 656e  d 'a' for elemen
-00031c10: 7473 2073 7065 6369 6669 6564 2062 7920  ts specified by 
-00031c20: 2769 6e64 6963 6573 272e 0d0a 0d0a 2020  'indices'.....  
-00031c30: 2020 2020 2020 6966 206d 6574 686f 6420        if method 
-00031c40: 3d3d 2022 6174 223a 0d0a 2020 2020 2020  == "at":..      
-00031c50: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
-00031c60: 2020 2020 2020 2020 6966 2075 6675 6e63          if ufunc
-00031c70: 2e6e 6f75 7420 3d3d 2031 3a0d 0a20 2020  .nout == 1:..   
-00031c80: 2020 2020 2020 2020 2023 2063 6865 636b           # check
-00031c90: 2069 6620 7765 2075 7365 6420 6f75 7220   if we used our 
-00031ca0: 6f77 6e20 6f75 7470 7574 0d0a 0d0a 2020  own output....  
-00031cb0: 2020 2020 2020 2020 2020 2320 6966 2069            # if i
-00031cc0: 7369 6e73 7461 6e63 6528 6f75 7441 7272  sinstance(outArr
-00031cd0: 6179 2c20 6e70 2e6e 6461 7272 6179 293a  ay, np.ndarray):
-00031ce0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00031cf0: 2020 2072 6574 7572 6e20 6f75 7441 7272     return outArr
-00031d00: 6179 2e76 6965 7728 4661 7374 4172 7261  ay.view(FastArra
-00031d10: 7929 0d0a 0d0a 2020 2020 2020 2020 2020  y)....          
-00031d20: 2020 2320 6966 2028 6669 6e61 6c5f 6474    # if (final_dt
-00031d30: 7970 6520 213d 204e 6f6e 6520 616e 6420  ype != None and 
-00031d40: 6669 6e61 6c5f 6474 7970 6520 213d 2072  final_dtype != r
-00031d50: 6573 756c 7473 2e64 7479 7065 293a 0d0a  esults.dtype):..
-00031d60: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-00031d70: 2070 7269 6e74 2822 2a2a 2a2a 2a2a 206d   print("****** m
-00031d80: 6973 7072 6564 6963 7465 6420 6669 6e61  ispredicted fina
-00031d90: 6c22 2c20 6669 6e61 6c5f 6474 7970 652c  l", final_dtype,
-00031da0: 2072 6573 756c 7473 2e64 7479 7065 2c20   results.dtype, 
-00031db0: 7566 756e 632c 2073 6361 6c61 7274 7970  ufunc, scalartyp
-00031dc0: 6573 2c20 6172 6773 2c20 6f75 7470 7574  es, args, output
-00031dd0: 732c 206b 7761 7267 7329 3b0d 0a20 2020  s, kwargs);..   
-00031de0: 2020 2020 2020 2020 2023 2072 6573 756c           # resul
-00031df0: 7473 203d 2028 7265 7375 6c74 732c 290d  ts = (results,).
-00031e00: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-00031e10: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-00031e20: 2872 6573 756c 7473 2c20 4661 7374 4172  (results, FastAr
-00031e30: 7261 7929 2061 6e64 2069 7369 6e73 7461  ray) and isinsta
-00031e40: 6e63 6528 7265 7375 6c74 732c 206e 702e  nce(results, np.
-00031e50: 6e64 6172 7261 7929 3a0d 0a20 2020 2020  ndarray):..     
-00031e60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00031e70: 6e20 7265 7375 6c74 732e 7669 6577 2846  n results.view(F
-00031e80: 6173 7441 7272 6179 290d 0a0d 0a20 2020  astArray)....   
-00031e90: 2020 2020 2020 2020 2023 2074 6869 6e6b           # think
-00031ea0: 2068 6974 2068 6572 6520 666f 7220 7375   hit here for su
-00031eb0: 6d20 7769 6863 6820 646f 6573 206e 6f74  m wihch does not
-00031ec0: 2072 6574 7572 6e20 616e 2061 7272 6179   return an array
-00031ed0: 2c20 6a75 7374 2061 206e 756d 6265 720d  , just a number.
-00031ee0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00031ef0: 7572 6e20 7265 7375 6c74 730d 0a0d 0a20  urn results.... 
-00031f00: 2020 2020 2020 2023 206d 6f72 6520 7468         # more th
-00031f10: 616e 206f 6e65 2069 7465 6d2c 2073 6f20  an one item, so 
-00031f20: 7765 2061 7265 206d 616b 696e 6720 6120  we are making a 
-00031f30: 7475 706c 650d 0a20 2020 2020 2020 2023  tuple..        #
-00031f40: 2063 616e 2072 6573 756c 7420 696e 205f   can result in _
-00031f50: 5f61 7272 6179 5f66 696e 616c 697a 655f  _array_finalize_
-00031f60: 5f20 6265 696e 6720 6361 6c6c 6564 0d0a  _ being called..
-00031f70: 2020 2020 2020 2020 7265 7375 6c74 7320          results 
-00031f80: 3d20 7475 706c 6528 0d0a 2020 2020 2020  = tuple(..      
-00031f90: 2020 2020 2020 286e 702e 6173 6172 7261        (np.asarra
-00031fa0: 7928 7265 7375 6c74 292e 7669 6577 2846  y(result).view(F
-00031fb0: 6173 7441 7272 6179 2920 6966 206f 7574  astArray) if out
-00031fc0: 7075 7420 6973 204e 6f6e 6520 656c 7365  put is None else
-00031fd0: 206f 7574 7075 7429 0d0a 2020 2020 2020   output)..      
-00031fe0: 2020 2020 2020 666f 7220 7265 7375 6c74        for result
-00031ff0: 2c20 6f75 7470 7574 2069 6e20 7a69 7028  , output in zip(
-00032000: 7265 7375 6c74 732c 206f 7574 7075 7473  results, outputs
-00032010: 290d 0a20 2020 2020 2020 2029 0d0a 0d0a  )..        )....
-00032020: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
-00032030: 6966 2077 6520 6861 7665 2061 2074 7570  if we have a tup
-00032040: 6c65 206f 6620 6f6e 6520 6974 656d 2c20  le of one item, 
-00032050: 6966 2073 6f20 6a75 7374 2072 6574 7572  if so just retur
-00032060: 6e20 7468 6520 6f6e 6520 6974 656d 0d0a  n the one item..
-00032070: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
-00032080: 6573 756c 7473 2920 3d3d 2031 3a0d 0a20  esults) == 1:.. 
-00032090: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000320a0: 7473 203d 2072 6573 756c 7473 5b30 5d0d  ts = results[0].
-000320b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000320c0: 7265 7375 6c74 730d 0a0d 0a20 2020 2040  results....    @
-000320d0: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
-000320e0: 6620 6e75 6d62 6173 7472 696e 6728 7365  f numbastring(se
-000320f0: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
-00032100: 220d 0a20 2020 2020 2020 2063 6f6e 7665  "..        conve
-00032110: 7274 7320 6279 7465 2073 7472 696e 6720  rts byte string 
-00032120: 616e 6420 756e 6963 6f64 6520 7374 7269  and unicode stri
-00032130: 6e67 7320 746f 2061 2032 6469 6d65 6e73  ngs to a 2dimens
-00032140: 696f 6e61 6c20 6172 7261 790d 0a20 2020  ional array..   
-00032150: 2020 2020 2073 6f20 7468 6174 206e 756d       so that num
-00032160: 6261 2063 616e 2070 726f 6365 7373 2069  ba can process i
-00032170: 7420 636f 7272 6563 746c 790d 0a0d 0a20  t correctly.... 
-00032180: 2020 2020 2020 2045 7861 6d70 6c65 730d         Examples.
-00032190: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000321a0: 2d0d 0a20 2020 2020 2020 203e 3e3e 2040  -..        >>> @
-000321b0: 6e75 6d62 612e 6a69 7428 6e6f 7079 7468  numba.jit(nopyth
-000321c0: 6f6e 3d54 7275 6529 0d0a 2020 2020 2020  on=True)..      
-000321d0: 2020 2e2e 2e20 6465 6620 6e75 6d62 615f    ... def numba_
-000321e0: 7374 7228 7478 7429 3a0d 0a20 2020 2020  str(txt):..     
-000321f0: 2020 202e 2e2e 2020 2020 2078 3d30 0d0a     ...     x=0..
-00032200: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-00032210: 666f 7220 6920 696e 2072 616e 6765 2874  for i in range(t
-00032220: 7874 2e73 6861 7065 5b30 5d29 3a0d 0a20  xt.shape[0]):.. 
-00032230: 2020 2020 2020 202e 2e2e 2020 2020 2020         ...      
-00032240: 2020 2069 6620 2874 7874 5b69 2c30 5d3d     if (txt[i,0]=
-00032250: 3d31 3136 2061 6e64 2020 2320 2774 270d  =116 and  # 't'.
-00032260: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
-00032270: 2020 2020 2020 2020 2074 7874 5b69 2c31           txt[i,1
-00032280: 5d3d 3d31 3031 2061 6e64 2020 2320 2765  ]==101 and  # 'e
-00032290: 270d 0a20 2020 2020 2020 202e 2e2e 2020  '..        ...  
-000322a0: 2020 2020 2020 2020 2020 2074 7874 5b69             txt[i
-000322b0: 2c32 5d3d 3d31 3230 2061 6e64 2020 2320  ,2]==120 and  # 
-000322c0: 2778 270d 0a20 2020 2020 2020 202e 2e2e  'x'..        ...
-000322d0: 2020 2020 2020 2020 2020 2020 2074 7874               txt
-000322e0: 5b69 2c33 5d3d 3d31 3136 293a 2020 2020  [i,3]==116):    
-000322f0: 2320 2774 270d 0a20 2020 2020 2020 202e  # 't'..        .
-00032300: 2e2e 2020 2020 2020 2020 2020 2020 2078  ..             x
-00032310: 202b 3d20 310d 0a20 2020 2020 2020 202e   += 1..        .
-00032320: 2e2e 2020 2020 2072 6574 7572 6e20 780d  ..     return x.
-00032330: 0a20 2020 2020 2020 203e 3e3e 0d0a 2020  .        >>>..  
-00032340: 2020 2020 2020 3e3e 3e20 783d 4661 7374        >>> x=Fast
-00032350: 4172 7261 7928 5b27 736f 6d65 272c 2774  Array(['some','t
-00032360: 6578 7427 2c27 7468 6973 272c 2769 7327  ext','this','is'
-00032370: 5d29 0d0a 2020 2020 2020 2020 3e3e 3e20  ])..        >>> 
-00032380: 6e75 6d62 615f 7374 7228 782e 7669 6577  numba_str(x.view
-00032390: 286e 702e 7569 6e74 3829 2e72 6573 6861  (np.uint8).resha
-000323a0: 7065 2828 6c65 6e28 7829 2c20 782e 6974  pe((len(x), x.it
-000323b0: 656d 7369 7a65 2929 290d 0a20 2020 2020  emsize)))..     
-000323c0: 2020 203e 3e3e 206e 756d 6261 5f73 7472     >>> numba_str
-000323d0: 2878 2e6e 756d 6261 7374 7269 6e67 290d  (x.numbastring).
-000323e0: 0a20 2020 2020 2020 2022 2222 0d0a 0d0a  .        """....
-000323f0: 2020 2020 2020 2020 696e 7479 7065 203d          intype =
-00032400: 2073 656c 662e 6474 7970 652e 5f5f 7374   self.dtype.__st
-00032410: 725f 5f28 290d 0a20 2020 2020 2020 2069  r__()..        i
-00032420: 6620 696e 7479 7065 5b30 5d20 3d3d 2022  f intype[0] == "
-00032430: 7c22 206f 7220 696e 7479 7065 5b30 5d20  |" or intype[0] 
-00032440: 3d3d 2022 3c22 3a0d 0a20 2020 2020 2020  == "<":..       
-00032450: 2020 2020 2069 6620 696e 7479 7065 5b31       if intype[1
-00032460: 5d20 3d3d 2022 5322 3a0d 0a20 2020 2020  ] == "S":..     
-00032470: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00032480: 6e20 7365 6c66 2e76 6965 7728 6e70 2e75  n self.view(np.u
-00032490: 696e 7438 292e 7265 7368 6170 6528 286c  int8).reshape((l
-000324a0: 656e 2873 656c 6629 2c20 7365 6c66 2e69  en(self), self.i
-000324b0: 7465 6d73 697a 6529 290d 0a20 2020 2020  temsize))..     
-000324c0: 2020 2020 2020 2069 6620 696e 7479 7065         if intype
-000324d0: 5b31 5d20 3d3d 2022 5522 3a0d 0a20 2020  [1] == "U":..   
-000324e0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-000324f0: 7572 6e20 7365 6c66 2e76 6965 7728 6e70  urn self.view(np
-00032500: 2e75 696e 7433 3229 2e72 6573 6861 7065  .uint32).reshape
-00032510: 2828 6c65 6e28 7365 6c66 292c 2073 656c  ((len(self), sel
-00032520: 662e 6974 656d 7369 7a65 202f 2f20 3429  f.itemsize // 4)
-00032530: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00032540: 6e20 7365 6c66 0d0a 0d0a 2020 2020 2320  n self....    # 
-00032550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000313e0: 2020 2020 2020 2020 6f75 745f 6172 6773          out_args
+000313f0: 2e61 7070 656e 6428 6f75 7470 7574 2e76  .append(output.v
+00031400: 6965 7728 6e70 2e6e 6461 7272 6179 2929  iew(np.ndarray))
+00031410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00031420: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00031430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00031440: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00031450: 5f61 7267 732e 6170 7065 6e64 286f 7574  _args.append(out
+00031460: 7075 7429 0d0a 2020 2020 2020 2020 2020  put)..          
+00031470: 2020 2020 2020 2020 2020 2320 7265 706c            # repl
+00031480: 6163 6520 6f75 740d 0a20 2020 2020 2020  ace out..       
+00031490: 2020 2020 2020 2020 2020 2020 206b 7761               kwa
+000314a0: 7267 735b 226f 7574 225d 203d 2074 7570  rgs["out"] = tup
+000314b0: 6c65 286f 7574 5f61 7267 7329 0d0a 0d0a  le(out_args)....
+000314c0: 2020 2020 2020 2020 2020 2020 2320 4e4f              # NO
+000314d0: 5445 3a20 4966 2074 6865 2073 7065 6369  TE: If the speci
+000314e0: 6669 6564 2075 6675 6e63 202b 2069 6e70  fied ufunc + inp
+000314f0: 7574 7320 636f 6d62 696e 6174 696f 6e20  uts combination 
+00031500: 6973 6e27 7420 7375 7070 6f72 7465 6420  isn't supported 
+00031510: 6279 206e 756d 7079 2065 6974 6865 722c  by numpy either,
+00031520: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00031530: 2020 2020 2020 6173 206f 6620 6e75 6d70        as of nump
+00031540: 7920 312e 3137 2e78 2074 6869 7320 6361  y 1.17.x this ca
+00031550: 6c6c 2077 696c 6c20 656e 6420 7570 2072  ll will end up r
+00031560: 6169 7369 6e67 2061 2055 4675 6e63 5479  aising a UFuncTy
+00031570: 7065 4572 726f 7220 736f 2074 6865 2072  peError so the r
+00031580: 6573 740d 0a20 2020 2020 2020 2020 2020  est..           
+00031590: 2023 2020 2020 2020 206f 6620 7468 6520   #       of the 
+000315a0: 4661 7374 4172 7261 792e 5f5f 6172 7261  FastArray.__arra
+000315b0: 795f 7566 756e 635f 5f20 626f 6479 2028  y_ufunc__ body (
+000315c0: 6265 6c6f 7729 2077 6f6e 2774 2065 6e64  below) won't end
+000315d0: 2075 7020 6578 6563 7574 696e 672e 0d0a   up executing...
+000315e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000315f0: 6c74 7320 3d20 5479 7065 5265 6769 7374  lts = TypeRegist
+00031600: 6572 2e4d 6174 684c 6564 6765 722e 5f41  er.MathLedger._A
+00031610: 5252 4159 5f55 4655 4e43 2873 7570 6572  RRAY_UFUNC(super
+00031620: 2846 6173 7441 7272 6179 2c20 7365 6c66  (FastArray, self
+00031630: 292c 2075 6675 6e63 2c20 6d65 7468 6f64  ), ufunc, method
+00031640: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
+00031650: 7329 0d0a 0d0a 2020 2020 2020 2020 2320  s)....        # 
+00031660: 4966 2072 6970 7461 626c 6520 6861 7320  If riptable has 
+00031670: 6e6f 7420 696d 706c 656d 656e 7465 6420  not implemented 
+00031680: 6120 6365 7274 6169 6e20 7566 756e 6320  a certain ufunc 
+00031690: 286f 7220 646f 6573 6e27 7420 7375 7070  (or doesn't supp
+000316a0: 6f72 7420 6974 2066 6f72 2074 6865 2067  ort it for the g
+000316b0: 6976 656e 2061 7267 756d 656e 7473 292c  iven arguments),
+000316c0: 0d0a 2020 2020 2020 2020 2320 656d 6974  ..        # emit
+000316d0: 2061 2077 6172 6e69 6e67 2061 626f 7574   a warning about
+000316e0: 2069 7420 746f 206c 6574 2074 6865 2075   it to let the u
+000316f0: 7365 7220 6b6e 6f77 2e0d 0a20 2020 2020  ser know...     
+00031700: 2020 2023 2057 6865 6e20 6e75 6d70 7920     # When numpy 
+00031710: 646f 6573 206e 6f74 2073 7570 706f 7274  does not support
+00031720: 2074 6865 2075 6675 6e63 2b69 6e70 7574   the ufunc+input
+00031730: 7320 6569 7468 6572 2c20 7765 2077 6f6e  s either, we won
+00031740: 2774 2072 6561 6368 2074 6869 7320 706f  't reach this po
+00031750: 696e 7420 2861 7320 6f66 206e 756d 7079  int (as of numpy
+00031760: 2031 2e31 372e 7829 2c0d 0a20 2020 2020   1.17.x),..     
+00031770: 2020 2023 2073 696e 6365 206e 756d 7079     # since numpy
+00031780: 2077 696c 6c20 7261 6973 6520 6120 5546   will raise a UF
+00031790: 756e 6354 7970 6545 7272 6f72 2065 6172  uncTypeError ear
+000317a0: 6c69 6572 2028 6265 666f 7265 2074 6869  lier (before thi
+000317b0: 7320 706f 696e 7429 2072 6174 6865 7220  s point) rather 
+000317c0: 7468 616e 2061 6674 6572 2077 6520 7265  than after we re
+000317d0: 7475 726e 204e 6f74 496d 706c 656d 656e  turn NotImplemen
+000317e0: 7465 642e 0d0a 2020 2020 2020 2020 6966  ted...        if
+000317f0: 2072 6573 756c 7473 2069 7320 4e6f 7449   results is NotI
+00031800: 6d70 6c65 6d65 6e74 6564 3a0d 0a20 2020  mplemented:..   
+00031810: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+00031820: 732e 7761 726e 2866 222a 2a2a 7566 756e  s.warn(f"***ufun
+00031830: 6320 7b75 6675 6e63 7d20 7b61 7267 737d  c {ufunc} {args}
+00031840: 207b 6b77 6172 6773 7d20 6973 206e 6f74   {kwargs} is not
+00031850: 2069 6d70 6c65 6d65 6e74 6564 2229 0d0a   implemented")..
+00031860: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00031870: 726e 204e 6f74 496d 706c 656d 656e 7465  rn NotImplemente
+00031880: 640d 0a0d 0a20 2020 2020 2020 2023 2055  d....        # U
+00031890: 6675 6e63 7320 616c 736f 2068 6176 6520  funcs also have 
+000318a0: 6120 6669 6674 6820 6d65 7468 6f64 2074  a fifth method t
+000318b0: 6861 7420 616c 6c6f 7773 2069 6e20 706c  hat allows in pl
+000318c0: 6163 6520 6f70 6572 6174 696f 6e73 2074  ace operations t
+000318d0: 6f20 6265 2070 6572 666f 726d 6564 2075  o be performed u
+000318e0: 7369 6e67 2066 616e 6379 2069 6e64 6578  sing fancy index
+000318f0: 696e 672e 0d0a 2020 2020 2020 2020 2320  ing...        # 
+00031900: 4e6f 2062 7566 6665 7269 6e67 2069 7320  No buffering is 
+00031910: 7573 6564 206f 6e20 7468 6520 6469 6d65  used on the dime
+00031920: 6e73 696f 6e73 2077 6865 7265 2066 616e  nsions where fan
+00031930: 6379 2069 6e64 6578 696e 6720 6973 2075  cy indexing is u
+00031940: 7365 642c 2073 6f20 7468 6520 6661 6e63  sed, so the fanc
+00031950: 7920 696e 6465 7820 6361 6e20 6c69 7374  y index can list
+00031960: 2061 6e20 6974 656d 206d 6f72 6520 7468   an item more th
+00031970: 616e 206f 6e63 650d 0a20 2020 2020 2020  an once..       
+00031980: 2023 2020 2020 2061 6e64 2074 6865 206f   #     and the o
+00031990: 7065 7261 7469 6f6e 2077 696c 6c20 6265  peration will be
+000319a0: 2070 6572 666f 726d 6564 206f 6e20 7468   performed on th
+000319b0: 6520 7265 7375 6c74 206f 6620 7468 6520  e result of the 
+000319c0: 7072 6576 696f 7573 206f 7065 7261 7469  previous operati
+000319d0: 6f6e 2066 6f72 2074 6861 7420 6974 656d  on for that item
+000319e0: 2e0d 0a20 2020 2020 2020 2023 2075 6675  ...        # ufu
+000319f0: 6e63 2e72 6564 7563 6528 615b 2c20 6178  nc.reduce(a[, ax
+00031a00: 6973 2c20 6474 7970 652c 206f 7574 2c20  is, dtype, out, 
+00031a10: 6b65 6570 6469 6d73 5d29 0952 6564 7563  keepdims]).Reduc
+00031a20: 6573 2061 2773 2064 696d 656e 7369 6f6e  es a's dimension
+00031a30: 2062 7920 6f6e 652c 2062 7920 6170 706c   by one, by appl
+00031a40: 7969 6e67 2075 6675 6e63 2061 6c6f 6e67  ying ufunc along
+00031a50: 206f 6e65 2061 7869 732e 0d0a 2020 2020   one axis...    
+00031a60: 2020 2020 2320 7566 756e 632e 6163 6375      # ufunc.accu
+00031a70: 6d75 6c61 7465 2861 7272 6179 5b2c 2061  mulate(array[, a
+00031a80: 7869 732c 2064 7479 7065 2c20 6f75 745d  xis, dtype, out]
+00031a90: 2909 4163 6375 6d75 6c61 7465 2074 6865  ).Accumulate the
+00031aa0: 2072 6573 756c 7420 6f66 2061 7070 6c79   result of apply
+00031ab0: 696e 6720 7468 6520 6f70 6572 6174 6f72  ing the operator
+00031ac0: 2074 6f20 616c 6c20 656c 656d 656e 7473   to all elements
+00031ad0: 2e0d 0a20 2020 2020 2020 2023 2075 6675  ...        # ufu
+00031ae0: 6e63 2e72 6564 7563 6561 7428 612c 2069  nc.reduceat(a, i
+00031af0: 6e64 6963 6573 5b2c 2061 7869 732c 2064  ndices[, axis, d
+00031b00: 7479 7065 2c20 6f75 745d 2909 5065 7266  type, out]).Perf
+00031b10: 6f72 6d73 2061 2028 6c6f 6361 6c29 2072  orms a (local) r
+00031b20: 6564 7563 6520 7769 7468 2073 7065 6369  educe with speci
+00031b30: 6669 6564 2073 6c69 6365 7320 6f76 6572  fied slices over
+00031b40: 2061 2073 696e 676c 6520 6178 6973 2e0d   a single axis..
+00031b50: 0a20 2020 2020 2020 2023 2075 6675 6e63  .        # ufunc
+00031b60: 2e6f 7574 6572 2841 2c20 4229 0941 7070  .outer(A, B).App
+00031b70: 6c79 2074 6865 2075 6675 6e63 206f 7020  ly the ufunc op 
+00031b80: 746f 2061 6c6c 2070 6169 7273 2028 612c  to all pairs (a,
+00031b90: 2062 2920 7769 7468 2061 2069 6e20 4120   b) with a in A 
+00031ba0: 616e 6420 6220 696e 2042 2e0d 0a20 2020  and b in B...   
+00031bb0: 2020 2020 2023 2075 6675 6e63 2e61 7428       # ufunc.at(
+00031bc0: 612c 2069 6e64 6963 6573 5b2c 2062 5d29  a, indices[, b])
+00031bd0: 0950 6572 666f 726d 7320 756e 6275 6666  .Performs unbuff
+00031be0: 6572 6564 2069 6e20 706c 6163 6520 6f70  ered in place op
+00031bf0: 6572 6174 696f 6e20 6f6e 206f 7065 7261  eration on opera
+00031c00: 6e64 2027 6127 2066 6f72 2065 6c65 6d65  nd 'a' for eleme
+00031c10: 6e74 7320 7370 6563 6966 6965 6420 6279  nts specified by
+00031c20: 2027 696e 6469 6365 7327 2e0d 0a0d 0a20   'indices'..... 
+00031c30: 2020 2020 2020 2069 6620 6d65 7468 6f64         if method
+00031c40: 203d 3d20 2261 7422 3a0d 0a20 2020 2020   == "at":..     
+00031c50: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
+00031c60: 0a20 2020 2020 2020 2069 6620 7566 756e  .        if ufun
+00031c70: 632e 6e6f 7574 203d 3d20 313a 0d0a 2020  c.nout == 1:..  
+00031c80: 2020 2020 2020 2020 2020 2320 6368 6563            # chec
+00031c90: 6b20 6966 2077 6520 7573 6564 206f 7572  k if we used our
+00031ca0: 206f 776e 206f 7574 7075 740d 0a0d 0a20   own output.... 
+00031cb0: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
+00031cc0: 6973 696e 7374 616e 6365 286f 7574 4172  isinstance(outAr
+00031cd0: 7261 792c 206e 702e 6e64 6172 7261 7929  ray, np.ndarray)
+00031ce0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+00031cf0: 2020 2020 7265 7475 726e 206f 7574 4172      return outAr
+00031d00: 7261 792e 7669 6577 2846 6173 7441 7272  ray.view(FastArr
+00031d10: 6179 290d 0a0d 0a20 2020 2020 2020 2020  ay)....         
+00031d20: 2020 2023 2069 6620 2866 696e 616c 5f64     # if (final_d
+00031d30: 7479 7065 2021 3d20 4e6f 6e65 2061 6e64  type != None and
+00031d40: 2066 696e 616c 5f64 7479 7065 2021 3d20   final_dtype != 
+00031d50: 7265 7375 6c74 732e 6474 7970 6529 3a0d  results.dtype):.
+00031d60: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+00031d70: 2020 7072 696e 7428 222a 2a2a 2a2a 2a20    print("****** 
+00031d80: 6d69 7370 7265 6469 6374 6564 2066 696e  mispredicted fin
+00031d90: 616c 222c 2066 696e 616c 5f64 7479 7065  al", final_dtype
+00031da0: 2c20 7265 7375 6c74 732e 6474 7970 652c  , results.dtype,
+00031db0: 2075 6675 6e63 2c20 7363 616c 6172 7479   ufunc, scalarty
+00031dc0: 7065 732c 2061 7267 732c 206f 7574 7075  pes, args, outpu
+00031dd0: 7473 2c20 6b77 6172 6773 293b 0d0a 2020  ts, kwargs);..  
+00031de0: 2020 2020 2020 2020 2020 2320 7265 7375            # resu
+00031df0: 6c74 7320 3d20 2872 6573 756c 7473 2c29  lts = (results,)
+00031e00: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00031e10: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00031e20: 6528 7265 7375 6c74 732c 2046 6173 7441  e(results, FastA
+00031e30: 7272 6179 2920 616e 6420 6973 696e 7374  rray) and isinst
+00031e40: 616e 6365 2872 6573 756c 7473 2c20 6e70  ance(results, np
+00031e50: 2e6e 6461 7272 6179 293a 0d0a 2020 2020  .ndarray):..    
+00031e60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00031e70: 726e 2072 6573 756c 7473 2e76 6965 7728  rn results.view(
+00031e80: 4661 7374 4172 7261 7929 0d0a 0d0a 2020  FastArray)....  
+00031e90: 2020 2020 2020 2020 2020 2320 7468 696e            # thin
+00031ea0: 6b20 6869 7420 6865 7265 2066 6f72 2073  k hit here for s
+00031eb0: 756d 2077 6968 6368 2064 6f65 7320 6e6f  um wihch does no
+00031ec0: 7420 7265 7475 726e 2061 6e20 6172 7261  t return an arra
+00031ed0: 792c 206a 7573 7420 6120 6e75 6d62 6572  y, just a number
+00031ee0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00031ef0: 7475 726e 2072 6573 756c 7473 0d0a 0d0a  turn results....
+00031f00: 2020 2020 2020 2020 2320 6d6f 7265 2074          # more t
+00031f10: 6861 6e20 6f6e 6520 6974 656d 2c20 736f  han one item, so
+00031f20: 2077 6520 6172 6520 6d61 6b69 6e67 2061   we are making a
+00031f30: 2074 7570 6c65 0d0a 2020 2020 2020 2020   tuple..        
+00031f40: 2320 6361 6e20 7265 7375 6c74 2069 6e20  # can result in 
+00031f50: 5f5f 6172 7261 795f 6669 6e61 6c69 7a65  __array_finalize
+00031f60: 5f5f 2062 6569 6e67 2063 616c 6c65 640d  __ being called.
+00031f70: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
+00031f80: 203d 2074 7570 6c65 280d 0a20 2020 2020   = tuple(..     
+00031f90: 2020 2020 2020 2028 6e70 2e61 7361 7272         (np.asarr
+00031fa0: 6179 2872 6573 756c 7429 2e76 6965 7728  ay(result).view(
+00031fb0: 4661 7374 4172 7261 7929 2069 6620 6f75  FastArray) if ou
+00031fc0: 7470 7574 2069 7320 4e6f 6e65 2065 6c73  tput is None els
+00031fd0: 6520 6f75 7470 7574 290d 0a20 2020 2020  e output)..     
+00031fe0: 2020 2020 2020 2066 6f72 2072 6573 756c         for resul
+00031ff0: 742c 206f 7574 7075 7420 696e 207a 6970  t, output in zip
+00032000: 2872 6573 756c 7473 2c20 6f75 7470 7574  (results, output
+00032010: 7329 0d0a 2020 2020 2020 2020 290d 0a0d  s)..        )...
+00032020: 0a20 2020 2020 2020 2023 2063 6865 636b  .        # check
+00032030: 2069 6620 7765 2068 6176 6520 6120 7475   if we have a tu
+00032040: 706c 6520 6f66 206f 6e65 2069 7465 6d2c  ple of one item,
+00032050: 2069 6620 736f 206a 7573 7420 7265 7475   if so just retu
+00032060: 726e 2074 6865 206f 6e65 2069 7465 6d0d  rn the one item.
+00032070: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00032080: 7265 7375 6c74 7329 203d 3d20 313a 0d0a  results) == 1:..
+00032090: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000320a0: 6c74 7320 3d20 7265 7375 6c74 735b 305d  lts = results[0]
+000320b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000320c0: 2072 6573 756c 7473 0d0a 0d0a 2020 2020   results....    
+000320d0: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+000320e0: 6566 206e 756d 6261 7374 7269 6e67 2873  ef numbastring(s
+000320f0: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
+00032100: 2222 0d0a 2020 2020 2020 2020 636f 6e76  ""..        conv
+00032110: 6572 7473 2062 7974 6520 7374 7269 6e67  erts byte string
+00032120: 2061 6e64 2075 6e69 636f 6465 2073 7472   and unicode str
+00032130: 696e 6773 2074 6f20 6120 3264 696d 656e  ings to a 2dimen
+00032140: 7369 6f6e 616c 2061 7272 6179 0d0a 2020  sional array..  
+00032150: 2020 2020 2020 736f 2074 6861 7420 6e75        so that nu
+00032160: 6d62 6120 6361 6e20 7072 6f63 6573 7320  mba can process 
+00032170: 6974 2063 6f72 7265 6374 6c79 0d0a 0d0a  it correctly....
+00032180: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
+00032190: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+000321a0: 2d2d 0d0a 2020 2020 2020 2020 3e3e 3e20  --..        >>> 
+000321b0: 406e 756d 6261 2e6a 6974 286e 6f70 7974  @numba.jit(nopyt
+000321c0: 686f 6e3d 5472 7565 290d 0a20 2020 2020  hon=True)..     
+000321d0: 2020 202e 2e2e 2064 6566 206e 756d 6261     ... def numba
+000321e0: 5f73 7472 2874 7874 293a 0d0a 2020 2020  _str(txt):..    
+000321f0: 2020 2020 2e2e 2e20 2020 2020 783d 300d      ...     x=0.
+00032200: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
+00032210: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00032220: 7478 742e 7368 6170 655b 305d 293a 0d0a  txt.shape[0]):..
+00032230: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+00032240: 2020 2020 6966 2028 7478 745b 692c 305d      if (txt[i,0]
+00032250: 3d3d 3131 3620 616e 6420 2023 2027 7427  ==116 and  # 't'
+00032260: 0d0a 2020 2020 2020 2020 2e2e 2e20 2020  ..        ...   
+00032270: 2020 2020 2020 2020 2020 7478 745b 692c            txt[i,
+00032280: 315d 3d3d 3130 3120 616e 6420 2023 2027  1]==101 and  # '
+00032290: 6527 0d0a 2020 2020 2020 2020 2e2e 2e20  e'..        ... 
+000322a0: 2020 2020 2020 2020 2020 2020 7478 745b              txt[
+000322b0: 692c 325d 3d3d 3132 3020 616e 6420 2023  i,2]==120 and  #
+000322c0: 2027 7827 0d0a 2020 2020 2020 2020 2e2e   'x'..        ..
+000322d0: 2e20 2020 2020 2020 2020 2020 2020 7478  .             tx
+000322e0: 745b 692c 335d 3d3d 3131 3629 3a20 2020  t[i,3]==116):   
+000322f0: 2023 2027 7427 0d0a 2020 2020 2020 2020   # 't'..        
+00032300: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
+00032310: 7820 2b3d 2031 0d0a 2020 2020 2020 2020  x += 1..        
+00032320: 2e2e 2e20 2020 2020 7265 7475 726e 2078  ...     return x
+00032330: 0d0a 2020 2020 2020 2020 3e3e 3e0d 0a20  ..        >>>.. 
+00032340: 2020 2020 2020 203e 3e3e 2078 3d46 6173         >>> x=Fas
+00032350: 7441 7272 6179 285b 2773 6f6d 6527 2c27  tArray(['some','
+00032360: 7465 7874 272c 2774 6869 7327 2c27 6973  text','this','is
+00032370: 275d 290d 0a20 2020 2020 2020 203e 3e3e  '])..        >>>
+00032380: 206e 756d 6261 5f73 7472 2878 2e76 6965   numba_str(x.vie
+00032390: 7728 6e70 2e75 696e 7438 292e 7265 7368  w(np.uint8).resh
+000323a0: 6170 6528 286c 656e 2878 292c 2078 2e69  ape((len(x), x.i
+000323b0: 7465 6d73 697a 6529 2929 0d0a 2020 2020  temsize)))..    
+000323c0: 2020 2020 3e3e 3e20 6e75 6d62 615f 7374      >>> numba_st
+000323d0: 7228 782e 6e75 6d62 6173 7472 696e 6729  r(x.numbastring)
+000323e0: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
+000323f0: 0a20 2020 2020 2020 2069 6e74 7970 6520  .        intype 
+00032400: 3d20 7365 6c66 2e64 7479 7065 2e5f 5f73  = self.dtype.__s
+00032410: 7472 5f5f 2829 0d0a 2020 2020 2020 2020  tr__()..        
+00032420: 6966 2069 6e74 7970 655b 305d 203d 3d20  if intype[0] == 
+00032430: 227c 2220 6f72 2069 6e74 7970 655b 305d  "|" or intype[0]
+00032440: 203d 3d20 223c 223a 0d0a 2020 2020 2020   == "<":..      
+00032450: 2020 2020 2020 6966 2069 6e74 7970 655b        if intype[
+00032460: 315d 203d 3d20 2253 223a 0d0a 2020 2020  1] == "S":..    
+00032470: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00032480: 726e 2073 656c 662e 7669 6577 286e 702e  rn self.view(np.
+00032490: 7569 6e74 3829 2e72 6573 6861 7065 2828  uint8).reshape((
+000324a0: 6c65 6e28 7365 6c66 292c 2073 656c 662e  len(self), self.
+000324b0: 6974 656d 7369 7a65 2929 0d0a 2020 2020  itemsize))..    
+000324c0: 2020 2020 2020 2020 6966 2069 6e74 7970          if intyp
+000324d0: 655b 315d 203d 3d20 2255 223a 0d0a 2020  e[1] == "U":..  
+000324e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000324f0: 7475 726e 2073 656c 662e 7669 6577 286e  turn self.view(n
+00032500: 702e 7569 6e74 3332 292e 7265 7368 6170  p.uint32).reshap
+00032510: 6528 286c 656e 2873 656c 6629 2c20 7365  e((len(self), se
+00032520: 6c66 2e69 7465 6d73 697a 6520 2f2f 2034  lf.itemsize // 4
+00032530: 2929 0d0a 2020 2020 2020 2020 7265 7475  ))..        retu
+00032540: 726e 2073 656c 660d 0a0d 0a20 2020 2023  rn self....    #
+00032550: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
 00032560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00032570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00032580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020  -----------..   
-00032590: 2064 6566 2061 7070 6c79 5f6e 756d 6261   def apply_numba
-000325a0: 2873 656c 662c 202a 6172 6773 2c20 6f74  (self, *args, ot
-000325b0: 7970 653d 4e6f 6e65 2c20 6d79 6675 6e63  ype=None, myfunc
-000325c0: 3d22 6d79 6675 6e63 222c 206e 616d 653d  ="myfunc", name=
-000325d0: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
-000325e0: 2222 220d 0a20 2020 2020 2020 2050 7269  """..        Pri
-000325f0: 6e74 2074 6f20 7363 7265 656e 2061 6e20  nt to screen an 
-00032600: 6578 616d 706c 6520 6e75 6d62 6120 7369  example numba si
-00032610: 676e 6174 7572 6520 666f 7220 7468 6520  gnature for the 
-00032620: 6172 7261 792e 0d0a 0d0a 2020 2020 2020  array.....      
-00032630: 2020 596f 7520 6361 6e20 7468 656e 2063    You can then c
-00032640: 6f70 7920 7468 6973 2065 7861 6d70 6c65  opy this example
-00032650: 2074 6f20 6275 696c 6420 796f 7572 206f   to build your o
-00032660: 776e 206e 756d 6261 2066 756e 6374 696f  wn numba functio
-00032670: 6e2e 0d0a 0d0a 2020 2020 2020 2020 5061  n.....        Pa
-00032680: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
-00032690: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
-000326a0: 2020 2020 2020 2a61 7267 733a 0d0a 2020        *args:..  
-000326b0: 2020 2020 2020 2020 2020 5465 7374 2061            Test a
-000326c0: 7267 756d 656e 7473 0d0a 0d0a 2020 2020  rguments....    
-000326d0: 2020 2020 6f74 7970 653a 2073 7472 2c20      otype: str, 
-000326e0: 6465 6661 756c 7420 4e6f 6e65 0d0a 2020  default None..  
-000326f0: 2020 2020 2020 2020 2020 4120 6469 6666            A diff
-00032700: 6572 656e 7420 6f75 7470 7574 2064 6174  erent output dat
-00032710: 6120 7479 7065 0d0a 0d0a 2020 2020 2020  a type....      
-00032720: 2020 6d79 6675 6e63 3a20 7374 722c 2064    myfunc: str, d
-00032730: 6566 6175 6c74 2027 6d79 6675 6e63 270d  efault 'myfunc'.
-00032740: 0a20 2020 2020 2020 2020 2020 2041 2073  .            A s
-00032750: 7472 696e 6720 746f 2063 616c 6c20 7468  tring to call th
-00032760: 6520 6675 6e63 7469 6f6e 0d0a 0d0a 2020  e function....  
-00032770: 2020 2020 2020 6e61 6d65 3a20 7374 722c        name: str,
-00032780: 2064 6566 6175 6c74 204e 6f6e 650d 0a20   default None.. 
-00032790: 2020 2020 2020 2020 2020 2041 2073 7472             A str
-000327a0: 696e 6720 746f 206e 616d 6520 7468 6520  ing to name the 
-000327b0: 6172 7261 790d 0a0d 0a20 2020 2020 2020  array....       
-000327c0: 2045 7861 6d70 6c65 730d 0a20 2020 2020   Examples..     
-000327d0: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
-000327e0: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
-000327f0: 6e75 6d62 610d 0a20 2020 2020 2020 203e  numba..        >
-00032800: 3e3e 2040 6e75 6d62 612e 6775 7665 6374  >> @numba.guvect
-00032810: 6f72 697a 6528 5b27 766f 6964 2869 6e74  orize(['void(int
-00032820: 3634 5b3a 5d2c 2069 6e74 3634 5b3a 5d29  64[:], int64[:])
-00032830: 275d 2c20 2728 6e29 2d3e 286e 2927 290d  '], '(n)->(n)').
-00032840: 0a20 2020 2020 2020 202e 2e2e 2064 6566  .        ... def
-00032850: 2073 7175 6172 6576 2878 2c6f 7574 293a   squarev(x,out):
-00032860: 0d0a 2020 2020 2020 2020 2e2e 2e20 2020  ..        ...   
-00032870: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00032880: 286c 656e 2878 2929 3a0d 0a20 2020 2020  (len(x)):..     
-00032890: 2020 202e 2e2e 2020 2020 2020 2020 206f     ...         o
-000328a0: 7574 5b69 5d3d 785b 695d 2a2a 320d 0a20  ut[i]=x[i]**2.. 
-000328b0: 2020 2020 2020 202e 2e2e 0d0a 2020 2020         .....    
-000328c0: 2020 2020 3e3e 3e20 613d 6172 616e 6765      >>> a=arange
-000328d0: 2831 5f30 3030 5f30 3030 292e 6173 7479  (1_000_000).asty
-000328e0: 7065 286e 702e 696e 7436 3429 0d0a 2020  pe(np.int64)..  
-000328f0: 2020 2020 2020 3e3e 3e20 7371 7561 7265        >>> square
-00032900: 7628 6129 0d0a 2020 2020 2020 2020 4661  v(a)..        Fa
-00032910: 7374 4172 7261 7928 5b20 2020 2020 2020  stArray([       
-00032920: 2020 2020 302c 2020 2020 2020 2020 2020      0,          
-00032930: 2020 312c 2020 2020 2020 2020 2020 2020    1,            
-00032940: 342c 202e 2e2e 2c20 3939 3939 3934 3030  4, ..., 99999400
-00032950: 3030 3039 2c0d 0a20 2020 2020 2020 2020  0009,..         
-00032960: 2020 2020 2020 2020 2020 3939 3939 3936            999996
-00032970: 3030 3030 3034 2c20 3939 3939 3938 3030  000004, 99999800
-00032980: 3030 3031 5d2c 2064 7479 7065 3d69 6e74  0001], dtype=int
-00032990: 3634 290d 0a20 2020 2020 2020 2022 2222  64)..        """
-000329a0: 0d0a 2020 2020 2020 2020 6966 206e 616d  ..        if nam
-000329b0: 6520 6973 204e 6f6e 653a 0d0a 2020 2020  e is None:..    
-000329c0: 2020 2020 2020 2020 2320 7472 7920 6669          # try fi
-000329d0: 7273 7420 746f 2067 6574 2074 6865 206e  rst to get the n
-000329e0: 616d 650d 0a20 2020 2020 2020 2020 2020  ame..           
-000329f0: 206e 616d 6520 3d20 7365 6c66 2e67 6574   name = self.get
-00032a00: 5f6e 616d 6528 290d 0a0d 0a20 2020 2020  _name()....     
-00032a10: 2020 2020 2020 2069 6620 6e61 6d65 2069         if name i
-00032a20: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00032a30: 2020 2020 2020 2020 206e 616d 6520 3d20           name = 
-00032a40: 2261 220d 0a0d 0a20 2020 2020 2020 2069  "a"....        i
-00032a50: 6e74 7970 6520 3d20 7365 6c66 2e64 7479  ntype = self.dty
-00032a60: 7065 2e5f 5f73 7472 5f5f 2829 0d0a 0d0a  pe.__str__()....
-00032a70: 2020 2020 2020 2020 6966 206f 7479 7065          if otype
-00032a80: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00032a90: 2020 2020 2020 206f 7574 7479 7065 203d         outtype =
-00032aa0: 2073 656c 662e 6474 7970 652e 5f5f 7374   self.dtype.__st
-00032ab0: 725f 5f28 290d 0a20 2020 2020 2020 2065  r__()..        e
-00032ac0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00032ad0: 2020 6f75 7474 7970 6520 3d20 6e70 2e64    outtype = np.d
-00032ae0: 7479 7065 286f 7479 7065 292e 5f5f 7374  type(otype).__st
-00032af0: 725f 5f28 290d 0a0d 0a20 2020 2020 2020  r__()....       
-00032b00: 2023 2054 4f44 4f3a 2077 6861 7420 6966   # TODO: what if
-00032b10: 2075 6e69 636f 6465 206f 7220 7374 7269   unicode or stri
-00032b20: 6e67 3f20 202e 6672 6f6d 6275 6666 6572  ng?  .frombuffer
-00032b30: 2f2e 7669 6577 286e 702e 7569 6e74 3829  /.view(np.uint8)
-00032b40: 0d0a 0d0a 2020 2020 2020 2020 7072 6561  ....        prea
-00032b50: 6d62 6c65 203d 2022 696d 706f 7274 206e  mble = "import n
-00032b60: 756d 6261 5c6e 406e 756d 6261 2e67 7576  umba\n@numba.guv
-00032b70: 6563 746f 7269 7a65 285b 5c6e 220d 0a0d  ectorize([\n"...
-00032b80: 0a20 2020 2020 2020 206d 6964 646c 6520  .        middle 
-00032b90: 3d20 6622 2776 6f69 6428 7b69 6e74 7970  = f"'void({intyp
-00032ba0: 657d 5b3a 5d2c 207b 6f75 7474 7970 657d  e}[:], {outtype}
-00032bb0: 5b3a 5d29 272c 2020 2020 2020 2023 203c  [:])',       # <
-00032bc0: 2d2d 2063 616e 2073 7461 636b 206d 756c  -- can stack mul
-00032bd0: 7469 706c 6520 6469 6666 6572 656e 7420  tiple different 
-00032be0: 6474 7970 6573 2020 782e 7669 6577 286e  dtypes  x.view(n
-00032bf0: 702e 7569 6e74 3829 2e72 6573 6861 7065  p.uint8).reshape
-00032c00: 282d 312c 2078 2e69 7465 6d73 697a 6529  (-1, x.itemsize)
-00032c10: 5c6e 220d 0a0d 0a20 2020 2020 2020 2070  \n"....        p
-00032c20: 6f73 7461 6d62 6c65 203d 2022 2020 2020  ostamble = "    
-00032c30: 5d2c 2027 286e 292d 3e28 6e29 272c 2074  ], '(n)->(n)', t
-00032c40: 6172 6765 743d 2763 7075 2729 5c6e 220d  arget='cpu')\n".
-00032c50: 0a20 2020 2020 2020 2063 6f64 6520 3d20  .        code = 
-00032c60: 6622 6465 6620 7b6d 7966 756e 637d 2864  f"def {myfunc}(d
-00032c70: 6174 615f 696e 2c20 6461 7461 5f6f 7574  ata_in, data_out
-00032c80: 293a 5c6e 2020 2020 666f 7220 6920 696e  ):\n    for i in
-00032c90: 2072 616e 6765 286c 656e 2864 6174 615f   range(len(data_
-00032ca0: 696e 2929 3a5c 6e20 2020 2020 2020 2064  in)):\n        d
-00032cb0: 6174 615f 6f75 745b 695d 3d64 6174 615f  ata_out[i]=data_
-00032cc0: 696e 5b69 5d20 2020 233c 2d2d 2070 7574  in[i]   #<-- put
-00032cd0: 2079 6f75 7220 636f 6465 2068 6572 655c   your code here\
-00032ce0: 6e22 0d0a 2020 2020 2020 2020 6578 6563  n"..        exec
-00032cf0: 203d 2070 7265 616d 626c 6520 2b20 6d69   = preamble + mi
-00032d00: 6464 6c65 202b 2070 6f73 7461 6d62 6c65  ddle + postamble
-00032d10: 202b 2063 6f64 650d 0a0d 0a20 2020 2020   + code....     
-00032d20: 2020 2070 7269 6e74 2822 436f 7079 2074     print("Copy t
-00032d30: 6865 2063 6f64 6520 736e 6970 7065 7420  he code snippet 
-00032d40: 6265 6c6f 7720 616e 6420 7265 6e61 6d65  below and rename
-00032d50: 206d 7966 756e 6322 290d 0a20 2020 2020   myfunc")..     
-00032d60: 2020 2070 7269 6e74 2822 2d2d 2d2d 2d2d     print("------
+00032580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020  ------------..  
+00032590: 2020 6465 6620 6170 706c 795f 6e75 6d62    def apply_numb
+000325a0: 6128 7365 6c66 2c20 2a61 7267 732c 206f  a(self, *args, o
+000325b0: 7479 7065 3d4e 6f6e 652c 206d 7966 756e  type=None, myfun
+000325c0: 633d 226d 7966 756e 6322 2c20 6e61 6d65  c="myfunc", name
+000325d0: 3d4e 6f6e 6529 3a0d 0a20 2020 2020 2020  =None):..       
+000325e0: 2022 2222 0d0a 2020 2020 2020 2020 5072   """..        Pr
+000325f0: 696e 7420 746f 2073 6372 6565 6e20 616e  int to screen an
+00032600: 2065 7861 6d70 6c65 206e 756d 6261 2073   example numba s
+00032610: 6967 6e61 7475 7265 2066 6f72 2074 6865  ignature for the
+00032620: 2061 7272 6179 2e0d 0a0d 0a20 2020 2020   array.....     
+00032630: 2020 2059 6f75 2063 616e 2074 6865 6e20     You can then 
+00032640: 636f 7079 2074 6869 7320 6578 616d 706c  copy this exampl
+00032650: 6520 746f 2062 7569 6c64 2079 6f75 7220  e to build your 
+00032660: 6f77 6e20 6e75 6d62 6120 6675 6e63 7469  own numba functi
+00032670: 6f6e 2e0d 0a0d 0a20 2020 2020 2020 2050  on.....        P
+00032680: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
+00032690: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+000326a0: 2020 2020 2020 202a 6172 6773 3a0d 0a20         *args:.. 
+000326b0: 2020 2020 2020 2020 2020 2054 6573 7420             Test 
+000326c0: 6172 6775 6d65 6e74 730d 0a0d 0a20 2020  arguments....   
+000326d0: 2020 2020 206f 7479 7065 3a20 7374 722c       otype: str,
+000326e0: 2064 6566 6175 6c74 204e 6f6e 650d 0a20   default None.. 
+000326f0: 2020 2020 2020 2020 2020 2041 2064 6966             A dif
+00032700: 6665 7265 6e74 206f 7574 7075 7420 6461  ferent output da
+00032710: 7461 2074 7970 650d 0a0d 0a20 2020 2020  ta type....     
+00032720: 2020 206d 7966 756e 633a 2073 7472 2c20     myfunc: str, 
+00032730: 6465 6661 756c 7420 276d 7966 756e 6327  default 'myfunc'
+00032740: 0d0a 2020 2020 2020 2020 2020 2020 4120  ..            A 
+00032750: 7374 7269 6e67 2074 6f20 6361 6c6c 2074  string to call t
+00032760: 6865 2066 756e 6374 696f 6e0d 0a0d 0a20  he function.... 
+00032770: 2020 2020 2020 206e 616d 653a 2073 7472         name: str
+00032780: 2c20 6465 6661 756c 7420 4e6f 6e65 0d0a  , default None..
+00032790: 2020 2020 2020 2020 2020 2020 4120 7374              A st
+000327a0: 7269 6e67 2074 6f20 6e61 6d65 2074 6865  ring to name the
+000327b0: 2061 7272 6179 0d0a 0d0a 2020 2020 2020   array....      
+000327c0: 2020 4578 616d 706c 6573 0d0a 2020 2020    Examples..    
+000327d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020      --------..  
+000327e0: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
+000327f0: 206e 756d 6261 0d0a 2020 2020 2020 2020   numba..        
+00032800: 3e3e 3e20 406e 756d 6261 2e67 7576 6563  >>> @numba.guvec
+00032810: 746f 7269 7a65 285b 2776 6f69 6428 696e  torize(['void(in
+00032820: 7436 345b 3a5d 2c20 696e 7436 345b 3a5d  t64[:], int64[:]
+00032830: 2927 5d2c 2027 286e 292d 3e28 6e29 2729  )'], '(n)->(n)')
+00032840: 0d0a 2020 2020 2020 2020 2e2e 2e20 6465  ..        ... de
+00032850: 6620 7371 7561 7265 7628 782c 6f75 7429  f squarev(x,out)
+00032860: 3a0d 0a20 2020 2020 2020 202e 2e2e 2020  :..        ...  
+00032870: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00032880: 6528 6c65 6e28 7829 293a 0d0a 2020 2020  e(len(x)):..    
+00032890: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
+000328a0: 6f75 745b 695d 3d78 5b69 5d2a 2a32 0d0a  out[i]=x[i]**2..
+000328b0: 2020 2020 2020 2020 2e2e 2e0d 0a20 2020          .....   
+000328c0: 2020 2020 203e 3e3e 2061 3d61 7261 6e67       >>> a=arang
+000328d0: 6528 315f 3030 305f 3030 3029 2e61 7374  e(1_000_000).ast
+000328e0: 7970 6528 6e70 2e69 6e74 3634 290d 0a20  ype(np.int64).. 
+000328f0: 2020 2020 2020 203e 3e3e 2073 7175 6172         >>> squar
+00032900: 6576 2861 290d 0a20 2020 2020 2020 2046  ev(a)..        F
+00032910: 6173 7441 7272 6179 285b 2020 2020 2020  astArray([      
+00032920: 2020 2020 2030 2c20 2020 2020 2020 2020       0,         
+00032930: 2020 2031 2c20 2020 2020 2020 2020 2020     1,           
+00032940: 2034 2c20 2e2e 2e2c 2039 3939 3939 3430   4, ..., 9999940
+00032950: 3030 3030 392c 0d0a 2020 2020 2020 2020  00009,..        
+00032960: 2020 2020 2020 2020 2020 2039 3939 3939             99999
+00032970: 3630 3030 3030 342c 2039 3939 3939 3830  6000004, 9999980
+00032980: 3030 3030 315d 2c20 6474 7970 653d 696e  00001], dtype=in
+00032990: 7436 3429 0d0a 2020 2020 2020 2020 2222  t64)..        ""
+000329a0: 220d 0a20 2020 2020 2020 2069 6620 6e61  "..        if na
+000329b0: 6d65 2069 7320 4e6f 6e65 3a0d 0a20 2020  me is None:..   
+000329c0: 2020 2020 2020 2020 2023 2074 7279 2066           # try f
+000329d0: 6972 7374 2074 6f20 6765 7420 7468 6520  irst to get the 
+000329e0: 6e61 6d65 0d0a 2020 2020 2020 2020 2020  name..          
+000329f0: 2020 6e61 6d65 203d 2073 656c 662e 6765    name = self.ge
+00032a00: 745f 6e61 6d65 2829 0d0a 0d0a 2020 2020  t_name()....    
+00032a10: 2020 2020 2020 2020 6966 206e 616d 6520          if name 
+00032a20: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+00032a30: 2020 2020 2020 2020 2020 6e61 6d65 203d            name =
+00032a40: 2022 6122 0d0a 0d0a 2020 2020 2020 2020   "a"....        
+00032a50: 696e 7479 7065 203d 2073 656c 662e 6474  intype = self.dt
+00032a60: 7970 652e 5f5f 7374 725f 5f28 290d 0a0d  ype.__str__()...
+00032a70: 0a20 2020 2020 2020 2069 6620 6f74 7970  .        if otyp
+00032a80: 6520 6973 204e 6f6e 653a 0d0a 2020 2020  e is None:..    
+00032a90: 2020 2020 2020 2020 6f75 7474 7970 6520          outtype 
+00032aa0: 3d20 7365 6c66 2e64 7479 7065 2e5f 5f73  = self.dtype.__s
+00032ab0: 7472 5f5f 2829 0d0a 2020 2020 2020 2020  tr__()..        
+00032ac0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00032ad0: 2020 206f 7574 7479 7065 203d 206e 702e     outtype = np.
+00032ae0: 6474 7970 6528 6f74 7970 6529 2e5f 5f73  dtype(otype).__s
+00032af0: 7472 5f5f 2829 0d0a 0d0a 2020 2020 2020  tr__()....      
+00032b00: 2020 2320 544f 444f 3a20 7768 6174 2069    # TODO: what i
+00032b10: 6620 756e 6963 6f64 6520 6f72 2073 7472  f unicode or str
+00032b20: 696e 673f 2020 2e66 726f 6d62 7566 6665  ing?  .frombuffe
+00032b30: 722f 2e76 6965 7728 6e70 2e75 696e 7438  r/.view(np.uint8
+00032b40: 290d 0a0d 0a20 2020 2020 2020 2070 7265  )....        pre
+00032b50: 616d 626c 6520 3d20 2269 6d70 6f72 7420  amble = "import 
+00032b60: 6e75 6d62 615c 6e40 6e75 6d62 612e 6775  numba\n@numba.gu
+00032b70: 7665 6374 6f72 697a 6528 5b5c 6e22 0d0a  vectorize([\n"..
+00032b80: 0d0a 2020 2020 2020 2020 6d69 6464 6c65  ..        middle
+00032b90: 203d 2066 2227 766f 6964 287b 696e 7479   = f"'void({inty
+00032ba0: 7065 7d5b 3a5d 2c20 7b6f 7574 7479 7065  pe}[:], {outtype
+00032bb0: 7d5b 3a5d 2927 2c20 2020 2020 2020 2320  }[:])',       # 
+00032bc0: 3c2d 2d20 6361 6e20 7374 6163 6b20 6d75  <-- can stack mu
+00032bd0: 6c74 6970 6c65 2064 6966 6665 7265 6e74  ltiple different
+00032be0: 2064 7479 7065 7320 2078 2e76 6965 7728   dtypes  x.view(
+00032bf0: 6e70 2e75 696e 7438 292e 7265 7368 6170  np.uint8).reshap
+00032c00: 6528 2d31 2c20 782e 6974 656d 7369 7a65  e(-1, x.itemsize
+00032c10: 295c 6e22 0d0a 0d0a 2020 2020 2020 2020  )\n"....        
+00032c20: 706f 7374 616d 626c 6520 3d20 2220 2020  postamble = "   
+00032c30: 205d 2c20 2728 6e29 2d3e 286e 2927 2c20   ], '(n)->(n)', 
+00032c40: 7461 7267 6574 3d27 6370 7527 295c 6e22  target='cpu')\n"
+00032c50: 0d0a 2020 2020 2020 2020 636f 6465 203d  ..        code =
+00032c60: 2066 2264 6566 207b 6d79 6675 6e63 7d28   f"def {myfunc}(
+00032c70: 6461 7461 5f69 6e2c 2064 6174 615f 6f75  data_in, data_ou
+00032c80: 7429 3a5c 6e20 2020 2066 6f72 2069 2069  t):\n    for i i
+00032c90: 6e20 7261 6e67 6528 6c65 6e28 6461 7461  n range(len(data
+00032ca0: 5f69 6e29 293a 5c6e 2020 2020 2020 2020  _in)):\n        
+00032cb0: 6461 7461 5f6f 7574 5b69 5d3d 6461 7461  data_out[i]=data
+00032cc0: 5f69 6e5b 695d 2020 2023 3c2d 2d20 7075  _in[i]   #<-- pu
+00032cd0: 7420 796f 7572 2063 6f64 6520 6865 7265  t your code here
+00032ce0: 5c6e 220d 0a20 2020 2020 2020 2065 7865  \n"..        exe
+00032cf0: 6320 3d20 7072 6561 6d62 6c65 202b 206d  c = preamble + m
+00032d00: 6964 646c 6520 2b20 706f 7374 616d 626c  iddle + postambl
+00032d10: 6520 2b20 636f 6465 0d0a 0d0a 2020 2020  e + code....    
+00032d20: 2020 2020 7072 696e 7428 2243 6f70 7920      print("Copy 
+00032d30: 7468 6520 636f 6465 2073 6e69 7070 6574  the code snippet
+00032d40: 2062 656c 6f77 2061 6e64 2072 656e 616d   below and renam
+00032d50: 6520 6d79 6675 6e63 2229 0d0a 2020 2020  e myfunc")..    
+00032d60: 2020 2020 7072 696e 7428 222d 2d2d 2d2d      print("-----
 00032d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00032d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00032d90: 2d2d 2d2d 2d2d 2d22 290d 0a20 2020 2020  -------")..     
-00032da0: 2020 2070 7269 6e74 2865 7865 6329 0d0a     print(exec)..
-00032db0: 2020 2020 2020 2020 7072 696e 7428 222d          print("-
+00032d90: 2d2d 2d2d 2d2d 2d2d 2229 0d0a 2020 2020  --------")..    
+00032da0: 2020 2020 7072 696e 7428 6578 6563 290d      print(exec).
+00032db0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
 00032dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00032dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00032de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2229 0d0a  ------------")..
-00032df0: 2020 2020 2020 2020 6966 2069 6e74 7970          if intyp
-00032e00: 655b 305d 203d 3d20 227c 2220 6f72 2069  e[0] == "|" or i
-00032e10: 6e74 7970 655b 305d 203d 3d20 223c 223a  ntype[0] == "<":
-00032e20: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00032e30: 2069 6e74 7970 655b 315d 203d 3d20 2253   intype[1] == "S
-00032e40: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-00032e50: 2020 2020 7072 696e 7428 0d0a 2020 2020      print(..    
+00032de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d22 290d  -------------").
+00032df0: 0a20 2020 2020 2020 2069 6620 696e 7479  .        if inty
+00032e00: 7065 5b30 5d20 3d3d 2022 7c22 206f 7220  pe[0] == "|" or 
+00032e10: 696e 7479 7065 5b30 5d20 3d3d 2022 3c22  intype[0] == "<"
+00032e20: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00032e30: 6620 696e 7479 7065 5b31 5d20 3d3d 2022  f intype[1] == "
+00032e40: 5322 3a0d 0a20 2020 2020 2020 2020 2020  S":..           
+00032e50: 2020 2020 2070 7269 6e74 280d 0a20 2020       print(..   
 00032e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032e70: 6622 5468 656e 2063 616c 6c20 7b6d 7966  f"Then call {myf
-00032e80: 756e 637d 287b 6e61 6d65 7d2e 6e75 6d62  unc}({name}.numb
-00032e90: 6173 7472 696e 672c 656d 7074 795f 6c69  astring,empty_li
-00032ea0: 6b65 287b 6e61 6d65 7d29 2e6e 756d 6261  ke({name}).numba
-00032eb0: 7374 7269 6e67 2920 7768 6572 6520 7b6e  string) where {n
-00032ec0: 616d 657d 2069 7320 7468 6520 696e 7075  ame} is the inpu
-00032ed0: 7420 6172 7261 7922 0d0a 2020 2020 2020  t array"..      
-00032ee0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00032ef0: 2020 2020 2020 2020 2065 6c69 6620 696e           elif in
-00032f00: 7479 7065 5b31 5d20 3d3d 2022 5522 3a0d  type[1] == "U":.
-00032f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00032f20: 2070 7269 6e74 280d 0a20 2020 2020 2020   print(..       
-00032f30: 2020 2020 2020 2020 2020 2020 2066 2254               f"T
-00032f40: 6865 6e20 6361 6c6c 207b 6d79 6675 6e63  hen call {myfunc
-00032f50: 7d28 7b6e 616d 657d 2e6e 756d 6261 7374  }({name}.numbast
-00032f60: 7269 6e67 2c65 6d70 7479 5f6c 696b 6528  ring,empty_like(
-00032f70: 7b6e 616d 657d 292e 6e75 6d62 6173 7472  {name}).numbastr
-00032f80: 696e 6729 2077 6865 7265 207b 6e61 6d65  ing) where {name
-00032f90: 7d20 6973 2074 6865 2069 6e70 7574 2061  } is the input a
-00032fa0: 7272 6179 220d 0a20 2020 2020 2020 2020  rray"..         
-00032fb0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00032fc0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00032fd0: 2020 2020 2070 7269 6e74 2866 2254 6865       print(f"The
-00032fe0: 6e20 6361 6c6c 207b 6d79 6675 6e63 7d28  n call {myfunc}(
-00032ff0: 7b6e 616d 657d 2c65 6d70 7479 5f6c 696b  {name},empty_lik
-00033000: 6528 7b6e 616d 657d 2929 2077 6865 7265  e({name})) where
-00033010: 207b 6e61 6d65 7d20 6973 2074 6865 2069   {name} is the i
-00033020: 6e70 7574 2061 7272 6179 2229 0d0a 2020  nput array")..  
-00033030: 2020 2020 2020 2320 7265 7475 726e 2065        # return e
-00033040: 7865 630d 0a0d 0a20 2020 2064 6566 2061  xec....    def a
-00033050: 7070 6c79 2873 656c 662c 2070 7966 756e  pply(self, pyfun
-00033060: 632c 202a 6172 6773 2c20 6f74 7970 6573  c, *args, otypes
-00033070: 3d4e 6f6e 652c 2064 6f63 3d4e 6f6e 652c  =None, doc=None,
-00033080: 2065 7863 6c75 6465 643d 4e6f 6e65 2c20   excluded=None, 
-00033090: 6361 6368 653d 4661 6c73 652c 2073 6967  cache=False, sig
-000330a0: 6e61 7475 7265 3d4e 6f6e 6529 3a0d 0a20  nature=None):.. 
-000330b0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-000330c0: 2020 2020 4765 6e65 7261 6c69 7a65 6420      Generalized 
-000330d0: 6675 6e63 7469 6f6e 2063 6c61 7373 2e20  function class. 
-000330e0: 2073 6565 3a20 6e70 2e76 6563 746f 7269   see: np.vectori
-000330f0: 7a65 0d0a 0d0a 2020 2020 2020 2020 4372  ze....        Cr
-00033100: 6561 7465 7320 616e 6420 7468 656e 2061  eates and then a
-00033110: 7070 6c69 6573 2061 2076 6563 746f 7269  pplies a vectori
-00033120: 7a65 6420 6675 6e63 7469 6f6e 2077 6869  zed function whi
-00033130: 6368 2074 616b 6573 2061 206e 6573 7465  ch takes a neste
-00033140: 6420 7365 7175 656e 6365 206f 6620 6f62  d sequence of ob
-00033150: 6a65 6374 7320 6f72 0d0a 2020 2020 2020  jects or..      
-00033160: 2020 6e75 6d70 7920 6172 7261 7973 2061    numpy arrays a
-00033170: 7320 696e 7075 7473 2061 6e64 2072 6574  s inputs and ret
-00033180: 7572 6e73 2061 6e20 7369 6e67 6c65 206f  urns an single o
-00033190: 7220 7475 706c 6520 6f66 206e 756d 7079  r tuple of numpy
-000331a0: 2061 7272 6179 2061 730d 0a20 2020 2020   array as..     
-000331b0: 2020 206f 7574 7075 742e 2054 6865 2076     output. The v
-000331c0: 6563 746f 7269 7a65 6420 6675 6e63 7469  ectorized functi
-000331d0: 6f6e 2065 7661 6c75 6174 6573 2060 7079  on evaluates `py
-000331e0: 6675 6e63 6020 6f76 6572 2073 7563 6365  func` over succe
-000331f0: 7373 6976 6520 7475 706c 6573 0d0a 2020  ssive tuples..  
-00033200: 2020 2020 2020 6f66 2074 6865 2069 6e70        of the inp
-00033210: 7574 2061 7272 6179 7320 6c69 6b65 2074  ut arrays like t
-00033220: 6865 2070 7974 686f 6e20 6d61 7020 6675  he python map fu
-00033230: 6e63 7469 6f6e 2c20 6578 6365 7074 2069  nction, except i
-00033240: 7420 7573 6573 2074 6865 0d0a 2020 2020  t uses the..    
-00033250: 2020 2020 6272 6f61 6463 6173 7469 6e67      broadcasting
-00033260: 2072 756c 6573 206f 6620 6e75 6d70 792e   rules of numpy.
-00033270: 0d0a 0d0a 2020 2020 2020 2020 5468 6520  ....        The 
-00033280: 6461 7461 2074 7970 6520 6f66 2074 6865  data type of the
-00033290: 206f 7574 7075 7420 6f66 2060 7665 6374   output of `vect
-000332a0: 6f72 697a 6564 6020 6973 2064 6574 6572  orized` is deter
-000332b0: 6d69 6e65 6420 6279 2063 616c 6c69 6e67  mined by calling
-000332c0: 0d0a 2020 2020 2020 2020 7468 6520 6675  ..        the fu
-000332d0: 6e63 7469 6f6e 2077 6974 6820 7468 6520  nction with the 
-000332e0: 6669 7273 7420 656c 656d 656e 7420 6f66  first element of
-000332f0: 2074 6865 2069 6e70 7574 2e20 2054 6869   the input.  Thi
-00033300: 7320 6361 6e20 6265 2061 766f 6964 6564  s can be avoided
-00033310: 0d0a 2020 2020 2020 2020 6279 2073 7065  ..        by spe
-00033320: 6369 6679 696e 6720 7468 6520 606f 7479  cifying the `oty
-00033330: 7065 7360 2061 7267 756d 656e 742e 0d0a  pes` argument...
-00033340: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00033350: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
-00033360: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00033370: 2020 7079 6675 6e63 203a 2063 616c 6c61    pyfunc : calla
-00033380: 626c 650d 0a20 2020 2020 2020 2020 2020  ble..           
-00033390: 2041 2070 7974 686f 6e20 6675 6e63 7469   A python functi
-000333a0: 6f6e 206f 7220 6d65 7468 6f64 2e0d 0a20  on or method... 
-000333b0: 2020 2020 2020 206f 7479 7065 7320 3a20         otypes : 
-000333c0: 7374 7220 6f72 206c 6973 7420 6f66 2064  str or list of d
-000333d0: 7479 7065 732c 206f 7074 696f 6e61 6c0d  types, optional.
-000333e0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-000333f0: 206f 7574 7075 7420 6461 7461 2074 7970   output data typ
-00033400: 652e 2049 7420 6d75 7374 2062 6520 7370  e. It must be sp
-00033410: 6563 6966 6965 6420 6173 2065 6974 6865  ecified as eithe
-00033420: 7220 6120 7374 7269 6e67 206f 660d 0a20  r a string of.. 
-00033430: 2020 2020 2020 2020 2020 2074 7970 6563             typec
-00033440: 6f64 6520 6368 6172 6163 7465 7273 206f  ode characters o
-00033450: 7220 6120 6c69 7374 206f 6620 6461 7461  r a list of data
-00033460: 2074 7970 6520 7370 6563 6966 6965 7273   type specifiers
-00033470: 2e20 5468 6572 6520 7368 6f75 6c64 0d0a  . There should..
-00033480: 2020 2020 2020 2020 2020 2020 6265 206f              be o
-00033490: 6e65 2064 6174 6120 7479 7065 2073 7065  ne data type spe
-000334a0: 6369 6669 6572 2066 6f72 2065 6163 6820  cifier for each 
-000334b0: 6f75 7470 7574 2e0d 0a20 2020 2020 2020  output...       
-000334c0: 2064 6f63 203a 2073 7472 2c20 6f70 7469   doc : str, opti
-000334d0: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
-000334e0: 2020 5468 6520 646f 6373 7472 696e 6720    The docstring 
-000334f0: 666f 7220 7468 6520 6675 6e63 7469 6f6e  for the function
-00033500: 2e20 4966 2060 4e6f 6e65 602c 2074 6865  . If `None`, the
-00033510: 2064 6f63 7374 7269 6e67 2077 696c 6c20   docstring will 
-00033520: 6265 2074 6865 0d0a 2020 2020 2020 2020  be the..        
-00033530: 2020 2020 6060 7079 6675 6e63 2e5f 5f64      ``pyfunc.__d
-00033540: 6f63 5f5f 6060 2e0d 0a20 2020 2020 2020  oc__``...       
-00033550: 2065 7863 6c75 6465 6420 3a20 7365 742c   excluded : set,
-00033560: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-00033570: 2020 2020 2020 2053 6574 206f 6620 7374         Set of st
-00033580: 7269 6e67 7320 6f72 2069 6e74 6567 6572  rings or integer
-00033590: 7320 7265 7072 6573 656e 7469 6e67 2074  s representing t
-000335a0: 6865 2070 6f73 6974 696f 6e61 6c20 6f72  he positional or
-000335b0: 206b 6579 776f 7264 0d0a 2020 2020 2020   keyword..      
-000335c0: 2020 2020 2020 6172 6775 6d65 6e74 7320        arguments 
-000335d0: 666f 7220 7768 6963 6820 7468 6520 6675  for which the fu
-000335e0: 6e63 7469 6f6e 2077 696c 6c20 6e6f 7420  nction will not 
-000335f0: 6265 2076 6563 746f 7269 7a65 642e 2020  be vectorized.  
-00033600: 5468 6573 6520 7769 6c6c 2062 650d 0a20  These will be.. 
-00033610: 2020 2020 2020 2020 2020 2070 6173 7365             passe
-00033620: 6420 6469 7265 6374 6c79 2074 6f20 6070  d directly to `p
-00033630: 7966 756e 6360 2075 6e6d 6f64 6966 6965  yfunc` unmodifie
-00033640: 642e 0d0a 0d0a 2020 2020 2020 2020 2020  d.....          
-00033650: 2020 2e2e 2076 6572 7369 6f6e 6164 6465    .. versionadde
-00033660: 643a 3a20 312e 372e 300d 0a0d 0a20 2020  d:: 1.7.0....   
-00033670: 2020 2020 2063 6163 6865 203a 2062 6f6f       cache : boo
-00033680: 6c2c 206f 7074 696f 6e61 6c0d 0a20 2020  l, optional..   
-00033690: 2020 2020 2020 2020 4966 2060 5472 7565          If `True
-000336a0: 602c 2074 6865 6e20 6361 6368 6520 7468  `, then cache th
-000336b0: 6520 6669 7273 7420 6675 6e63 7469 6f6e  e first function
-000336c0: 2063 616c 6c20 7468 6174 2064 6574 6572   call that deter
-000336d0: 6d69 6e65 7320 7468 6520 6e75 6d62 6572  mines the number
-000336e0: 0d0a 2020 2020 2020 2020 2020 206f 6620  ..           of 
-000336f0: 6f75 7470 7574 7320 6966 2060 6f74 7970  outputs if `otyp
-00033700: 6573 6020 6973 206e 6f74 2070 726f 7669  es` is not provi
-00033710: 6465 642e 0d0a 0d0a 2020 2020 2020 2020  ded.....        
-00033720: 2020 2020 2e2e 2076 6572 7369 6f6e 6164      .. versionad
-00033730: 6465 643a 3a20 312e 372e 300d 0a0d 0a20  ded:: 1.7.0.... 
-00033740: 2020 2020 2020 2073 6967 6e61 7475 7265         signature
-00033750: 203a 2073 7472 696e 672c 206f 7074 696f   : string, optio
-00033760: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
-00033770: 2047 656e 6572 616c 697a 6564 2075 6e69   Generalized uni
-00033780: 7665 7273 616c 2066 756e 6374 696f 6e20  versal function 
-00033790: 7369 676e 6174 7572 652c 2065 2e67 2e2c  signature, e.g.,
-000337a0: 2060 6028 6d2c 6e29 2c28 6e29 2d3e 286d   ``(m,n),(n)->(m
-000337b0: 2960 6020 666f 720d 0a20 2020 2020 2020  )`` for..       
-000337c0: 2020 2020 2076 6563 746f 7269 7a65 6420       vectorized 
-000337d0: 6d61 7472 6978 2d76 6563 746f 7220 6d75  matrix-vector mu
-000337e0: 6c74 6970 6c69 6361 7469 6f6e 2e20 4966  ltiplication. If
-000337f0: 2070 726f 7669 6465 642c 2060 6070 7966   provided, ``pyf
-00033800: 756e 6360 6020 7769 6c6c 0d0a 2020 2020  unc`` will..    
-00033810: 2020 2020 2020 2020 6265 2063 616c 6c65          be calle
-00033820: 6420 7769 7468 2028 616e 6420 6578 7065  d with (and expe
-00033830: 6374 6564 2074 6f20 7265 7475 726e 2920  cted to return) 
-00033840: 6172 7261 7973 2077 6974 6820 7368 6170  arrays with shap
-00033850: 6573 2067 6976 656e 2062 7920 7468 650d  es given by the.
-00033860: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-00033870: 6520 6f66 2063 6f72 7265 7370 6f6e 6469  e of correspondi
-00033880: 6e67 2063 6f72 6520 6469 6d65 6e73 696f  ng core dimensio
-00033890: 6e73 2e20 4279 2064 6566 6175 6c74 2c20  ns. By default, 
-000338a0: 6060 7079 6675 6e63 6060 2069 730d 0a20  ``pyfunc`` is.. 
-000338b0: 2020 2020 2020 2020 2020 2061 7373 756d             assum
-000338c0: 6564 2074 6f20 7461 6b65 2073 6361 6c61  ed to take scala
-000338d0: 7273 2061 7320 696e 7075 7420 616e 6420  rs as input and 
-000338e0: 6f75 7470 7574 2e0d 0a0d 0a20 2020 2020  output.....     
-000338f0: 2020 2020 2020 202e 2e20 7665 7273 696f         .. versio
-00033900: 6e61 6464 6564 3a3a 2031 2e31 322e 300d  nadded:: 1.12.0.
-00033910: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00033920: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
-00033930: 2d2d 2d0d 0a20 2020 2020 2020 2076 6563  ---..        vec
-00033940: 746f 7269 7a65 6420 3a20 6361 6c6c 6162  torized : callab
-00033950: 6c65 0d0a 2020 2020 2020 2020 2020 2020  le..            
-00033960: 5665 6374 6f72 697a 6564 2066 756e 6374  Vectorized funct
-00033970: 696f 6e2e 0d0a 0d0a 2020 2020 2020 2020  ion.....        
-00033980: 5365 6520 416c 736f 0d0a 2020 2020 2020  See Also..      
-00033990: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
-000339a0: 2020 2020 4661 7374 4172 7261 792e 6170      FastArray.ap
-000339b0: 706c 795f 6e75 6d62 610d 0a20 2020 2020  ply_numba..     
-000339c0: 2020 2046 6173 7441 7272 6179 2e61 7070     FastArray.app
-000339d0: 6c79 5f70 616e 6461 730d 0a0d 0a20 2020  ly_pandas....   
-000339e0: 2020 2020 2045 7861 6d70 6c65 730d 0a20       Examples.. 
-000339f0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0d         --------.
-00033a00: 0a20 2020 2020 2020 203e 3e3e 2064 6566  .        >>> def
-00033a10: 206d 7966 756e 6328 612c 2062 293a 0d0a   myfunc(a, b):..
-00033a20: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-00033a30: 2252 6574 7572 6e20 612d 6220 6966 2061  "Return a-b if a
-00033a40: 3e62 2c20 6f74 6865 7277 6973 6520 7265  >b, otherwise re
-00033a50: 7475 726e 2061 2b62 220d 0a20 2020 2020  turn a+b"..     
-00033a60: 2020 202e 2e2e 2020 2020 2069 6620 6120     ...     if a 
-00033a70: 3e20 623a 0d0a 2020 2020 2020 2020 2e2e  > b:..        ..
-00033a80: 2e20 2020 2020 2020 2020 7265 7475 726e  .         return
-00033a90: 2061 202d 2062 0d0a 2020 2020 2020 2020   a - b..        
-00033aa0: 2e2e 2e20 2020 2020 656c 7365 3a0d 0a20  ...     else:.. 
-00033ab0: 2020 2020 2020 202e 2e2e 2020 2020 2020         ...      
-00033ac0: 2020 2072 6574 7572 6e20 6120 2b20 620d     return a + b.
-00033ad0: 0a20 2020 2020 2020 203e 3e3e 0d0a 2020  .        >>>..  
-00033ae0: 2020 2020 2020 3e3e 3e20 613d 6172 616e        >>> a=aran
-00033af0: 6765 2831 3029 0d0a 2020 2020 2020 2020  ge(10)..        
-00033b00: 3e3e 3e20 623d 6172 616e 6765 2831 3029  >>> b=arange(10)
-00033b10: 2b31 0d0a 2020 2020 2020 2020 3e3e 3e20  +1..        >>> 
-00033b20: 612e 6170 706c 7928 6d79 6675 6e63 2c62  a.apply(myfunc,b
-00033b30: 290d 0a20 2020 2020 2020 2046 6173 7441  )..        FastA
-00033b40: 7272 6179 285b 2031 2c20 2033 2c20 2035  rray([ 1,  3,  5
-00033b50: 2c20 2037 2c20 2039 2c20 3131 2c20 3133  ,  7,  9, 11, 13
-00033b60: 2c20 3135 2c20 3137 2c20 3139 5d29 0d0a  , 15, 17, 19])..
-00033b70: 0d0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-00033b80: 6520 7769 7468 206f 6e65 2069 6e70 7574  e with one input
-00033b90: 2061 7272 6179 0d0a 0d0a 2020 2020 2020   array....      
-00033ba0: 2020 3e3e 3e20 6465 6620 7371 7561 7265    >>> def square
-00033bb0: 2878 293a 0d0a 2020 2020 2020 2020 2e2e  (x):..        ..
-00033bc0: 2e20 2020 2020 7265 7475 726e 2078 2a2a  .     return x**
-00033bd0: 320d 0a20 2020 2020 2020 203e 3e3e 0d0a  2..        >>>..
-00033be0: 2020 2020 2020 2020 3e3e 3e20 613d 6172          >>> a=ar
-00033bf0: 616e 6765 2831 3029 0d0a 2020 2020 2020  ange(10)..      
-00033c00: 2020 3e3e 3e20 612e 6170 706c 7928 7371    >>> a.apply(sq
-00033c10: 7561 7265 290d 0a20 2020 2020 2020 2046  uare)..        F
-00033c20: 6173 7441 7272 6179 285b 2030 2c20 2031  astArray([ 0,  1
-00033c30: 2c20 2034 2c20 2039 2c20 3136 2c20 3235  ,  4,  9, 16, 25
-00033c40: 2c20 3336 2c20 3439 2c20 3634 2c20 3831  , 36, 49, 64, 81
-00033c50: 5d29 0d0a 0d0a 2020 2020 2020 2020 4578  ])....        Ex
-00033c60: 616d 706c 6520 7769 7468 206c 616d 6264  ample with lambd
-00033c70: 610d 0a0d 0a20 2020 2020 2020 203e 3e3e  a....        >>>
-00033c80: 2061 3d61 7261 6e67 6528 3130 290d 0a20   a=arange(10).. 
-00033c90: 2020 2020 2020 203e 3e3e 2061 2e61 7070         >>> a.app
-00033ca0: 6c79 286c 616d 6264 6120 783a 2078 2a2a  ly(lambda x: x**
-00033cb0: 3229 0d0a 2020 2020 2020 2020 4661 7374  2)..        Fast
-00033cc0: 4172 7261 7928 5b20 302c 2020 312c 2020  Array([ 0,  1,  
-00033cd0: 342c 2020 392c 2031 362c 2032 352c 2033  4,  9, 16, 25, 3
-00033ce0: 362c 2034 392c 2036 342c 2038 315d 290d  6, 49, 64, 81]).
-00033cf0: 0a0d 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
-00033d00: 6c65 2077 6974 6820 6e75 6d62 610d 0a0d  le with numba...
-00033d10: 0a20 2020 2020 2020 203e 3e3e 2066 726f  .        >>> fro
-00033d20: 6d20 6e75 6d62 6120 696d 706f 7274 206a  m numba import j
-00033d30: 6974 0d0a 2020 2020 2020 2020 3e3e 3e20  it..        >>> 
-00033d40: 406a 6974 0d0a 2020 2020 2020 2020 2e2e  @jit..        ..
-00033d50: 2e20 6465 6620 7371 7561 7265 6974 2878  . def squareit(x
-00033d60: 293a 0d0a 2020 2020 2020 2020 2e2e 2e20  ):..        ... 
-00033d70: 2020 2020 7265 7475 726e 2078 2a2a 320d      return x**2.
-00033d80: 0a20 2020 2020 2020 203e 3e3e 2061 2e61  .        >>> a.a
-00033d90: 7070 6c79 2873 7175 6172 6569 7429 0d0a  pply(squareit)..
-00033da0: 2020 2020 2020 2020 4661 7374 4172 7261          FastArra
-00033db0: 7928 5b20 302c 2020 312c 2020 342c 2020  y([ 0,  1,  4,  
-00033dc0: 392c 2031 362c 2032 352c 2033 362c 2034  9, 16, 25, 36, 4
-00033dd0: 392c 2036 342c 2038 315d 290d 0a0d 0a20  9, 64, 81]).... 
-00033de0: 2020 2020 2020 2045 7861 6d70 6c65 7320         Examples 
-00033df0: 746f 2075 7365 2065 7869 7374 696e 6720  to use existing 
-00033e00: 6275 696c 7469 6e20 6f63 7420 6675 6e63  builtin oct func
-00033e10: 7469 6f6e 2062 7574 2063 6861 6e67 6520  tion but change 
-00033e20: 7468 6520 6f75 7470 7574 2066 726f 6d20  the output from 
-00033e30: 7374 7269 6e67 2c20 746f 2075 6e69 636f  string, to unico
-00033e40: 6465 2c20 746f 206f 626a 6563 740d 0a0d  de, to object...
-00033e50: 0a20 2020 2020 2020 203e 3e3e 2061 3d61  .        >>> a=a
-00033e60: 7261 6e67 6528 3130 290d 0a20 2020 2020  range(10)..     
-00033e70: 2020 203e 3e3e 2061 2e61 7070 6c79 286f     >>> a.apply(o
-00033e80: 6374 2c20 6f74 7970 6573 3d5b 2753 275d  ct, otypes=['S']
-00033e90: 290d 0a20 2020 2020 2020 2046 6173 7441  )..        FastA
-00033ea0: 7272 6179 285b 6227 306f 3027 2c20 6227  rray([b'0o0', b'
-00033eb0: 306f 3127 2c20 6227 306f 3227 2c20 6227  0o1', b'0o2', b'
-00033ec0: 306f 3327 2c20 6227 306f 3427 2c20 6227  0o3', b'0o4', b'
-00033ed0: 306f 3527 2c20 6227 306f 3627 2c20 6227  0o5', b'0o6', b'
-00033ee0: 306f 3727 2c20 6227 306f 3130 272c 2062  0o7', b'0o10', b
-00033ef0: 2730 6f31 3127 5d2c 2064 7479 7065 3d27  '0o11'], dtype='
-00033f00: 7c53 3427 290d 0a0d 0a20 2020 2020 2020  |S4')....       
-00033f10: 203e 3e3e 2061 3d61 7261 6e67 6528 3130   >>> a=arange(10
-00033f20: 290d 0a20 2020 2020 2020 203e 3e3e 2061  )..        >>> a
-00033f30: 2e61 7070 6c79 286f 6374 2c20 6f74 7970  .apply(oct, otyp
-00033f40: 6573 3d5b 2755 275d 290d 0a20 2020 2020  es=['U'])..     
-00033f50: 2020 2046 6173 7441 7272 6179 285b 2730     FastArray(['0
-00033f60: 6f30 272c 2027 306f 3127 2c20 2730 6f32  o0', '0o1', '0o2
-00033f70: 272c 2027 306f 3327 2c20 2730 6f34 272c  ', '0o3', '0o4',
-00033f80: 2027 306f 3527 2c20 2730 6f36 272c 2027   '0o5', '0o6', '
-00033f90: 306f 3727 2c20 2730 6f31 3027 2c20 2730  0o7', '0o10', '0
-00033fa0: 6f31 3127 5d2c 2064 7479 7065 3d27 3c55  o11'], dtype='<U
-00033fb0: 3427 290d 0a0d 0a20 2020 2020 2020 203e  4')....        >
-00033fc0: 3e3e 2061 3d61 7261 6e67 6528 3130 290d  >> a=arange(10).
-00033fd0: 0a20 2020 2020 2020 203e 3e3e 2061 2e61  .        >>> a.a
-00033fe0: 7070 6c79 286f 6374 2c20 6f74 7970 6573  pply(oct, otypes
-00033ff0: 3d5b 274f 275d 290d 0a20 2020 2020 2020  =['O'])..       
-00034000: 2046 6173 7441 7272 6179 285b 2730 6f30   FastArray(['0o0
-00034010: 272c 2027 306f 3127 2c20 2730 6f32 272c  ', '0o1', '0o2',
-00034020: 2027 306f 3327 2c20 2730 6f34 272c 2027   '0o3', '0o4', '
-00034030: 306f 3527 2c20 2730 6f36 272c 2027 306f  0o5', '0o6', '0o
-00034040: 3727 2c20 2730 6f31 3027 2c20 2730 6f31  7', '0o10', '0o1
-00034050: 3127 5d2c 2064 7479 7065 3d6f 626a 6563  1'], dtype=objec
-00034060: 7429 0d0a 0d0a 2020 2020 2020 2020 2222  t)....        ""
-00034070: 220d 0a0d 0a20 2020 2020 2020 2076 6675  "....        vfu
-00034080: 6e63 203d 206e 702e 7665 6374 6f72 697a  nc = np.vectoriz
-00034090: 6528 7079 6675 6e63 2c20 6f74 7970 6573  e(pyfunc, otypes
-000340a0: 3d6f 7479 7065 732c 2064 6f63 3d64 6f63  =otypes, doc=doc
-000340b0: 2c20 6578 636c 7564 6564 3d65 7863 6c75  , excluded=exclu
-000340c0: 6465 642c 2063 6163 6865 3d63 6163 6865  ded, cache=cache
-000340d0: 2c20 7369 676e 6174 7572 653d 7369 676e  , signature=sign
-000340e0: 6174 7572 6529 0d0a 2020 2020 2020 2020  ature)..        
-000340f0: 7265 7375 6c74 203d 2076 6675 6e63 2873  result = vfunc(s
-00034100: 656c 662c 202a 6172 6773 290d 0a20 2020  elf, *args)..   
-00034110: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00034120: 6c74 0d0a 0d0a 2020 2020 2320 2d2d 2d2d  lt....    # ----
+00032e70: 2066 2254 6865 6e20 6361 6c6c 207b 6d79   f"Then call {my
+00032e80: 6675 6e63 7d28 7b6e 616d 657d 2e6e 756d  func}({name}.num
+00032e90: 6261 7374 7269 6e67 2c65 6d70 7479 5f6c  bastring,empty_l
+00032ea0: 696b 6528 7b6e 616d 657d 292e 6e75 6d62  ike({name}).numb
+00032eb0: 6173 7472 696e 6729 2077 6865 7265 207b  astring) where {
+00032ec0: 6e61 6d65 7d20 6973 2074 6865 2069 6e70  name} is the inp
+00032ed0: 7574 2061 7272 6179 220d 0a20 2020 2020  ut array"..     
+00032ee0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00032ef0: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
+00032f00: 6e74 7970 655b 315d 203d 3d20 2255 223a  ntype[1] == "U":
+00032f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00032f20: 2020 7072 696e 7428 0d0a 2020 2020 2020    print(..      
+00032f30: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00032f40: 5468 656e 2063 616c 6c20 7b6d 7966 756e  Then call {myfun
+00032f50: 637d 287b 6e61 6d65 7d2e 6e75 6d62 6173  c}({name}.numbas
+00032f60: 7472 696e 672c 656d 7074 795f 6c69 6b65  tring,empty_like
+00032f70: 287b 6e61 6d65 7d29 2e6e 756d 6261 7374  ({name}).numbast
+00032f80: 7269 6e67 2920 7768 6572 6520 7b6e 616d  ring) where {nam
+00032f90: 657d 2069 7320 7468 6520 696e 7075 7420  e} is the input 
+00032fa0: 6172 7261 7922 0d0a 2020 2020 2020 2020  array"..        
+00032fb0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00032fc0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00032fd0: 2020 2020 2020 7072 696e 7428 6622 5468        print(f"Th
+00032fe0: 656e 2063 616c 6c20 7b6d 7966 756e 637d  en call {myfunc}
+00032ff0: 287b 6e61 6d65 7d2c 656d 7074 795f 6c69  ({name},empty_li
+00033000: 6b65 287b 6e61 6d65 7d29 2920 7768 6572  ke({name})) wher
+00033010: 6520 7b6e 616d 657d 2069 7320 7468 6520  e {name} is the 
+00033020: 696e 7075 7420 6172 7261 7922 290d 0a20  input array").. 
+00033030: 2020 2020 2020 2023 2072 6574 7572 6e20         # return 
+00033040: 6578 6563 0d0a 0d0a 2020 2020 6465 6620  exec....    def 
+00033050: 6170 706c 7928 7365 6c66 2c20 7079 6675  apply(self, pyfu
+00033060: 6e63 2c20 2a61 7267 732c 206f 7479 7065  nc, *args, otype
+00033070: 733d 4e6f 6e65 2c20 646f 633d 4e6f 6e65  s=None, doc=None
+00033080: 2c20 6578 636c 7564 6564 3d4e 6f6e 652c  , excluded=None,
+00033090: 2063 6163 6865 3d46 616c 7365 2c20 7369   cache=False, si
+000330a0: 676e 6174 7572 653d 4e6f 6e65 293a 0d0a  gnature=None):..
+000330b0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+000330c0: 2020 2020 2047 656e 6572 616c 697a 6564       Generalized
+000330d0: 2066 756e 6374 696f 6e20 636c 6173 732e   function class.
+000330e0: 2020 7365 653a 206e 702e 7665 6374 6f72    see: np.vector
+000330f0: 697a 650d 0a0d 0a20 2020 2020 2020 2043  ize....        C
+00033100: 7265 6174 6573 2061 6e64 2074 6865 6e20  reates and then 
+00033110: 6170 706c 6965 7320 6120 7665 6374 6f72  applies a vector
+00033120: 697a 6564 2066 756e 6374 696f 6e20 7768  ized function wh
+00033130: 6963 6820 7461 6b65 7320 6120 6e65 7374  ich takes a nest
+00033140: 6564 2073 6571 7565 6e63 6520 6f66 206f  ed sequence of o
+00033150: 626a 6563 7473 206f 720d 0a20 2020 2020  bjects or..     
+00033160: 2020 206e 756d 7079 2061 7272 6179 7320     numpy arrays 
+00033170: 6173 2069 6e70 7574 7320 616e 6420 7265  as inputs and re
+00033180: 7475 726e 7320 616e 2073 696e 676c 6520  turns an single 
+00033190: 6f72 2074 7570 6c65 206f 6620 6e75 6d70  or tuple of nump
+000331a0: 7920 6172 7261 7920 6173 0d0a 2020 2020  y array as..    
+000331b0: 2020 2020 6f75 7470 7574 2e20 5468 6520      output. The 
+000331c0: 7665 6374 6f72 697a 6564 2066 756e 6374  vectorized funct
+000331d0: 696f 6e20 6576 616c 7561 7465 7320 6070  ion evaluates `p
+000331e0: 7966 756e 6360 206f 7665 7220 7375 6363  yfunc` over succ
+000331f0: 6573 7369 7665 2074 7570 6c65 730d 0a20  essive tuples.. 
+00033200: 2020 2020 2020 206f 6620 7468 6520 696e         of the in
+00033210: 7075 7420 6172 7261 7973 206c 696b 6520  put arrays like 
+00033220: 7468 6520 7079 7468 6f6e 206d 6170 2066  the python map f
+00033230: 756e 6374 696f 6e2c 2065 7863 6570 7420  unction, except 
+00033240: 6974 2075 7365 7320 7468 650d 0a20 2020  it uses the..   
+00033250: 2020 2020 2062 726f 6164 6361 7374 696e       broadcastin
+00033260: 6720 7275 6c65 7320 6f66 206e 756d 7079  g rules of numpy
+00033270: 2e0d 0a0d 0a20 2020 2020 2020 2054 6865  .....        The
+00033280: 2064 6174 6120 7479 7065 206f 6620 7468   data type of th
+00033290: 6520 6f75 7470 7574 206f 6620 6076 6563  e output of `vec
+000332a0: 746f 7269 7a65 6460 2069 7320 6465 7465  torized` is dete
+000332b0: 726d 696e 6564 2062 7920 6361 6c6c 696e  rmined by callin
+000332c0: 670d 0a20 2020 2020 2020 2074 6865 2066  g..        the f
+000332d0: 756e 6374 696f 6e20 7769 7468 2074 6865  unction with the
+000332e0: 2066 6972 7374 2065 6c65 6d65 6e74 206f   first element o
+000332f0: 6620 7468 6520 696e 7075 742e 2020 5468  f the input.  Th
+00033300: 6973 2063 616e 2062 6520 6176 6f69 6465  is can be avoide
+00033310: 640d 0a20 2020 2020 2020 2062 7920 7370  d..        by sp
+00033320: 6563 6966 7969 6e67 2074 6865 2060 6f74  ecifying the `ot
+00033330: 7970 6573 6020 6172 6775 6d65 6e74 2e0d  ypes` argument..
+00033340: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00033350: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
+00033360: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
+00033370: 2020 2070 7966 756e 6320 3a20 6361 6c6c     pyfunc : call
+00033380: 6162 6c65 0d0a 2020 2020 2020 2020 2020  able..          
+00033390: 2020 4120 7079 7468 6f6e 2066 756e 6374    A python funct
+000333a0: 696f 6e20 6f72 206d 6574 686f 642e 0d0a  ion or method...
+000333b0: 2020 2020 2020 2020 6f74 7970 6573 203a          otypes :
+000333c0: 2073 7472 206f 7220 6c69 7374 206f 6620   str or list of 
+000333d0: 6474 7970 6573 2c20 6f70 7469 6f6e 616c  dtypes, optional
+000333e0: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+000333f0: 6520 6f75 7470 7574 2064 6174 6120 7479  e output data ty
+00033400: 7065 2e20 4974 206d 7573 7420 6265 2073  pe. It must be s
+00033410: 7065 6369 6669 6564 2061 7320 6569 7468  pecified as eith
+00033420: 6572 2061 2073 7472 696e 6720 6f66 0d0a  er a string of..
+00033430: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00033440: 636f 6465 2063 6861 7261 6374 6572 7320  code characters 
+00033450: 6f72 2061 206c 6973 7420 6f66 2064 6174  or a list of dat
+00033460: 6120 7479 7065 2073 7065 6369 6669 6572  a type specifier
+00033470: 732e 2054 6865 7265 2073 686f 756c 640d  s. There should.
+00033480: 0a20 2020 2020 2020 2020 2020 2062 6520  .            be 
+00033490: 6f6e 6520 6461 7461 2074 7970 6520 7370  one data type sp
+000334a0: 6563 6966 6965 7220 666f 7220 6561 6368  ecifier for each
+000334b0: 206f 7574 7075 742e 0d0a 2020 2020 2020   output...      
+000334c0: 2020 646f 6320 3a20 7374 722c 206f 7074    doc : str, opt
+000334d0: 696f 6e61 6c0d 0a20 2020 2020 2020 2020  ional..         
+000334e0: 2020 2054 6865 2064 6f63 7374 7269 6e67     The docstring
+000334f0: 2066 6f72 2074 6865 2066 756e 6374 696f   for the functio
+00033500: 6e2e 2049 6620 604e 6f6e 6560 2c20 7468  n. If `None`, th
+00033510: 6520 646f 6373 7472 696e 6720 7769 6c6c  e docstring will
+00033520: 2062 6520 7468 650d 0a20 2020 2020 2020   be the..       
+00033530: 2020 2020 2060 6070 7966 756e 632e 5f5f       ``pyfunc.__
+00033540: 646f 635f 5f60 602e 0d0a 2020 2020 2020  doc__``...      
+00033550: 2020 6578 636c 7564 6564 203a 2073 6574    excluded : set
+00033560: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00033570: 2020 2020 2020 2020 5365 7420 6f66 2073          Set of s
+00033580: 7472 696e 6773 206f 7220 696e 7465 6765  trings or intege
+00033590: 7273 2072 6570 7265 7365 6e74 696e 6720  rs representing 
+000335a0: 7468 6520 706f 7369 7469 6f6e 616c 206f  the positional o
+000335b0: 7220 6b65 7977 6f72 640d 0a20 2020 2020  r keyword..     
+000335c0: 2020 2020 2020 2061 7267 756d 656e 7473         arguments
+000335d0: 2066 6f72 2077 6869 6368 2074 6865 2066   for which the f
+000335e0: 756e 6374 696f 6e20 7769 6c6c 206e 6f74  unction will not
+000335f0: 2062 6520 7665 6374 6f72 697a 6564 2e20   be vectorized. 
+00033600: 2054 6865 7365 2077 696c 6c20 6265 0d0a   These will be..
+00033610: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00033620: 6564 2064 6972 6563 746c 7920 746f 2060  ed directly to `
+00033630: 7079 6675 6e63 6020 756e 6d6f 6469 6669  pyfunc` unmodifi
+00033640: 6564 2e0d 0a0d 0a20 2020 2020 2020 2020  ed.....         
+00033650: 2020 202e 2e20 7665 7273 696f 6e61 6464     .. versionadd
+00033660: 6564 3a3a 2031 2e37 2e30 0d0a 0d0a 2020  ed:: 1.7.0....  
+00033670: 2020 2020 2020 6361 6368 6520 3a20 626f        cache : bo
+00033680: 6f6c 2c20 6f70 7469 6f6e 616c 0d0a 2020  ol, optional..  
+00033690: 2020 2020 2020 2020 2049 6620 6054 7275           If `Tru
+000336a0: 6560 2c20 7468 656e 2063 6163 6865 2074  e`, then cache t
+000336b0: 6865 2066 6972 7374 2066 756e 6374 696f  he first functio
+000336c0: 6e20 6361 6c6c 2074 6861 7420 6465 7465  n call that dete
+000336d0: 726d 696e 6573 2074 6865 206e 756d 6265  rmines the numbe
+000336e0: 720d 0a20 2020 2020 2020 2020 2020 6f66  r..           of
+000336f0: 206f 7574 7075 7473 2069 6620 606f 7479   outputs if `oty
+00033700: 7065 7360 2069 7320 6e6f 7420 7072 6f76  pes` is not prov
+00033710: 6964 6564 2e0d 0a0d 0a20 2020 2020 2020  ided.....       
+00033720: 2020 2020 202e 2e20 7665 7273 696f 6e61       .. versiona
+00033730: 6464 6564 3a3a 2031 2e37 2e30 0d0a 0d0a  dded:: 1.7.0....
+00033740: 2020 2020 2020 2020 7369 676e 6174 7572          signatur
+00033750: 6520 3a20 7374 7269 6e67 2c20 6f70 7469  e : string, opti
+00033760: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
+00033770: 2020 4765 6e65 7261 6c69 7a65 6420 756e    Generalized un
+00033780: 6976 6572 7361 6c20 6675 6e63 7469 6f6e  iversal function
+00033790: 2073 6967 6e61 7475 7265 2c20 652e 672e   signature, e.g.
+000337a0: 2c20 6060 286d 2c6e 292c 286e 292d 3e28  , ``(m,n),(n)->(
+000337b0: 6d29 6060 2066 6f72 0d0a 2020 2020 2020  m)`` for..      
+000337c0: 2020 2020 2020 7665 6374 6f72 697a 6564        vectorized
+000337d0: 206d 6174 7269 782d 7665 6374 6f72 206d   matrix-vector m
+000337e0: 756c 7469 706c 6963 6174 696f 6e2e 2049  ultiplication. I
+000337f0: 6620 7072 6f76 6964 6564 2c20 6060 7079  f provided, ``py
+00033800: 6675 6e63 6060 2077 696c 6c0d 0a20 2020  func`` will..   
+00033810: 2020 2020 2020 2020 2062 6520 6361 6c6c           be call
+00033820: 6564 2077 6974 6820 2861 6e64 2065 7870  ed with (and exp
+00033830: 6563 7465 6420 746f 2072 6574 7572 6e29  ected to return)
+00033840: 2061 7272 6179 7320 7769 7468 2073 6861   arrays with sha
+00033850: 7065 7320 6769 7665 6e20 6279 2074 6865  pes given by the
+00033860: 0d0a 2020 2020 2020 2020 2020 2020 7369  ..            si
+00033870: 7a65 206f 6620 636f 7272 6573 706f 6e64  ze of correspond
+00033880: 696e 6720 636f 7265 2064 696d 656e 7369  ing core dimensi
+00033890: 6f6e 732e 2042 7920 6465 6661 756c 742c  ons. By default,
+000338a0: 2060 6070 7966 756e 6360 6020 6973 0d0a   ``pyfunc`` is..
+000338b0: 2020 2020 2020 2020 2020 2020 6173 7375              assu
+000338c0: 6d65 6420 746f 2074 616b 6520 7363 616c  med to take scal
+000338d0: 6172 7320 6173 2069 6e70 7574 2061 6e64  ars as input and
+000338e0: 206f 7574 7075 742e 0d0a 0d0a 2020 2020   output.....    
+000338f0: 2020 2020 2020 2020 2e2e 2076 6572 7369          .. versi
+00033900: 6f6e 6164 6465 643a 3a20 312e 3132 2e30  onadded:: 1.12.0
+00033910: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00033920: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
+00033930: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7665  ----..        ve
+00033940: 6374 6f72 697a 6564 203a 2063 616c 6c61  ctorized : calla
+00033950: 626c 650d 0a20 2020 2020 2020 2020 2020  ble..           
+00033960: 2056 6563 746f 7269 7a65 6420 6675 6e63   Vectorized func
+00033970: 7469 6f6e 2e0d 0a0d 0a20 2020 2020 2020  tion.....       
+00033980: 2053 6565 2041 6c73 6f0d 0a20 2020 2020   See Also..     
+00033990: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
+000339a0: 2020 2020 2046 6173 7441 7272 6179 2e61       FastArray.a
+000339b0: 7070 6c79 5f6e 756d 6261 0d0a 2020 2020  pply_numba..    
+000339c0: 2020 2020 4661 7374 4172 7261 792e 6170      FastArray.ap
+000339d0: 706c 795f 7061 6e64 6173 0d0a 0d0a 2020  ply_pandas....  
+000339e0: 2020 2020 2020 4578 616d 706c 6573 0d0a        Examples..
+000339f0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00033a00: 0d0a 2020 2020 2020 2020 3e3e 3e20 6465  ..        >>> de
+00033a10: 6620 6d79 6675 6e63 2861 2c20 6229 3a0d  f myfunc(a, b):.
+00033a20: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
+00033a30: 2022 5265 7475 726e 2061 2d62 2069 6620   "Return a-b if 
+00033a40: 613e 622c 206f 7468 6572 7769 7365 2072  a>b, otherwise r
+00033a50: 6574 7572 6e20 612b 6222 0d0a 2020 2020  eturn a+b"..    
+00033a60: 2020 2020 2e2e 2e20 2020 2020 6966 2061      ...     if a
+00033a70: 203e 2062 3a0d 0a20 2020 2020 2020 202e   > b:..        .
+00033a80: 2e2e 2020 2020 2020 2020 2072 6574 7572  ..         retur
+00033a90: 6e20 6120 2d20 620d 0a20 2020 2020 2020  n a - b..       
+00033aa0: 202e 2e2e 2020 2020 2065 6c73 653a 0d0a   ...     else:..
+00033ab0: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+00033ac0: 2020 2020 7265 7475 726e 2061 202b 2062      return a + b
+00033ad0: 0d0a 2020 2020 2020 2020 3e3e 3e0d 0a20  ..        >>>.. 
+00033ae0: 2020 2020 2020 203e 3e3e 2061 3d61 7261         >>> a=ara
+00033af0: 6e67 6528 3130 290d 0a20 2020 2020 2020  nge(10)..       
+00033b00: 203e 3e3e 2062 3d61 7261 6e67 6528 3130   >>> b=arange(10
+00033b10: 292b 310d 0a20 2020 2020 2020 203e 3e3e  )+1..        >>>
+00033b20: 2061 2e61 7070 6c79 286d 7966 756e 632c   a.apply(myfunc,
+00033b30: 6229 0d0a 2020 2020 2020 2020 4661 7374  b)..        Fast
+00033b40: 4172 7261 7928 5b20 312c 2020 332c 2020  Array([ 1,  3,  
+00033b50: 352c 2020 372c 2020 392c 2031 312c 2031  5,  7,  9, 11, 1
+00033b60: 332c 2031 352c 2031 372c 2031 395d 290d  3, 15, 17, 19]).
+00033b70: 0a0d 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+00033b80: 6c65 2077 6974 6820 6f6e 6520 696e 7075  le with one inpu
+00033b90: 7420 6172 7261 790d 0a0d 0a20 2020 2020  t array....     
+00033ba0: 2020 203e 3e3e 2064 6566 2073 7175 6172     >>> def squar
+00033bb0: 6528 7829 3a0d 0a20 2020 2020 2020 202e  e(x):..        .
+00033bc0: 2e2e 2020 2020 2072 6574 7572 6e20 782a  ..     return x*
+00033bd0: 2a32 0d0a 2020 2020 2020 2020 3e3e 3e0d  *2..        >>>.
+00033be0: 0a20 2020 2020 2020 203e 3e3e 2061 3d61  .        >>> a=a
+00033bf0: 7261 6e67 6528 3130 290d 0a20 2020 2020  range(10)..     
+00033c00: 2020 203e 3e3e 2061 2e61 7070 6c79 2873     >>> a.apply(s
+00033c10: 7175 6172 6529 0d0a 2020 2020 2020 2020  quare)..        
+00033c20: 4661 7374 4172 7261 7928 5b20 302c 2020  FastArray([ 0,  
+00033c30: 312c 2020 342c 2020 392c 2031 362c 2032  1,  4,  9, 16, 2
+00033c40: 352c 2033 362c 2034 392c 2036 342c 2038  5, 36, 49, 64, 8
+00033c50: 315d 290d 0a0d 0a20 2020 2020 2020 2045  1])....        E
+00033c60: 7861 6d70 6c65 2077 6974 6820 6c61 6d62  xample with lamb
+00033c70: 6461 0d0a 0d0a 2020 2020 2020 2020 3e3e  da....        >>
+00033c80: 3e20 613d 6172 616e 6765 2831 3029 0d0a  > a=arange(10)..
+00033c90: 2020 2020 2020 2020 3e3e 3e20 612e 6170          >>> a.ap
+00033ca0: 706c 7928 6c61 6d62 6461 2078 3a20 782a  ply(lambda x: x*
+00033cb0: 2a32 290d 0a20 2020 2020 2020 2046 6173  *2)..        Fas
+00033cc0: 7441 7272 6179 285b 2030 2c20 2031 2c20  tArray([ 0,  1, 
+00033cd0: 2034 2c20 2039 2c20 3136 2c20 3235 2c20   4,  9, 16, 25, 
+00033ce0: 3336 2c20 3439 2c20 3634 2c20 3831 5d29  36, 49, 64, 81])
+00033cf0: 0d0a 0d0a 2020 2020 2020 2020 4578 616d  ....        Exam
+00033d00: 706c 6520 7769 7468 206e 756d 6261 0d0a  ple with numba..
+00033d10: 0d0a 2020 2020 2020 2020 3e3e 3e20 6672  ..        >>> fr
+00033d20: 6f6d 206e 756d 6261 2069 6d70 6f72 7420  om numba import 
+00033d30: 6a69 740d 0a20 2020 2020 2020 203e 3e3e  jit..        >>>
+00033d40: 2040 6a69 740d 0a20 2020 2020 2020 202e   @jit..        .
+00033d50: 2e2e 2064 6566 2073 7175 6172 6569 7428  .. def squareit(
+00033d60: 7829 3a0d 0a20 2020 2020 2020 202e 2e2e  x):..        ...
+00033d70: 2020 2020 2072 6574 7572 6e20 782a 2a32       return x**2
+00033d80: 0d0a 2020 2020 2020 2020 3e3e 3e20 612e  ..        >>> a.
+00033d90: 6170 706c 7928 7371 7561 7265 6974 290d  apply(squareit).
+00033da0: 0a20 2020 2020 2020 2046 6173 7441 7272  .        FastArr
+00033db0: 6179 285b 2030 2c20 2031 2c20 2034 2c20  ay([ 0,  1,  4, 
+00033dc0: 2039 2c20 3136 2c20 3235 2c20 3336 2c20   9, 16, 25, 36, 
+00033dd0: 3439 2c20 3634 2c20 3831 5d29 0d0a 0d0a  49, 64, 81])....
+00033de0: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
+00033df0: 2074 6f20 7573 6520 6578 6973 7469 6e67   to use existing
+00033e00: 2062 7569 6c74 696e 206f 6374 2066 756e   builtin oct fun
+00033e10: 6374 696f 6e20 6275 7420 6368 616e 6765  ction but change
+00033e20: 2074 6865 206f 7574 7075 7420 6672 6f6d   the output from
+00033e30: 2073 7472 696e 672c 2074 6f20 756e 6963   string, to unic
+00033e40: 6f64 652c 2074 6f20 6f62 6a65 6374 0d0a  ode, to object..
+00033e50: 0d0a 2020 2020 2020 2020 3e3e 3e20 613d  ..        >>> a=
+00033e60: 6172 616e 6765 2831 3029 0d0a 2020 2020  arange(10)..    
+00033e70: 2020 2020 3e3e 3e20 612e 6170 706c 7928      >>> a.apply(
+00033e80: 6f63 742c 206f 7479 7065 733d 5b27 5327  oct, otypes=['S'
+00033e90: 5d29 0d0a 2020 2020 2020 2020 4661 7374  ])..        Fast
+00033ea0: 4172 7261 7928 5b62 2730 6f30 272c 2062  Array([b'0o0', b
+00033eb0: 2730 6f31 272c 2062 2730 6f32 272c 2062  '0o1', b'0o2', b
+00033ec0: 2730 6f33 272c 2062 2730 6f34 272c 2062  '0o3', b'0o4', b
+00033ed0: 2730 6f35 272c 2062 2730 6f36 272c 2062  '0o5', b'0o6', b
+00033ee0: 2730 6f37 272c 2062 2730 6f31 3027 2c20  '0o7', b'0o10', 
+00033ef0: 6227 306f 3131 275d 2c20 6474 7970 653d  b'0o11'], dtype=
+00033f00: 277c 5334 2729 0d0a 0d0a 2020 2020 2020  '|S4')....      
+00033f10: 2020 3e3e 3e20 613d 6172 616e 6765 2831    >>> a=arange(1
+00033f20: 3029 0d0a 2020 2020 2020 2020 3e3e 3e20  0)..        >>> 
+00033f30: 612e 6170 706c 7928 6f63 742c 206f 7479  a.apply(oct, oty
+00033f40: 7065 733d 5b27 5527 5d29 0d0a 2020 2020  pes=['U'])..    
+00033f50: 2020 2020 4661 7374 4172 7261 7928 5b27      FastArray(['
+00033f60: 306f 3027 2c20 2730 6f31 272c 2027 306f  0o0', '0o1', '0o
+00033f70: 3227 2c20 2730 6f33 272c 2027 306f 3427  2', '0o3', '0o4'
+00033f80: 2c20 2730 6f35 272c 2027 306f 3627 2c20  , '0o5', '0o6', 
+00033f90: 2730 6f37 272c 2027 306f 3130 272c 2027  '0o7', '0o10', '
+00033fa0: 306f 3131 275d 2c20 6474 7970 653d 273c  0o11'], dtype='<
+00033fb0: 5534 2729 0d0a 0d0a 2020 2020 2020 2020  U4')....        
+00033fc0: 3e3e 3e20 613d 6172 616e 6765 2831 3029  >>> a=arange(10)
+00033fd0: 0d0a 2020 2020 2020 2020 3e3e 3e20 612e  ..        >>> a.
+00033fe0: 6170 706c 7928 6f63 742c 206f 7479 7065  apply(oct, otype
+00033ff0: 733d 5b27 4f27 5d29 0d0a 2020 2020 2020  s=['O'])..      
+00034000: 2020 4661 7374 4172 7261 7928 5b27 306f    FastArray(['0o
+00034010: 3027 2c20 2730 6f31 272c 2027 306f 3227  0', '0o1', '0o2'
+00034020: 2c20 2730 6f33 272c 2027 306f 3427 2c20  , '0o3', '0o4', 
+00034030: 2730 6f35 272c 2027 306f 3627 2c20 2730  '0o5', '0o6', '0
+00034040: 6f37 272c 2027 306f 3130 272c 2027 306f  o7', '0o10', '0o
+00034050: 3131 275d 2c20 6474 7970 653d 6f62 6a65  11'], dtype=obje
+00034060: 6374 290d 0a0d 0a20 2020 2020 2020 2022  ct)....        "
+00034070: 2222 0d0a 0d0a 2020 2020 2020 2020 7666  ""....        vf
+00034080: 756e 6320 3d20 6e70 2e76 6563 746f 7269  unc = np.vectori
+00034090: 7a65 2870 7966 756e 632c 206f 7479 7065  ze(pyfunc, otype
+000340a0: 733d 6f74 7970 6573 2c20 646f 633d 646f  s=otypes, doc=do
+000340b0: 632c 2065 7863 6c75 6465 643d 6578 636c  c, excluded=excl
+000340c0: 7564 6564 2c20 6361 6368 653d 6361 6368  uded, cache=cach
+000340d0: 652c 2073 6967 6e61 7475 7265 3d73 6967  e, signature=sig
+000340e0: 6e61 7475 7265 290d 0a20 2020 2020 2020  nature)..       
+000340f0: 2072 6573 756c 7420 3d20 7666 756e 6328   result = vfunc(
+00034100: 7365 6c66 2c20 2a61 7267 7329 0d0a 2020  self, *args)..  
+00034110: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00034120: 756c 740d 0a0d 0a20 2020 2023 202d 2d2d  ult....    # ---
 00034130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00034160: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2064 6566  -------..    def
-00034170: 2061 7070 6c79 5f70 616e 6461 7328 7365   apply_pandas(se
-00034180: 6c66 2c20 6675 6e63 2c20 636f 6e76 6572  lf, func, conver
-00034190: 745f 6474 7970 653d 5472 7565 2c20 6172  t_dtype=True, ar
-000341a0: 6773 3d28 292c 202a 2a6b 7764 7329 3a0d  gs=(), **kwds):.
-000341b0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-000341c0: 2020 2020 2020 496e 766f 6b65 2066 756e        Invoke fun
-000341d0: 6374 696f 6e20 6f6e 2076 616c 7565 7320  ction on values 
-000341e0: 6f66 2046 6173 7441 7272 6179 2e20 4361  of FastArray. Ca
-000341f0: 6e20 6265 2075 6675 6e63 2028 6120 4e75  n be ufunc (a Nu
-00034200: 6d50 7920 6675 6e63 7469 6f6e 0d0a 2020  mPy function..  
-00034210: 2020 2020 2020 7468 6174 2061 7070 6c69        that appli
-00034220: 6573 2074 6f20 7468 6520 656e 7469 7265  es to the entire
-00034230: 2046 6173 7441 7272 6179 2920 6f72 2061   FastArray) or a
-00034240: 2050 7974 686f 6e20 6675 6e63 7469 6f6e   Python function
-00034250: 2074 6861 7420 6f6e 6c79 2077 6f72 6b73   that only works
-00034260: 0d0a 2020 2020 2020 2020 6f6e 2073 696e  ..        on sin
-00034270: 676c 6520 7661 6c75 6573 0d0a 0d0a 2020  gle values....  
-00034280: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00034290: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-000342a0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6675  ----..        fu
-000342b0: 6e63 203a 2066 756e 6374 696f 6e0d 0a20  nc : function.. 
-000342c0: 2020 2020 2020 2063 6f6e 7665 7274 5f64         convert_d
-000342d0: 7479 7065 203a 2062 6f6f 6c65 616e 2c20  type : boolean, 
-000342e0: 6465 6661 756c 7420 5472 7565 0d0a 2020  default True..  
-000342f0: 2020 2020 2020 2020 2020 5472 7920 746f            Try to
-00034300: 2066 696e 6420 6265 7474 6572 2064 7479   find better dty
-00034310: 7065 2066 6f72 2065 6c65 6d65 6e74 7769  pe for elementwi
-00034320: 7365 2066 756e 6374 696f 6e20 7265 7375  se function resu
-00034330: 6c74 732e 2049 660d 0a20 2020 2020 2020  lts. If..       
-00034340: 2020 2020 2046 616c 7365 2c20 6c65 6176       False, leav
-00034350: 6520 6173 2064 7479 7065 3d6f 626a 6563  e as dtype=objec
-00034360: 740d 0a20 2020 2020 2020 2061 7267 7320  t..        args 
-00034370: 3a20 7475 706c 650d 0a20 2020 2020 2020  : tuple..       
-00034380: 2020 2020 2050 6f73 6974 696f 6e61 6c20       Positional 
-00034390: 6172 6775 6d65 6e74 7320 746f 2070 6173  arguments to pas
-000343a0: 7320 746f 2066 756e 6374 696f 6e20 696e  s to function in
-000343b0: 2061 6464 6974 696f 6e20 746f 2074 6865   addition to the
-000343c0: 2076 616c 7565 0d0a 2020 2020 2020 2020   value..        
-000343d0: 4164 6469 7469 6f6e 616c 206b 6579 776f  Additional keywo
-000343e0: 7264 2061 7267 756d 656e 7473 2077 696c  rd arguments wil
-000343f0: 6c20 6265 2070 6173 7365 6420 6173 206b  l be passed as k
-00034400: 6579 776f 7264 7320 746f 2074 6865 2066  eywords to the f
-00034410: 756e 6374 696f 6e0d 0a0d 0a20 2020 2020  unction....     
-00034420: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-00034430: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-00034440: 2020 2020 2079 203a 2046 6173 7441 7272       y : FastArr
-00034450: 6179 206f 7220 4461 7461 7365 7420 6966  ay or Dataset if
-00034460: 2066 756e 6320 7265 7475 726e 7320 6120   func returns a 
-00034470: 4661 7374 4172 7261 790d 0a0d 0a20 2020  FastArray....   
-00034480: 2020 2020 2053 6565 2041 6c73 6f0d 0a20       See Also.. 
-00034490: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0d         --------.
-000344a0: 0a20 2020 2020 2020 2046 6173 7441 7272  .        FastArr
-000344b0: 6179 2e6d 6170 3a20 466f 7220 656c 656d  ay.map: For elem
-000344c0: 656e 742d 7769 7365 206f 7065 7261 7469  ent-wise operati
-000344d0: 6f6e 730d 0a20 2020 2020 2020 2046 6173  ons..        Fas
-000344e0: 7441 7272 6179 2e61 6767 3a20 6f6e 6c79  tArray.agg: only
-000344f0: 2070 6572 666f 726d 2061 6767 7265 6761   perform aggrega
-00034500: 7469 6e67 2074 7970 6520 6f70 6572 6174  ting type operat
-00034510: 696f 6e73 0d0a 2020 2020 2020 2020 4661  ions..        Fa
-00034520: 7374 4172 7261 792e 7472 616e 7366 6f72  stArray.transfor
-00034530: 6d3a 206f 6e6c 7920 7065 7266 6f72 6d20  m: only perform 
-00034540: 7472 616e 7366 6f72 6d69 6e67 2074 7970  transforming typ
-00034550: 6520 6f70 6572 6174 696f 6e73 0d0a 0d0a  e operations....
-00034560: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
-00034570: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00034580: 2d2d 0d0a 2020 2020 2020 2020 4372 6561  --..        Crea
-00034590: 7465 2061 2046 6173 7441 7272 6179 2077  te a FastArray w
-000345a0: 6974 6820 7479 7069 6361 6c20 7375 6d6d  ith typical summ
-000345b0: 6572 2074 656d 7065 7261 7475 7265 7320  er temperatures 
-000345c0: 666f 7220 6561 6368 2063 6974 792e 0d0a  for each city...
-000345d0: 0d0a 2020 2020 2020 2020 3e3e 3e20 6661  ..        >>> fa
-000345e0: 203d 2072 742e 4661 7374 4172 7261 7928   = rt.FastArray(
-000345f0: 5b32 302c 2032 312c 2031 325d 2c20 696e  [20, 21, 12], in
-00034600: 6465 783d 5b27 4c6f 6e64 6f6e 272c 2027  dex=['London', '
-00034610: 4e65 7720 596f 726b 272c 2748 656c 7369  New York','Helsi
-00034620: 6e6b 6927 5d29 0d0a 2020 2020 2020 2020  nki'])..        
-00034630: 3e3e 3e20 6661 0d0a 2020 2020 2020 2020  >>> fa..        
-00034640: 4c6f 6e64 6f6e 2020 2020 2020 3230 0d0a  London      20..
-00034650: 2020 2020 2020 2020 4e65 7720 596f 726b          New York
-00034660: 2020 2020 3231 0d0a 2020 2020 2020 2020      21..        
-00034670: 4865 6c73 696e 6b69 2020 2020 3132 0d0a  Helsinki    12..
-00034680: 2020 2020 2020 2020 6474 7970 653a 2069          dtype: i
-00034690: 6e74 3634 0d0a 0d0a 2020 2020 2020 2020  nt64....        
-000346a0: 5371 7561 7265 2074 6865 2076 616c 7565  Square the value
-000346b0: 7320 6279 2064 6566 696e 696e 6720 6120  s by defining a 
-000346c0: 6675 6e63 7469 6f6e 2061 6e64 2070 6173  function and pas
-000346d0: 7369 6e67 2069 7420 6173 2061 6e0d 0a20  sing it as an.. 
-000346e0: 2020 2020 2020 2061 7267 756d 656e 7420         argument 
-000346f0: 746f 2060 6061 7070 6c79 2829 6060 2e0d  to ``apply()``..
-00034700: 0a0d 0a20 2020 2020 2020 203e 3e3e 2064  ...        >>> d
-00034710: 6566 2073 7175 6172 6528 7829 3a0d 0a20  ef square(x):.. 
-00034720: 2020 2020 2020 202e 2e2e 2020 2020 2072         ...     r
-00034730: 6574 7572 6e20 782a 2a32 0d0a 2020 2020  eturn x**2..    
-00034740: 2020 2020 3e3e 3e20 6661 2e61 7070 6c79      >>> fa.apply
-00034750: 2873 7175 6172 6529 0d0a 2020 2020 2020  (square)..      
-00034760: 2020 4c6f 6e64 6f6e 2020 2020 2020 3430    London      40
-00034770: 300d 0a20 2020 2020 2020 204e 6577 2059  0..        New Y
-00034780: 6f72 6b20 2020 2034 3431 0d0a 2020 2020  ork    441..    
-00034790: 2020 2020 4865 6c73 696e 6b69 2020 2020      Helsinki    
-000347a0: 3134 340d 0a20 2020 2020 2020 2064 7479  144..        dty
-000347b0: 7065 3a20 696e 7436 340d 0a0d 0a20 2020  pe: int64....   
-000347c0: 2020 2020 2053 7175 6172 6520 7468 6520       Square the 
-000347d0: 7661 6c75 6573 2062 7920 7061 7373 696e  values by passin
-000347e0: 6720 616e 2061 6e6f 6e79 6d6f 7573 2066  g an anonymous f
-000347f0: 756e 6374 696f 6e20 6173 2061 6e0d 0a20  unction as an.. 
-00034800: 2020 2020 2020 2061 7267 756d 656e 7420         argument 
-00034810: 746f 2060 6061 7070 6c79 2829 6060 2e0d  to ``apply()``..
-00034820: 0a0d 0a20 2020 2020 2020 203e 3e3e 2066  ...        >>> f
-00034830: 612e 6170 706c 7928 6c61 6d62 6461 2078  a.apply(lambda x
-00034840: 3a20 782a 2a32 290d 0a20 2020 2020 2020  : x**2)..       
-00034850: 204c 6f6e 646f 6e20 2020 2020 2034 3030   London      400
-00034860: 0d0a 2020 2020 2020 2020 4e65 7720 596f  ..        New Yo
-00034870: 726b 2020 2020 3434 310d 0a20 2020 2020  rk    441..     
-00034880: 2020 2048 656c 7369 6e6b 6920 2020 2031     Helsinki    1
-00034890: 3434 0d0a 2020 2020 2020 2020 6474 7970  44..        dtyp
-000348a0: 653a 2069 6e74 3634 0d0a 0d0a 2020 2020  e: int64....    
-000348b0: 2020 2020 4465 6669 6e65 2061 2063 7573      Define a cus
-000348c0: 746f 6d20 6675 6e63 7469 6f6e 2074 6861  tom function tha
-000348d0: 7420 6e65 6564 7320 6164 6469 7469 6f6e  t needs addition
-000348e0: 616c 2070 6f73 6974 696f 6e61 6c0d 0a20  al positional.. 
-000348f0: 2020 2020 2020 2061 7267 756d 656e 7473         arguments
-00034900: 2061 6e64 2070 6173 7320 7468 6573 6520   and pass these 
-00034910: 6164 6469 7469 6f6e 616c 2061 7267 756d  additional argum
-00034920: 656e 7473 2075 7369 6e67 2074 6865 0d0a  ents using the..
-00034930: 2020 2020 2020 2020 6060 6172 6773 6060          ``args``
-00034940: 206b 6579 776f 7264 2e0d 0a0d 0a20 2020   keyword.....   
-00034950: 2020 2020 203e 3e3e 2064 6566 2073 7562       >>> def sub
-00034960: 7472 6163 745f 6375 7374 6f6d 5f76 616c  tract_custom_val
-00034970: 7565 2878 2c20 6375 7374 6f6d 5f76 616c  ue(x, custom_val
-00034980: 7565 293a 0d0a 2020 2020 2020 2020 2e2e  ue):..        ..
-00034990: 2e20 2020 2020 7265 7475 726e 2078 2d63  .     return x-c
-000349a0: 7573 746f 6d5f 7661 6c75 650d 0a20 2020  ustom_value..   
-000349b0: 2020 2020 203e 3e3e 2066 612e 6170 706c       >>> fa.appl
-000349c0: 7928 7375 6274 7261 6374 5f63 7573 746f  y(subtract_custo
-000349d0: 6d5f 7661 6c75 652c 2061 7267 733d 2835  m_value, args=(5
-000349e0: 2c29 290d 0a20 2020 2020 2020 204c 6f6e  ,))..        Lon
-000349f0: 646f 6e20 2020 2020 2031 350d 0a20 2020  don      15..   
-00034a00: 2020 2020 204e 6577 2059 6f72 6b20 2020       New York   
-00034a10: 2031 360d 0a20 2020 2020 2020 2048 656c   16..        Hel
-00034a20: 7369 6e6b 6920 2020 2020 370d 0a20 2020  sinki     7..   
-00034a30: 2020 2020 2064 7479 7065 3a20 696e 7436       dtype: int6
-00034a40: 340d 0a0d 0a20 2020 2020 2020 2044 6566  4....        Def
-00034a50: 696e 6520 6120 6375 7374 6f6d 2066 756e  ine a custom fun
-00034a60: 6374 696f 6e20 7468 6174 2074 616b 6573  ction that takes
-00034a70: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-00034a80: 7473 0d0a 2020 2020 2020 2020 616e 6420  ts..        and 
-00034a90: 7061 7373 2074 6865 7365 2061 7267 756d  pass these argum
-00034aa0: 656e 7473 2074 6f20 6060 6170 706c 7960  ents to ``apply`
-00034ab0: 602e 0d0a 0d0a 2020 2020 2020 2020 3e3e  `.....        >>
-00034ac0: 3e20 6465 6620 6164 645f 6375 7374 6f6d  > def add_custom
-00034ad0: 5f76 616c 7565 7328 782c 202a 2a6b 7761  _values(x, **kwa
-00034ae0: 7267 7329 3a0d 0a20 2020 2020 2020 202e  rgs):..        .
-00034af0: 2e2e 2020 2020 2066 6f72 206d 6f6e 7468  ..     for month
-00034b00: 2069 6e20 6b77 6172 6773 3a0d 0a20 2020   in kwargs:..   
-00034b10: 2020 2020 202e 2e2e 2020 2020 2020 2020       ...        
-00034b20: 2078 2b3d 6b77 6172 6773 5b6d 6f6e 7468   x+=kwargs[month
-00034b30: 5d0d 0a20 2020 2020 2020 202e 2e2e 2020  ]..        ...  
-00034b40: 2020 2072 6574 7572 6e20 780d 0a20 2020     return x..   
-00034b50: 2020 2020 203e 3e3e 2066 612e 6170 706c       >>> fa.appl
-00034b60: 7928 6164 645f 6375 7374 6f6d 5f76 616c  y(add_custom_val
-00034b70: 7565 732c 206a 756e 653d 3330 2c20 6a75  ues, june=30, ju
-00034b80: 6c79 3d32 302c 2061 7567 7573 743d 3235  ly=20, august=25
-00034b90: 290d 0a20 2020 2020 2020 204c 6f6e 646f  )..        Londo
-00034ba0: 6e20 2020 2020 2039 350d 0a20 2020 2020  n      95..     
-00034bb0: 2020 204e 6577 2059 6f72 6b20 2020 2039     New York    9
-00034bc0: 360d 0a20 2020 2020 2020 2048 656c 7369  6..        Helsi
-00034bd0: 6e6b 6920 2020 2038 370d 0a20 2020 2020  nki    87..     
-00034be0: 2020 2064 7479 7065 3a20 696e 7436 340d     dtype: int64.
-00034bf0: 0a0d 0a20 2020 2020 2020 2055 7365 2061  ...        Use a
-00034c00: 2066 756e 6374 696f 6e20 6672 6f6d 2074   function from t
-00034c10: 6865 204e 756d 7079 206c 6962 7261 7279  he Numpy library
-00034c20: 2e0d 0a0d 0a20 2020 2020 2020 203e 3e3e  .....        >>>
-00034c30: 2066 612e 6170 706c 7928 6e70 2e6c 6f67   fa.apply(np.log
-00034c40: 290d 0a20 2020 2020 2020 204c 6f6e 646f  )..        Londo
-00034c50: 6e20 2020 2020 2032 2e39 3935 3733 320d  n      2.995732.
-00034c60: 0a20 2020 2020 2020 204e 6577 2059 6f72  .        New Yor
-00034c70: 6b20 2020 2033 2e30 3434 3532 320d 0a20  k    3.044522.. 
-00034c80: 2020 2020 2020 2048 656c 7369 6e6b 6920         Helsinki 
-00034c90: 2020 2032 2e34 3834 3930 370d 0a20 2020     2.484907..   
-00034ca0: 2020 2020 2064 7479 7065 3a20 666c 6f61       dtype: floa
-00034cb0: 7436 340d 0a20 2020 2020 2020 2022 2222  t64..        """
-00034cc0: 0d0a 2020 2020 2020 2020 696d 706f 7274  ..        import
-00034cd0: 2070 616e 6461 7320 6173 2070 640d 0a0d   pandas as pd...
-00034ce0: 0a20 2020 2020 2020 2073 6572 6965 7320  .        series 
-00034cf0: 3d20 7064 2e53 6572 6965 7328 7365 6c66  = pd.Series(self
-00034d00: 290d 0a20 2020 2020 2020 2072 6573 756c  )..        resul
-00034d10: 7420 3d20 7365 7269 6573 2e61 7070 6c79  t = series.apply
-00034d20: 2866 756e 632c 2063 6f6e 7665 7274 5f64  (func, convert_d
-00034d30: 7479 7065 3d63 6f6e 7665 7274 5f64 7479  type=convert_dty
-00034d40: 7065 2c20 6172 6773 3d61 7267 732c 202a  pe, args=args, *
-00034d50: 2a6b 7764 7329 0d0a 2020 2020 2020 2020  *kwds)..        
-00034d60: 7265 7475 726e 2072 6573 756c 742e 7661  return result.va
-00034d70: 6c75 6573 0d0a 0d0a 2020 2020 2320 2d2d  lues....    # --
+00034160: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 6465  --------..    de
+00034170: 6620 6170 706c 795f 7061 6e64 6173 2873  f apply_pandas(s
+00034180: 656c 662c 2066 756e 632c 2063 6f6e 7665  elf, func, conve
+00034190: 7274 5f64 7479 7065 3d54 7275 652c 2061  rt_dtype=True, a
+000341a0: 7267 733d 2829 2c20 2a2a 6b77 6473 293a  rgs=(), **kwds):
+000341b0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000341c0: 2020 2020 2020 2049 6e76 6f6b 6520 6675         Invoke fu
+000341d0: 6e63 7469 6f6e 206f 6e20 7661 6c75 6573  nction on values
+000341e0: 206f 6620 4661 7374 4172 7261 792e 2043   of FastArray. C
+000341f0: 616e 2062 6520 7566 756e 6320 2861 204e  an be ufunc (a N
+00034200: 756d 5079 2066 756e 6374 696f 6e0d 0a20  umPy function.. 
+00034210: 2020 2020 2020 2074 6861 7420 6170 706c         that appl
+00034220: 6965 7320 746f 2074 6865 2065 6e74 6972  ies to the entir
+00034230: 6520 4661 7374 4172 7261 7929 206f 7220  e FastArray) or 
+00034240: 6120 5079 7468 6f6e 2066 756e 6374 696f  a Python functio
+00034250: 6e20 7468 6174 206f 6e6c 7920 776f 726b  n that only work
+00034260: 730d 0a20 2020 2020 2020 206f 6e20 7369  s..        on si
+00034270: 6e67 6c65 2076 616c 7565 730d 0a0d 0a20  ngle values.... 
+00034280: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00034290: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+000342a0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2066  -----..        f
+000342b0: 756e 6320 3a20 6675 6e63 7469 6f6e 0d0a  unc : function..
+000342c0: 2020 2020 2020 2020 636f 6e76 6572 745f          convert_
+000342d0: 6474 7970 6520 3a20 626f 6f6c 6561 6e2c  dtype : boolean,
+000342e0: 2064 6566 6175 6c74 2054 7275 650d 0a20   default True.. 
+000342f0: 2020 2020 2020 2020 2020 2054 7279 2074             Try t
+00034300: 6f20 6669 6e64 2062 6574 7465 7220 6474  o find better dt
+00034310: 7970 6520 666f 7220 656c 656d 656e 7477  ype for elementw
+00034320: 6973 6520 6675 6e63 7469 6f6e 2072 6573  ise function res
+00034330: 756c 7473 2e20 4966 0d0a 2020 2020 2020  ults. If..      
+00034340: 2020 2020 2020 4661 6c73 652c 206c 6561        False, lea
+00034350: 7665 2061 7320 6474 7970 653d 6f62 6a65  ve as dtype=obje
+00034360: 6374 0d0a 2020 2020 2020 2020 6172 6773  ct..        args
+00034370: 203a 2074 7570 6c65 0d0a 2020 2020 2020   : tuple..      
+00034380: 2020 2020 2020 506f 7369 7469 6f6e 616c        Positional
+00034390: 2061 7267 756d 656e 7473 2074 6f20 7061   arguments to pa
+000343a0: 7373 2074 6f20 6675 6e63 7469 6f6e 2069  ss to function i
+000343b0: 6e20 6164 6469 7469 6f6e 2074 6f20 7468  n addition to th
+000343c0: 6520 7661 6c75 650d 0a20 2020 2020 2020  e value..       
+000343d0: 2041 6464 6974 696f 6e61 6c20 6b65 7977   Additional keyw
+000343e0: 6f72 6420 6172 6775 6d65 6e74 7320 7769  ord arguments wi
+000343f0: 6c6c 2062 6520 7061 7373 6564 2061 7320  ll be passed as 
+00034400: 6b65 7977 6f72 6473 2074 6f20 7468 6520  keywords to the 
+00034410: 6675 6e63 7469 6f6e 0d0a 0d0a 2020 2020  function....    
+00034420: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
+00034430: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
+00034440: 2020 2020 2020 7920 3a20 4661 7374 4172        y : FastAr
+00034450: 7261 7920 6f72 2044 6174 6173 6574 2069  ray or Dataset i
+00034460: 6620 6675 6e63 2072 6574 7572 6e73 2061  f func returns a
+00034470: 2046 6173 7441 7272 6179 0d0a 0d0a 2020   FastArray....  
+00034480: 2020 2020 2020 5365 6520 416c 736f 0d0a        See Also..
+00034490: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000344a0: 0d0a 2020 2020 2020 2020 4661 7374 4172  ..        FastAr
+000344b0: 7261 792e 6d61 703a 2046 6f72 2065 6c65  ray.map: For ele
+000344c0: 6d65 6e74 2d77 6973 6520 6f70 6572 6174  ment-wise operat
+000344d0: 696f 6e73 0d0a 2020 2020 2020 2020 4661  ions..        Fa
+000344e0: 7374 4172 7261 792e 6167 673a 206f 6e6c  stArray.agg: onl
+000344f0: 7920 7065 7266 6f72 6d20 6167 6772 6567  y perform aggreg
+00034500: 6174 696e 6720 7479 7065 206f 7065 7261  ating type opera
+00034510: 7469 6f6e 730d 0a20 2020 2020 2020 2046  tions..        F
+00034520: 6173 7441 7272 6179 2e74 7261 6e73 666f  astArray.transfo
+00034530: 726d 3a20 6f6e 6c79 2070 6572 666f 726d  rm: only perform
+00034540: 2074 7261 6e73 666f 726d 696e 6720 7479   transforming ty
+00034550: 7065 206f 7065 7261 7469 6f6e 730d 0a0d  pe operations...
+00034560: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+00034570: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+00034580: 2d2d 2d0d 0a20 2020 2020 2020 2043 7265  ---..        Cre
+00034590: 6174 6520 6120 4661 7374 4172 7261 7920  ate a FastArray 
+000345a0: 7769 7468 2074 7970 6963 616c 2073 756d  with typical sum
+000345b0: 6d65 7220 7465 6d70 6572 6174 7572 6573  mer temperatures
+000345c0: 2066 6f72 2065 6163 6820 6369 7479 2e0d   for each city..
+000345d0: 0a0d 0a20 2020 2020 2020 203e 3e3e 2066  ...        >>> f
+000345e0: 6120 3d20 7274 2e46 6173 7441 7272 6179  a = rt.FastArray
+000345f0: 285b 3230 2c20 3231 2c20 3132 5d2c 2069  ([20, 21, 12], i
+00034600: 6e64 6578 3d5b 274c 6f6e 646f 6e27 2c20  ndex=['London', 
+00034610: 274e 6577 2059 6f72 6b27 2c27 4865 6c73  'New York','Hels
+00034620: 696e 6b69 275d 290d 0a20 2020 2020 2020  inki'])..       
+00034630: 203e 3e3e 2066 610d 0a20 2020 2020 2020   >>> fa..       
+00034640: 204c 6f6e 646f 6e20 2020 2020 2032 300d   London      20.
+00034650: 0a20 2020 2020 2020 204e 6577 2059 6f72  .        New Yor
+00034660: 6b20 2020 2032 310d 0a20 2020 2020 2020  k    21..       
+00034670: 2048 656c 7369 6e6b 6920 2020 2031 320d   Helsinki    12.
+00034680: 0a20 2020 2020 2020 2064 7479 7065 3a20  .        dtype: 
+00034690: 696e 7436 340d 0a0d 0a20 2020 2020 2020  int64....       
+000346a0: 2053 7175 6172 6520 7468 6520 7661 6c75   Square the valu
+000346b0: 6573 2062 7920 6465 6669 6e69 6e67 2061  es by defining a
+000346c0: 2066 756e 6374 696f 6e20 616e 6420 7061   function and pa
+000346d0: 7373 696e 6720 6974 2061 7320 616e 0d0a  ssing it as an..
+000346e0: 2020 2020 2020 2020 6172 6775 6d65 6e74          argument
+000346f0: 2074 6f20 6060 6170 706c 7928 2960 602e   to ``apply()``.
+00034700: 0d0a 0d0a 2020 2020 2020 2020 3e3e 3e20  ....        >>> 
+00034710: 6465 6620 7371 7561 7265 2878 293a 0d0a  def square(x):..
+00034720: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+00034730: 7265 7475 726e 2078 2a2a 320d 0a20 2020  return x**2..   
+00034740: 2020 2020 203e 3e3e 2066 612e 6170 706c       >>> fa.appl
+00034750: 7928 7371 7561 7265 290d 0a20 2020 2020  y(square)..     
+00034760: 2020 204c 6f6e 646f 6e20 2020 2020 2034     London      4
+00034770: 3030 0d0a 2020 2020 2020 2020 4e65 7720  00..        New 
+00034780: 596f 726b 2020 2020 3434 310d 0a20 2020  York    441..   
+00034790: 2020 2020 2048 656c 7369 6e6b 6920 2020       Helsinki   
+000347a0: 2031 3434 0d0a 2020 2020 2020 2020 6474   144..        dt
+000347b0: 7970 653a 2069 6e74 3634 0d0a 0d0a 2020  ype: int64....  
+000347c0: 2020 2020 2020 5371 7561 7265 2074 6865        Square the
+000347d0: 2076 616c 7565 7320 6279 2070 6173 7369   values by passi
+000347e0: 6e67 2061 6e20 616e 6f6e 796d 6f75 7320  ng an anonymous 
+000347f0: 6675 6e63 7469 6f6e 2061 7320 616e 0d0a  function as an..
+00034800: 2020 2020 2020 2020 6172 6775 6d65 6e74          argument
+00034810: 2074 6f20 6060 6170 706c 7928 2960 602e   to ``apply()``.
+00034820: 0d0a 0d0a 2020 2020 2020 2020 3e3e 3e20  ....        >>> 
+00034830: 6661 2e61 7070 6c79 286c 616d 6264 6120  fa.apply(lambda 
+00034840: 783a 2078 2a2a 3229 0d0a 2020 2020 2020  x: x**2)..      
+00034850: 2020 4c6f 6e64 6f6e 2020 2020 2020 3430    London      40
+00034860: 300d 0a20 2020 2020 2020 204e 6577 2059  0..        New Y
+00034870: 6f72 6b20 2020 2034 3431 0d0a 2020 2020  ork    441..    
+00034880: 2020 2020 4865 6c73 696e 6b69 2020 2020      Helsinki    
+00034890: 3134 340d 0a20 2020 2020 2020 2064 7479  144..        dty
+000348a0: 7065 3a20 696e 7436 340d 0a0d 0a20 2020  pe: int64....   
+000348b0: 2020 2020 2044 6566 696e 6520 6120 6375       Define a cu
+000348c0: 7374 6f6d 2066 756e 6374 696f 6e20 7468  stom function th
+000348d0: 6174 206e 6565 6473 2061 6464 6974 696f  at needs additio
+000348e0: 6e61 6c20 706f 7369 7469 6f6e 616c 0d0a  nal positional..
+000348f0: 2020 2020 2020 2020 6172 6775 6d65 6e74          argument
+00034900: 7320 616e 6420 7061 7373 2074 6865 7365  s and pass these
+00034910: 2061 6464 6974 696f 6e61 6c20 6172 6775   additional argu
+00034920: 6d65 6e74 7320 7573 696e 6720 7468 650d  ments using the.
+00034930: 0a20 2020 2020 2020 2060 6061 7267 7360  .        ``args`
+00034940: 6020 6b65 7977 6f72 642e 0d0a 0d0a 2020  ` keyword.....  
+00034950: 2020 2020 2020 3e3e 3e20 6465 6620 7375        >>> def su
+00034960: 6274 7261 6374 5f63 7573 746f 6d5f 7661  btract_custom_va
+00034970: 6c75 6528 782c 2063 7573 746f 6d5f 7661  lue(x, custom_va
+00034980: 6c75 6529 3a0d 0a20 2020 2020 2020 202e  lue):..        .
+00034990: 2e2e 2020 2020 2072 6574 7572 6e20 782d  ..     return x-
+000349a0: 6375 7374 6f6d 5f76 616c 7565 0d0a 2020  custom_value..  
+000349b0: 2020 2020 2020 3e3e 3e20 6661 2e61 7070        >>> fa.app
+000349c0: 6c79 2873 7562 7472 6163 745f 6375 7374  ly(subtract_cust
+000349d0: 6f6d 5f76 616c 7565 2c20 6172 6773 3d28  om_value, args=(
+000349e0: 352c 2929 0d0a 2020 2020 2020 2020 4c6f  5,))..        Lo
+000349f0: 6e64 6f6e 2020 2020 2020 3135 0d0a 2020  ndon      15..  
+00034a00: 2020 2020 2020 4e65 7720 596f 726b 2020        New York  
+00034a10: 2020 3136 0d0a 2020 2020 2020 2020 4865    16..        He
+00034a20: 6c73 696e 6b69 2020 2020 2037 0d0a 2020  lsinki     7..  
+00034a30: 2020 2020 2020 6474 7970 653a 2069 6e74        dtype: int
+00034a40: 3634 0d0a 0d0a 2020 2020 2020 2020 4465  64....        De
+00034a50: 6669 6e65 2061 2063 7573 746f 6d20 6675  fine a custom fu
+00034a60: 6e63 7469 6f6e 2074 6861 7420 7461 6b65  nction that take
+00034a70: 7320 6b65 7977 6f72 6420 6172 6775 6d65  s keyword argume
+00034a80: 6e74 730d 0a20 2020 2020 2020 2061 6e64  nts..        and
+00034a90: 2070 6173 7320 7468 6573 6520 6172 6775   pass these argu
+00034aa0: 6d65 6e74 7320 746f 2060 6061 7070 6c79  ments to ``apply
+00034ab0: 6060 2e0d 0a0d 0a20 2020 2020 2020 203e  ``.....        >
+00034ac0: 3e3e 2064 6566 2061 6464 5f63 7573 746f  >> def add_custo
+00034ad0: 6d5f 7661 6c75 6573 2878 2c20 2a2a 6b77  m_values(x, **kw
+00034ae0: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+00034af0: 2e2e 2e20 2020 2020 666f 7220 6d6f 6e74  ...     for mont
+00034b00: 6820 696e 206b 7761 7267 733a 0d0a 2020  h in kwargs:..  
+00034b10: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
+00034b20: 2020 782b 3d6b 7761 7267 735b 6d6f 6e74    x+=kwargs[mont
+00034b30: 685d 0d0a 2020 2020 2020 2020 2e2e 2e20  h]..        ... 
+00034b40: 2020 2020 7265 7475 726e 2078 0d0a 2020      return x..  
+00034b50: 2020 2020 2020 3e3e 3e20 6661 2e61 7070        >>> fa.app
+00034b60: 6c79 2861 6464 5f63 7573 746f 6d5f 7661  ly(add_custom_va
+00034b70: 6c75 6573 2c20 6a75 6e65 3d33 302c 206a  lues, june=30, j
+00034b80: 756c 793d 3230 2c20 6175 6775 7374 3d32  uly=20, august=2
+00034b90: 3529 0d0a 2020 2020 2020 2020 4c6f 6e64  5)..        Lond
+00034ba0: 6f6e 2020 2020 2020 3935 0d0a 2020 2020  on      95..    
+00034bb0: 2020 2020 4e65 7720 596f 726b 2020 2020      New York    
+00034bc0: 3936 0d0a 2020 2020 2020 2020 4865 6c73  96..        Hels
+00034bd0: 696e 6b69 2020 2020 3837 0d0a 2020 2020  inki    87..    
+00034be0: 2020 2020 6474 7970 653a 2069 6e74 3634      dtype: int64
+00034bf0: 0d0a 0d0a 2020 2020 2020 2020 5573 6520  ....        Use 
+00034c00: 6120 6675 6e63 7469 6f6e 2066 726f 6d20  a function from 
+00034c10: 7468 6520 4e75 6d70 7920 6c69 6272 6172  the Numpy librar
+00034c20: 792e 0d0a 0d0a 2020 2020 2020 2020 3e3e  y.....        >>
+00034c30: 3e20 6661 2e61 7070 6c79 286e 702e 6c6f  > fa.apply(np.lo
+00034c40: 6729 0d0a 2020 2020 2020 2020 4c6f 6e64  g)..        Lond
+00034c50: 6f6e 2020 2020 2020 322e 3939 3537 3332  on      2.995732
+00034c60: 0d0a 2020 2020 2020 2020 4e65 7720 596f  ..        New Yo
+00034c70: 726b 2020 2020 332e 3034 3435 3232 0d0a  rk    3.044522..
+00034c80: 2020 2020 2020 2020 4865 6c73 696e 6b69          Helsinki
+00034c90: 2020 2020 322e 3438 3439 3037 0d0a 2020      2.484907..  
+00034ca0: 2020 2020 2020 6474 7970 653a 2066 6c6f        dtype: flo
+00034cb0: 6174 3634 0d0a 2020 2020 2020 2020 2222  at64..        ""
+00034cc0: 220d 0a20 2020 2020 2020 2069 6d70 6f72  "..        impor
+00034cd0: 7420 7061 6e64 6173 2061 7320 7064 0d0a  t pandas as pd..
+00034ce0: 0d0a 2020 2020 2020 2020 7365 7269 6573  ..        series
+00034cf0: 203d 2070 642e 5365 7269 6573 2873 656c   = pd.Series(sel
+00034d00: 6629 0d0a 2020 2020 2020 2020 7265 7375  f)..        resu
+00034d10: 6c74 203d 2073 6572 6965 732e 6170 706c  lt = series.appl
+00034d20: 7928 6675 6e63 2c20 636f 6e76 6572 745f  y(func, convert_
+00034d30: 6474 7970 653d 636f 6e76 6572 745f 6474  dtype=convert_dt
+00034d40: 7970 652c 2061 7267 733d 6172 6773 2c20  ype, args=args, 
+00034d50: 2a2a 6b77 6473 290d 0a20 2020 2020 2020  **kwds)..       
+00034d60: 2072 6574 7572 6e20 7265 7375 6c74 2e76   return result.v
+00034d70: 616c 7565 730d 0a0d 0a20 2020 2023 202d  alues....    # -
 00034d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00034db0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2040  ---------..    @
-00034dc0: 6361 6368 6564 5f77 6561 6b72 6566 5f70  cached_weakref_p
-00034dd0: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
-00034de0: 2073 7472 2873 656c 6629 202d 3e20 2246   str(self) -> "F
-00034df0: 4153 7472 696e 6722 3a0d 0a20 2020 2020  AString":..     
-00034e00: 2020 2072 2222 2243 6173 7473 2061 6e20     r"""Casts an 
-00034e10: 6172 7261 7920 6f66 2062 7974 6520 7374  array of byte st
-00034e20: 7269 6e67 7320 6f72 2075 6e69 636f 6465  rings or unicode
-00034e30: 2061 7320 6060 4641 5374 7269 6e67 6060   as ``FAString``
-00034e40: 2e0d 0a0d 0a20 2020 2020 2020 2045 6e61  .....        Ena
-00034e50: 626c 6573 2061 2076 6172 6965 7479 206f  bles a variety o
-00034e60: 6620 7573 6566 756c 2073 7472 696e 6720  f useful string 
-00034e70: 6d61 6e69 7075 6c61 7469 6f6e 206d 6574  manipulation met
-00034e80: 686f 6473 2e0d 0a0d 0a20 2020 2020 2020  hods.....       
-00034e90: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-00034ea0: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-00034eb0: 2020 2046 4153 7472 696e 670d 0a0d 0a20     FAString.... 
-00034ec0: 2020 2020 2020 2052 6169 7365 730d 0a20         Raises.. 
-00034ed0: 2020 2020 2020 202d 2d2d 2d2d 2d0d 0a20         ------.. 
-00034ee0: 2020 2020 2020 2054 7970 6545 7272 6f72         TypeError
-00034ef0: 0d0a 2020 2020 2020 2020 2020 2020 4966  ..            If
-00034f00: 2074 6865 2046 6173 7441 7272 6179 2069   the FastArray i
-00034f10: 7320 6f66 2064 7479 7065 206f 7468 6572  s of dtype other
-00034f20: 2074 6861 6e20 6279 7465 2073 7472 696e   than byte strin
-00034f30: 6720 6f72 2075 6e69 636f 6465 0d0a 0d0a  g or unicode....
-00034f40: 2020 2020 2020 2020 5365 6520 416c 736f          See Also
-00034f50: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00034f60: 2d2d 0d0a 2020 2020 2020 2020 6e70 2e63  --..        np.c
-00034f70: 6861 7261 7272 6179 0d0a 2020 2020 2020  hararray..      
-00034f80: 2020 6e70 2e63 6861 720d 0a20 2020 2020    np.char..     
-00034f90: 2020 2072 742e 4641 5374 7269 6e67 2e61     rt.FAString.a
-00034fa0: 7070 6c79 0d0a 0d0a 2020 2020 2020 2020  pply....        
-00034fb0: 4578 616d 706c 6573 0d0a 2020 2020 2020  Examples..      
-00034fc0: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
-00034fd0: 2020 2020 3e3e 3e20 733d 4641 285b 2774      >>> s=FA(['t
-00034fe0: 6869 7327 2c27 7468 6174 272c 2774 6573  his','that','tes
-00034ff0: 7420 275d 2a31 3030 5f30 3030 290d 0a20  t ']*100_000).. 
-00035000: 2020 2020 2020 203e 3e3e 2073 2e73 7472         >>> s.str
-00035010: 2e75 7070 6572 0d0a 2020 2020 2020 2020  .upper..        
-00035020: 4661 7374 4172 7261 7928 5b62 2754 4849  FastArray([b'THI
-00035030: 5327 2c20 6227 5448 4154 272c 2062 2754  S', b'THAT', b'T
-00035040: 4553 5420 272c 202e 2e2e 2c20 6227 5448  EST ', ..., b'TH
-00035050: 4953 272c 2062 2754 4841 5427 2c20 6227  IS', b'THAT', b'
-00035060: 5445 5354 2027 5d2c 0d0a 2020 2020 2020  TEST '],..      
-00035070: 2020 2020 2020 2020 2020 2020 6474 7970              dtyp
-00035080: 653d 277c 5335 2729 0d0a 0d0a 2020 2020  e='|S5')....    
-00035090: 2020 2020 3e3e 3e20 732e 7374 722e 6c6f      >>> s.str.lo
-000350a0: 7765 720d 0a20 2020 2020 2020 2046 6173  wer..        Fas
-000350b0: 7441 7272 6179 285b 6227 7468 6973 272c  tArray([b'this',
-000350c0: 2062 2774 6861 7427 2c20 6227 7465 7374   b'that', b'test
-000350d0: 2027 2c20 2e2e 2e2c 2062 2774 6869 7327   ', ..., b'this'
-000350e0: 2c20 6227 7468 6174 272c 2062 2774 6573  , b'that', b'tes
-000350f0: 7420 275d 2c0d 0a20 2020 2020 2020 2020  t '],..         
-00035100: 2020 2020 2020 2020 2064 7479 7065 3d27           dtype='
-00035110: 7c53 3527 290d 0a0d 0a20 2020 2020 2020  |S5')....       
-00035120: 203e 3e3e 2073 2e73 7472 2e72 656d 6f76   >>> s.str.remov
-00035130: 6574 7261 696c 696e 6728 290d 0a20 2020  etrailing()..   
-00035140: 2020 2020 2046 6173 7441 7272 6179 285b       FastArray([
-00035150: 6227 7468 6973 272c 2062 2774 6861 7427  b'this', b'that'
-00035160: 2c20 6227 7465 7374 272c 202e 2e2e 2c20  , b'test', ..., 
-00035170: 6227 7468 6973 272c 2062 2774 6861 7427  b'this', b'that'
-00035180: 2c20 6227 7465 7374 275d 2c0d 0a20 2020  , b'test'],..   
-00035190: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000351a0: 7479 7065 3d27 7c53 3527 290d 0a20 2020  type='|S5')..   
-000351b0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000351c0: 2020 6966 2073 656c 662e 6474 7970 652e    if self.dtype.
-000351d0: 6368 6172 2069 6e20 2255 5322 3a0d 0a20  char in "US":.. 
-000351e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000351f0: 6e20 5479 7065 5265 6769 7374 6572 2e46  n TypeRegister.F
-00035200: 4153 7472 696e 6728 7365 6c66 290d 0a20  AString(self).. 
-00035210: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00035220: 7479 7065 2e63 6861 7220 3d3d 2022 4f22  type.char == "O"
-00035230: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-00035240: 2074 7279 2074 6f20 636f 6e76 6572 7420   try to convert 
-00035250: 746f 2073 7472 696e 6720 286d 6967 6874  to string (might
-00035260: 2068 6176 6520 636f 6d65 2066 726f 6d20   have come from 
-00035270: 7061 6e64 6173 290d 0a20 2020 2020 2020  pandas)..       
-00035280: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00035290: 2020 2020 2020 2020 2020 2063 6f6e 7620             conv 
-000352a0: 3d20 7365 6c66 2e61 7374 7970 6528 2253  = self.astype("S
-000352b0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-000352c0: 6578 6365 7074 3a0d 0a20 2020 2020 2020  except:..       
-000352d0: 2020 2020 2020 2020 2063 6f6e 7620 3d20           conv = 
-000352e0: 7365 6c66 2e61 7374 7970 6528 2255 2229  self.astype("U")
-000352f0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00035300: 7475 726e 2054 7970 6552 6567 6973 7465  turn TypeRegiste
-00035310: 722e 4641 5374 7269 6e67 2863 6f6e 7629  r.FAString(conv)
-00035320: 0d0a 0d0a 2020 2020 2020 2020 7261 6973  ....        rais
-00035330: 6520 5479 7065 4572 726f 7228 6622 5468  e TypeError(f"Th
-00035340: 6520 2e73 7472 2066 756e 6374 696f 6e20  e .str function 
-00035350: 6361 6e20 6f6e 6c79 2062 6520 7573 6564  can only be used
-00035360: 206f 6e20 6279 7465 2073 7472 696e 6720   on byte string 
-00035370: 616e 6420 756e 6963 6f64 6520 6e6f 7420  and unicode not 
-00035380: 7b73 656c 662e 6474 7970 6521 727d 2229  {self.dtype!r}")
-00035390: 0d0a 0d0a 2020 2020 4073 7461 7469 636d  ....    @staticm
-000353a0: 6574 686f 640d 0a20 2020 2064 6566 2066  ethod..    def f
-000353b0: 726f 6d5f 6172 726f 7728 0d0a 2020 2020  rom_arrow(..    
-000353c0: 2020 2020 6172 723a 2055 6e69 6f6e 5b22      arr: Union["
-000353d0: 7061 2e41 7272 6179 222c 2022 7061 2e43  pa.Array", "pa.C
-000353e0: 6875 6e6b 6564 4172 7261 7922 5d2c 0d0a  hunkedArray"],..
-000353f0: 2020 2020 2020 2020 7a65 726f 5f63 6f70          zero_cop
-00035400: 795f 6f6e 6c79 3a20 626f 6f6c 203d 2054  y_only: bool = T
-00035410: 7275 652c 0d0a 2020 2020 2020 2020 7772  rue,..        wr
-00035420: 6974 6162 6c65 3a20 626f 6f6c 203d 2046  itable: bool = F
-00035430: 616c 7365 2c0d 0a20 2020 2020 2020 2061  alse,..        a
-00035440: 7574 6f5f 7769 6465 6e3a 2062 6f6f 6c20  uto_widen: bool 
-00035450: 3d20 4661 6c73 652c 0d0a 2020 2020 2920  = False,..    ) 
-00035460: 2d3e 2022 4661 7374 4172 7261 7922 3a0d  -> "FastArray":.
-00035470: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00035480: 2020 2020 2020 436f 6e76 6572 7420 6120        Convert a 
-00035490: 7079 6172 726f 7720 6041 7272 6179 6020  pyarrow `Array` 
-000354a0: 746f 2061 2072 6970 7461 626c 6520 6046  to a riptable `F
-000354b0: 6173 7441 7272 6179 602e 0d0a 0d0a 2020  astArray`.....  
-000354c0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-000354d0: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-000354e0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6172  ----..        ar
-000354f0: 7220 3a20 7079 6172 726f 772e 4172 7261  r : pyarrow.Arra
-00035500: 7920 6f72 2070 7961 7272 6f77 2e43 6875  y or pyarrow.Chu
-00035510: 6e6b 6564 4172 7261 790d 0a20 2020 2020  nkedArray..     
-00035520: 2020 207a 6572 6f5f 636f 7079 5f6f 6e6c     zero_copy_onl
-00035530: 7920 3a20 626f 6f6c 2c20 6465 6661 756c  y : bool, defaul
-00035540: 7420 5472 7565 0d0a 2020 2020 2020 2020  t True..        
-00035550: 2020 2020 4966 2054 7275 652c 2061 6e20      If True, an 
-00035560: 6578 6365 7074 696f 6e20 7769 6c6c 2062  exception will b
-00035570: 6520 7261 6973 6564 2069 6620 7468 6520  e raised if the 
-00035580: 636f 6e76 6572 7369 6f6e 2074 6f20 6120  conversion to a 
-00035590: 6046 6173 7441 7272 6179 6020 776f 756c  `FastArray` woul
-000355a0: 6420 7265 7175 6972 6520 636f 7079 696e  d require copyin
-000355b0: 6720 7468 650d 0a20 2020 2020 2020 2020  g the..         
-000355c0: 2020 2075 6e64 6572 6c79 696e 6720 6461     underlying da
-000355d0: 7461 2028 652e 672e 2069 6e20 7072 6573  ta (e.g. in pres
-000355e0: 656e 6365 206f 6620 6e75 6c6c 732c 206f  ence of nulls, o
-000355f0: 7220 666f 7220 6e6f 6e2d 7072 696d 6974  r for non-primit
-00035600: 6976 6520 7479 7065 7329 2e0d 0a20 2020  ive types)...   
-00035610: 2020 2020 2077 7269 7461 626c 6520 3a20       writable : 
-00035620: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-00035630: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-00035640: 2046 6f72 2061 2060 4661 7374 4172 7261   For a `FastArra
-00035650: 7960 2063 7265 6174 6564 2077 6974 6820  y` created with 
-00035660: 7a65 726f 2063 6f70 7920 2876 6965 7720  zero copy (view 
-00035670: 6f6e 2074 6865 2041 7272 6f77 2064 6174  on the Arrow dat
-00035680: 6129 2c20 7468 6520 7265 7375 6c74 696e  a), the resultin
-00035690: 6720 6172 7261 7920 6973 206e 6f74 2077  g array is not w
-000356a0: 7269 7461 626c 6520 2841 7272 6f77 2064  ritable (Arrow d
-000356b0: 6174 6120 6973 2069 6d6d 7574 6162 6c65  ata is immutable
-000356c0: 292e 0d0a 2020 2020 2020 2020 2020 2020  )...            
-000356d0: 4279 2073 6574 7469 6e67 2074 6869 7320  By setting this 
-000356e0: 746f 2054 7275 652c 2061 2063 6f70 7920  to True, a copy 
-000356f0: 6f66 2074 6865 2061 7272 6179 2069 7320  of the array is 
-00035700: 6d61 6465 2074 6f20 656e 7375 7265 2069  made to ensure i
-00035710: 7420 6973 2077 7269 7461 626c 652e 0d0a  t is writable...
-00035720: 2020 2020 2020 2020 6175 746f 5f77 6964          auto_wid
-00035730: 656e 203a 2062 6f6f 6c2c 206f 7074 696f  en : bool, optio
-00035740: 6e61 6c2c 2064 6566 6175 6c74 2074 6f20  nal, default to 
-00035750: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-00035760: 2020 2057 6865 6e20 4661 6c73 6520 2874     When False (t
-00035770: 6865 2064 6566 6175 6c74 292c 2069 6620  he default), if 
-00035780: 616e 2061 7272 6f77 2061 7272 6179 2063  an arrow array c
-00035790: 6f6e 7461 696e 7320 6120 7661 6c75 6520  ontains a value 
-000357a0: 7768 6963 6820 776f 756c 6420 6265 2063  which would be c
-000357b0: 6f6e 7369 6465 7265 640d 0a20 2020 2020  onsidered..     
-000357c0: 2020 2020 2020 2074 6865 2027 696e 7661         the 'inva
-000357d0: 6c69 6427 2f4e 4120 7661 6c75 6520 666f  lid'/NA value fo
-000357e0: 7220 7468 6520 6571 7569 7661 6c65 6e74  r the equivalent
-000357f0: 2064 7479 7065 2069 6e20 6120 6046 6173   dtype in a `Fas
-00035800: 7441 7272 6179 602c 2072 6169 7365 2061  tArray`, raise a
-00035810: 6e20 6578 6365 7074 696f 6e0d 0a20 2020  n exception..   
-00035820: 2020 2020 2020 2020 2062 6563 6175 7365           because
-00035830: 2064 6972 6563 7420 636f 6e76 6572 7369   direct conversi
-00035840: 6f6e 2077 6f75 6c64 2062 6520 6c6f 7373  on would be loss
-00035850: 7920 2f20 6368 616e 6765 2074 6865 2073  y / change the s
-00035860: 656d 616e 7469 6320 6d65 616e 696e 6720  emantic meaning 
-00035870: 6f66 2074 6865 2064 6174 612e 0d0a 2020  of the data...  
-00035880: 2020 2020 2020 2020 2020 5768 656e 2054            When T
-00035890: 7275 652c 2074 6865 2063 6f6e 7665 7274  rue, the convert
-000358a0: 6564 2061 7272 6179 2077 696c 6c20 6265  ed array will be
-000358b0: 2077 6964 656e 6564 2028 6966 2070 6f73   widened (if pos
-000358c0: 7369 626c 6529 2074 6f20 7468 6520 6e65  sible) to the ne
-000358d0: 7874 2d6c 6172 6765 7374 2064 7479 7065  xt-largest dtype
-000358e0: 0d0a 2020 2020 2020 2020 2020 2020 746f  ..            to
-000358f0: 2065 6e73 7572 6520 7468 6520 6461 7461   ensure the data
-00035900: 2077 696c 6c20 6265 2069 6e74 6572 7072   will be interpr
-00035910: 6574 6564 2069 6e20 7468 6520 7361 6d65  eted in the same
-00035920: 2077 6179 2e0d 0a0d 0a20 2020 2020 2020   way.....       
-00035930: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-00035940: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-00035950: 2020 2046 6173 7441 7272 6179 0d0a 2020     FastArray..  
-00035960: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00035970: 2020 2069 6d70 6f72 7420 7079 6172 726f     import pyarro
-00035980: 772e 7479 7065 7320 6173 2070 6174 0d0a  w.types as pat..
-00035990: 0d0a 2020 2020 2020 2020 2320 4261 7365  ..        # Base
-000359a0: 6420 6f6e 2074 6865 2074 7970 6520 6f66  d on the type of
-000359b0: 2074 6865 2061 7272 6179 2c20 6469 7370   the array, disp
-000359c0: 6174 6368 2074 6f20 7479 7065 2d73 7065  atch to type-spe
-000359d0: 6369 6669 6320 696d 706c 656d 656e 7461  cific implementa
-000359e0: 7469 6f6e 7320 6f66 202e 6672 6f6d 5f61  tions of .from_a
-000359f0: 7272 6f77 2829 2e0d 0a20 2020 2020 2020  rrow()...       
-00035a00: 2070 615f 6172 725f 7479 7065 203d 2061   pa_arr_type = a
-00035a10: 7272 2e74 7970 650d 0a20 2020 2020 2020  rr.type..       
-00035a20: 2069 6620 280d 0a20 2020 2020 2020 2020   if (..         
-00035a30: 2020 2070 6174 2e69 735f 626f 6f6c 6561     pat.is_boolea
-00035a40: 6e28 7061 5f61 7272 5f74 7970 6529 0d0a  n(pa_arr_type)..
-00035a50: 2020 2020 2020 2020 2020 2020 6f72 2070              or p
-00035a60: 6174 2e69 735f 696e 7465 6765 7228 7061  at.is_integer(pa
-00035a70: 5f61 7272 5f74 7970 6529 0d0a 2020 2020  _arr_type)..    
-00035a80: 2020 2020 2020 2020 6f72 2070 6174 2e69          or pat.i
-00035a90: 735f 666c 6f61 7469 6e67 2870 615f 6172  s_floating(pa_ar
-00035aa0: 725f 7479 7065 290d 0a20 2020 2020 2020  r_type)..       
-00035ab0: 2020 2020 206f 7220 7061 742e 6973 5f73       or pat.is_s
-00035ac0: 7472 696e 6728 7061 5f61 7272 5f74 7970  tring(pa_arr_typ
-00035ad0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00035ae0: 6f72 2070 6174 2e69 735f 6269 6e61 7279  or pat.is_binary
-00035af0: 2870 615f 6172 725f 7479 7065 290d 0a20  (pa_arr_type).. 
-00035b00: 2020 2020 2020 2020 2020 206f 7220 7061             or pa
-00035b10: 742e 6973 5f66 6978 6564 5f73 697a 655f  t.is_fixed_size_
-00035b20: 6269 6e61 7279 2870 615f 6172 725f 7479  binary(pa_arr_ty
-00035b30: 7065 290d 0a20 2020 2020 2020 2029 3a0d  pe)..        ):.
-00035b40: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-00035b50: 4f44 4f3a 2043 6865 636b 2077 6865 7468  ODO: Check wheth
-00035b60: 6572 2074 6869 7320 636f 6c75 6d6e 2068  er this column h
-00035b70: 6173 2061 2075 7365 722d 7370 6563 6966  as a user-specif
-00035b80: 6965 6420 6669 6c6c 2076 616c 7565 2070  ied fill value p
-00035b90: 726f 7669 6465 643b 2069 6620 736f 2c20  rovided; if so, 
-00035ba0: 7061 7373 2069 7420 616c 6f6e 6720 746f  pass it along to
-00035bb0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00035bc0: 2020 2020 2020 7468 6520 4661 7374 4172        the FastAr
-00035bd0: 7261 792e 6672 6f6d 5f61 7272 6f77 2829  ray.from_arrow()
-00035be0: 206d 6574 686f 6420 6361 6c6c 2062 656c   method call bel
-00035bf0: 6f77 2e0d 0a20 2020 2020 2020 2020 2020  ow...           
-00035c00: 2072 6574 7572 6e20 4661 7374 4172 7261   return FastArra
-00035c10: 792e 5f66 726f 6d5f 6172 726f 7728 6172  y._from_arrow(ar
-00035c20: 722c 207a 6572 6f5f 636f 7079 5f6f 6e6c  r, zero_copy_onl
-00035c30: 793d 7a65 726f 5f63 6f70 795f 6f6e 6c79  y=zero_copy_only
-00035c40: 2c20 7772 6974 6162 6c65 3d77 7269 7461  , writable=writa
-00035c50: 626c 652c 2061 7574 6f5f 7769 6465 6e3d  ble, auto_widen=
-00035c60: 6175 746f 5f77 6964 656e 290d 0a0d 0a20  auto_widen).... 
-00035c70: 2020 2020 2020 2065 6c69 6620 7061 742e         elif pat.
-00035c80: 6973 5f64 6963 7469 6f6e 6172 7928 7061  is_dictionary(pa
-00035c90: 5f61 7272 5f74 7970 6529 206f 7220 7061  _arr_type) or pa
-00035ca0: 742e 6973 5f73 7472 7563 7428 7061 5f61  t.is_struct(pa_a
-00035cb0: 7272 5f74 7970 6529 3a0d 0a20 2020 2020  rr_type):..     
-00035cc0: 2020 2020 2020 2072 6574 7572 6e20 5479         return Ty
-00035cd0: 7065 5265 6769 7374 6572 2e43 6174 6567  peRegister.Categ
-00035ce0: 6f72 6963 616c 2e5f 6672 6f6d 5f61 7272  orical._from_arr
-00035cf0: 6f77 2861 7272 2c20 7a65 726f 5f63 6f70  ow(arr, zero_cop
-00035d00: 795f 6f6e 6c79 3d7a 6572 6f5f 636f 7079  y_only=zero_copy
-00035d10: 5f6f 6e6c 792c 2077 7269 7461 626c 653d  _only, writable=
-00035d20: 7772 6974 6162 6c65 290d 0a0d 0a20 2020  writable)....   
-00035d30: 2020 2020 2065 6c69 6620 7061 742e 6973       elif pat.is
-00035d40: 5f74 696d 6573 7461 6d70 2870 615f 6172  _timestamp(pa_ar
-00035d50: 725f 7479 7065 293a 0d0a 2020 2020 2020  r_type):..      
-00035d60: 2020 2020 2020 7265 7475 726e 2054 7970        return Typ
-00035d70: 6552 6567 6973 7465 722e 4461 7465 5469  eRegister.DateTi
-00035d80: 6d65 4e61 6e6f 2e5f 6672 6f6d 5f61 7272  meNano._from_arr
-00035d90: 6f77 2861 7272 2c20 7a65 726f 5f63 6f70  ow(arr, zero_cop
-00035da0: 795f 6f6e 6c79 3d7a 6572 6f5f 636f 7079  y_only=zero_copy
-00035db0: 5f6f 6e6c 792c 2077 7269 7461 626c 653d  _only, writable=
-00035dc0: 7772 6974 6162 6c65 290d 0a0d 0a20 2020  writable)....   
-00035dd0: 2020 2020 2065 6c69 6620 7061 742e 6973       elif pat.is
-00035de0: 5f64 6174 6528 7061 5f61 7272 5f74 7970  _date(pa_arr_typ
-00035df0: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00035e00: 2072 6574 7572 6e20 5479 7065 5265 6769   return TypeRegi
-00035e10: 7374 6572 2e44 6174 652e 5f66 726f 6d5f  ster.Date._from_
-00035e20: 6172 726f 7728 6172 722c 207a 6572 6f5f  arrow(arr, zero_
-00035e30: 636f 7079 5f6f 6e6c 793d 7a65 726f 5f63  copy_only=zero_c
-00035e40: 6f70 795f 6f6e 6c79 2c20 7772 6974 6162  opy_only, writab
-00035e50: 6c65 3d77 7269 7461 626c 6529 0d0a 0d0a  le=writable)....
-00035e60: 2020 2020 2020 2020 656c 6966 2070 6174          elif pat
-00035e70: 2e69 735f 6475 7261 7469 6f6e 2870 615f  .is_duration(pa_
-00035e80: 6172 725f 7479 7065 293a 0d0a 2020 2020  arr_type):..    
-00035e90: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00035ea0: 7970 6552 6567 6973 7465 722e 5469 6d65  ypeRegister.Time
-00035eb0: 5370 616e 2e5f 6672 6f6d 5f61 7272 6f77  Span._from_arrow
-00035ec0: 2861 7272 2c20 7a65 726f 5f63 6f70 795f  (arr, zero_copy_
-00035ed0: 6f6e 6c79 3d7a 6572 6f5f 636f 7079 5f6f  only=zero_copy_o
-00035ee0: 6e6c 792c 2077 7269 7461 626c 653d 7772  nly, writable=wr
-00035ef0: 6974 6162 6c65 290d 0a0d 0a20 2020 2020  itable)....     
-00035f00: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00035f10: 2020 2020 2020 2320 556e 6b6e 6f77 6e2f        # Unknown/
-00035f20: 756e 7375 7070 6f72 7465 6420 6172 7261  unsupported arra
-00035f30: 7920 7479 7065 202d 2d20 6361 6e27 7420  y type -- can't 
-00035f40: 636f 6e76 6572 742e 0d0a 2020 2020 2020  convert...      
-00035f50: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
-00035f60: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
-00035f70: 6622 7079 6172 726f 7720 6172 7261 7973  f"pyarrow arrays
-00035f80: 206f 6620 7479 7065 2027 7b70 615f 6172   of type '{pa_ar
-00035f90: 725f 7479 7065 7d27 2063 616e 2774 2062  r_type}' can't b
-00035fa0: 6520 636f 6e76 6572 7465 6420 746f 2072  e converted to r
-00035fb0: 6970 7461 626c 6520 6172 7261 7973 2e22  iptable arrays."
-00035fc0: 290d 0a0d 0a20 2020 2040 7374 6174 6963  )....    @static
-00035fd0: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
-00035fe0: 5f66 726f 6d5f 6172 726f 7728 0d0a 2020  _from_arrow(..  
-00035ff0: 2020 2020 2020 6172 723a 2055 6e69 6f6e        arr: Union
-00036000: 5b22 7061 2e41 7272 6179 222c 2022 7061  ["pa.Array", "pa
-00036010: 2e43 6875 6e6b 6564 4172 7261 7922 5d2c  .ChunkedArray"],
-00036020: 0d0a 2020 2020 2020 2020 7a65 726f 5f63  ..        zero_c
-00036030: 6f70 795f 6f6e 6c79 3a20 626f 6f6c 203d  opy_only: bool =
-00036040: 2054 7275 652c 0d0a 2020 2020 2020 2020   True,..        
-00036050: 7772 6974 6162 6c65 3a20 626f 6f6c 203d  writable: bool =
-00036060: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
-00036070: 2061 7574 6f5f 7769 6465 6e3a 2062 6f6f   auto_widen: boo
-00036080: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
-00036090: 2920 2d3e 2022 4661 7374 4172 7261 7922  ) -> "FastArray"
-000360a0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-000360b0: 2020 2020 2020 2020 436f 6e76 6572 7420          Convert 
-000360c0: 6120 7079 6172 726f 7720 6041 7272 6179  a pyarrow `Array
-000360d0: 6020 746f 2061 2072 6970 7461 626c 6520  ` to a riptable 
-000360e0: 6046 6173 7441 7272 6179 602e 0d0a 0d0a  `FastArray`.....
-000360f0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00036100: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
-00036110: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-00036120: 6172 7220 3a20 7079 6172 726f 772e 4172  arr : pyarrow.Ar
-00036130: 7261 7920 6f72 2070 7961 7272 6f77 2e43  ray or pyarrow.C
-00036140: 6875 6e6b 6564 4172 7261 790d 0a20 2020  hunkedArray..   
-00036150: 2020 2020 207a 6572 6f5f 636f 7079 5f6f       zero_copy_o
-00036160: 6e6c 7920 3a20 626f 6f6c 2c20 6465 6661  nly : bool, defa
-00036170: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
-00036180: 2020 2020 2020 4966 2054 7275 652c 2061        If True, a
-00036190: 6e20 6578 6365 7074 696f 6e20 7769 6c6c  n exception will
-000361a0: 2062 6520 7261 6973 6564 2069 6620 7468   be raised if th
-000361b0: 6520 636f 6e76 6572 7369 6f6e 2074 6f20  e conversion to 
-000361c0: 6120 6046 6173 7441 7272 6179 6020 776f  a `FastArray` wo
-000361d0: 756c 6420 7265 7175 6972 6520 636f 7079  uld require copy
-000361e0: 696e 6720 7468 650d 0a20 2020 2020 2020  ing the..       
-000361f0: 2020 2020 2075 6e64 6572 6c79 696e 6720       underlying 
-00036200: 6461 7461 2028 652e 672e 2069 6e20 7072  data (e.g. in pr
-00036210: 6573 656e 6365 206f 6620 6e75 6c6c 732c  esence of nulls,
-00036220: 206f 7220 666f 7220 6e6f 6e2d 7072 696d   or for non-prim
-00036230: 6974 6976 6520 7479 7065 7329 2e0d 0a20  itive types)... 
-00036240: 2020 2020 2020 2077 7269 7461 626c 6520         writable 
-00036250: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-00036260: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-00036270: 2020 2046 6f72 2061 2060 4661 7374 4172     For a `FastAr
-00036280: 7261 7960 2063 7265 6174 6564 2077 6974  ray` created wit
-00036290: 6820 7a65 726f 2063 6f70 7920 2876 6965  h zero copy (vie
-000362a0: 7720 6f6e 2074 6865 2041 7272 6f77 2064  w on the Arrow d
-000362b0: 6174 6129 2c20 7468 6520 7265 7375 6c74  ata), the result
-000362c0: 696e 6720 6172 7261 7920 6973 206e 6f74  ing array is not
-000362d0: 2077 7269 7461 626c 6520 2841 7272 6f77   writable (Arrow
-000362e0: 2064 6174 6120 6973 2069 6d6d 7574 6162   data is immutab
-000362f0: 6c65 292e 0d0a 2020 2020 2020 2020 2020  le)...          
-00036300: 2020 4279 2073 6574 7469 6e67 2074 6869    By setting thi
-00036310: 7320 746f 2054 7275 652c 2061 2063 6f70  s to True, a cop
-00036320: 7920 6f66 2074 6865 2061 7272 6179 2069  y of the array i
-00036330: 7320 6d61 6465 2074 6f20 656e 7375 7265  s made to ensure
-00036340: 2069 7420 6973 2077 7269 7461 626c 652e   it is writable.
-00036350: 0d0a 2020 2020 2020 2020 6175 746f 5f77  ..        auto_w
-00036360: 6964 656e 203a 2062 6f6f 6c2c 206f 7074  iden : bool, opt
-00036370: 696f 6e61 6c2c 2064 6566 6175 6c74 2074  ional, default t
-00036380: 6f20 4661 6c73 650d 0a20 2020 2020 2020  o False..       
-00036390: 2020 2020 2057 6865 6e20 4661 6c73 6520       When False 
-000363a0: 2874 6865 2064 6566 6175 6c74 292c 2069  (the default), i
-000363b0: 6620 616e 2061 7272 6f77 2061 7272 6179  f an arrow array
-000363c0: 2063 6f6e 7461 696e 7320 6120 7661 6c75   contains a valu
-000363d0: 6520 7768 6963 6820 776f 756c 6420 6265  e which would be
-000363e0: 2063 6f6e 7369 6465 7265 640d 0a20 2020   considered..   
-000363f0: 2020 2020 2020 2020 2074 6865 2027 696e           the 'in
-00036400: 7661 6c69 6427 2f4e 4120 7661 6c75 6520  valid'/NA value 
-00036410: 666f 7220 7468 6520 6571 7569 7661 6c65  for the equivale
-00036420: 6e74 2064 7479 7065 2069 6e20 6120 6046  nt dtype in a `F
-00036430: 6173 7441 7272 6179 602c 2072 6169 7365  astArray`, raise
-00036440: 2061 6e20 6578 6365 7074 696f 6e0d 0a20   an exception.. 
-00036450: 2020 2020 2020 2020 2020 2062 6563 6175             becau
-00036460: 7365 2064 6972 6563 7420 636f 6e76 6572  se direct conver
-00036470: 7369 6f6e 2077 6f75 6c64 2062 6520 6c6f  sion would be lo
-00036480: 7373 7920 2f20 6368 616e 6765 2074 6865  ssy / change the
-00036490: 2073 656d 616e 7469 6320 6d65 616e 696e   semantic meanin
-000364a0: 6720 6f66 2074 6865 2064 6174 612e 0d0a  g of the data...
-000364b0: 2020 2020 2020 2020 2020 2020 5768 656e              When
-000364c0: 2054 7275 652c 2074 6865 2063 6f6e 7665   True, the conve
-000364d0: 7274 6564 2061 7272 6179 2077 696c 6c20  rted array will 
-000364e0: 6265 2077 6964 656e 6564 2028 6966 2070  be widened (if p
-000364f0: 6f73 7369 626c 6529 2074 6f20 7468 6520  ossible) to the 
-00036500: 6e65 7874 2d6c 6172 6765 7374 2064 7479  next-largest dty
-00036510: 7065 0d0a 2020 2020 2020 2020 2020 2020  pe..            
-00036520: 746f 2065 6e73 7572 6520 7468 6520 6461  to ensure the da
-00036530: 7461 2077 696c 6c20 6265 2069 6e74 6572  ta will be inter
-00036540: 7072 6574 6564 2069 6e20 7468 6520 7361  preted in the sa
-00036550: 6d65 2077 6179 2e0d 0a0d 0a20 2020 2020  me way.....     
-00036560: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-00036570: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-00036580: 2020 2020 2046 6173 7441 7272 6179 0d0a       FastArray..
-00036590: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-000365a0: 2020 2020 2069 6d70 6f72 7420 7079 6172       import pyar
-000365b0: 726f 7720 6173 2070 610d 0a20 2020 2020  row as pa..     
-000365c0: 2020 2069 6d70 6f72 7420 7079 6172 726f     import pyarro
-000365d0: 772e 636f 6d70 7574 6520 6173 2070 630d  w.compute as pc.
-000365e0: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-000365f0: 7079 6172 726f 772e 7479 7065 7320 6173  pyarrow.types as
-00036600: 2070 6174 0d0a 0d0a 2020 2020 2020 2020   pat....        
-00036610: 2320 4d61 6b65 2073 7572 6520 7468 6520  # Make sure the 
-00036620: 696e 7075 7420 6172 7261 7920 6973 206f  input array is o
-00036630: 6e65 206f 6620 7468 6520 7079 6172 726f  ne of the pyarro
-00036640: 7720 6172 7261 7920 7479 7065 732e 0d0a  w array types...
-00036650: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00036660: 7369 6e73 7461 6e63 6528 6172 722c 2028  sinstance(arr, (
-00036670: 7061 2e41 7272 6179 2c20 7061 2e43 6875  pa.Array, pa.Chu
-00036680: 6e6b 6564 4172 7261 7929 293a 0d0a 2020  nkedArray)):..  
-00036690: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000366a0: 5479 7065 4572 726f 7228 2254 6865 2061  TypeError("The a
-000366b0: 7272 6179 2069 7320 6e6f 7420 616e 2069  rray is not an i
-000366c0: 6e73 7461 6e63 6520 6f66 2060 7079 6172  nstance of `pyar
-000366d0: 726f 772e 4172 7261 7960 206f 7220 6070  row.Array` or `p
-000366e0: 7961 7272 6f77 2e43 6875 6e6b 6564 4172  yarrow.ChunkedAr
-000366f0: 7261 7960 2e22 290d 0a0d 0a20 2020 2020  ray`.")....     
-00036700: 2020 2023 2043 6875 6e6b 6564 4172 7261     # ChunkedArra
-00036710: 7973 206e 6565 6420 7370 6563 6961 6c20  ys need special 
-00036720: 6861 6e64 6c69 6e67 2e0d 0a20 2020 2020  handling...     
-00036730: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00036740: 2861 7272 2c20 7061 2e43 6875 6e6b 6564  (arr, pa.Chunked
-00036750: 4172 7261 7929 3a0d 0a20 2020 2020 2020  Array):..       
-00036760: 2020 2020 2023 2041 2073 696e 676c 652d       # A single-
-00036770: 6368 756e 6b20 4368 756e 6b65 6441 7272  chunk ChunkedArr
-00036780: 6179 2063 616e 2062 6520 6861 6e64 6c65  ay can be handle
-00036790: 6420 6279 206a 7573 7420 6578 7472 6163  d by just extrac
-000367a0: 7469 6e67 2074 6861 7420 6368 756e 6b0d  ting that chunk.
-000367b0: 0a20 2020 2020 2020 2020 2020 2023 2061  .            # a
-000367c0: 6e64 2072 6563 7572 7369 7665 6c79 2070  nd recursively p
-000367d0: 726f 6365 7373 696e 6720 6974 2e0d 0a20  rocessing it... 
-000367e0: 2020 2020 2020 2020 2020 2069 6620 6172             if ar
-000367f0: 722e 6e75 6d5f 6368 756e 6b73 203d 3d20  r.num_chunks == 
-00036800: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-00036810: 2020 2020 7265 7475 726e 2046 6173 7441      return FastA
-00036820: 7272 6179 2e5f 6672 6f6d 5f61 7272 6f77  rray._from_arrow
-00036830: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00036840: 2020 2020 2020 2061 7272 2e63 6875 6e6b         arr.chunk
-00036850: 2830 292c 207a 6572 6f5f 636f 7079 5f6f  (0), zero_copy_o
-00036860: 6e6c 793d 7a65 726f 5f63 6f70 795f 6f6e  nly=zero_copy_on
-00036870: 6c79 2c20 7772 6974 6162 6c65 3d77 7269  ly, writable=wri
-00036880: 7461 626c 652c 2061 7574 6f5f 7769 6465  table, auto_wide
-00036890: 6e3d 6175 746f 5f77 6964 656e 0d0a 2020  n=auto_widen..  
-000368a0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-000368b0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000368c0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000368d0: 2020 2020 2320 544f 444f 3a20 4265 6e63      # TODO: Benc
-000368e0: 686d 6172 6b20 7468 6973 2076 732e 2075  hmark this vs. u
-000368f0: 7369 6e67 2043 6875 6e6b 6564 4172 7261  sing ChunkedArra
-00036900: 792e 636f 6d62 696e 655f 6368 756e 6b73  y.combine_chunks
-00036910: 2829 2074 6865 6e20 636f 6e76 6572 7469  () then converti
-00036920: 6e67 2e0d 0a20 2020 2020 2020 2020 2020  ng...           
-00036930: 2020 2020 2023 2054 4f44 4f3a 204c 6f6f       # TODO: Loo
-00036940: 6b20 6174 2060 7a65 726f 5f63 6f70 795f  k at `zero_copy_
-00036950: 6f6e 6c79 6020 616e 6420 6077 7269 7461  only` and `writa
-00036960: 626c 6560 202d 2d20 7468 6520 636f 6e76  ble` -- the conv
-00036970: 6572 7465 6420 6172 7261 7973 2063 6f75  erted arrays cou
-00036980: 6c64 2062 6520 6465 7374 726f 7965 6420  ld be destroyed 
-00036990: 7768 696c 6520 6873 7461 636b 696e 670d  while hstacking.
-000369a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000369b0: 2023 2020 2020 2020 2073 696e 6365 2077   #       since w
-000369c0: 6520 6b6e 6f77 2074 6865 7927 6c6c 2068  e know they'll h
-000369d0: 6176 6520 6a75 7374 2062 6565 6e20 6372  ave just been cr
-000369e0: 6561 7465 643b 2074 6869 7320 636f 756c  eated; this coul
-000369f0: 6420 7265 6475 6365 2070 6561 6b20 6d65  d reduce peak me
-00036a00: 6d6f 7279 2075 7469 6c69 7a61 7469 6f6e  mory utilization
-00036a10: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00036a20: 2020 2072 6574 7572 6e20 6873 7461 636b     return hstack
-00036a30: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00036a40: 2020 2020 2020 205b 0d0a 2020 2020 2020         [..      
+00034db0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+00034dc0: 4063 6163 6865 645f 7765 616b 7265 665f  @cached_weakref_
+00034dd0: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+00034de0: 6620 7374 7228 7365 6c66 2920 2d3e 2022  f str(self) -> "
+00034df0: 4641 5374 7269 6e67 223a 0d0a 2020 2020  FAString":..    
+00034e00: 2020 2020 7222 2222 4361 7374 7320 616e      r"""Casts an
+00034e10: 2061 7272 6179 206f 6620 6279 7465 2073   array of byte s
+00034e20: 7472 696e 6773 206f 7220 756e 6963 6f64  trings or unicod
+00034e30: 6520 6173 2060 6046 4153 7472 696e 6760  e as ``FAString`
+00034e40: 602e 0d0a 0d0a 2020 2020 2020 2020 456e  `.....        En
+00034e50: 6162 6c65 7320 6120 7661 7269 6574 7920  ables a variety 
+00034e60: 6f66 2075 7365 6675 6c20 7374 7269 6e67  of useful string
+00034e70: 206d 616e 6970 756c 6174 696f 6e20 6d65   manipulation me
+00034e80: 7468 6f64 732e 0d0a 0d0a 2020 2020 2020  thods.....      
+00034e90: 2020 5265 7475 726e 730d 0a20 2020 2020    Returns..     
+00034ea0: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
+00034eb0: 2020 2020 4641 5374 7269 6e67 0d0a 0d0a      FAString....
+00034ec0: 2020 2020 2020 2020 5261 6973 6573 0d0a          Raises..
+00034ed0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0d0a          ------..
+00034ee0: 2020 2020 2020 2020 5479 7065 4572 726f          TypeErro
+00034ef0: 720d 0a20 2020 2020 2020 2020 2020 2049  r..            I
+00034f00: 6620 7468 6520 4661 7374 4172 7261 7920  f the FastArray 
+00034f10: 6973 206f 6620 6474 7970 6520 6f74 6865  is of dtype othe
+00034f20: 7220 7468 616e 2062 7974 6520 7374 7269  r than byte stri
+00034f30: 6e67 206f 7220 756e 6963 6f64 650d 0a0d  ng or unicode...
+00034f40: 0a20 2020 2020 2020 2053 6565 2041 6c73  .        See Als
+00034f50: 6f0d 0a20 2020 2020 2020 202d 2d2d 2d2d  o..        -----
+00034f60: 2d2d 2d0d 0a20 2020 2020 2020 206e 702e  ---..        np.
+00034f70: 6368 6172 6172 7261 790d 0a20 2020 2020  chararray..     
+00034f80: 2020 206e 702e 6368 6172 0d0a 2020 2020     np.char..    
+00034f90: 2020 2020 7274 2e46 4153 7472 696e 672e      rt.FAString.
+00034fa0: 6170 706c 790d 0a0d 0a20 2020 2020 2020  apply....       
+00034fb0: 2045 7861 6d70 6c65 730d 0a20 2020 2020   Examples..     
+00034fc0: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
+00034fd0: 2020 2020 203e 3e3e 2073 3d46 4128 5b27       >>> s=FA(['
+00034fe0: 7468 6973 272c 2774 6861 7427 2c27 7465  this','that','te
+00034ff0: 7374 2027 5d2a 3130 305f 3030 3029 0d0a  st ']*100_000)..
+00035000: 2020 2020 2020 2020 3e3e 3e20 732e 7374          >>> s.st
+00035010: 722e 7570 7065 720d 0a20 2020 2020 2020  r.upper..       
+00035020: 2046 6173 7441 7272 6179 285b 6227 5448   FastArray([b'TH
+00035030: 4953 272c 2062 2754 4841 5427 2c20 6227  IS', b'THAT', b'
+00035040: 5445 5354 2027 2c20 2e2e 2e2c 2062 2754  TEST ', ..., b'T
+00035050: 4849 5327 2c20 6227 5448 4154 272c 2062  HIS', b'THAT', b
+00035060: 2754 4553 5420 275d 2c0d 0a20 2020 2020  'TEST '],..     
+00035070: 2020 2020 2020 2020 2020 2020 2064 7479               dty
+00035080: 7065 3d27 7c53 3527 290d 0a0d 0a20 2020  pe='|S5')....   
+00035090: 2020 2020 203e 3e3e 2073 2e73 7472 2e6c       >>> s.str.l
+000350a0: 6f77 6572 0d0a 2020 2020 2020 2020 4661  ower..        Fa
+000350b0: 7374 4172 7261 7928 5b62 2774 6869 7327  stArray([b'this'
+000350c0: 2c20 6227 7468 6174 272c 2062 2774 6573  , b'that', b'tes
+000350d0: 7420 272c 202e 2e2e 2c20 6227 7468 6973  t ', ..., b'this
+000350e0: 272c 2062 2774 6861 7427 2c20 6227 7465  ', b'that', b'te
+000350f0: 7374 2027 5d2c 0d0a 2020 2020 2020 2020  st '],..        
+00035100: 2020 2020 2020 2020 2020 6474 7970 653d            dtype=
+00035110: 277c 5335 2729 0d0a 0d0a 2020 2020 2020  '|S5')....      
+00035120: 2020 3e3e 3e20 732e 7374 722e 7265 6d6f    >>> s.str.remo
+00035130: 7665 7472 6169 6c69 6e67 2829 0d0a 2020  vetrailing()..  
+00035140: 2020 2020 2020 4661 7374 4172 7261 7928        FastArray(
+00035150: 5b62 2774 6869 7327 2c20 6227 7468 6174  [b'this', b'that
+00035160: 272c 2062 2774 6573 7427 2c20 2e2e 2e2c  ', b'test', ...,
+00035170: 2062 2774 6869 7327 2c20 6227 7468 6174   b'this', b'that
+00035180: 272c 2062 2774 6573 7427 5d2c 0d0a 2020  ', b'test'],..  
+00035190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000351a0: 6474 7970 653d 277c 5335 2729 0d0a 2020  dtype='|S5')..  
+000351b0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+000351c0: 2020 2069 6620 7365 6c66 2e64 7479 7065     if self.dtype
+000351d0: 2e63 6861 7220 696e 2022 5553 223a 0d0a  .char in "US":..
+000351e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000351f0: 726e 2054 7970 6552 6567 6973 7465 722e  rn TypeRegister.
+00035200: 4641 5374 7269 6e67 2873 656c 6629 0d0a  FAString(self)..
+00035210: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00035220: 6474 7970 652e 6368 6172 203d 3d20 224f  dtype.char == "O
+00035230: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+00035240: 2320 7472 7920 746f 2063 6f6e 7665 7274  # try to convert
+00035250: 2074 6f20 7374 7269 6e67 2028 6d69 6768   to string (migh
+00035260: 7420 6861 7665 2063 6f6d 6520 6672 6f6d  t have come from
+00035270: 2070 616e 6461 7329 0d0a 2020 2020 2020   pandas)..      
+00035280: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00035290: 2020 2020 2020 2020 2020 2020 636f 6e76              conv
+000352a0: 203d 2073 656c 662e 6173 7479 7065 2822   = self.astype("
+000352b0: 5322 290d 0a20 2020 2020 2020 2020 2020  S")..           
+000352c0: 2065 7863 6570 743a 0d0a 2020 2020 2020   except:..      
+000352d0: 2020 2020 2020 2020 2020 636f 6e76 203d            conv =
+000352e0: 2073 656c 662e 6173 7479 7065 2822 5522   self.astype("U"
+000352f0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00035300: 6574 7572 6e20 5479 7065 5265 6769 7374  eturn TypeRegist
+00035310: 6572 2e46 4153 7472 696e 6728 636f 6e76  er.FAString(conv
+00035320: 290d 0a0d 0a20 2020 2020 2020 2072 6169  )....        rai
+00035330: 7365 2054 7970 6545 7272 6f72 2866 2254  se TypeError(f"T
+00035340: 6865 202e 7374 7220 6675 6e63 7469 6f6e  he .str function
+00035350: 2063 616e 206f 6e6c 7920 6265 2075 7365   can only be use
+00035360: 6420 6f6e 2062 7974 6520 7374 7269 6e67  d on byte string
+00035370: 2061 6e64 2075 6e69 636f 6465 206e 6f74   and unicode not
+00035380: 207b 7365 6c66 2e64 7479 7065 2172 7d22   {self.dtype!r}"
+00035390: 290d 0a0d 0a20 2020 2040 7374 6174 6963  )....    @static
+000353a0: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
+000353b0: 6672 6f6d 5f61 7272 6f77 280d 0a20 2020  from_arrow(..   
+000353c0: 2020 2020 2061 7272 3a20 556e 696f 6e5b       arr: Union[
+000353d0: 2270 612e 4172 7261 7922 2c20 2270 612e  "pa.Array", "pa.
+000353e0: 4368 756e 6b65 6441 7272 6179 225d 2c0d  ChunkedArray"],.
+000353f0: 0a20 2020 2020 2020 207a 6572 6f5f 636f  .        zero_co
+00035400: 7079 5f6f 6e6c 793a 2062 6f6f 6c20 3d20  py_only: bool = 
+00035410: 5472 7565 2c0d 0a20 2020 2020 2020 2077  True,..        w
+00035420: 7269 7461 626c 653a 2062 6f6f 6c20 3d20  ritable: bool = 
+00035430: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00035440: 6175 746f 5f77 6964 656e 3a20 626f 6f6c  auto_widen: bool
+00035450: 203d 2046 616c 7365 2c0d 0a20 2020 2029   = False,..    )
+00035460: 202d 3e20 2246 6173 7441 7272 6179 223a   -> "FastArray":
+00035470: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00035480: 2020 2020 2020 2043 6f6e 7665 7274 2061         Convert a
+00035490: 2070 7961 7272 6f77 2060 4172 7261 7960   pyarrow `Array`
+000354a0: 2074 6f20 6120 7269 7074 6162 6c65 2060   to a riptable `
+000354b0: 4661 7374 4172 7261 7960 2e0d 0a0d 0a20  FastArray`..... 
+000354c0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+000354d0: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+000354e0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2061  -----..        a
+000354f0: 7272 203a 2070 7961 7272 6f77 2e41 7272  rr : pyarrow.Arr
+00035500: 6179 206f 7220 7079 6172 726f 772e 4368  ay or pyarrow.Ch
+00035510: 756e 6b65 6441 7272 6179 0d0a 2020 2020  unkedArray..    
+00035520: 2020 2020 7a65 726f 5f63 6f70 795f 6f6e      zero_copy_on
+00035530: 6c79 203a 2062 6f6f 6c2c 2064 6566 6175  ly : bool, defau
+00035540: 6c74 2054 7275 650d 0a20 2020 2020 2020  lt True..       
+00035550: 2020 2020 2049 6620 5472 7565 2c20 616e       If True, an
+00035560: 2065 7863 6570 7469 6f6e 2077 696c 6c20   exception will 
+00035570: 6265 2072 6169 7365 6420 6966 2074 6865  be raised if the
+00035580: 2063 6f6e 7665 7273 696f 6e20 746f 2061   conversion to a
+00035590: 2060 4661 7374 4172 7261 7960 2077 6f75   `FastArray` wou
+000355a0: 6c64 2072 6571 7569 7265 2063 6f70 7969  ld require copyi
+000355b0: 6e67 2074 6865 0d0a 2020 2020 2020 2020  ng the..        
+000355c0: 2020 2020 756e 6465 726c 7969 6e67 2064      underlying d
+000355d0: 6174 6120 2865 2e67 2e20 696e 2070 7265  ata (e.g. in pre
+000355e0: 7365 6e63 6520 6f66 206e 756c 6c73 2c20  sence of nulls, 
+000355f0: 6f72 2066 6f72 206e 6f6e 2d70 7269 6d69  or for non-primi
+00035600: 7469 7665 2074 7970 6573 292e 0d0a 2020  tive types)...  
+00035610: 2020 2020 2020 7772 6974 6162 6c65 203a        writable :
+00035620: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
+00035630: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
+00035640: 2020 466f 7220 6120 6046 6173 7441 7272    For a `FastArr
+00035650: 6179 6020 6372 6561 7465 6420 7769 7468  ay` created with
+00035660: 207a 6572 6f20 636f 7079 2028 7669 6577   zero copy (view
+00035670: 206f 6e20 7468 6520 4172 726f 7720 6461   on the Arrow da
+00035680: 7461 292c 2074 6865 2072 6573 756c 7469  ta), the resulti
+00035690: 6e67 2061 7272 6179 2069 7320 6e6f 7420  ng array is not 
+000356a0: 7772 6974 6162 6c65 2028 4172 726f 7720  writable (Arrow 
+000356b0: 6461 7461 2069 7320 696d 6d75 7461 626c  data is immutabl
+000356c0: 6529 2e0d 0a20 2020 2020 2020 2020 2020  e)...           
+000356d0: 2042 7920 7365 7474 696e 6720 7468 6973   By setting this
+000356e0: 2074 6f20 5472 7565 2c20 6120 636f 7079   to True, a copy
+000356f0: 206f 6620 7468 6520 6172 7261 7920 6973   of the array is
+00035700: 206d 6164 6520 746f 2065 6e73 7572 6520   made to ensure 
+00035710: 6974 2069 7320 7772 6974 6162 6c65 2e0d  it is writable..
+00035720: 0a20 2020 2020 2020 2061 7574 6f5f 7769  .        auto_wi
+00035730: 6465 6e20 3a20 626f 6f6c 2c20 6f70 7469  den : bool, opti
+00035740: 6f6e 616c 2c20 6465 6661 756c 7420 746f  onal, default to
+00035750: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00035760: 2020 2020 5768 656e 2046 616c 7365 2028      When False (
+00035770: 7468 6520 6465 6661 756c 7429 2c20 6966  the default), if
+00035780: 2061 6e20 6172 726f 7720 6172 7261 7920   an arrow array 
+00035790: 636f 6e74 6169 6e73 2061 2076 616c 7565  contains a value
+000357a0: 2077 6869 6368 2077 6f75 6c64 2062 6520   which would be 
+000357b0: 636f 6e73 6964 6572 6564 0d0a 2020 2020  considered..    
+000357c0: 2020 2020 2020 2020 7468 6520 2769 6e76          the 'inv
+000357d0: 616c 6964 272f 4e41 2076 616c 7565 2066  alid'/NA value f
+000357e0: 6f72 2074 6865 2065 7175 6976 616c 656e  or the equivalen
+000357f0: 7420 6474 7970 6520 696e 2061 2060 4661  t dtype in a `Fa
+00035800: 7374 4172 7261 7960 2c20 7261 6973 6520  stArray`, raise 
+00035810: 616e 2065 7863 6570 7469 6f6e 0d0a 2020  an exception..  
+00035820: 2020 2020 2020 2020 2020 6265 6361 7573            becaus
+00035830: 6520 6469 7265 6374 2063 6f6e 7665 7273  e direct convers
+00035840: 696f 6e20 776f 756c 6420 6265 206c 6f73  ion would be los
+00035850: 7379 202f 2063 6861 6e67 6520 7468 6520  sy / change the 
+00035860: 7365 6d61 6e74 6963 206d 6561 6e69 6e67  semantic meaning
+00035870: 206f 6620 7468 6520 6461 7461 2e0d 0a20   of the data... 
+00035880: 2020 2020 2020 2020 2020 2057 6865 6e20             When 
+00035890: 5472 7565 2c20 7468 6520 636f 6e76 6572  True, the conver
+000358a0: 7465 6420 6172 7261 7920 7769 6c6c 2062  ted array will b
+000358b0: 6520 7769 6465 6e65 6420 2869 6620 706f  e widened (if po
+000358c0: 7373 6962 6c65 2920 746f 2074 6865 206e  ssible) to the n
+000358d0: 6578 742d 6c61 7267 6573 7420 6474 7970  ext-largest dtyp
+000358e0: 650d 0a20 2020 2020 2020 2020 2020 2074  e..            t
+000358f0: 6f20 656e 7375 7265 2074 6865 2064 6174  o ensure the dat
+00035900: 6120 7769 6c6c 2062 6520 696e 7465 7270  a will be interp
+00035910: 7265 7465 6420 696e 2074 6865 2073 616d  reted in the sam
+00035920: 6520 7761 792e 0d0a 0d0a 2020 2020 2020  e way.....      
+00035930: 2020 5265 7475 726e 730d 0a20 2020 2020    Returns..     
+00035940: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
+00035950: 2020 2020 4661 7374 4172 7261 790d 0a20      FastArray.. 
+00035960: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00035970: 2020 2020 696d 706f 7274 2070 7961 7272      import pyarr
+00035980: 6f77 2e74 7970 6573 2061 7320 7061 740d  ow.types as pat.
+00035990: 0a0d 0a20 2020 2020 2020 2023 2042 6173  ...        # Bas
+000359a0: 6564 206f 6e20 7468 6520 7479 7065 206f  ed on the type o
+000359b0: 6620 7468 6520 6172 7261 792c 2064 6973  f the array, dis
+000359c0: 7061 7463 6820 746f 2074 7970 652d 7370  patch to type-sp
+000359d0: 6563 6966 6963 2069 6d70 6c65 6d65 6e74  ecific implement
+000359e0: 6174 696f 6e73 206f 6620 2e66 726f 6d5f  ations of .from_
+000359f0: 6172 726f 7728 292e 0d0a 2020 2020 2020  arrow()...      
+00035a00: 2020 7061 5f61 7272 5f74 7970 6520 3d20    pa_arr_type = 
+00035a10: 6172 722e 7479 7065 0d0a 2020 2020 2020  arr.type..      
+00035a20: 2020 6966 2028 0d0a 2020 2020 2020 2020    if (..        
+00035a30: 2020 2020 7061 742e 6973 5f62 6f6f 6c65      pat.is_boole
+00035a40: 616e 2870 615f 6172 725f 7479 7065 290d  an(pa_arr_type).
+00035a50: 0a20 2020 2020 2020 2020 2020 206f 7220  .            or 
+00035a60: 7061 742e 6973 5f69 6e74 6567 6572 2870  pat.is_integer(p
+00035a70: 615f 6172 725f 7479 7065 290d 0a20 2020  a_arr_type)..   
+00035a80: 2020 2020 2020 2020 206f 7220 7061 742e           or pat.
+00035a90: 6973 5f66 6c6f 6174 696e 6728 7061 5f61  is_floating(pa_a
+00035aa0: 7272 5f74 7970 6529 0d0a 2020 2020 2020  rr_type)..      
+00035ab0: 2020 2020 2020 6f72 2070 6174 2e69 735f        or pat.is_
+00035ac0: 7374 7269 6e67 2870 615f 6172 725f 7479  string(pa_arr_ty
+00035ad0: 7065 290d 0a20 2020 2020 2020 2020 2020  pe)..           
+00035ae0: 206f 7220 7061 742e 6973 5f62 696e 6172   or pat.is_binar
+00035af0: 7928 7061 5f61 7272 5f74 7970 6529 0d0a  y(pa_arr_type)..
+00035b00: 2020 2020 2020 2020 2020 2020 6f72 2070              or p
+00035b10: 6174 2e69 735f 6669 7865 645f 7369 7a65  at.is_fixed_size
+00035b20: 5f62 696e 6172 7928 7061 5f61 7272 5f74  _binary(pa_arr_t
+00035b30: 7970 6529 0d0a 2020 2020 2020 2020 293a  ype)..        ):
+00035b40: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00035b50: 544f 444f 3a20 4368 6563 6b20 7768 6574  TODO: Check whet
+00035b60: 6865 7220 7468 6973 2063 6f6c 756d 6e20  her this column 
+00035b70: 6861 7320 6120 7573 6572 2d73 7065 6369  has a user-speci
+00035b80: 6669 6564 2066 696c 6c20 7661 6c75 6520  fied fill value 
+00035b90: 7072 6f76 6964 6564 3b20 6966 2073 6f2c  provided; if so,
+00035ba0: 2070 6173 7320 6974 2061 6c6f 6e67 2074   pass it along t
+00035bb0: 6f0d 0a20 2020 2020 2020 2020 2020 2023  o..            #
+00035bc0: 2020 2020 2020 2074 6865 2046 6173 7441         the FastA
+00035bd0: 7272 6179 2e66 726f 6d5f 6172 726f 7728  rray.from_arrow(
+00035be0: 2920 6d65 7468 6f64 2063 616c 6c20 6265  ) method call be
+00035bf0: 6c6f 772e 0d0a 2020 2020 2020 2020 2020  low...          
+00035c00: 2020 7265 7475 726e 2046 6173 7441 7272    return FastArr
+00035c10: 6179 2e5f 6672 6f6d 5f61 7272 6f77 2861  ay._from_arrow(a
+00035c20: 7272 2c20 7a65 726f 5f63 6f70 795f 6f6e  rr, zero_copy_on
+00035c30: 6c79 3d7a 6572 6f5f 636f 7079 5f6f 6e6c  ly=zero_copy_onl
+00035c40: 792c 2077 7269 7461 626c 653d 7772 6974  y, writable=writ
+00035c50: 6162 6c65 2c20 6175 746f 5f77 6964 656e  able, auto_widen
+00035c60: 3d61 7574 6f5f 7769 6465 6e29 0d0a 0d0a  =auto_widen)....
+00035c70: 2020 2020 2020 2020 656c 6966 2070 6174          elif pat
+00035c80: 2e69 735f 6469 6374 696f 6e61 7279 2870  .is_dictionary(p
+00035c90: 615f 6172 725f 7479 7065 2920 6f72 2070  a_arr_type) or p
+00035ca0: 6174 2e69 735f 7374 7275 6374 2870 615f  at.is_struct(pa_
+00035cb0: 6172 725f 7479 7065 293a 0d0a 2020 2020  arr_type):..    
+00035cc0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00035cd0: 7970 6552 6567 6973 7465 722e 4361 7465  ypeRegister.Cate
+00035ce0: 676f 7269 6361 6c2e 5f66 726f 6d5f 6172  gorical._from_ar
+00035cf0: 726f 7728 6172 722c 207a 6572 6f5f 636f  row(arr, zero_co
+00035d00: 7079 5f6f 6e6c 793d 7a65 726f 5f63 6f70  py_only=zero_cop
+00035d10: 795f 6f6e 6c79 2c20 7772 6974 6162 6c65  y_only, writable
+00035d20: 3d77 7269 7461 626c 6529 0d0a 0d0a 2020  =writable)....  
+00035d30: 2020 2020 2020 656c 6966 2070 6174 2e69        elif pat.i
+00035d40: 735f 7469 6d65 7374 616d 7028 7061 5f61  s_timestamp(pa_a
+00035d50: 7272 5f74 7970 6529 3a0d 0a20 2020 2020  rr_type):..     
+00035d60: 2020 2020 2020 2072 6574 7572 6e20 5479         return Ty
+00035d70: 7065 5265 6769 7374 6572 2e44 6174 6554  peRegister.DateT
+00035d80: 696d 654e 616e 6f2e 5f66 726f 6d5f 6172  imeNano._from_ar
+00035d90: 726f 7728 6172 722c 207a 6572 6f5f 636f  row(arr, zero_co
+00035da0: 7079 5f6f 6e6c 793d 7a65 726f 5f63 6f70  py_only=zero_cop
+00035db0: 795f 6f6e 6c79 2c20 7772 6974 6162 6c65  y_only, writable
+00035dc0: 3d77 7269 7461 626c 6529 0d0a 0d0a 2020  =writable)....  
+00035dd0: 2020 2020 2020 656c 6966 2070 6174 2e69        elif pat.i
+00035de0: 735f 6461 7465 2870 615f 6172 725f 7479  s_date(pa_arr_ty
+00035df0: 7065 293a 0d0a 2020 2020 2020 2020 2020  pe):..          
+00035e00: 2020 7265 7475 726e 2054 7970 6552 6567    return TypeReg
+00035e10: 6973 7465 722e 4461 7465 2e5f 6672 6f6d  ister.Date._from
+00035e20: 5f61 7272 6f77 2861 7272 2c20 7a65 726f  _arrow(arr, zero
+00035e30: 5f63 6f70 795f 6f6e 6c79 3d7a 6572 6f5f  _copy_only=zero_
+00035e40: 636f 7079 5f6f 6e6c 792c 2077 7269 7461  copy_only, writa
+00035e50: 626c 653d 7772 6974 6162 6c65 290d 0a0d  ble=writable)...
+00035e60: 0a20 2020 2020 2020 2065 6c69 6620 7061  .        elif pa
+00035e70: 742e 6973 5f64 7572 6174 696f 6e28 7061  t.is_duration(pa
+00035e80: 5f61 7272 5f74 7970 6529 3a0d 0a20 2020  _arr_type):..   
+00035e90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00035ea0: 5479 7065 5265 6769 7374 6572 2e54 696d  TypeRegister.Tim
+00035eb0: 6553 7061 6e2e 5f66 726f 6d5f 6172 726f  eSpan._from_arro
+00035ec0: 7728 6172 722c 207a 6572 6f5f 636f 7079  w(arr, zero_copy
+00035ed0: 5f6f 6e6c 793d 7a65 726f 5f63 6f70 795f  _only=zero_copy_
+00035ee0: 6f6e 6c79 2c20 7772 6974 6162 6c65 3d77  only, writable=w
+00035ef0: 7269 7461 626c 6529 0d0a 0d0a 2020 2020  ritable)....    
+00035f00: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00035f10: 2020 2020 2020 2023 2055 6e6b 6e6f 776e         # Unknown
+00035f20: 2f75 6e73 7570 706f 7274 6564 2061 7272  /unsupported arr
+00035f30: 6179 2074 7970 6520 2d2d 2063 616e 2774  ay type -- can't
+00035f40: 2063 6f6e 7665 7274 2e0d 0a20 2020 2020   convert...     
+00035f50: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+00035f60: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00035f70: 2866 2270 7961 7272 6f77 2061 7272 6179  (f"pyarrow array
+00035f80: 7320 6f66 2074 7970 6520 277b 7061 5f61  s of type '{pa_a
+00035f90: 7272 5f74 7970 657d 2720 6361 6e27 7420  rr_type}' can't 
+00035fa0: 6265 2063 6f6e 7665 7274 6564 2074 6f20  be converted to 
+00035fb0: 7269 7074 6162 6c65 2061 7272 6179 732e  riptable arrays.
+00035fc0: 2229 0d0a 0d0a 2020 2020 4073 7461 7469  ")....    @stati
+00035fd0: 636d 6574 686f 640d 0a20 2020 2064 6566  cmethod..    def
+00035fe0: 205f 6672 6f6d 5f61 7272 6f77 280d 0a20   _from_arrow(.. 
+00035ff0: 2020 2020 2020 2061 7272 3a20 556e 696f         arr: Unio
+00036000: 6e5b 2270 612e 4172 7261 7922 2c20 2270  n["pa.Array", "p
+00036010: 612e 4368 756e 6b65 6441 7272 6179 225d  a.ChunkedArray"]
+00036020: 2c0d 0a20 2020 2020 2020 207a 6572 6f5f  ,..        zero_
+00036030: 636f 7079 5f6f 6e6c 793a 2062 6f6f 6c20  copy_only: bool 
+00036040: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
+00036050: 2077 7269 7461 626c 653a 2062 6f6f 6c20   writable: bool 
+00036060: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
+00036070: 2020 6175 746f 5f77 6964 656e 3a20 626f    auto_widen: bo
+00036080: 6f6c 203d 2046 616c 7365 2c0d 0a20 2020  ol = False,..   
+00036090: 2029 202d 3e20 2246 6173 7441 7272 6179   ) -> "FastArray
+000360a0: 223a 0d0a 2020 2020 2020 2020 2222 220d  ":..        """.
+000360b0: 0a20 2020 2020 2020 2043 6f6e 7665 7274  .        Convert
+000360c0: 2061 2070 7961 7272 6f77 2060 4172 7261   a pyarrow `Arra
+000360d0: 7960 2074 6f20 6120 7269 7074 6162 6c65  y` to a riptable
+000360e0: 2060 4661 7374 4172 7261 7960 2e0d 0a0d   `FastArray`....
+000360f0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00036100: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
+00036110: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+00036120: 2061 7272 203a 2070 7961 7272 6f77 2e41   arr : pyarrow.A
+00036130: 7272 6179 206f 7220 7079 6172 726f 772e  rray or pyarrow.
+00036140: 4368 756e 6b65 6441 7272 6179 0d0a 2020  ChunkedArray..  
+00036150: 2020 2020 2020 7a65 726f 5f63 6f70 795f        zero_copy_
+00036160: 6f6e 6c79 203a 2062 6f6f 6c2c 2064 6566  only : bool, def
+00036170: 6175 6c74 2054 7275 650d 0a20 2020 2020  ault True..     
+00036180: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+00036190: 616e 2065 7863 6570 7469 6f6e 2077 696c  an exception wil
+000361a0: 6c20 6265 2072 6169 7365 6420 6966 2074  l be raised if t
+000361b0: 6865 2063 6f6e 7665 7273 696f 6e20 746f  he conversion to
+000361c0: 2061 2060 4661 7374 4172 7261 7960 2077   a `FastArray` w
+000361d0: 6f75 6c64 2072 6571 7569 7265 2063 6f70  ould require cop
+000361e0: 7969 6e67 2074 6865 0d0a 2020 2020 2020  ying the..      
+000361f0: 2020 2020 2020 756e 6465 726c 7969 6e67        underlying
+00036200: 2064 6174 6120 2865 2e67 2e20 696e 2070   data (e.g. in p
+00036210: 7265 7365 6e63 6520 6f66 206e 756c 6c73  resence of nulls
+00036220: 2c20 6f72 2066 6f72 206e 6f6e 2d70 7269  , or for non-pri
+00036230: 6d69 7469 7665 2074 7970 6573 292e 0d0a  mitive types)...
+00036240: 2020 2020 2020 2020 7772 6974 6162 6c65          writable
+00036250: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+00036260: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00036270: 2020 2020 466f 7220 6120 6046 6173 7441      For a `FastA
+00036280: 7272 6179 6020 6372 6561 7465 6420 7769  rray` created wi
+00036290: 7468 207a 6572 6f20 636f 7079 2028 7669  th zero copy (vi
+000362a0: 6577 206f 6e20 7468 6520 4172 726f 7720  ew on the Arrow 
+000362b0: 6461 7461 292c 2074 6865 2072 6573 756c  data), the resul
+000362c0: 7469 6e67 2061 7272 6179 2069 7320 6e6f  ting array is no
+000362d0: 7420 7772 6974 6162 6c65 2028 4172 726f  t writable (Arro
+000362e0: 7720 6461 7461 2069 7320 696d 6d75 7461  w data is immuta
+000362f0: 626c 6529 2e0d 0a20 2020 2020 2020 2020  ble)...         
+00036300: 2020 2042 7920 7365 7474 696e 6720 7468     By setting th
+00036310: 6973 2074 6f20 5472 7565 2c20 6120 636f  is to True, a co
+00036320: 7079 206f 6620 7468 6520 6172 7261 7920  py of the array 
+00036330: 6973 206d 6164 6520 746f 2065 6e73 7572  is made to ensur
+00036340: 6520 6974 2069 7320 7772 6974 6162 6c65  e it is writable
+00036350: 2e0d 0a20 2020 2020 2020 2061 7574 6f5f  ...        auto_
+00036360: 7769 6465 6e20 3a20 626f 6f6c 2c20 6f70  widen : bool, op
+00036370: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
+00036380: 746f 2046 616c 7365 0d0a 2020 2020 2020  to False..      
+00036390: 2020 2020 2020 5768 656e 2046 616c 7365        When False
+000363a0: 2028 7468 6520 6465 6661 756c 7429 2c20   (the default), 
+000363b0: 6966 2061 6e20 6172 726f 7720 6172 7261  if an arrow arra
+000363c0: 7920 636f 6e74 6169 6e73 2061 2076 616c  y contains a val
+000363d0: 7565 2077 6869 6368 2077 6f75 6c64 2062  ue which would b
+000363e0: 6520 636f 6e73 6964 6572 6564 0d0a 2020  e considered..  
+000363f0: 2020 2020 2020 2020 2020 7468 6520 2769            the 'i
+00036400: 6e76 616c 6964 272f 4e41 2076 616c 7565  nvalid'/NA value
+00036410: 2066 6f72 2074 6865 2065 7175 6976 616c   for the equival
+00036420: 656e 7420 6474 7970 6520 696e 2061 2060  ent dtype in a `
+00036430: 4661 7374 4172 7261 7960 2c20 7261 6973  FastArray`, rais
+00036440: 6520 616e 2065 7863 6570 7469 6f6e 0d0a  e an exception..
+00036450: 2020 2020 2020 2020 2020 2020 6265 6361              beca
+00036460: 7573 6520 6469 7265 6374 2063 6f6e 7665  use direct conve
+00036470: 7273 696f 6e20 776f 756c 6420 6265 206c  rsion would be l
+00036480: 6f73 7379 202f 2063 6861 6e67 6520 7468  ossy / change th
+00036490: 6520 7365 6d61 6e74 6963 206d 6561 6e69  e semantic meani
+000364a0: 6e67 206f 6620 7468 6520 6461 7461 2e0d  ng of the data..
+000364b0: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+000364c0: 6e20 5472 7565 2c20 7468 6520 636f 6e76  n True, the conv
+000364d0: 6572 7465 6420 6172 7261 7920 7769 6c6c  erted array will
+000364e0: 2062 6520 7769 6465 6e65 6420 2869 6620   be widened (if 
+000364f0: 706f 7373 6962 6c65 2920 746f 2074 6865  possible) to the
+00036500: 206e 6578 742d 6c61 7267 6573 7420 6474   next-largest dt
+00036510: 7970 650d 0a20 2020 2020 2020 2020 2020  ype..           
+00036520: 2074 6f20 656e 7375 7265 2074 6865 2064   to ensure the d
+00036530: 6174 6120 7769 6c6c 2062 6520 696e 7465  ata will be inte
+00036540: 7270 7265 7465 6420 696e 2074 6865 2073  rpreted in the s
+00036550: 616d 6520 7761 792e 0d0a 0d0a 2020 2020  ame way.....    
+00036560: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
+00036570: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
+00036580: 2020 2020 2020 4661 7374 4172 7261 790d        FastArray.
+00036590: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000365a0: 2020 2020 2020 696d 706f 7274 2070 7961        import pya
+000365b0: 7272 6f77 2061 7320 7061 0d0a 2020 2020  rrow as pa..    
+000365c0: 2020 2020 696d 706f 7274 2070 7961 7272      import pyarr
+000365d0: 6f77 2e63 6f6d 7075 7465 2061 7320 7063  ow.compute as pc
+000365e0: 0d0a 2020 2020 2020 2020 696d 706f 7274  ..        import
+000365f0: 2070 7961 7272 6f77 2e74 7970 6573 2061   pyarrow.types a
+00036600: 7320 7061 740d 0a0d 0a20 2020 2020 2020  s pat....       
+00036610: 2023 204d 616b 6520 7375 7265 2074 6865   # Make sure the
+00036620: 2069 6e70 7574 2061 7272 6179 2069 7320   input array is 
+00036630: 6f6e 6520 6f66 2074 6865 2070 7961 7272  one of the pyarr
+00036640: 6f77 2061 7272 6179 2074 7970 6573 2e0d  ow array types..
+00036650: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00036660: 6973 696e 7374 616e 6365 2861 7272 2c20  isinstance(arr, 
+00036670: 2870 612e 4172 7261 792c 2070 612e 4368  (pa.Array, pa.Ch
+00036680: 756e 6b65 6441 7272 6179 2929 3a0d 0a20  unkedArray)):.. 
+00036690: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000366a0: 2054 7970 6545 7272 6f72 2822 5468 6520   TypeError("The 
+000366b0: 6172 7261 7920 6973 206e 6f74 2061 6e20  array is not an 
+000366c0: 696e 7374 616e 6365 206f 6620 6070 7961  instance of `pya
+000366d0: 7272 6f77 2e41 7272 6179 6020 6f72 2060  rrow.Array` or `
+000366e0: 7079 6172 726f 772e 4368 756e 6b65 6441  pyarrow.ChunkedA
+000366f0: 7272 6179 602e 2229 0d0a 0d0a 2020 2020  rray`.")....    
+00036700: 2020 2020 2320 4368 756e 6b65 6441 7272      # ChunkedArr
+00036710: 6179 7320 6e65 6564 2073 7065 6369 616c  ays need special
+00036720: 2068 616e 646c 696e 672e 0d0a 2020 2020   handling...    
+00036730: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00036740: 6528 6172 722c 2070 612e 4368 756e 6b65  e(arr, pa.Chunke
+00036750: 6441 7272 6179 293a 0d0a 2020 2020 2020  dArray):..      
+00036760: 2020 2020 2020 2320 4120 7369 6e67 6c65        # A single
+00036770: 2d63 6875 6e6b 2043 6875 6e6b 6564 4172  -chunk ChunkedAr
+00036780: 7261 7920 6361 6e20 6265 2068 616e 646c  ray can be handl
+00036790: 6564 2062 7920 6a75 7374 2065 7874 7261  ed by just extra
+000367a0: 6374 696e 6720 7468 6174 2063 6875 6e6b  cting that chunk
+000367b0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+000367c0: 616e 6420 7265 6375 7273 6976 656c 7920  and recursively 
+000367d0: 7072 6f63 6573 7369 6e67 2069 742e 0d0a  processing it...
+000367e0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+000367f0: 7272 2e6e 756d 5f63 6875 6e6b 7320 3d3d  rr.num_chunks ==
+00036800: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+00036810: 2020 2020 2072 6574 7572 6e20 4661 7374       return Fast
+00036820: 4172 7261 792e 5f66 726f 6d5f 6172 726f  Array._from_arro
+00036830: 7728 0d0a 2020 2020 2020 2020 2020 2020  w(..            
+00036840: 2020 2020 2020 2020 6172 722e 6368 756e          arr.chun
+00036850: 6b28 3029 2c20 7a65 726f 5f63 6f70 795f  k(0), zero_copy_
+00036860: 6f6e 6c79 3d7a 6572 6f5f 636f 7079 5f6f  only=zero_copy_o
+00036870: 6e6c 792c 2077 7269 7461 626c 653d 7772  nly, writable=wr
+00036880: 6974 6162 6c65 2c20 6175 746f 5f77 6964  itable, auto_wid
+00036890: 656e 3d61 7574 6f5f 7769 6465 6e0d 0a20  en=auto_widen.. 
+000368a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000368b0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+000368c0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+000368d0: 2020 2020 2023 2054 4f44 4f3a 2042 656e       # TODO: Ben
+000368e0: 6368 6d61 726b 2074 6869 7320 7673 2e20  chmark this vs. 
+000368f0: 7573 696e 6720 4368 756e 6b65 6441 7272  using ChunkedArr
+00036900: 6179 2e63 6f6d 6269 6e65 5f63 6875 6e6b  ay.combine_chunk
+00036910: 7328 2920 7468 656e 2063 6f6e 7665 7274  s() then convert
+00036920: 696e 672e 0d0a 2020 2020 2020 2020 2020  ing...          
+00036930: 2020 2020 2020 2320 544f 444f 3a20 4c6f        # TODO: Lo
+00036940: 6f6b 2061 7420 607a 6572 6f5f 636f 7079  ok at `zero_copy
+00036950: 5f6f 6e6c 7960 2061 6e64 2060 7772 6974  _only` and `writ
+00036960: 6162 6c65 6020 2d2d 2074 6865 2063 6f6e  able` -- the con
+00036970: 7665 7274 6564 2061 7272 6179 7320 636f  verted arrays co
+00036980: 756c 6420 6265 2064 6573 7472 6f79 6564  uld be destroyed
+00036990: 2077 6869 6c65 2068 7374 6163 6b69 6e67   while hstacking
+000369a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000369b0: 2020 2320 2020 2020 2020 7369 6e63 6520    #       since 
+000369c0: 7765 206b 6e6f 7720 7468 6579 276c 6c20  we know they'll 
+000369d0: 6861 7665 206a 7573 7420 6265 656e 2063  have just been c
+000369e0: 7265 6174 6564 3b20 7468 6973 2063 6f75  reated; this cou
+000369f0: 6c64 2072 6564 7563 6520 7065 616b 206d  ld reduce peak m
+00036a00: 656d 6f72 7920 7574 696c 697a 6174 696f  emory utilizatio
+00036a10: 6e2e 0d0a 2020 2020 2020 2020 2020 2020  n...            
+00036a20: 2020 2020 7265 7475 726e 2068 7374 6163      return hstac
+00036a30: 6b28 0d0a 2020 2020 2020 2020 2020 2020  k(..            
+00036a40: 2020 2020 2020 2020 5b0d 0a20 2020 2020          [..     
 00036a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036a60: 2020 4661 7374 4172 7261 792e 5f66 726f    FastArray._fro
-00036a70: 6d5f 6172 726f 7728 0d0a 2020 2020 2020  m_arrow(..      
+00036a60: 2020 2046 6173 7441 7272 6179 2e5f 6672     FastArray._fr
+00036a70: 6f6d 5f61 7272 6f77 280d 0a20 2020 2020  om_arrow(..     
 00036a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036a90: 2020 2020 2020 6172 725f 6368 756e 6b2c        arr_chunk,
-00036aa0: 207a 6572 6f5f 636f 7079 5f6f 6e6c 793d   zero_copy_only=
-00036ab0: 7a65 726f 5f63 6f70 795f 6f6e 6c79 2c20  zero_copy_only, 
-00036ac0: 7772 6974 6162 6c65 3d77 7269 7461 626c  writable=writabl
-00036ad0: 652c 2061 7574 6f5f 7769 6465 6e3d 6175  e, auto_widen=au
-00036ae0: 746f 5f77 6964 656e 0d0a 2020 2020 2020  to_widen..      
+00036a90: 2020 2020 2020 2061 7272 5f63 6875 6e6b         arr_chunk
+00036aa0: 2c20 7a65 726f 5f63 6f70 795f 6f6e 6c79  , zero_copy_only
+00036ab0: 3d7a 6572 6f5f 636f 7079 5f6f 6e6c 792c  =zero_copy_only,
+00036ac0: 2077 7269 7461 626c 653d 7772 6974 6162   writable=writab
+00036ad0: 6c65 2c20 6175 746f 5f77 6964 656e 3d61  le, auto_widen=a
+00036ae0: 7574 6f5f 7769 6465 6e0d 0a20 2020 2020  uto_widen..     
 00036af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036b00: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00036b10: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00036b20: 2061 7272 5f63 6875 6e6b 2069 6e20 6172   arr_chunk in ar
-00036b30: 722e 6974 6572 6368 756e 6b73 2829 0d0a  r.iterchunks()..
-00036b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036b50: 2020 2020 5d0d 0a20 2020 2020 2020 2020      ]..         
-00036b60: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-00036b70: 2020 2020 2320 4861 6e64 6c65 2062 6173      # Handle bas
-00036b80: 6564 206f 6e20 7468 6520 7479 7065 206f  ed on the type o
-00036b90: 6620 7468 6520 696e 7075 7420 6172 7261  f the input arra
-00036ba0: 792e 0d0a 2020 2020 2020 2020 6966 2070  y...        if p
-00036bb0: 6174 2e69 735f 696e 7465 6765 7228 6172  at.is_integer(ar
-00036bc0: 722e 7479 7065 293a 0d0a 2020 2020 2020  r.type):..      
-00036bd0: 2020 2020 2020 2320 466f 7220 6172 7261        # For arra
-00036be0: 7973 206f 6620 7072 696d 6974 6976 6520  ys of primitive 
-00036bf0: 7479 7065 732c 2070 612e 4461 7461 5479  types, pa.DataTy
-00036c00: 7065 2e74 6f5f 7061 6e64 6173 5f64 7479  pe.to_pandas_dty
-00036c10: 7065 2829 2061 6374 7561 6c6c 7920 7265  pe() actually re
-00036c20: 7475 726e 7320 7468 6520 6571 7569 7661  turns the equiva
-00036c30: 6c65 6e74 206e 756d 7079 2064 7479 7065  lent numpy dtype
-00036c40: 2e0d 0a20 2020 2020 2020 2020 2020 2061  ...            a
-00036c50: 7272 5f64 7479 7065 203d 2061 7272 2e74  rr_dtype = arr.t
-00036c60: 7970 652e 746f 5f70 616e 6461 735f 6474  ype.to_pandas_dt
-00036c70: 7970 6528 290d 0a0d 0a20 2020 2020 2020  ype()....       
-00036c80: 2020 2020 2023 2047 6574 2074 6865 2072       # Get the r
-00036c90: 6970 7461 626c 6520 696e 7661 6c69 6420  iptable invalid 
-00036ca0: 7661 6c75 6520 666f 7220 7468 6973 2061  value for this a
-00036cb0: 7272 6179 2074 7970 652e 0d0a 2020 2020  rray type...    
-00036cc0: 2020 2020 2020 2020 6172 725f 7274 5f69          arr_rt_i
-00036cd0: 6e76 203d 2049 4e56 414c 4944 5f44 4943  nv = INVALID_DIC
-00036ce0: 545b 6e70 2e64 7479 7065 2861 7272 5f64  T[np.dtype(arr_d
-00036cf0: 7479 7065 292e 6e75 6d5d 0d0a 0d0a 2020  type).num]....  
-00036d00: 2020 2020 2020 2020 2020 2320 4765 7420            # Get 
-00036d10: 6d69 6e20 616e 6420 6d61 7820 7661 6c75  min and max valu
-00036d20: 6520 6f66 2074 6865 2069 6e70 7574 2061  e of the input a
-00036d30: 7272 6179 2c20 736f 2077 6520 6b6e 6f77  rray, so we know
-00036d40: 2069 6620 7765 206e 6565 6420 746f 2070   if we need to p
-00036d50: 726f 6d6f 7465 0d0a 2020 2020 2020 2020  romote..        
-00036d60: 2020 2020 2320 746f 2074 6865 206e 6578      # to the nex
-00036d70: 742d 6c61 7267 6573 7420 6474 7970 6520  t-largest dtype 
-00036d80: 746f 2062 6520 6162 6c65 2074 6f20 636f  to be able to co
-00036d90: 7272 6563 746c 7920 7265 7072 6573 656e  rrectly represen
-00036da0: 7420 6e75 6c6c 732e 0d0a 2020 2020 2020  t nulls...      
-00036db0: 2020 2020 2020 2320 5468 6973 206d 7573        # This mus
-00036dc0: 7420 6265 2064 6f6e 6520 6576 656e 2069  t be done even i
-00036dd0: 6620 7468 6520 696e 7075 7420 6172 7261  f the input arra
-00036de0: 7920 6861 7320 6e6f 206e 756c 6c73 2c20  y has no nulls, 
-00036df0: 6265 6361 7573 6520 6f74 6865 7277 6973  because otherwis
-00036e00: 6520 7468 6520 6e6f 6e2d 6e75 6c6c 0d0a  e the non-null..
-00036e10: 2020 2020 2020 2020 2020 2020 2320 7661              # va
-00036e20: 6c75 6573 2069 6e20 7468 6520 696e 7075  lues in the inpu
-00036e30: 7420 636f 7272 6573 706f 6e64 696e 6720  t corresponding 
-00036e40: 746f 2072 6970 7461 626c 6520 696e 7465  to riptable inte
-00036e50: 6765 7220 696e 7661 6c69 6473 2077 6f75  ger invalids wou
-00036e60: 6c64 2074 6865 6e20 6265 2072 6563 6f67  ld then be recog
-00036e70: 6e69 7a65 640d 0a20 2020 2020 2020 2020  nized..         
-00036e80: 2020 2023 2061 7320 7375 6368 2061 6674     # as such aft
-00036e90: 6572 2063 6f6e 7665 7273 696f 6e2e 0d0a  er conversion...
-00036ea0: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
-00036eb0: 6d61 785f 7265 7375 6c74 3a20 7061 2e53  max_result: pa.S
-00036ec0: 7472 7563 7453 6361 6c61 7220 3d20 7063  tructScalar = pc
-00036ed0: 2e6d 696e 5f6d 6178 2861 7272 290d 0a20  .min_max(arr).. 
-00036ee0: 2020 2020 2020 2020 2020 206d 696e 5f76             min_v
-00036ef0: 616c 7565 203d 206d 696e 5f6d 6178 5f72  alue = min_max_r
-00036f00: 6573 756c 745b 226d 696e 225d 0d0a 2020  esult["min"]..  
-00036f10: 2020 2020 2020 2020 2020 6d61 785f 7661            max_va
-00036f20: 6c75 6520 3d20 6d69 6e5f 6d61 785f 7265  lue = min_max_re
-00036f30: 7375 6c74 5b22 6d61 7822 5d0d 0a0d 0a20  sult["max"].... 
-00036f40: 2020 2020 2020 2020 2020 2061 7272 5f70             arr_p
-00036f50: 615f 6474 7970 655f 7769 6465 6e65 643a  a_dtype_widened:
-00036f60: 204f 7074 696f 6e61 6c5b 7061 2e44 6174   Optional[pa.Dat
-00036f70: 6154 7970 655d 203d 204e 6f6e 650d 0a20  aType] = None.. 
-00036f80: 2020 2020 2020 2020 2020 2069 6620 6d69             if mi
-00036f90: 6e5f 7661 6c75 6520 3d3d 2061 7272 5f72  n_value == arr_r
-00036fa0: 745f 696e 7620 6f72 206d 6178 5f76 616c  t_inv or max_val
-00036fb0: 7565 203d 3d20 6172 725f 7274 5f69 6e76  ue == arr_rt_inv
-00036fc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00036fd0: 2020 2023 2049 6620 7468 6520 696e 7075     # If the inpu
-00036fe0: 7420 6172 7261 7920 686f 6c64 7320 3634  t array holds 64
-00036ff0: 2d62 6974 2069 6e74 6567 6572 7320 2873  -bit integers (s
-00037000: 6967 6e65 6420 6f72 2075 6e73 6967 6e65  igned or unsigne
-00037010: 6429 2c20 7765 2063 616e 2774 2064 6f20  d), we can't do 
-00037020: 6120 6c6f 7373 6c65 7373 2063 6f6e 7665  a lossless conve
-00037030: 7273 696f 6e2c 0d0a 2020 2020 2020 2020  rsion,..        
-00037040: 2020 2020 2020 2020 2320 7369 6e63 6520          # since 
-00037050: 7468 6572 6520 6973 206e 6f20 7769 6465  there is no wide
-00037060: 7220 696e 7465 6765 7220 6176 6169 6c61  r integer availa
-00037070: 626c 652e 0d0a 2020 2020 2020 2020 2020  ble...          
-00037080: 2020 2020 2020 6966 207a 6572 6f5f 636f        if zero_co
-00037090: 7079 5f6f 6e6c 793a 0d0a 2020 2020 2020  py_only:..      
-000370a0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000370b0: 6973 6520 5661 6c75 6545 7272 6f72 280d  ise ValueError(.
-000370c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000370d0: 2020 2020 2020 2020 2022 4361 6e6e 6f74           "Cannot
-000370e0: 2070 6572 666f 726d 2061 207a 6572 6f2d   perform a zero-
-000370f0: 636f 7079 2063 6f6e 7665 7273 696f 6e20  copy conversion 
-00037100: 6f66 2061 6e20 6172 726f 7720 6172 7261  of an arrow arra
-00037110: 7920 636f 6e74 6169 6e69 6e67 2074 6865  y containing the
-00037120: 2072 6970 7461 626c 6520 696e 7661 6c69   riptable invali
-00037130: 6420 7661 6c75 6520 666f 7220 7468 6520  d value for the 
-00037140: 6172 7261 7920 6474 7970 652e 220d 0a20  array dtype.".. 
+00036b00: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+00036b10: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00036b20: 7220 6172 725f 6368 756e 6b20 696e 2061  r arr_chunk in a
+00036b30: 7272 2e69 7465 7263 6875 6e6b 7328 290d  rr.iterchunks().
+00036b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00036b50: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
+00036b60: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
+00036b70: 2020 2020 2023 2048 616e 646c 6520 6261       # Handle ba
+00036b80: 7365 6420 6f6e 2074 6865 2074 7970 6520  sed on the type 
+00036b90: 6f66 2074 6865 2069 6e70 7574 2061 7272  of the input arr
+00036ba0: 6179 2e0d 0a20 2020 2020 2020 2069 6620  ay...        if 
+00036bb0: 7061 742e 6973 5f69 6e74 6567 6572 2861  pat.is_integer(a
+00036bc0: 7272 2e74 7970 6529 3a0d 0a20 2020 2020  rr.type):..     
+00036bd0: 2020 2020 2020 2023 2046 6f72 2061 7272         # For arr
+00036be0: 6179 7320 6f66 2070 7269 6d69 7469 7665  ays of primitive
+00036bf0: 2074 7970 6573 2c20 7061 2e44 6174 6154   types, pa.DataT
+00036c00: 7970 652e 746f 5f70 616e 6461 735f 6474  ype.to_pandas_dt
+00036c10: 7970 6528 2920 6163 7475 616c 6c79 2072  ype() actually r
+00036c20: 6574 7572 6e73 2074 6865 2065 7175 6976  eturns the equiv
+00036c30: 616c 656e 7420 6e75 6d70 7920 6474 7970  alent numpy dtyp
+00036c40: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
+00036c50: 6172 725f 6474 7970 6520 3d20 6172 722e  arr_dtype = arr.
+00036c60: 7479 7065 2e74 6f5f 7061 6e64 6173 5f64  type.to_pandas_d
+00036c70: 7479 7065 2829 0d0a 0d0a 2020 2020 2020  type()....      
+00036c80: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
+00036c90: 7269 7074 6162 6c65 2069 6e76 616c 6964  riptable invalid
+00036ca0: 2076 616c 7565 2066 6f72 2074 6869 7320   value for this 
+00036cb0: 6172 7261 7920 7479 7065 2e0d 0a20 2020  array type...   
+00036cc0: 2020 2020 2020 2020 2061 7272 5f72 745f           arr_rt_
+00036cd0: 696e 7620 3d20 494e 5641 4c49 445f 4449  inv = INVALID_DI
+00036ce0: 4354 5b6e 702e 6474 7970 6528 6172 725f  CT[np.dtype(arr_
+00036cf0: 6474 7970 6529 2e6e 756d 5d0d 0a0d 0a20  dtype).num].... 
+00036d00: 2020 2020 2020 2020 2020 2023 2047 6574             # Get
+00036d10: 206d 696e 2061 6e64 206d 6178 2076 616c   min and max val
+00036d20: 7565 206f 6620 7468 6520 696e 7075 7420  ue of the input 
+00036d30: 6172 7261 792c 2073 6f20 7765 206b 6e6f  array, so we kno
+00036d40: 7720 6966 2077 6520 6e65 6564 2074 6f20  w if we need to 
+00036d50: 7072 6f6d 6f74 650d 0a20 2020 2020 2020  promote..       
+00036d60: 2020 2020 2023 2074 6f20 7468 6520 6e65       # to the ne
+00036d70: 7874 2d6c 6172 6765 7374 2064 7479 7065  xt-largest dtype
+00036d80: 2074 6f20 6265 2061 626c 6520 746f 2063   to be able to c
+00036d90: 6f72 7265 6374 6c79 2072 6570 7265 7365  orrectly represe
+00036da0: 6e74 206e 756c 6c73 2e0d 0a20 2020 2020  nt nulls...     
+00036db0: 2020 2020 2020 2023 2054 6869 7320 6d75         # This mu
+00036dc0: 7374 2062 6520 646f 6e65 2065 7665 6e20  st be done even 
+00036dd0: 6966 2074 6865 2069 6e70 7574 2061 7272  if the input arr
+00036de0: 6179 2068 6173 206e 6f20 6e75 6c6c 732c  ay has no nulls,
+00036df0: 2062 6563 6175 7365 206f 7468 6572 7769   because otherwi
+00036e00: 7365 2074 6865 206e 6f6e 2d6e 756c 6c0d  se the non-null.
+00036e10: 0a20 2020 2020 2020 2020 2020 2023 2076  .            # v
+00036e20: 616c 7565 7320 696e 2074 6865 2069 6e70  alues in the inp
+00036e30: 7574 2063 6f72 7265 7370 6f6e 6469 6e67  ut corresponding
+00036e40: 2074 6f20 7269 7074 6162 6c65 2069 6e74   to riptable int
+00036e50: 6567 6572 2069 6e76 616c 6964 7320 776f  eger invalids wo
+00036e60: 756c 6420 7468 656e 2062 6520 7265 636f  uld then be reco
+00036e70: 676e 697a 6564 0d0a 2020 2020 2020 2020  gnized..        
+00036e80: 2020 2020 2320 6173 2073 7563 6820 6166      # as such af
+00036e90: 7465 7220 636f 6e76 6572 7369 6f6e 2e0d  ter conversion..
+00036ea0: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
+00036eb0: 5f6d 6178 5f72 6573 756c 743a 2070 612e  _max_result: pa.
+00036ec0: 5374 7275 6374 5363 616c 6172 203d 2070  StructScalar = p
+00036ed0: 632e 6d69 6e5f 6d61 7828 6172 7229 0d0a  c.min_max(arr)..
+00036ee0: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
+00036ef0: 7661 6c75 6520 3d20 6d69 6e5f 6d61 785f  value = min_max_
+00036f00: 7265 7375 6c74 5b22 6d69 6e22 5d0d 0a20  result["min"].. 
+00036f10: 2020 2020 2020 2020 2020 206d 6178 5f76             max_v
+00036f20: 616c 7565 203d 206d 696e 5f6d 6178 5f72  alue = min_max_r
+00036f30: 6573 756c 745b 226d 6178 225d 0d0a 0d0a  esult["max"]....
+00036f40: 2020 2020 2020 2020 2020 2020 6172 725f              arr_
+00036f50: 7061 5f64 7479 7065 5f77 6964 656e 6564  pa_dtype_widened
+00036f60: 3a20 4f70 7469 6f6e 616c 5b70 612e 4461  : Optional[pa.Da
+00036f70: 7461 5479 7065 5d20 3d20 4e6f 6e65 0d0a  taType] = None..
+00036f80: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00036f90: 696e 5f76 616c 7565 203d 3d20 6172 725f  in_value == arr_
+00036fa0: 7274 5f69 6e76 206f 7220 6d61 785f 7661  rt_inv or max_va
+00036fb0: 6c75 6520 3d3d 2061 7272 5f72 745f 696e  lue == arr_rt_in
+00036fc0: 763a 0d0a 2020 2020 2020 2020 2020 2020  v:..            
+00036fd0: 2020 2020 2320 4966 2074 6865 2069 6e70      # If the inp
+00036fe0: 7574 2061 7272 6179 2068 6f6c 6473 2036  ut array holds 6
+00036ff0: 342d 6269 7420 696e 7465 6765 7273 2028  4-bit integers (
+00037000: 7369 676e 6564 206f 7220 756e 7369 676e  signed or unsign
+00037010: 6564 292c 2077 6520 6361 6e27 7420 646f  ed), we can't do
+00037020: 2061 206c 6f73 736c 6573 7320 636f 6e76   a lossless conv
+00037030: 6572 7369 6f6e 2c0d 0a20 2020 2020 2020  ersion,..       
+00037040: 2020 2020 2020 2020 2023 2073 696e 6365           # since
+00037050: 2074 6865 7265 2069 7320 6e6f 2077 6964   there is no wid
+00037060: 6572 2069 6e74 6567 6572 2061 7661 696c  er integer avail
+00037070: 6162 6c65 2e0d 0a20 2020 2020 2020 2020  able...         
+00037080: 2020 2020 2020 2069 6620 7a65 726f 5f63         if zero_c
+00037090: 6f70 795f 6f6e 6c79 3a0d 0a20 2020 2020  opy_only:..     
+000370a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000370b0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000370c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000370d0: 2020 2020 2020 2020 2020 2243 616e 6e6f            "Canno
+000370e0: 7420 7065 7266 6f72 6d20 6120 7a65 726f  t perform a zero
+000370f0: 2d63 6f70 7920 636f 6e76 6572 7369 6f6e  -copy conversion
+00037100: 206f 6620 616e 2061 7272 6f77 2061 7272   of an arrow arr
+00037110: 6179 2063 6f6e 7461 696e 696e 6720 7468  ay containing th
+00037120: 6520 7269 7074 6162 6c65 2069 6e76 616c  e riptable inval
+00037130: 6964 2076 616c 7565 2066 6f72 2074 6865  id value for the
+00037140: 2061 7272 6179 2064 7479 7065 2e22 0d0a   array dtype."..
 00037150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00037160: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-00037170: 2020 2020 2020 656c 6966 2061 7272 5f64        elif arr_d
-00037180: 7479 7065 2e69 7465 6d73 697a 6520 3d3d  type.itemsize ==
-00037190: 2038 3a0d 0a20 2020 2020 2020 2020 2020   8:..           
-000371a0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-000371b0: 616c 7565 4572 726f 7228 0d0a 2020 2020  alueError(..    
+00037160: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00037170: 2020 2020 2020 2065 6c69 6620 6172 725f         elif arr_
+00037180: 6474 7970 652e 6974 656d 7369 7a65 203d  dtype.itemsize =
+00037190: 3d20 383a 0d0a 2020 2020 2020 2020 2020  = 8:..          
+000371a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000371b0: 5661 6c75 6545 7272 6f72 280d 0a20 2020  ValueError(..   
 000371c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000371d0: 2020 2020 2243 616e 6e6f 7420 6c6f 7373      "Cannot loss
-000371e0: 6c65 7373 6c79 2063 6f6e 7665 7274 2061  lessly convert a
-000371f0: 6e20 6172 726f 7720 6172 7261 7920 6f66  n arrow array of
-00037200: 2028 7529 696e 7436 3420 636f 6e74 6169   (u)int64 contai
-00037210: 6e69 6e67 2074 6865 2072 6970 7461 626c  ning the riptabl
-00037220: 6520 696e 7661 6c69 6420 7661 6c75 6520  e invalid value 
-00037230: 746f 2061 2072 6970 7461 626c 6520 6172  to a riptable ar
-00037240: 7261 792e 220d 0a20 2020 2020 2020 2020  ray."..         
-00037250: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-00037260: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00037270: 6966 206e 6f74 2061 7574 6f5f 7769 6465  if not auto_wide
-00037280: 6e3a 0d0a 2020 2020 2020 2020 2020 2020  n:..            
-00037290: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-000372a0: 6c75 6545 7272 6f72 280d 0a20 2020 2020  lueError(..     
+000371d0: 2020 2020 2022 4361 6e6e 6f74 206c 6f73       "Cannot los
+000371e0: 736c 6573 736c 7920 636f 6e76 6572 7420  slessly convert 
+000371f0: 616e 2061 7272 6f77 2061 7272 6179 206f  an arrow array o
+00037200: 6620 2875 2969 6e74 3634 2063 6f6e 7461  f (u)int64 conta
+00037210: 696e 696e 6720 7468 6520 7269 7074 6162  ining the riptab
+00037220: 6c65 2069 6e76 616c 6964 2076 616c 7565  le invalid value
+00037230: 2074 6f20 6120 7269 7074 6162 6c65 2061   to a riptable a
+00037240: 7272 6179 2e22 0d0a 2020 2020 2020 2020  rray."..        
+00037250: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00037260: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00037270: 6c69 6620 6e6f 7420 6175 746f 5f77 6964  lif not auto_wid
+00037280: 656e 3a0d 0a20 2020 2020 2020 2020 2020  en:..           
+00037290: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+000372a0: 616c 7565 4572 726f 7228 0d0a 2020 2020  alueError(..    
 000372b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000372c0: 2020 2022 496e 7075 7420 6172 7261 7920     "Input array 
-000372d0: 7265 7175 6972 6573 2077 6964 656e 696e  requires widenin
-000372e0: 6720 666f 7220 6c6f 7373 6c65 7373 2063  g for lossless c
-000372f0: 6f6e 7665 7273 696f 6e2e 2053 7065 6369  onversion. Speci
-00037300: 6679 2061 7574 6f5f 7769 6465 6e3d 5472  fy auto_widen=Tr
-00037310: 7565 2069 6620 796f 7520 7761 6e74 2074  ue if you want t
-00037320: 6f20 616c 6c6f 7720 7468 6520 7769 6465  o allow the wide
-00037330: 6e69 6e67 2063 6f6e 7665 7273 696f 6e20  ning conversion 
-00037340: 2877 6869 6368 2072 6571 7569 7265 7320  (which requires 
-00037350: 616e 2061 7272 6179 2063 6f70 7929 2e22  an array copy)."
-00037360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00037370: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00037380: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00037390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000373a0: 2020 2020 2320 5769 6465 6e20 7468 6520      # Widen the 
-000373b0: 6474 7970 6520 6f66 2074 6865 206f 7574  dtype of the out
-000373c0: 7075 7420 6172 7261 792e 0d0a 2020 2020  put array...    
+000372c0: 2020 2020 2249 6e70 7574 2061 7272 6179      "Input array
+000372d0: 2072 6571 7569 7265 7320 7769 6465 6e69   requires wideni
+000372e0: 6e67 2066 6f72 206c 6f73 736c 6573 7320  ng for lossless 
+000372f0: 636f 6e76 6572 7369 6f6e 2e20 5370 6563  conversion. Spec
+00037300: 6966 7920 6175 746f 5f77 6964 656e 3d54  ify auto_widen=T
+00037310: 7275 6520 6966 2079 6f75 2077 616e 7420  rue if you want 
+00037320: 746f 2061 6c6c 6f77 2074 6865 2077 6964  to allow the wid
+00037330: 656e 696e 6720 636f 6e76 6572 7369 6f6e  ening conversion
+00037340: 2028 7768 6963 6820 7265 7175 6972 6573   (which requires
+00037350: 2061 6e20 6172 7261 7920 636f 7079 292e   an array copy).
+00037360: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00037370: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00037380: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00037390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000373a0: 2020 2020 2023 2057 6964 656e 2074 6865       # Widen the
+000373b0: 2064 7479 7065 206f 6620 7468 6520 6f75   dtype of the ou
+000373c0: 7470 7574 2061 7272 6179 2e0d 0a20 2020  tput array...   
 000373d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000373e0: 6f75 7470 7574 5f64 7479 7065 203d 206e  output_dtype = n
-000373f0: 702e 6d69 6e5f 7363 616c 6172 5f74 7970  p.min_scalar_typ
-00037400: 6528 3220 2a20 6172 725f 7274 5f69 6e76  e(2 * arr_rt_inv
-00037410: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00037420: 2020 2020 2020 2061 7272 5f70 615f 6474         arr_pa_dt
-00037430: 7970 655f 7769 6465 6e65 6420 3d20 7061  ype_widened = pa
-00037440: 2e66 726f 6d5f 6e75 6d70 795f 6474 7970  .from_numpy_dtyp
-00037450: 6528 6f75 7470 7574 5f64 7479 7065 290d  e(output_dtype).
-00037460: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
-00037470: 2043 7265 6174 6520 7468 6520 6f75 7470   Create the outp
-00037480: 7574 2061 7272 6179 2c20 7065 7266 6f72  ut array, perfor
-00037490: 6d69 6e67 2061 2077 6964 656e 696e 6720  ming a widening 
-000374a0: 636f 6e76 6572 7369 6f6e 202b 2066 696c  conversion + fil
-000374b0: 6c69 6e67 2069 6e20 6e75 6c6c 7320 7769  ling in nulls wi
-000374c0: 7468 2074 6865 2072 6970 7461 626c 6520  th the riptable 
-000374d0: 696e 7661 6c69 6420 6966 206e 6563 6573  invalid if neces
-000374e0: 7361 7279 2e0d 0a20 2020 2020 2020 2020  sary...         
-000374f0: 2020 2023 2054 4f44 4f3a 2054 6869 7320     # TODO: This 
-00037500: 636f 756c 6420 6265 2066 6173 7465 7220  could be faster 
-00037510: 2d2d 2069 6620 7468 6572 6527 7320 6120  -- if there's a 
-00037520: 7761 7920 746f 2067 6574 2061 206e 756d  way to get a num
-00037530: 7079 2062 6f6f 6c65 616e 2061 7272 6179  py boolean array
-00037540: 2066 726f 6d20 6120 7079 6172 726f 7720   from a pyarrow 
-00037550: 6172 7261 7927 7320 6e75 6c6c 2d6d 6173  array's null-mas
-00037560: 6b2c 0d0a 2020 2020 2020 2020 2020 2020  k,..            
-00037570: 2320 2020 2020 2020 7765 2063 616e 2063  #       we can c
-00037580: 6f6e 7665 7274 2064 6972 6563 746c 7920  onvert directly 
-00037590: 746f 206e 756d 7079 2f72 6970 7461 626c  to numpy/riptabl
-000375a0: 653b 2074 6865 6e2c 2077 6964 656e 2074  e; then, widen t
-000375b0: 6865 2046 6173 7441 7272 6179 2028 7768  he FastArray (wh
-000375c0: 6963 6827 6c6c 2062 6520 7061 7261 6c6c  ich'll be parall
-000375d0: 656c 697a 6564 293b 0d0a 2020 2020 2020  elized);..      
-000375e0: 2020 2020 2020 2320 2020 2020 2020 7468        #       th
-000375f0: 656e 2075 7365 2072 742e 636f 7079 5f74  en use rt.copy_t
-00037600: 6f28 2920 2f20 7274 2e70 7574 6d61 736b  o() / rt.putmask
-00037610: 2829 2074 6f20 6f76 6572 7772 6974 6520  () to overwrite 
-00037620: 7468 6520 656c 656d 656e 7473 206f 6620  the elements of 
-00037630: 7468 6520 7769 6465 6e65 6420 4661 7374  the widened Fast
-00037640: 4172 7261 790d 0a20 2020 2020 2020 2020  Array..         
-00037650: 2020 2023 2020 2020 2020 2063 6f72 7265     #       corre
-00037660: 7370 6f6e 6469 6e67 2074 6f20 7468 6520  sponding to the 
-00037670: 6e75 6c6c 7320 6672 6f6d 2074 6865 206d  nulls from the m
-00037680: 6173 6b20 7769 7468 2074 6865 2072 6970  ask with the rip
-00037690: 7461 626c 6520 696e 7661 6c69 6420 7661  table invalid va
-000376a0: 6c75 6520 666f 7220 7468 6520 6f75 7470  lue for the outp
-000376b0: 7574 2061 7272 6179 2074 7970 652e 0d0a  ut array type...
-000376c0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-000376d0: 7272 5f70 615f 6474 7970 655f 7769 6465  rr_pa_dtype_wide
-000376e0: 6e65 6420 6973 206e 6f74 204e 6f6e 653a  ned is not None:
-000376f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00037700: 2020 6172 723a 2070 612e 4172 7261 7920    arr: pa.Array 
-00037710: 3d20 6172 722e 6361 7374 2861 7272 5f70  = arr.cast(arr_p
-00037720: 615f 6474 7970 655f 7769 6465 6e65 6429  a_dtype_widened)
-00037730: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00037740: 7265 7475 726e 2061 7272 2e66 696c 6c5f  return arr.fill_
-00037750: 6e75 6c6c 2861 7272 5f72 745f 696e 7629  null(arr_rt_inv)
-00037760: 2e74 6f5f 6e75 6d70 7928 7a65 726f 5f63  .to_numpy(zero_c
-00037770: 6f70 795f 6f6e 6c79 3d46 616c 7365 2c20  opy_only=False, 
-00037780: 7772 6974 6162 6c65 3d77 7269 7461 626c  writable=writabl
-00037790: 6529 2e76 6965 7728 4661 7374 4172 7261  e).view(FastArra
-000377a0: 7929 0d0a 0d0a 2020 2020 2020 2020 656c  y)....        el
-000377b0: 6966 2070 6174 2e69 735f 666c 6f61 7469  if pat.is_floati
-000377c0: 6e67 2861 7272 2e74 7970 6529 3a0d 0a20  ng(arr.type):.. 
-000377d0: 2020 2020 2020 2020 2020 2023 2046 6c6f             # Flo
-000377e0: 6174 696e 672d 706f 696e 7420 6172 7261  ating-point arra
-000377f0: 7973 2063 616e 2062 6520 636f 6e76 6572  ys can be conver
-00037800: 7465 6420 6469 7265 6374 6c79 2074 6f20  ted directly to 
-00037810: 6e75 6d70 792c 2073 696e 6365 2070 7961  numpy, since pya
-00037820: 7272 6f77 2077 696c 6c20 6175 746f 6d61  rrow will automa
-00037830: 7469 6361 6c6c 790d 0a20 2020 2020 2020  tically..       
-00037840: 2020 2020 2023 2066 696c 6c20 6e75 6c6c       # fill null
-00037850: 2076 616c 7565 7320 7769 7468 204e 614e   values with NaN
-00037860: 2e0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
-00037870: 6574 7572 6e20 6172 722e 746f 5f6e 756d  eturn arr.to_num
-00037880: 7079 287a 6572 6f5f 636f 7079 5f6f 6e6c  py(zero_copy_onl
-00037890: 793d 7a65 726f 5f63 6f70 795f 6f6e 6c79  y=zero_copy_only
-000378a0: 2c20 7772 6974 6162 6c65 3d77 7269 7461  , writable=writa
-000378b0: 626c 6529 2e76 6965 7728 4661 7374 4172  ble).view(FastAr
-000378c0: 7261 7929 0d0a 0d0a 2020 2020 2020 2020  ray)....        
-000378d0: 656c 6966 2070 6174 2e69 735f 626f 6f6c  elif pat.is_bool
-000378e0: 6561 6e28 6172 722e 7479 7065 293a 0d0a  ean(arr.type):..
-000378f0: 2020 2020 2020 2020 2020 2020 2320 426f              # Bo
-00037900: 6f6c 6561 6e20 6172 7261 7973 2063 616e  olean arrays can
-00037910: 206f 6e6c 7920 6265 2063 6f6e 7665 7274   only be convert
-00037920: 6564 2077 6865 6e20 7468 6579 2064 6f20  ed when they do 
-00037930: 6e6f 7420 636f 6e74 6169 6e20 6e75 6c6c  not contain null
-00037940: 732e 0d0a 2020 2020 2020 2020 2020 2020  s...            
-00037950: 2320 7269 7074 6162 6c65 2064 6f65 7320  # riptable does 
-00037960: 6e6f 7420 7375 7070 6f72 7420 616e 2027  not support an '
-00037970: 696e 7661 6c69 6427 2f4e 4120 7661 6c75  invalid'/NA valu
-00037980: 6520 666f 7220 626f 6f6c 6561 6e2c 2073  e for boolean, s
-00037990: 6f20 7079 6172 726f 7720 6172 7261 7973  o pyarrow arrays
-000379a0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000379b0: 7769 7468 206e 756c 6c73 2063 616e 2774  with nulls can't
-000379c0: 2062 6520 7265 7072 6573 656e 7465 6420   be represented 
-000379d0: 696e 2072 6970 7461 626c 652e 0d0a 2020  in riptable...  
-000379e0: 2020 2020 2020 2020 2020 6966 2061 7272            if arr
-000379f0: 2e6e 756c 6c5f 636f 756e 7420 3d3d 2030  .null_count == 0
-00037a00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00037a10: 2020 2072 6574 7572 6e20 6172 722e 746f     return arr.to
-00037a20: 5f6e 756d 7079 287a 6572 6f5f 636f 7079  _numpy(zero_copy
-00037a30: 5f6f 6e6c 793d 7a65 726f 5f63 6f70 795f  _only=zero_copy_
-00037a40: 6f6e 6c79 2c20 7772 6974 6162 6c65 3d77  only, writable=w
-00037a50: 7269 7461 626c 6529 2e76 6965 7728 4661  ritable).view(Fa
-00037a60: 7374 4172 7261 7929 0d0a 2020 2020 2020  stArray)..      
-00037a70: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00037a80: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00037a90: 7365 2056 616c 7565 4572 726f 7228 0d0a  se ValueError(..
-00037aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00037ab0: 2020 2020 2272 6970 7461 626c 6520 626f      "riptable bo
-00037ac0: 6f6c 6561 6e20 6172 7261 7973 2064 6f20  olean arrays do 
-00037ad0: 6e6f 7420 7375 7070 6f72 7420 616e 2069  not support an i
-00037ae0: 6e76 616c 6964 2076 616c 7565 2c20 736f  nvalid value, so
-00037af0: 2074 6865 7920 6361 6e6e 6f74 2062 6520   they cannot be 
-00037b00: 6372 6561 7465 6420 6672 6f6d 2070 7961  created from pya
-00037b10: 7272 6f77 2061 7272 6179 7320 636f 6e74  rrow arrays cont
-00037b20: 6169 6e69 6e67 206e 756c 6c73 2e22 0d0a  aining nulls."..
-00037b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00037b40: 290d 0a0d 0a20 2020 2020 2020 2065 6c69  )....        eli
-00037b50: 6620 7061 742e 6973 5f73 7472 696e 6728  f pat.is_string(
-00037b60: 6172 722e 7479 7065 2920 6f72 2070 6174  arr.type) or pat
-00037b70: 2e69 735f 6c61 7267 655f 7374 7269 6e67  .is_large_string
-00037b80: 2861 7272 2e74 7970 6529 3a0d 0a20 2020  (arr.type):..   
-00037b90: 2020 2020 2020 2020 2023 2070 7961 7272           # pyarr
-00037ba0: 6f77 2076 6172 6961 626c 652d 6c65 6e67  ow variable-leng
-00037bb0: 7468 2073 7472 696e 6720 6172 7261 7973  th string arrays
-00037bc0: 2063 616e 205f 6e65 7665 725f 2062 6520   can _never_ be 
-00037bd0: 7a65 726f 2d63 6f70 7920 636f 6e76 6572  zero-copy conver
-00037be0: 7465 6420 746f 2066 6978 6564 2d6c 656e  ted to fixed-len
-00037bf0: 6774 6820 6e75 6d70 792f 7269 7074 6162  gth numpy/riptab
-00037c00: 6c65 2061 7272 6179 730d 0a20 2020 2020  le arrays..     
-00037c10: 2020 2020 2020 2023 2062 6563 6175 7365         # because
-00037c20: 206f 6620 6469 6666 6572 656e 6365 7320   of differences 
-00037c30: 696e 2074 6865 206d 656d 6f72 7920 6c61  in the memory la
-00037c40: 796f 7574 2e0d 0a20 2020 2020 2020 2020  yout...         
-00037c50: 2020 2069 6620 7a65 726f 5f63 6f70 795f     if zero_copy_
-00037c60: 6f6e 6c79 3a0d 0a20 2020 2020 2020 2020  only:..         
-00037c70: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00037c80: 7565 4572 726f 7228 0d0a 2020 2020 2020  ueError(..      
-00037c90: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00037ca0: 7961 7272 6f77 2076 6172 6961 626c 652d  yarrow variable-
-00037cb0: 6c65 6e67 7468 2073 7472 696e 6720 6172  length string ar
-00037cc0: 7261 7973 2063 616e 6e6f 7420 6265 207a  rays cannot be z
-00037cd0: 6572 6f2d 636f 7079 2063 6f6e 7665 7274  ero-copy convert
-00037ce0: 6564 2074 6f20 7269 7074 6162 6c65 2061  ed to riptable a
-00037cf0: 7272 6179 732e 220d 0a20 2020 2020 2020  rrays."..       
-00037d00: 2020 2020 2020 2020 2029 0d0a 0d0a 2020           )....  
-00037d10: 2020 2020 2020 2020 2020 2320 4368 6563            # Chec
-00037d20: 6b20 666f 7220 7768 6574 6865 7220 7468  k for whether th
-00037d30: 6520 6172 7261 7920 636f 6e74 6169 6e73  e array contains
-00037d40: 206f 6e6c 7920 4153 4349 4920 7374 7269   only ASCII stri
-00037d50: 6e67 732e 0d0a 2020 2020 2020 2020 2020  ngs...          
-00037d60: 2020 2320 5468 6973 2069 7320 7573 6564    # This is used
-00037d70: 2074 6f20 6775 6964 6520 686f 7720 7468   to guide how th
-00037d80: 6520 4661 7374 4172 7261 7920 6973 2063  e FastArray is c
-00037d90: 7265 6174 6564 2e0d 0a20 2020 2020 2020  reated...       
-00037da0: 2020 2020 2068 6173 5f75 6e69 636f 6465       has_unicode
-00037db0: 203d 206e 6f74 2070 632e 616c 6c28 7063   = not pc.all(pc
-00037dc0: 2e73 7472 696e 675f 6973 5f61 7363 6969  .string_is_ascii
-00037dd0: 2861 7272 2929 0d0a 0d0a 2020 2020 2020  (arr))....      
-00037de0: 2020 2020 2020 2320 436f 6e76 6572 7420        # Convert 
-00037df0: 7468 6520 6172 7261 7920 746f 2061 206e  the array to a n
-00037e00: 756d 7079 2061 7272 6179 2e0d 0a20 2020  umpy array...   
-00037e10: 2020 2020 2020 2020 2023 2055 6e66 6f72           # Unfor
-00037e20: 7475 6e61 7465 6c79 2c20 6173 206f 6620  tunately, as of 
-00037e30: 7079 6172 726f 7720 342e 302c 2074 6869  pyarrow 4.0, thi
-00037e40: 7320 636f 6e76 6572 7369 6f6e 2061 6c77  s conversion alw
-00037e50: 6179 7320 7072 6f64 7563 6573 2061 206e  ays produces a n
-00037e60: 756d 7079 206f 626a 6563 7420 6172 7261  umpy object arra
-00037e70: 7920 636f 6e74 6169 6e69 6e67 2074 6865  y containing the
-00037e80: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00037e90: 7374 7269 6e67 7320 2861 7320 5079 7468  strings (as Pyth
-00037ea0: 6f6e 2073 7472 696e 6773 2920 7261 7468  on strings) rath
-00037eb0: 6572 2074 6861 6e20 6120 6e75 6d70 7920  er than a numpy 
-00037ec0: 7374 7269 6e67 2061 7272 6179 2e0d 0a20  string array... 
-00037ed0: 2020 2020 2020 2020 2020 2023 2057 6527             # We'
-00037ee0: 7265 2061 626c 6520 746f 2068 616e 646c  re able to handl
-00037ef0: 6520 7468 6973 2074 6f20 7265 7475 726e  e this to return
-00037f00: 2074 6865 2073 656e 7369 626c 6520 7468   the sensible th
-00037f10: 696e 6720 666f 7220 7269 7074 6162 6c65  ing for riptable
-00037f20: 2075 7365 7273 2c20 6275 7420 6974 2064   users, but it d
-00037f30: 6f65 7320 6d65 616e 2074 6869 7320 636f  oes mean this co
-00037f40: 6e76 6572 7369 6f6e 0d0a 2020 2020 2020  nversion..      
-00037f50: 2020 2020 2020 2320 6973 2073 6c6f 7765        # is slowe
-00037f60: 7220 7468 616e 206e 6563 6573 7361 7279  r than necessary
-00037f70: 2072 6967 6874 206e 6f77 2e0d 0a20 2020   right now...   
-00037f80: 2020 2020 2020 2020 2023 2054 4f44 4f3a           # TODO:
-00037f90: 2041 736b 2070 7961 7272 6f77 2d64 6576   Ask pyarrow-dev
-00037fa0: 2061 626f 7574 2069 6d70 6c65 6d65 6e74   about implement
-00037fb0: 696e 6720 616e 206f 7074 696f 6e20 746f  ing an option to
-00037fc0: 2072 6574 7572 6e20 6120 6e75 6d70 7920   return a numpy 
-00037fd0: 2753 2720 6f72 2027 5527 2061 7272 6179  'S' or 'U' array
-00037fe0: 2069 6e73 7465 6164 2c20 6974 276c 6c20   instead, it'll 
-00037ff0: 6265 0d0a 2020 2020 2020 2020 2020 2020  be..            
-00038000: 2320 2020 2020 2020 6d75 6368 206d 6f72  #       much mor
-00038010: 6520 6566 6669 6369 656e 742c 2065 7665  e efficient, eve
-00038020: 6e20 7468 6f75 6768 2073 6f6d 6520 7370  n though some sp
-00038030: 6163 6520 7769 6c6c 2062 6520 7761 7374  ace will be wast
-00038040: 6564 2064 7565 2074 6f20 6e75 6d70 7920  ed due to numpy 
-00038050: 6e6f 7420 7375 7070 6f72 7469 6e67 2076  not supporting v
-00038060: 6172 6961 626c 652d 6c65 6e67 7468 2073  ariable-length s
-00038070: 7472 696e 6773 2e0d 0a20 2020 2020 2020  trings...       
-00038080: 2020 2020 2023 2054 4f44 4f3a 2043 6f6e       # TODO: Con
-00038090: 7369 6465 7220 636f 6e76 6572 7469 6e67  sider converting
-000380a0: 2074 6865 2070 7961 7272 6f77 2061 7272   the pyarrow arr
-000380b0: 6179 2074 6f20 6120 6469 6374 696f 6e61  ay to a dictiona
-000380c0: 7279 2d65 6e63 6f64 6564 2061 7272 6179  ry-encoded array
-000380d0: 202d 2d20 6966 2074 6865 7265 2061 7265   -- if there are
-000380e0: 206f 6e6c 7920 6120 6665 7720 756e 6971   only a few uniq
-000380f0: 7565 732c 0d0a 2020 2020 2020 2020 2020  ues,..          
-00038100: 2020 2320 2020 2020 2020 6974 276c 6c20    #       it'll 
-00038110: 6265 206d 6f72 6520 6566 6669 6369 656e  be more efficien
-00038120: 7420 2865 7665 6e20 7468 6f75 6768 2064  t (even though d
-00038130: 6f69 6e67 206d 6f72 6520 776f 726b 2920  oing more work) 
-00038140: 6279 2061 766f 6964 696e 6720 7265 7065  by avoiding repe
-00038150: 7469 7469 7665 2063 7265 6174 696f 6e20  titive creation 
-00038160: 6f66 2074 6865 2050 7974 686f 6e20 7374  of the Python st
-00038170: 7269 6e67 206f 626a 6563 7473 2e0d 0a20  ring objects... 
-00038180: 2020 2020 2020 2020 2020 2069 6620 6172             if ar
-00038190: 722e 6e75 6c6c 5f63 6f75 6e74 203d 3d20  r.null_count == 
-000381a0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-000381b0: 2020 2020 746d 7020 3d20 6172 722e 746f      tmp = arr.to
-000381c0: 5f6e 756d 7079 287a 6572 6f5f 636f 7079  _numpy(zero_copy
-000381d0: 5f6f 6e6c 793d 4661 6c73 652c 2077 7269  _only=False, wri
-000381e0: 7461 626c 653d 7772 6974 6162 6c65 290d  table=writable).
-000381f0: 0a0d 0a20 2020 2020 2020 2020 2020 2065  ...            e
-00038200: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00038210: 2020 2020 2020 2320 4e65 6564 2074 6f20        # Need to 
-00038220: 6669 6c6c 206e 756c 6c73 2077 6974 6820  fill nulls with 
-00038230: 616e 2065 6d70 7479 2073 7472 696e 6720  an empty string 
-00038240: 6265 666f 7265 2063 6f6e 7665 7274 696e  before convertin
-00038250: 6720 746f 206e 756d 7079 2e0d 0a20 2020  g to numpy...   
-00038260: 2020 2020 2020 2020 2020 2020 2023 2028               # (
-00038270: 494e 5641 4c49 445f 4449 4354 5b6e 702e  INVALID_DICT[np.
-00038280: 6474 7970 6528 2755 2729 2e6e 756d 5d20  dtype('U').num] 
-00038290: 3d3d 2027 2729 2e0d 0a20 2020 2020 2020  == '')...       
-000382a0: 2020 2020 2020 2020 2074 6d70 203d 2061           tmp = a
-000382b0: 7272 2e66 696c 6c5f 6e75 6c6c 2822 2229  rr.fill_null("")
-000382c0: 2e74 6f5f 6e75 6d70 7928 7a65 726f 5f63  .to_numpy(zero_c
-000382d0: 6f70 795f 6f6e 6c79 3d46 616c 7365 2c20  opy_only=False, 
-000382e0: 7772 6974 6162 6c65 3d77 7269 7461 626c  writable=writabl
-000382f0: 6529 0d0a 0d0a 2020 2020 2020 2020 2020  e)....          
-00038300: 2020 7265 7375 6c74 203d 2046 6173 7441    result = FastA
-00038310: 7272 6179 2874 6d70 2c20 6474 7970 653d  rray(tmp, dtype=
-00038320: 7374 722c 2075 6e69 636f 6465 3d68 6173  str, unicode=has
-00038330: 5f75 6e69 636f 6465 290d 0a20 2020 2020  _unicode)..     
-00038340: 2020 2020 2020 2069 6620 6e6f 7420 7772         if not wr
-00038350: 6974 6162 6c65 3a0d 0a20 2020 2020 2020  itable:..       
-00038360: 2020 2020 2020 2020 2072 6573 756c 742e           result.
-00038370: 666c 6167 732e 7772 6974 6561 626c 6520  flags.writeable 
-00038380: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
-00038390: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-000383a0: 6c74 0d0a 0d0a 2020 2020 2020 2020 656c  lt....        el
-000383b0: 6966 2070 6174 2e69 735f 6669 7865 645f  if pat.is_fixed_
-000383c0: 7369 7a65 5f62 696e 6172 7928 6172 722e  size_binary(arr.
-000383d0: 7479 7065 293a 0d0a 2020 2020 2020 2020  type):..        
-000383e0: 2020 2020 6e75 6c6c 5f63 6f75 6e74 203d      null_count =
-000383f0: 2061 7272 2e6e 756c 6c5f 636f 756e 740d   arr.null_count.
-00038400: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00038410: 6e75 6c6c 5f63 6f75 6e74 2021 3d20 303a  null_count != 0:
-00038420: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00038430: 2020 6966 207a 6572 6f5f 636f 7079 5f6f    if zero_copy_o
-00038440: 6e6c 793a 0d0a 2020 2020 2020 2020 2020  nly:..          
-00038450: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00038460: 5661 6c75 6545 7272 6f72 280d 0a20 2020  ValueError(..   
+000373e0: 206f 7574 7075 745f 6474 7970 6520 3d20   output_dtype = 
+000373f0: 6e70 2e6d 696e 5f73 6361 6c61 725f 7479  np.min_scalar_ty
+00037400: 7065 2832 202a 2061 7272 5f72 745f 696e  pe(2 * arr_rt_in
+00037410: 7629 0d0a 2020 2020 2020 2020 2020 2020  v)..            
+00037420: 2020 2020 2020 2020 6172 725f 7061 5f64          arr_pa_d
+00037430: 7479 7065 5f77 6964 656e 6564 203d 2070  type_widened = p
+00037440: 612e 6672 6f6d 5f6e 756d 7079 5f64 7479  a.from_numpy_dty
+00037450: 7065 286f 7574 7075 745f 6474 7970 6529  pe(output_dtype)
+00037460: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00037470: 2320 4372 6561 7465 2074 6865 206f 7574  # Create the out
+00037480: 7075 7420 6172 7261 792c 2070 6572 666f  put array, perfo
+00037490: 726d 696e 6720 6120 7769 6465 6e69 6e67  rming a widening
+000374a0: 2063 6f6e 7665 7273 696f 6e20 2b20 6669   conversion + fi
+000374b0: 6c6c 696e 6720 696e 206e 756c 6c73 2077  lling in nulls w
+000374c0: 6974 6820 7468 6520 7269 7074 6162 6c65  ith the riptable
+000374d0: 2069 6e76 616c 6964 2069 6620 6e65 6365   invalid if nece
+000374e0: 7373 6172 792e 0d0a 2020 2020 2020 2020  ssary...        
+000374f0: 2020 2020 2320 544f 444f 3a20 5468 6973      # TODO: This
+00037500: 2063 6f75 6c64 2062 6520 6661 7374 6572   could be faster
+00037510: 202d 2d20 6966 2074 6865 7265 2773 2061   -- if there's a
+00037520: 2077 6179 2074 6f20 6765 7420 6120 6e75   way to get a nu
+00037530: 6d70 7920 626f 6f6c 6561 6e20 6172 7261  mpy boolean arra
+00037540: 7920 6672 6f6d 2061 2070 7961 7272 6f77  y from a pyarrow
+00037550: 2061 7272 6179 2773 206e 756c 6c2d 6d61   array's null-ma
+00037560: 736b 2c0d 0a20 2020 2020 2020 2020 2020  sk,..           
+00037570: 2023 2020 2020 2020 2077 6520 6361 6e20   #       we can 
+00037580: 636f 6e76 6572 7420 6469 7265 6374 6c79  convert directly
+00037590: 2074 6f20 6e75 6d70 792f 7269 7074 6162   to numpy/riptab
+000375a0: 6c65 3b20 7468 656e 2c20 7769 6465 6e20  le; then, widen 
+000375b0: 7468 6520 4661 7374 4172 7261 7920 2877  the FastArray (w
+000375c0: 6869 6368 276c 6c20 6265 2070 6172 616c  hich'll be paral
+000375d0: 6c65 6c69 7a65 6429 3b0d 0a20 2020 2020  lelized);..     
+000375e0: 2020 2020 2020 2023 2020 2020 2020 2074         #       t
+000375f0: 6865 6e20 7573 6520 7274 2e63 6f70 795f  hen use rt.copy_
+00037600: 746f 2829 202f 2072 742e 7075 746d 6173  to() / rt.putmas
+00037610: 6b28 2920 746f 206f 7665 7277 7269 7465  k() to overwrite
+00037620: 2074 6865 2065 6c65 6d65 6e74 7320 6f66   the elements of
+00037630: 2074 6865 2077 6964 656e 6564 2046 6173   the widened Fas
+00037640: 7441 7272 6179 0d0a 2020 2020 2020 2020  tArray..        
+00037650: 2020 2020 2320 2020 2020 2020 636f 7272      #       corr
+00037660: 6573 706f 6e64 696e 6720 746f 2074 6865  esponding to the
+00037670: 206e 756c 6c73 2066 726f 6d20 7468 6520   nulls from the 
+00037680: 6d61 736b 2077 6974 6820 7468 6520 7269  mask with the ri
+00037690: 7074 6162 6c65 2069 6e76 616c 6964 2076  ptable invalid v
+000376a0: 616c 7565 2066 6f72 2074 6865 206f 7574  alue for the out
+000376b0: 7075 7420 6172 7261 7920 7479 7065 2e0d  put array type..
+000376c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000376d0: 6172 725f 7061 5f64 7479 7065 5f77 6964  arr_pa_dtype_wid
+000376e0: 656e 6564 2069 7320 6e6f 7420 4e6f 6e65  ened is not None
+000376f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00037700: 2020 2061 7272 3a20 7061 2e41 7272 6179     arr: pa.Array
+00037710: 203d 2061 7272 2e63 6173 7428 6172 725f   = arr.cast(arr_
+00037720: 7061 5f64 7479 7065 5f77 6964 656e 6564  pa_dtype_widened
+00037730: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00037740: 2072 6574 7572 6e20 6172 722e 6669 6c6c   return arr.fill
+00037750: 5f6e 756c 6c28 6172 725f 7274 5f69 6e76  _null(arr_rt_inv
+00037760: 292e 746f 5f6e 756d 7079 287a 6572 6f5f  ).to_numpy(zero_
+00037770: 636f 7079 5f6f 6e6c 793d 4661 6c73 652c  copy_only=False,
+00037780: 2077 7269 7461 626c 653d 7772 6974 6162   writable=writab
+00037790: 6c65 292e 7669 6577 2846 6173 7441 7272  le).view(FastArr
+000377a0: 6179 290d 0a0d 0a20 2020 2020 2020 2065  ay)....        e
+000377b0: 6c69 6620 7061 742e 6973 5f66 6c6f 6174  lif pat.is_float
+000377c0: 696e 6728 6172 722e 7479 7065 293a 0d0a  ing(arr.type):..
+000377d0: 2020 2020 2020 2020 2020 2020 2320 466c              # Fl
+000377e0: 6f61 7469 6e67 2d70 6f69 6e74 2061 7272  oating-point arr
+000377f0: 6179 7320 6361 6e20 6265 2063 6f6e 7665  ays can be conve
+00037800: 7274 6564 2064 6972 6563 746c 7920 746f  rted directly to
+00037810: 206e 756d 7079 2c20 7369 6e63 6520 7079   numpy, since py
+00037820: 6172 726f 7720 7769 6c6c 2061 7574 6f6d  arrow will autom
+00037830: 6174 6963 616c 6c79 0d0a 2020 2020 2020  atically..      
+00037840: 2020 2020 2020 2320 6669 6c6c 206e 756c        # fill nul
+00037850: 6c20 7661 6c75 6573 2077 6974 6820 4e61  l values with Na
+00037860: 4e2e 0d0a 2020 2020 2020 2020 2020 2020  N...            
+00037870: 7265 7475 726e 2061 7272 2e74 6f5f 6e75  return arr.to_nu
+00037880: 6d70 7928 7a65 726f 5f63 6f70 795f 6f6e  mpy(zero_copy_on
+00037890: 6c79 3d7a 6572 6f5f 636f 7079 5f6f 6e6c  ly=zero_copy_onl
+000378a0: 792c 2077 7269 7461 626c 653d 7772 6974  y, writable=writ
+000378b0: 6162 6c65 292e 7669 6577 2846 6173 7441  able).view(FastA
+000378c0: 7272 6179 290d 0a0d 0a20 2020 2020 2020  rray)....       
+000378d0: 2065 6c69 6620 7061 742e 6973 5f62 6f6f   elif pat.is_boo
+000378e0: 6c65 616e 2861 7272 2e74 7970 6529 3a0d  lean(arr.type):.
+000378f0: 0a20 2020 2020 2020 2020 2020 2023 2042  .            # B
+00037900: 6f6f 6c65 616e 2061 7272 6179 7320 6361  oolean arrays ca
+00037910: 6e20 6f6e 6c79 2062 6520 636f 6e76 6572  n only be conver
+00037920: 7465 6420 7768 656e 2074 6865 7920 646f  ted when they do
+00037930: 206e 6f74 2063 6f6e 7461 696e 206e 756c   not contain nul
+00037940: 6c73 2e0d 0a20 2020 2020 2020 2020 2020  ls...           
+00037950: 2023 2072 6970 7461 626c 6520 646f 6573   # riptable does
+00037960: 206e 6f74 2073 7570 706f 7274 2061 6e20   not support an 
+00037970: 2769 6e76 616c 6964 272f 4e41 2076 616c  'invalid'/NA val
+00037980: 7565 2066 6f72 2062 6f6f 6c65 616e 2c20  ue for boolean, 
+00037990: 736f 2070 7961 7272 6f77 2061 7272 6179  so pyarrow array
+000379a0: 730d 0a20 2020 2020 2020 2020 2020 2023  s..            #
+000379b0: 2077 6974 6820 6e75 6c6c 7320 6361 6e27   with nulls can'
+000379c0: 7420 6265 2072 6570 7265 7365 6e74 6564  t be represented
+000379d0: 2069 6e20 7269 7074 6162 6c65 2e0d 0a20   in riptable... 
+000379e0: 2020 2020 2020 2020 2020 2069 6620 6172             if ar
+000379f0: 722e 6e75 6c6c 5f63 6f75 6e74 203d 3d20  r.null_count == 
+00037a00: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00037a10: 2020 2020 7265 7475 726e 2061 7272 2e74      return arr.t
+00037a20: 6f5f 6e75 6d70 7928 7a65 726f 5f63 6f70  o_numpy(zero_cop
+00037a30: 795f 6f6e 6c79 3d7a 6572 6f5f 636f 7079  y_only=zero_copy
+00037a40: 5f6f 6e6c 792c 2077 7269 7461 626c 653d  _only, writable=
+00037a50: 7772 6974 6162 6c65 292e 7669 6577 2846  writable).view(F
+00037a60: 6173 7441 7272 6179 290d 0a20 2020 2020  astArray)..     
+00037a70: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00037a80: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00037a90: 6973 6520 5661 6c75 6545 7272 6f72 280d  ise ValueError(.
+00037aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00037ab0: 2020 2020 2022 7269 7074 6162 6c65 2062       "riptable b
+00037ac0: 6f6f 6c65 616e 2061 7272 6179 7320 646f  oolean arrays do
+00037ad0: 206e 6f74 2073 7570 706f 7274 2061 6e20   not support an 
+00037ae0: 696e 7661 6c69 6420 7661 6c75 652c 2073  invalid value, s
+00037af0: 6f20 7468 6579 2063 616e 6e6f 7420 6265  o they cannot be
+00037b00: 2063 7265 6174 6564 2066 726f 6d20 7079   created from py
+00037b10: 6172 726f 7720 6172 7261 7973 2063 6f6e  arrow arrays con
+00037b20: 7461 696e 696e 6720 6e75 6c6c 732e 220d  taining nulls.".
+00037b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00037b40: 2029 0d0a 0d0a 2020 2020 2020 2020 656c   )....        el
+00037b50: 6966 2070 6174 2e69 735f 7374 7269 6e67  if pat.is_string
+00037b60: 2861 7272 2e74 7970 6529 206f 7220 7061  (arr.type) or pa
+00037b70: 742e 6973 5f6c 6172 6765 5f73 7472 696e  t.is_large_strin
+00037b80: 6728 6172 722e 7479 7065 293a 0d0a 2020  g(arr.type):..  
+00037b90: 2020 2020 2020 2020 2020 2320 7079 6172            # pyar
+00037ba0: 726f 7720 7661 7269 6162 6c65 2d6c 656e  row variable-len
+00037bb0: 6774 6820 7374 7269 6e67 2061 7272 6179  gth string array
+00037bc0: 7320 6361 6e20 5f6e 6576 6572 5f20 6265  s can _never_ be
+00037bd0: 207a 6572 6f2d 636f 7079 2063 6f6e 7665   zero-copy conve
+00037be0: 7274 6564 2074 6f20 6669 7865 642d 6c65  rted to fixed-le
+00037bf0: 6e67 7468 206e 756d 7079 2f72 6970 7461  ngth numpy/ripta
+00037c00: 626c 6520 6172 7261 7973 0d0a 2020 2020  ble arrays..    
+00037c10: 2020 2020 2020 2020 2320 6265 6361 7573          # becaus
+00037c20: 6520 6f66 2064 6966 6665 7265 6e63 6573  e of differences
+00037c30: 2069 6e20 7468 6520 6d65 6d6f 7279 206c   in the memory l
+00037c40: 6179 6f75 742e 0d0a 2020 2020 2020 2020  ayout...        
+00037c50: 2020 2020 6966 207a 6572 6f5f 636f 7079      if zero_copy
+00037c60: 5f6f 6e6c 793a 0d0a 2020 2020 2020 2020  _only:..        
+00037c70: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00037c80: 6c75 6545 7272 6f72 280d 0a20 2020 2020  lueError(..     
+00037c90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00037ca0: 7079 6172 726f 7720 7661 7269 6162 6c65  pyarrow variable
+00037cb0: 2d6c 656e 6774 6820 7374 7269 6e67 2061  -length string a
+00037cc0: 7272 6179 7320 6361 6e6e 6f74 2062 6520  rrays cannot be 
+00037cd0: 7a65 726f 2d63 6f70 7920 636f 6e76 6572  zero-copy conver
+00037ce0: 7465 6420 746f 2072 6970 7461 626c 6520  ted to riptable 
+00037cf0: 6172 7261 7973 2e22 0d0a 2020 2020 2020  arrays."..      
+00037d00: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
+00037d10: 2020 2020 2020 2020 2020 2023 2043 6865             # Che
+00037d20: 636b 2066 6f72 2077 6865 7468 6572 2074  ck for whether t
+00037d30: 6865 2061 7272 6179 2063 6f6e 7461 696e  he array contain
+00037d40: 7320 6f6e 6c79 2041 5343 4949 2073 7472  s only ASCII str
+00037d50: 696e 6773 2e0d 0a20 2020 2020 2020 2020  ings...         
+00037d60: 2020 2023 2054 6869 7320 6973 2075 7365     # This is use
+00037d70: 6420 746f 2067 7569 6465 2068 6f77 2074  d to guide how t
+00037d80: 6865 2046 6173 7441 7272 6179 2069 7320  he FastArray is 
+00037d90: 6372 6561 7465 642e 0d0a 2020 2020 2020  created...      
+00037da0: 2020 2020 2020 6861 735f 756e 6963 6f64        has_unicod
+00037db0: 6520 3d20 6e6f 7420 7063 2e61 6c6c 2870  e = not pc.all(p
+00037dc0: 632e 7374 7269 6e67 5f69 735f 6173 6369  c.string_is_asci
+00037dd0: 6928 6172 7229 290d 0a0d 0a20 2020 2020  i(arr))....     
+00037de0: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
+00037df0: 2074 6865 2061 7272 6179 2074 6f20 6120   the array to a 
+00037e00: 6e75 6d70 7920 6172 7261 792e 0d0a 2020  numpy array...  
+00037e10: 2020 2020 2020 2020 2020 2320 556e 666f            # Unfo
+00037e20: 7274 756e 6174 656c 792c 2061 7320 6f66  rtunately, as of
+00037e30: 2070 7961 7272 6f77 2034 2e30 2c20 7468   pyarrow 4.0, th
+00037e40: 6973 2063 6f6e 7665 7273 696f 6e20 616c  is conversion al
+00037e50: 7761 7973 2070 726f 6475 6365 7320 6120  ways produces a 
+00037e60: 6e75 6d70 7920 6f62 6a65 6374 2061 7272  numpy object arr
+00037e70: 6179 2063 6f6e 7461 696e 696e 6720 7468  ay containing th
+00037e80: 650d 0a20 2020 2020 2020 2020 2020 2023  e..            #
+00037e90: 2073 7472 696e 6773 2028 6173 2050 7974   strings (as Pyt
+00037ea0: 686f 6e20 7374 7269 6e67 7329 2072 6174  hon strings) rat
+00037eb0: 6865 7220 7468 616e 2061 206e 756d 7079  her than a numpy
+00037ec0: 2073 7472 696e 6720 6172 7261 792e 0d0a   string array...
+00037ed0: 2020 2020 2020 2020 2020 2020 2320 5765              # We
+00037ee0: 2772 6520 6162 6c65 2074 6f20 6861 6e64  're able to hand
+00037ef0: 6c65 2074 6869 7320 746f 2072 6574 7572  le this to retur
+00037f00: 6e20 7468 6520 7365 6e73 6962 6c65 2074  n the sensible t
+00037f10: 6869 6e67 2066 6f72 2072 6970 7461 626c  hing for riptabl
+00037f20: 6520 7573 6572 732c 2062 7574 2069 7420  e users, but it 
+00037f30: 646f 6573 206d 6561 6e20 7468 6973 2063  does mean this c
+00037f40: 6f6e 7665 7273 696f 6e0d 0a20 2020 2020  onversion..     
+00037f50: 2020 2020 2020 2023 2069 7320 736c 6f77         # is slow
+00037f60: 6572 2074 6861 6e20 6e65 6365 7373 6172  er than necessar
+00037f70: 7920 7269 6768 7420 6e6f 772e 0d0a 2020  y right now...  
+00037f80: 2020 2020 2020 2020 2020 2320 544f 444f            # TODO
+00037f90: 3a20 4173 6b20 7079 6172 726f 772d 6465  : Ask pyarrow-de
+00037fa0: 7620 6162 6f75 7420 696d 706c 656d 656e  v about implemen
+00037fb0: 7469 6e67 2061 6e20 6f70 7469 6f6e 2074  ting an option t
+00037fc0: 6f20 7265 7475 726e 2061 206e 756d 7079  o return a numpy
+00037fd0: 2027 5327 206f 7220 2755 2720 6172 7261   'S' or 'U' arra
+00037fe0: 7920 696e 7374 6561 642c 2069 7427 6c6c  y instead, it'll
+00037ff0: 2062 650d 0a20 2020 2020 2020 2020 2020   be..           
+00038000: 2023 2020 2020 2020 206d 7563 6820 6d6f   #       much mo
+00038010: 7265 2065 6666 6963 6965 6e74 2c20 6576  re efficient, ev
+00038020: 656e 2074 686f 7567 6820 736f 6d65 2073  en though some s
+00038030: 7061 6365 2077 696c 6c20 6265 2077 6173  pace will be was
+00038040: 7465 6420 6475 6520 746f 206e 756d 7079  ted due to numpy
+00038050: 206e 6f74 2073 7570 706f 7274 696e 6720   not supporting 
+00038060: 7661 7269 6162 6c65 2d6c 656e 6774 6820  variable-length 
+00038070: 7374 7269 6e67 732e 0d0a 2020 2020 2020  strings...      
+00038080: 2020 2020 2020 2320 544f 444f 3a20 436f        # TODO: Co
+00038090: 6e73 6964 6572 2063 6f6e 7665 7274 696e  nsider convertin
+000380a0: 6720 7468 6520 7079 6172 726f 7720 6172  g the pyarrow ar
+000380b0: 7261 7920 746f 2061 2064 6963 7469 6f6e  ray to a diction
+000380c0: 6172 792d 656e 636f 6465 6420 6172 7261  ary-encoded arra
+000380d0: 7920 2d2d 2069 6620 7468 6572 6520 6172  y -- if there ar
+000380e0: 6520 6f6e 6c79 2061 2066 6577 2075 6e69  e only a few uni
+000380f0: 7175 6573 2c0d 0a20 2020 2020 2020 2020  ques,..         
+00038100: 2020 2023 2020 2020 2020 2069 7427 6c6c     #       it'll
+00038110: 2062 6520 6d6f 7265 2065 6666 6963 6965   be more efficie
+00038120: 6e74 2028 6576 656e 2074 686f 7567 6820  nt (even though 
+00038130: 646f 696e 6720 6d6f 7265 2077 6f72 6b29  doing more work)
+00038140: 2062 7920 6176 6f69 6469 6e67 2072 6570   by avoiding rep
+00038150: 6574 6974 6976 6520 6372 6561 7469 6f6e  etitive creation
+00038160: 206f 6620 7468 6520 5079 7468 6f6e 2073   of the Python s
+00038170: 7472 696e 6720 6f62 6a65 6374 732e 0d0a  tring objects...
+00038180: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+00038190: 7272 2e6e 756c 6c5f 636f 756e 7420 3d3d  rr.null_count ==
+000381a0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+000381b0: 2020 2020 2074 6d70 203d 2061 7272 2e74       tmp = arr.t
+000381c0: 6f5f 6e75 6d70 7928 7a65 726f 5f63 6f70  o_numpy(zero_cop
+000381d0: 795f 6f6e 6c79 3d46 616c 7365 2c20 7772  y_only=False, wr
+000381e0: 6974 6162 6c65 3d77 7269 7461 626c 6529  itable=writable)
+000381f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00038200: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00038210: 2020 2020 2020 2023 204e 6565 6420 746f         # Need to
+00038220: 2066 696c 6c20 6e75 6c6c 7320 7769 7468   fill nulls with
+00038230: 2061 6e20 656d 7074 7920 7374 7269 6e67   an empty string
+00038240: 2062 6566 6f72 6520 636f 6e76 6572 7469   before converti
+00038250: 6e67 2074 6f20 6e75 6d70 792e 0d0a 2020  ng to numpy...  
+00038260: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00038270: 2849 4e56 414c 4944 5f44 4943 545b 6e70  (INVALID_DICT[np
+00038280: 2e64 7479 7065 2827 5527 292e 6e75 6d5d  .dtype('U').num]
+00038290: 203d 3d20 2727 292e 0d0a 2020 2020 2020   == '')...      
+000382a0: 2020 2020 2020 2020 2020 746d 7020 3d20            tmp = 
+000382b0: 6172 722e 6669 6c6c 5f6e 756c 6c28 2222  arr.fill_null(""
+000382c0: 292e 746f 5f6e 756d 7079 287a 6572 6f5f  ).to_numpy(zero_
+000382d0: 636f 7079 5f6f 6e6c 793d 4661 6c73 652c  copy_only=False,
+000382e0: 2077 7269 7461 626c 653d 7772 6974 6162   writable=writab
+000382f0: 6c65 290d 0a0d 0a20 2020 2020 2020 2020  le)....         
+00038300: 2020 2072 6573 756c 7420 3d20 4661 7374     result = Fast
+00038310: 4172 7261 7928 746d 702c 2064 7479 7065  Array(tmp, dtype
+00038320: 3d73 7472 2c20 756e 6963 6f64 653d 6861  =str, unicode=ha
+00038330: 735f 756e 6963 6f64 6529 0d0a 2020 2020  s_unicode)..    
+00038340: 2020 2020 2020 2020 6966 206e 6f74 2077          if not w
+00038350: 7269 7461 626c 653a 0d0a 2020 2020 2020  ritable:..      
+00038360: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00038370: 2e66 6c61 6773 2e77 7269 7465 6162 6c65  .flags.writeable
+00038380: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+00038390: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000383a0: 756c 740d 0a0d 0a20 2020 2020 2020 2065  ult....        e
+000383b0: 6c69 6620 7061 742e 6973 5f66 6978 6564  lif pat.is_fixed
+000383c0: 5f73 697a 655f 6269 6e61 7279 2861 7272  _size_binary(arr
+000383d0: 2e74 7970 6529 3a0d 0a20 2020 2020 2020  .type):..       
+000383e0: 2020 2020 206e 756c 6c5f 636f 756e 7420       null_count 
+000383f0: 3d20 6172 722e 6e75 6c6c 5f63 6f75 6e74  = arr.null_count
+00038400: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00038410: 206e 756c 6c5f 636f 756e 7420 213d 2030   null_count != 0
+00038420: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00038430: 2020 2069 6620 7a65 726f 5f63 6f70 795f     if zero_copy_
+00038440: 6f6e 6c79 3a0d 0a20 2020 2020 2020 2020  only:..         
+00038450: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00038460: 2056 616c 7565 4572 726f 7228 0d0a 2020   ValueError(..  
 00038470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00038480: 2020 2020 2022 4361 6e27 7420 7065 7266       "Can't perf
-00038490: 6f72 6d20 6120 7a65 726f 2d63 6f70 7920  orm a zero-copy 
-000384a0: 636f 6e76 6572 7369 6f6e 206f 6620 6120  conversion of a 
-000384b0: 6669 7865 642d 7369 7a65 2062 696e 6172  fixed-size binar
-000384c0: 7920 6172 7261 7920 746f 2072 6970 7461  y array to ripta
-000384d0: 626c 6520 7768 656e 2074 6865 2069 6e70  ble when the inp
-000384e0: 7574 2061 7272 6179 2063 6f6e 7461 696e  ut array contain
-000384f0: 7320 6e75 6c6c 732e 220d 0a20 2020 2020  s nulls."..     
-00038500: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00038510: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00038520: 2020 2020 6172 7220 3d20 6172 722e 6669      arr = arr.fi
-00038530: 6c6c 5f6e 756c 6c28 0d0a 2020 2020 2020  ll_null(..      
-00038540: 2020 2020 2020 2020 2020 2020 2020 6222                b"
-00038550: 5c78 3030 2220 2a20 6172 722e 7479 7065  \x00" * arr.type
-00038560: 2e62 7974 655f 7769 6474 680d 0a20 2020  .byte_width..   
-00038570: 2020 2020 2020 2020 2020 2020 2029 2020               )  
-00038580: 2320 6361 6e27 7420 6669 6c6c 2077 6974  # can't fill wit
-00038590: 6820 6222 222c 2073 696e 6365 2062 2222  h b"", since b""
-000385a0: 2069 7320 6e6f 7420 7661 6c69 6420 666f   is not valid fo
-000385b0: 7220 6669 7865 6420 7769 6474 6820 7479  r fixed width ty
-000385c0: 7065 0d0a 0d0a 2020 2020 2020 2020 2020  pe....          
-000385d0: 2020 2320 4361 6c6c 696e 6720 7061 2e41    # Calling pa.A
-000385e0: 7272 6179 2e74 6f5f 6e75 6d70 7920 7769  rray.to_numpy wi
-000385f0: 7468 207a 6572 6f5f 636f 7079 3d54 7275  th zero_copy=Tru
-00038600: 6520 7261 6973 6573 2061 6e20 6572 726f  e raises an erro
-00038610: 7220 7769 7468 2066 6978 6564 2073 697a  r with fixed siz
-00038620: 6564 2062 696e 6172 7920 7479 7065 2e0d  ed binary type..
-00038630: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
-00038640: 616c 6c69 6e67 2070 612e 4172 7261 792e  alling pa.Array.
-00038650: 746f 5f6e 756d 7079 2077 6974 6820 7a65  to_numpy with ze
-00038660: 726f 5f63 6f70 793d 4661 6c73 6520 7265  ro_copy=False re
-00038670: 7475 726e 7320 6120 6e75 6d70 7920 6172  turns a numpy ar
-00038680: 7261 7920 7768 6572 6520 7479 7065 7320  ray where types 
-00038690: 6172 6520 7079 7468 6f6e 2062 7974 6573  are python bytes
-000386a0: 206f 626a 6563 7473 2e0d 0a20 2020 2020   objects...     
-000386b0: 2020 2020 2020 2023 2057 6f72 6b61 726f         # Workaro
-000386c0: 756e 6420 6265 6c6f 7720 6372 6561 7465  und below create
-000386d0: 7320 7468 6520 6e75 6d70 7920 6275 6666  s the numpy buff
-000386e0: 6572 206f 6620 7479 7065 2022 5322 206d  er of type "S" m
-000386f0: 616e 7561 6c6c 792e 0d0a 2020 2020 2020  anually...      
-00038700: 2020 2020 2020 6275 6620 3d20 6e70 2e66        buf = np.f
-00038710: 726f 6d62 7566 6665 7228 0d0a 2020 2020  rombuffer(..    
-00038720: 2020 2020 2020 2020 2020 2020 6172 722e              arr.
-00038730: 6275 6666 6572 7328 295b 315d 2c0d 0a20  buffers()[1],.. 
-00038740: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00038750: 7479 7065 3d22 5322 202b 2073 7472 2861  type="S" + str(a
-00038760: 7272 2e74 7970 652e 6279 7465 5f77 6964  rr.type.byte_wid
-00038770: 7468 292c 0d0a 2020 2020 2020 2020 2020  th),..          
-00038780: 2020 290d 0a0d 0a20 2020 2020 2020 2020    )....         
-00038790: 2020 2069 6620 7772 6974 6162 6c65 2061     if writable a
-000387a0: 6e64 206e 756c 6c5f 636f 756e 7420 3d3d  nd null_count ==
-000387b0: 2030 3a20 2023 2061 6c72 6561 6479 206d   0:  # already m
-000387c0: 6164 6520 6120 636f 7079 2069 6620 6e75  ade a copy if nu
-000387d0: 6c6c 5f63 6f75 6e74 2021 3d20 300d 0a20  ll_count != 0.. 
-000387e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000387f0: 6573 756c 7420 3d20 4661 7374 4172 7261  esult = FastArra
-00038800: 7928 6e70 2e63 6f70 7928 6275 6629 290d  y(np.copy(buf)).
-00038810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00038820: 2072 6573 756c 742e 666c 6167 732e 7772   result.flags.wr
-00038830: 6974 6561 626c 6520 3d20 7772 6974 6162  iteable = writab
-00038840: 6c65 0d0a 2020 2020 2020 2020 2020 2020  le..            
-00038850: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00038860: 740d 0a0d 0a20 2020 2020 2020 2020 2020  t....           
-00038870: 2072 6573 756c 7420 3d20 4661 7374 4172   result = FastAr
-00038880: 7261 7928 6275 6629 0d0a 2020 2020 2020  ray(buf)..      
-00038890: 2020 2020 2020 7265 7375 6c74 2e66 6c61        result.fla
-000388a0: 6773 2e77 7269 7465 6162 6c65 203d 2077  gs.writeable = w
-000388b0: 7269 7461 626c 650d 0a20 2020 2020 2020  ritable..       
-000388c0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-000388d0: 6c74 0d0a 0d0a 2020 2020 2020 2020 656c  lt....        el
-000388e0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000388f0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00038900: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
-00038910: 2020 2020 6622 4661 7374 4172 7261 7920      f"FastArray 
-00038920: 6361 6e6e 6f74 2062 6520 6372 6561 7465  cannot be create
-00038930: 6420 6672 6f6d 2061 2070 7961 7272 6f77  d from a pyarrow
-00038940: 2061 7272 6179 206f 6620 7479 7065 2027   array of type '
-00038950: 7b61 7272 2e74 7970 657d 272e 2059 6f75  {arr.type}'. You
-00038960: 206d 6179 206e 6565 6420 746f 2063 616c   may need to cal
-00038970: 6c20 7468 6520 6066 726f 6d5f 6172 726f  l the `from_arro
-00038980: 7760 206d 6574 686f 6420 6f6e 206f 6e65  w` method on one
-00038990: 206f 6620 7468 6520 6465 7269 7665 6420   of the derived 
-000389a0: 7375 6263 6c61 7373 6573 2069 6e73 7465  subclasses inste
-000389b0: 6164 2e22 0d0a 2020 2020 2020 2020 2020  ad."..          
-000389c0: 2020 290d 0a0d 0a20 2020 2064 6566 2074    )....    def t
-000389d0: 6f5f 6172 726f 7728 0d0a 2020 2020 2020  o_arrow(..      
-000389e0: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-000389f0: 2074 7970 653a 204f 7074 696f 6e61 6c5b   type: Optional[
-00038a00: 2270 612e 4461 7461 5479 7065 225d 203d  "pa.DataType"] =
-00038a10: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00038a20: 2a2c 0d0a 2020 2020 2020 2020 7072 6573  *,..        pres
-00038a30: 6572 7665 5f66 6978 6564 5f62 7974 6573  erve_fixed_bytes
-00038a40: 3a20 626f 6f6c 203d 2046 616c 7365 2c0d  : bool = False,.
-00038a50: 0a20 2020 2020 2020 2065 6d70 7479 5f73  .        empty_s
-00038a60: 7472 696e 6773 5f74 6f5f 6e75 6c6c 3a20  trings_to_null: 
-00038a70: 626f 6f6c 203d 2054 7275 652c 0d0a 2020  bool = True,..  
-00038a80: 2020 2920 2d3e 2055 6e69 6f6e 5b22 7061    ) -> Union["pa
-00038a90: 2e41 7272 6179 222c 2022 7061 2e43 6875  .Array", "pa.Chu
-00038aa0: 6e6b 6564 4172 7261 7922 5d3a 0d0a 2020  nkedArray"]:..  
-00038ab0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00038ac0: 2020 2043 6f6e 7665 7274 2074 6869 7320     Convert this 
-00038ad0: 6046 6173 7441 7272 6179 6020 746f 2061  `FastArray` to a
-00038ae0: 2060 7079 6172 726f 772e 4172 7261 7960   `pyarrow.Array`
-00038af0: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
-00038b00: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
-00038b10: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
-00038b20: 2020 2020 2074 7970 6520 3a20 7079 6172       type : pyar
-00038b30: 726f 772e 4461 7461 5479 7065 2c20 6f70  row.DataType, op
-00038b40: 7469 6f6e 616c 2c20 6465 6661 756c 7473  tional, defaults
-00038b50: 2074 6f20 4e6f 6e65 0d0a 2020 2020 2020   to None..      
-00038b60: 2020 7072 6573 6572 7665 5f66 6978 6564    preserve_fixed
-00038b70: 5f62 7974 6573 203a 2062 6f6f 6c2c 206f  _bytes : bool, o
-00038b80: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
-00038b90: 7320 746f 2046 616c 7365 0d0a 2020 2020  s to False..    
-00038ba0: 2020 2020 2020 2020 4966 2074 6869 7320          If this 
-00038bb0: 6046 6173 7441 7272 6179 6020 6973 2061  `FastArray` is a
-00038bc0: 6e20 4153 4349 4920 7374 7269 6e67 2061  n ASCII string a
-00038bd0: 7272 6179 2028 6474 7970 652e 6b69 6e64  rray (dtype.kind
-00038be0: 203d 3d20 2753 2729 2c0d 0a20 2020 2020   == 'S'),..     
-00038bf0: 2020 2020 2020 2073 6574 2074 6869 7320         set this 
-00038c00: 7061 7261 6d65 7465 7220 746f 2054 7275  parameter to Tru
-00038c10: 6520 746f 2070 726f 6475 6365 2061 2066  e to produce a f
-00038c20: 6978 6564 2d6c 656e 6774 6820 6269 6e61  ixed-length bina
-00038c30: 7279 2061 7272 6179 0d0a 2020 2020 2020  ry array..      
-00038c40: 2020 2020 2020 696e 7374 6561 6420 6f66        instead of
-00038c50: 2061 2076 6172 6961 626c 652d 6c65 6e67   a variable-leng
-00038c60: 7468 2073 7472 696e 6720 6172 7261 792e  th string array.
-00038c70: 0d0a 2020 2020 2020 2020 656d 7074 795f  ..        empty_
-00038c80: 7374 7269 6e67 735f 746f 5f6e 756c 6c20  strings_to_null 
-00038c90: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
-00038ca0: 2c20 6465 6661 756c 7473 2054 6f20 5472  , defaults To Tr
-00038cb0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00038cc0: 4966 2074 6869 7320 6046 6173 7441 7272  If this `FastArr
-00038cd0: 6179 6020 6973 2061 6e20 4153 4349 4920  ay` is an ASCII 
-00038ce0: 6f72 2055 6e69 636f 6465 2073 7472 696e  or Unicode strin
-00038cf0: 6720 6172 7261 792c 0d0a 2020 2020 2020  g array,..      
-00038d00: 2020 2020 2020 7370 6563 6966 7920 5472        specify Tr
-00038d10: 7565 2066 6f72 2074 6869 7320 7061 7261  ue for this para
-00038d20: 6d65 7465 7220 746f 2063 6f6e 7665 7274  meter to convert
-00038d30: 2065 6d70 7479 2073 7472 696e 6773 2074   empty strings t
-00038d40: 6f20 6e75 6c6c 7320 696e 2074 6865 206f  o nulls in the o
-00038d50: 7574 7075 742e 0d0a 2020 2020 2020 2020  utput...        
-00038d60: 2020 2020 7269 7074 6162 6c65 2069 6e63      riptable inc
-00038d70: 6f6e 7369 7374 656e 746c 7920 7265 636f  onsistently reco
-00038d80: 676e 697a 6573 2074 6865 2065 6d70 7479  gnizes the empty
-00038d90: 2073 7472 696e 6720 6173 2061 6e20 2769   string as an 'i
-00038da0: 6e76 616c 6964 272c 0d0a 2020 2020 2020  nvalid',..      
-00038db0: 2020 2020 2020 736f 2074 6869 7320 7061        so this pa
-00038dc0: 7261 6d65 7465 7220 616c 6c6f 7773 2074  rameter allows t
-00038dd0: 6865 2063 616c 6c65 7220 746f 2073 7065  he caller to spe
-00038de0: 6369 6679 2077 6869 6368 2069 6e74 6572  cify which inter
-00038df0: 7072 6574 6174 696f 6e0d 0a20 2020 2020  pretation..     
-00038e00: 2020 2020 2020 2074 6865 7920 7761 6e74         they want
-00038e10: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
-00038e20: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
-00038e30: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2070  -----..        p
-00038e40: 7961 7272 6f77 2e41 7272 6179 206f 7220  yarrow.Array or 
-00038e50: 7079 6172 726f 772e 4368 756e 6b65 6441  pyarrow.ChunkedA
-00038e60: 7272 6179 0d0a 0d0a 2020 2020 2020 2020  rray....        
-00038e70: 4e6f 7465 730d 0a20 2020 2020 2020 202d  Notes..        -
-00038e80: 2d2d 2d2d 0d0a 2020 2020 2020 2020 544f  ----..        TO
-00038e90: 444f 3a20 4164 6420 626f 6f6c 2070 6172  DO: Add bool par
-00038ea0: 616d 6574 6572 2077 6869 6368 2064 6972  ameter which dir
-00038eb0: 6563 7473 2074 6865 2063 6f6e 7665 7273  ects the convers
-00038ec0: 696f 6e20 746f 2063 686f 6f73 6520 7468  ion to choose th
-00038ed0: 6520 6d6f 7374 2d63 6f6d 7061 6374 206f  e most-compact o
-00038ee0: 7574 7075 7420 7479 7065 2070 6f73 7369  utput type possi
-00038ef0: 626c 653f 0d0a 2020 2020 2020 2020 2020  ble?..          
-00038f00: 2020 2020 5468 6973 2077 6f75 6c64 2062      This would b
-00038f10: 6520 7265 6c65 7661 6e74 2074 6f20 696e  e relevant to in
-00038f20: 6469 6365 7320 6f66 2063 6174 6567 6f72  dices of categor
-00038f30: 6963 616c 2f64 6963 7469 6f6e 6172 792d  ical/dictionary-
-00038f40: 656e 636f 6465 6420 6172 7261 7973 2c20  encoded arrays, 
-00038f50: 6275 7420 636f 756c 6420 616c 736f 206d  but could also m
-00038f60: 616b 6520 7365 6e73 650d 0a20 2020 2020  ake sense..     
-00038f70: 2020 2020 2020 2020 2066 6f72 2072 6567           for reg
-00038f80: 756c 6172 2046 6173 7441 7272 6179 2074  ular FastArray t
-00038f90: 7970 6573 2028 652e 672e 2074 6f20 7573  ypes (e.g. to us
-00038fa0: 6520 616e 2069 6e74 3820 696e 7374 6561  e an int8 instea
-00038fb0: 6420 6f66 2061 6e20 696e 7433 3220 7768  d of an int32 wh
-00038fc0: 656e 2069 7427 6420 6265 2061 206c 6f73  en it'd be a los
-00038fd0: 736c 6573 7320 636f 6e76 6572 7369 6f6e  sless conversion
-00038fe0: 292e 0d0a 2020 2020 2020 2020 2222 220d  )...        """.
-00038ff0: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00039000: 6275 696c 7469 6e73 0d0a 0d0a 2020 2020  builtins....    
-00039010: 2020 2020 696d 706f 7274 2070 7961 7272      import pyarr
-00039020: 6f77 2061 7320 7061 0d0a 0d0a 2020 2020  ow as pa....    
-00039030: 2020 2020 2320 4465 7269 7665 6420 6172      # Derived ar
-00039040: 7261 7920 7479 7065 7320 4d55 5354 2069  ray types MUST i
-00039050: 6d70 6c65 6d65 6e74 2074 6865 6972 206f  mplement their o
-00039060: 776e 206f 7665 726c 6f61 6420 6f66 2074  wn overload of t
-00039070: 6869 7320 6675 6e63 7469 6f6e 0d0a 2020  his function..  
-00039080: 2020 2020 2020 2320 666f 7220 636f 7272        # for corr
-00039090: 6563 746e 6573 733b 2066 6f72 2074 6861  ectness; for tha
-000390a0: 7420 7265 6173 6f6e 2c20 7261 6973 6520  t reason, raise 
-000390b0: 616e 2065 7272 6f72 2069 6620 736f 6d65  an error if some
-000390c0: 6f6e 6520 6174 7465 6d70 7473 2074 6f0d  one attempts to.
-000390d0: 0a20 2020 2020 2020 2023 2063 616c 6c20  .        # call 
-000390e0: 2a74 6869 732a 2069 6d70 6c65 6d65 6e74  *this* implement
-000390f0: 6174 696f 6e20 6f66 2074 6865 206d 6574  ation of the met
-00039100: 686f 6420 666f 7220 6120 6465 7269 7665  hod for a derive
-00039110: 6420 6172 7261 7920 7479 7065 2e0d 0a20  d array type... 
-00039120: 2020 2020 2020 2069 6620 6275 696c 7469         if builti
-00039130: 6e73 2e74 7970 6528 7365 6c66 2920 213d  ns.type(self) !=
-00039140: 2046 6173 7441 7272 6179 3a0d 0a20 2020   FastArray:..   
-00039150: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
-00039160: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-00039170: 6f72 280d 0a20 2020 2020 2020 2020 2020  or(..           
-00039180: 2020 2020 2066 2254 6865 2060 7b62 7569       f"The `{bui
-00039190: 6c74 696e 732e 7479 7065 2873 656c 6629  ltins.type(self)
-000391a0: 2e5f 5f71 7561 6c6e 616d 655f 5f7d 6020  .__qualname__}` 
-000391b0: 7479 7065 206d 7573 7420 696d 706c 656d  type must implem
-000391c0: 656e 7420 6974 2773 206f 776e 206f 7665  ent it's own ove
-000391d0: 7272 6964 6520 6f66 2074 6865 2060 746f  rride of the `to
-000391e0: 5f61 7272 6f77 2829 6020 6d65 7468 6f64  _arrow()` method
-000391f0: 2e22 0d0a 2020 2020 2020 2020 2020 2020  ."..            
-00039200: 290d 0a0d 0a20 2020 2020 2020 2023 2072  )....        # r
-00039210: 6970 7461 626c 6520 2861 7420 6c65 6173  iptable (at leas
-00039220: 7420 6173 206f 6620 312e 302e 3536 2920  t as of 1.0.56) 
-00039230: 646f 6573 206e 6f74 202a 7472 756c 792a  does not *truly*
-00039240: 2073 7570 706f 7274 2069 6e76 616c 6964   support invalid
-00039250: 2f4e 4120 7661 6c75 6573 0d0a 2020 2020  /NA values..    
-00039260: 2020 2020 2320 696e 2062 6f6f 6c20 6f72      # in bool or
-00039270: 2061 7363 6969 2f75 6e69 636f 6465 2073   ascii/unicode s
-00039280: 7472 696e 672d 7479 7065 6420 6172 7261  tring-typed arra
-00039290: 7973 2e20 4861 6e64 6c65 2074 686f 7365  ys. Handle those
-000392a0: 2064 7479 7065 7320 7370 6563 6961 6c6c   dtypes speciall
-000392b0: 792e 0d0a 2020 2020 2020 2020 6966 206e  y...        if n
-000392c0: 702e 6973 7375 6264 7479 7065 2873 656c  p.issubdtype(sel
-000392d0: 662e 6474 7970 652c 206e 702e 696e 7465  f.dtype, np.inte
-000392e0: 6765 7229 3a0d 0a20 2020 2020 2020 2020  ger):..         
-000392f0: 2020 2023 2054 4f44 4f3a 2049 6620 7468     # TODO: If th
-00039300: 6973 2061 7272 6179 2068 6173 202e 6e64  is array has .nd
-00039310: 696d 7320 3e3d 2032 2c20 6e65 6564 2074  ims >= 2, need t
-00039320: 6f20 636f 6e76 6572 7420 746f 2070 7961  o convert to pya
-00039330: 7272 6f77 2075 7369 6e67 2070 612e 5465  rrow using pa.Te
-00039340: 6e73 6f72 2e66 726f 6d5f 6e75 6d70 7928  nsor.from_numpy(
-00039350: 2e2e 2e29 2e20 5468 6174 2064 6f65 736e  ...). That doesn
-00039360: 2774 2068 616e 646c 6520 6d61 736b 7320  't handle masks 
-00039370: 6173 206f 6620 7079 6172 726f 7720 342e  as of pyarrow 4.
-00039380: 302e 0d0a 0d0a 2020 2020 2020 2020 2020  0.....          
-00039390: 2020 2320 4765 7420 6120 6d61 736b 206f    # Get a mask o
-000393a0: 6620 696e 7661 6c69 6473 2e0d 0a20 2020  f invalids...   
-000393b0: 2020 2020 2020 2020 2069 6e76 616c 6964           invalid
-000393c0: 735f 6d61 736b 203d 2073 656c 662e 6973  s_mask = self.is
-000393d0: 6e61 6e28 290d 0a0d 0a20 2020 2020 2020  nan()....       
-000393e0: 2020 2020 2023 2049 6620 616c 6c20 7661       # If all va
-000393f0: 6c75 6573 2061 7265 2076 616c 6964 2c20  lues are valid, 
-00039400: 646f 6e27 7420 626f 7468 6572 2063 7265  don't bother cre
-00039410: 6174 696e 6720 616e 2061 6c6c 2d46 616c  ating an all-Fal
-00039420: 7365 206d 6173 6b2c 2069 7427 7320 6a75  se mask, it's ju
-00039430: 7374 2077 6173 7469 6e67 206d 656d 6f72  st wasting memor
-00039440: 792e 0d0a 2020 2020 2020 2020 2020 2020  y...            
-00039450: 6966 206e 6f74 2069 6e76 616c 6964 735f  if not invalids_
-00039460: 6d61 736b 2e61 6e79 2829 3a0d 0a20 2020  mask.any():..   
-00039470: 2020 2020 2020 2020 2020 2020 2069 6e76               inv
-00039480: 616c 6964 735f 6d61 736b 203d 204e 6f6e  alids_mask = Non
-00039490: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-000394a0: 2023 2043 7265 6174 6520 7468 6520 7079   # Create the py
-000394b0: 6172 726f 7720 6172 7261 7920 6672 6f6d  arrow array from
-000394c0: 2069 7420 2b20 7468 6973 2061 7272 6179   it + this array
-000394d0: 2e0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
-000394e0: 6574 7572 6e20 7061 2e61 7272 6179 2873  eturn pa.array(s
-000394f0: 656c 662e 5f6e 702c 206d 6173 6b3d 696e  elf._np, mask=in
-00039500: 7661 6c69 6473 5f6d 6173 6b2c 2074 7970  valids_mask, typ
-00039510: 653d 7479 7065 290d 0a0d 0a20 2020 2020  e=type)....     
-00039520: 2020 2065 6c69 6620 6e70 2e69 7373 7562     elif np.issub
-00039530: 6474 7970 6528 7365 6c66 2e64 7479 7065  dtype(self.dtype
-00039540: 2c20 6e70 2e66 6c6f 6174 696e 6729 3a0d  , np.floating):.
-00039550: 0a20 2020 2020 2020 2020 2020 2023 2055  .            # U
-00039560: 7369 6e67 2066 6c6f 6174 696e 672d 706f  sing floating-po
-00039570: 696e 7420 4e61 4e20 746f 2073 6967 6e61  int NaN to signa
-00039580: 6c20 626f 7468 204e 614e 2061 6e64 204e  l both NaN and N
-00039590: 412f 6e75 6c6c 2069 6e20 7269 7074 6162  A/null in riptab
-000395a0: 6c65 206d 6561 6e73 2077 650d 0a20 2020  le means we..   
-000395b0: 2020 2020 2020 2020 2023 206e 6565 6420           # need 
-000395c0: 746f 206d 616b 6520 6120 6465 6369 7369  to make a decisi
-000395d0: 6f6e 2068 6572 6520 6f6e 2077 6865 7468  on here on wheth
-000395e0: 6572 2074 6f20 6d61 726b 2074 686f 7365  er to mark those
-000395f0: 2076 616c 7565 7320 6173 204e 412f 6e75   values as NA/nu
-00039600: 6c6c 2076 616c 7565 730d 0a20 2020 2020  ll values..     
-00039610: 2020 2020 2020 2023 2069 6e20 7468 6520         # in the 
-00039620: 7265 7475 726e 6564 2070 7961 7272 6f77  returned pyarrow
-00039630: 2061 7272 6179 2e0d 0a20 2020 2020 2020   array...       
-00039640: 2020 2020 2023 2046 6f72 206e 6f77 2c20       # For now, 
-00039650: 7765 2064 6f6e 2774 202d 2d20 7765 206a  we don't -- we j
-00039660: 7573 7420 7061 7373 2074 6865 2064 6174  ust pass the dat
-00039670: 6120 616c 6f6e 6720 6469 7265 6374 6c79  a along directly
-00039680: 2c20 736f 2074 6865 2063 616c 6c65 7220  , so the caller 
-00039690: 6361 6e20 6465 6369 6465 0d0a 2020 2020  can decide..    
-000396a0: 2020 2020 2020 2020 2320 6f6e 2077 6865          # on whe
-000396b0: 7468 6572 2074 6865 7920 7761 6e74 2074  ther they want t
-000396c0: 6f20 6861 6e64 6c65 2074 6861 742e 2028  o handle that. (
-000396d0: 4964 6561 6c6c 792c 2077 6527 6420 6861  Ideally, we'd ha
-000396e0: 7665 2061 2077 6179 2074 6f20 7061 7261  ve a way to para
-000396f0: 6d65 7465 7269 7a65 2074 6869 730d 0a20  meterize this.. 
-00039700: 2020 2020 2020 2020 2020 2023 2062 7574             # but
-00039710: 2074 6865 2070 726f 746f 636f 6c20 646f   the protocol do
-00039720: 6573 6e27 7420 7375 7070 6f72 7420 6974  esn't support it
-00039730: 2061 7320 6f66 2070 7961 7272 6f77 2034   as of pyarrow 4
-00039740: 2e30 2e20 496e 2061 6e79 2063 6173 652c  .0. In any case,
-00039750: 206f 6e6c 7920 7468 6520 6269 746d 6173   only the bitmas
-00039760: 6b0d 0a20 2020 2020 2020 2020 2020 2023  k..            #
-00039770: 206e 6565 6473 2074 6f20 6265 2072 652d   needs to be re-
-00039780: 6372 6561 7465 6420 6c61 7465 7220 6966  created later if
-00039790: 2074 6865 2075 7365 7220 7761 6e74 7320   the user wants 
-000397a0: 746f 2063 6f6e 7369 6465 7220 7468 6520  to consider the 
-000397b0: 4e61 4e73 2061 7320 4e41 2f6e 756c 6c20  NaNs as NA/null 
-000397c0: 7661 6c75 6573 2e29 0d0a 2020 2020 2020  values.)..      
-000397d0: 2020 2020 2020 6966 2073 656c 662e 6e64        if self.nd
-000397e0: 696d 203e 3d20 323a 0d0a 2020 2020 2020  im >= 2:..      
-000397f0: 2020 2020 2020 2020 2020 2320 4e4f 5445            # NOTE
-00039800: 3a20 4173 206f 6620 7079 6172 726f 7720  : As of pyarrow 
-00039810: 342e 302c 2074 6869 7320 6d65 7468 6f64  4.0, this method
-00039820: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
-00039830: 2061 2060 7479 7065 6020 6172 6775 6d65   a `type` argume
-00039840: 6e74 2e0d 0a20 2020 2020 2020 2020 2020  nt...           
-00039850: 2020 2020 2072 6574 7572 6e20 7061 2e54       return pa.T
-00039860: 656e 736f 722e 6672 6f6d 5f6e 756d 7079  ensor.from_numpy
-00039870: 2873 656c 662e 5f6e 7029 0d0a 2020 2020  (self._np)..    
-00039880: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00039890: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000398a0: 6574 7572 6e20 7061 2e61 7272 6179 2873  eturn pa.array(s
-000398b0: 656c 662e 5f6e 702c 2074 7970 653d 7479  elf._np, type=ty
-000398c0: 7065 290d 0a0d 0a20 2020 2020 2020 2065  pe)....        e
-000398d0: 6c69 6620 6e70 2e69 7373 7562 6474 7970  lif np.issubdtyp
-000398e0: 6528 7365 6c66 2e64 7479 7065 2c20 626f  e(self.dtype, bo
-000398f0: 6f6c 293a 0d0a 2020 2020 2020 2020 2020  ol):..          
-00039900: 2020 6966 2073 656c 662e 6e64 696d 203e    if self.ndim >
-00039910: 3d20 323a 0d0a 2020 2020 2020 2020 2020  = 2:..          
-00039920: 2020 2020 2020 2320 4e4f 5445 3a20 4173        # NOTE: As
-00039930: 206f 6620 7079 6172 726f 7720 342e 302c   of pyarrow 4.0,
-00039940: 2074 6869 7320 6d65 7468 6f64 2064 6f65   this method doe
-00039950: 736e 2774 2073 7570 706f 7274 2061 2060  sn't support a `
-00039960: 7479 7065 6020 6172 6775 6d65 6e74 2e0d  type` argument..
-00039970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00039980: 2072 6574 7572 6e20 7061 2e54 656e 736f   return pa.Tenso
-00039990: 722e 6672 6f6d 5f6e 756d 7079 2873 656c  r.from_numpy(sel
-000399a0: 662e 5f6e 7029 0d0a 2020 2020 2020 2020  f._np)..        
-000399b0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000399c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000399d0: 6e20 7061 2e61 7272 6179 2873 656c 662e  n pa.array(self.
-000399e0: 5f6e 702c 2074 7970 653d 7479 7065 290d  _np, type=type).
-000399f0: 0a0d 0a20 2020 2020 2020 2065 6c69 6620  ...        elif 
-00039a00: 6e70 2e69 7373 7562 6474 7970 6528 7365  np.issubdtype(se
-00039a10: 6c66 2e64 7479 7065 2c20 6279 7465 7329  lf.dtype, bytes)
-00039a20: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-00039a30: 2049 6620 7468 6520 6361 6c6c 6572 2077   If the caller w
-00039a40: 616e 7473 2074 6f20 636f 6e76 6572 7420  ants to convert 
-00039a50: 656d 7074 7920 7374 7269 6e67 7320 746f  empty strings to
-00039a60: 206e 756c 6c73 2c20 6765 7420 6120 6d61   nulls, get a ma
-00039a70: 736b 206f 6620 696e 7661 6c69 6473 2e0d  sk of invalids..
-00039a80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00039a90: 656d 7074 795f 7374 7269 6e67 735f 746f  empty_strings_to
-00039aa0: 5f6e 756c 6c3a 0d0a 2020 2020 2020 2020  _null:..        
-00039ab0: 2020 2020 2020 2020 696e 7661 6c69 6473          invalids
-00039ac0: 5f6d 6173 6b20 3d20 7365 6c66 203d 3d20  _mask = self == 
-00039ad0: 7365 6c66 2e69 6e76 0d0a 0d0a 2020 2020  self.inv....    
-00039ae0: 2020 2020 2020 2020 2020 2020 2320 4966              # If
-00039af0: 2061 6c6c 2076 616c 7565 7320 6172 6520   all values are 
-00039b00: 7661 6c69 642c 2064 6f6e 2774 2062 6f74  valid, don't bot
-00039b10: 6865 7220 6372 6561 7469 6e67 2061 6e20  her creating an 
-00039b20: 616c 6c2d 4661 6c73 6520 6d61 736b 2c20  all-False mask, 
-00039b30: 6974 2773 206a 7573 7420 7761 7374 696e  it's just wastin
-00039b40: 6720 6d65 6d6f 7279 2e0d 0a20 2020 2020  g memory...     
-00039b50: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00039b60: 7420 696e 7661 6c69 6473 5f6d 6173 6b2e  t invalids_mask.
-00039b70: 616e 7928 293a 0d0a 2020 2020 2020 2020  any():..        
-00039b80: 2020 2020 2020 2020 2020 2020 696e 7661              inva
-00039b90: 6c69 6473 5f6d 6173 6b20 3d20 4e6f 6e65  lids_mask = None
-00039ba0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00039bb0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00039bc0: 2020 2020 2069 6e76 616c 6964 735f 6d61       invalids_ma
-00039bd0: 736b 203d 204e 6f6e 650d 0a0d 0a20 2020  sk = None....   
-00039be0: 2020 2020 2020 2020 2023 2044 6f65 7320           # Does 
-00039bf0: 7468 6520 6361 6c6c 6572 2077 616e 7420  the caller want 
-00039c00: 746f 2070 7265 7365 7276 6520 7468 6520  to preserve the 
-00039c10: 6669 7865 642d 6c65 6e67 7468 2062 696e  fixed-length bin
-00039c20: 6172 7920 6461 7461 3f0d 0a20 2020 2020  ary data?..     
-00039c30: 2020 2020 2020 2069 6620 7072 6573 6572         if preser
-00039c40: 7665 5f66 6978 6564 5f62 7974 6573 3a0d  ve_fixed_bytes:.
-00039c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00039c60: 2023 2043 6f6e 7665 7274 2074 6f20 6120   # Convert to a 
-00039c70: 6669 7865 642d 6c65 6e67 7468 2062 696e  fixed-length bin
-00039c80: 6172 7920 2827 6279 7465 7327 2920 7479  ary ('bytes') ty
-00039c90: 7065 2e0d 0a20 2020 2020 2020 2020 2020  pe...           
-00039ca0: 2020 2020 2065 6c65 6d65 6e74 5f73 7472       element_str
-00039cb0: 5f6c 656e 6774 6820 3d20 6e70 2e64 7479  _length = np.dty
-00039cc0: 7065 2873 656c 662e 6474 7970 6529 2e69  pe(self.dtype).i
-00039cd0: 7465 6d73 697a 650d 0a20 2020 2020 2020  temsize..       
-00039ce0: 2020 2020 2020 2020 2061 7272 5f74 7970           arr_typ
-00039cf0: 6520 3d20 7061 2e62 696e 6172 7928 656c  e = pa.binary(el
-00039d00: 656d 656e 745f 7374 725f 6c65 6e67 7468  ement_str_length
-00039d10: 2920 6966 2074 7970 6520 6973 204e 6f6e  ) if type is Non
-00039d20: 6520 656c 7365 2074 7970 650d 0a20 2020  e else type..   
-00039d30: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00039d40: 7572 6e20 7061 2e61 7272 6179 2873 656c  urn pa.array(sel
-00039d50: 662e 5f6e 702c 206d 6173 6b3d 696e 7661  f._np, mask=inva
-00039d60: 6c69 6473 5f6d 6173 6b2c 2074 7970 653d  lids_mask, type=
-00039d70: 6172 725f 7479 7065 290d 0a20 2020 2020  arr_type)..     
-00039d80: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00039d90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00039da0: 436f 6e76 6572 7420 7468 6973 2061 7272  Convert this arr
-00039db0: 6179 2074 6f20 6120 7079 6172 726f 7720  ay to a pyarrow 
-00039dc0: 7661 7269 6162 6c65 2d6c 656e 6774 6820  variable-length 
-00039dd0: 7374 7269 6e67 2061 7272 6179 2e0d 0a20  string array... 
-00039de0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00039df0: 6620 7479 7065 2069 7320 4e6f 6e65 3a0d  f type is None:.
-00039e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00039e10: 2020 2020 2074 7970 6520 3d20 7061 2e73       type = pa.s
-00039e20: 7472 696e 6728 290d 0a20 2020 2020 2020  tring()..       
-00039e30: 2020 2020 2020 2020 2023 2043 6f6e 7665           # Conve
-00039e40: 7274 2061 7320 556e 6963 6f64 6520 6e64  rt as Unicode nd
-00039e50: 6172 7261 7920 746f 2073 7472 696e 6761  array to stringa
-00039e60: 7272 6179 2c20 6173 2062 7974 6573 7472  rray, as bytestr
-00039e70: 696e 6720 646f 6573 206e 6f74 2070 7265  ing does not pre
-00039e80: 7365 7276 6520 656c 656d 656e 7420 6c65  serve element le
-00039e90: 6e67 7468 2028 7269 7074 6162 6c65 2332  ngth (riptable#2
-00039ea0: 3439 290d 0a20 2020 2020 2020 2020 2020  49)..           
-00039eb0: 2020 2020 2072 6574 7572 6e20 7061 2e61       return pa.a
-00039ec0: 7272 6179 286e 702e 6172 7261 7928 7365  rray(np.array(se
-00039ed0: 6c66 2e5f 6e70 2c20 6474 7970 653d 2255  lf._np, dtype="U
-00039ee0: 2229 2c20 6d61 736b 3d69 6e76 616c 6964  "), mask=invalid
-00039ef0: 735f 6d61 736b 2c20 7479 7065 3d74 7970  s_mask, type=typ
-00039f00: 6529 0d0a 0d0a 2020 2020 2020 2020 656c  e)....        el
-00039f10: 6966 206e 702e 6973 7375 6264 7479 7065  if np.issubdtype
-00039f20: 2873 656c 662e 6474 7970 652c 2073 7472  (self.dtype, str
-00039f30: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00039f40: 2320 4966 2074 6865 2063 616c 6c65 7220  # If the caller 
-00039f50: 7761 6e74 7320 746f 2063 6f6e 7665 7274  wants to convert
-00039f60: 2065 6d70 7479 2073 7472 696e 6773 2074   empty strings t
-00039f70: 6f20 6e75 6c6c 732c 2067 6574 2061 206d  o nulls, get a m
-00039f80: 6173 6b20 6f66 2069 6e76 616c 6964 732e  ask of invalids.
-00039f90: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00039fa0: 2065 6d70 7479 5f73 7472 696e 6773 5f74   empty_strings_t
-00039fb0: 6f5f 6e75 6c6c 3a0d 0a20 2020 2020 2020  o_null:..       
-00039fc0: 2020 2020 2020 2020 2069 6e76 616c 6964           invalid
-00039fd0: 735f 6d61 736b 203d 2073 656c 6620 3d3d  s_mask = self ==
-00039fe0: 2073 656c 662e 696e 760d 0a0d 0a20 2020   self.inv....   
-00039ff0: 2020 2020 2020 2020 2020 2020 2023 2049               # I
-0003a000: 6620 616c 6c20 7661 6c75 6573 2061 7265  f all values are
-0003a010: 2076 616c 6964 2c20 646f 6e27 7420 626f   valid, don't bo
-0003a020: 7468 6572 2063 7265 6174 696e 6720 616e  ther creating an
-0003a030: 2061 6c6c 2d46 616c 7365 206d 6173 6b2c   all-False mask,
-0003a040: 2069 7427 7320 6a75 7374 2077 6173 7469   it's just wasti
-0003a050: 6e67 206d 656d 6f72 792e 0d0a 2020 2020  ng memory...    
-0003a060: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0003a070: 6f74 2069 6e76 616c 6964 735f 6d61 736b  ot invalids_mask
-0003a080: 2e61 6e79 2829 3a0d 0a20 2020 2020 2020  .any():..       
-0003a090: 2020 2020 2020 2020 2020 2020 2069 6e76               inv
-0003a0a0: 616c 6964 735f 6d61 736b 203d 204e 6f6e  alids_mask = Non
-0003a0b0: 650d 0a20 2020 2020 2020 2020 2020 2065  e..            e
-0003a0c0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0003a0d0: 2020 2020 2020 696e 7661 6c69 6473 5f6d        invalids_m
-0003a0e0: 6173 6b20 3d20 4e6f 6e65 0d0a 0d0a 2020  ask = None....  
-0003a0f0: 2020 2020 2020 2020 2020 2320 7079 6172            # pyar
-0003a100: 726f 7720 2861 7320 6f66 2076 342e 3029  row (as of v4.0)
-0003a110: 2064 6f65 7320 6e6f 7420 6861 7665 2061   does not have a
-0003a120: 2066 6978 6564 2d73 697a 6520 556e 6963   fixed-size Unic
-0003a130: 6f64 6520 7374 7269 6e67 2064 6174 6120  ode string data 
-0003a140: 7479 7065 2c20 736f 2075 6e6c 696b 6520  type, so unlike 
-0003a150: 7468 6520 2762 7974 6573 270d 0a20 2020  the 'bytes'..   
-0003a160: 2020 2020 2020 2020 2023 2068 616e 646c           # handl
-0003a170: 696e 6720 6162 6f76 6520 666f 7220 4153  ing above for AS
-0003a180: 4349 4920 7374 7269 6e67 732c 2077 6520  CII strings, we 
-0003a190: 6861 7665 2074 6f20 7573 6520 7468 6520  have to use the 
-0003a1a0: 7661 7269 6162 6c65 2d6c 656e 6774 6820  variable-length 
-0003a1b0: 7374 7269 6e67 2061 7272 6179 2074 7970  string array typ
-0003a1c0: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
-0003a1d0: 6966 2074 7970 6520 6973 204e 6f6e 653a  if type is None:
-0003a1e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0003a1f0: 2020 7479 7065 203d 2070 612e 7374 7269    type = pa.stri
-0003a200: 6e67 2829 0d0a 2020 2020 2020 2020 2020  ng()..          
-0003a210: 2020 7265 7475 726e 2070 612e 6172 7261    return pa.arra
-0003a220: 7928 7365 6c66 2e5f 6e70 2c20 6d61 736b  y(self._np, mask
-0003a230: 3d69 6e76 616c 6964 735f 6d61 736b 2c20  =invalids_mask, 
-0003a240: 7479 7065 3d74 7970 6529 0d0a 0d0a 2020  type=type)....  
-0003a250: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0003a260: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
-0003a270: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-0003a280: 6f72 2866 2246 6173 7441 7272 6179 2077  or(f"FastArray w
-0003a290: 6974 6820 6474 7970 6520 277b 6e70 2e64  ith dtype '{np.d
-0003a2a0: 7479 7065 2873 656c 662e 6474 7970 6529  type(self.dtype)
-0003a2b0: 7d27 2069 7320 6e6f 7420 7375 7070 6f72  }' is not suppor
-0003a2c0: 7465 642e 2229 0d0a 0d0a 2020 2020 6465  ted.")....    de
-0003a2d0: 6620 5f5f 6172 726f 775f 6172 7261 795f  f __arrow_array_
-0003a2e0: 5f28 7365 6c66 2c20 7479 7065 3a20 4f70  _(self, type: Op
-0003a2f0: 7469 6f6e 616c 5b22 7061 2e44 6174 6154  tional["pa.DataT
-0003a300: 7970 6522 5d20 3d20 4e6f 6e65 2920 2d3e  ype"] = None) ->
-0003a310: 2055 6e69 6f6e 5b22 7061 2e41 7272 6179   Union["pa.Array
-0003a320: 222c 2022 7061 2e43 6875 6e6b 6564 4172  ", "pa.ChunkedAr
-0003a330: 7261 7922 5d3a 0d0a 2020 2020 2020 2020  ray"]:..        
-0003a340: 2222 220d 0a20 2020 2020 2020 2049 6d70  """..        Imp
-0003a350: 6c65 6d65 6e74 6174 696f 6e20 6f66 2074  lementation of t
-0003a360: 6865 2060 605f 5f61 7272 6f77 5f61 7272  he ``__arrow_arr
-0003a370: 6179 5f5f 6060 2070 726f 746f 636f 6c20  ay__`` protocol 
-0003a380: 666f 7220 636f 6e76 6572 7369 6f6e 2074  for conversion t
-0003a390: 6f20 6120 7079 6172 726f 7720 6172 7261  o a pyarrow arra
-0003a3a0: 792e 0d0a 0d0a 2020 2020 2020 2020 5061  y.....        Pa
-0003a3b0: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
-0003a3c0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
-0003a3d0: 2020 2020 2020 7479 7065 203a 2070 7961        type : pya
-0003a3e0: 7272 6f77 2e44 6174 6154 7970 652c 206f  rrow.DataType, o
-0003a3f0: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
-0003a400: 7320 746f 204e 6f6e 650d 0a0d 0a20 2020  s to None....   
-0003a410: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
-0003a420: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
-0003a430: 2020 2020 2020 2070 7961 7272 6f77 2e41         pyarrow.A
-0003a440: 7272 6179 206f 7220 7079 6172 726f 772e  rray or pyarrow.
-0003a450: 4368 756e 6b65 6441 7272 6179 0d0a 0d0a  ChunkedArray....
-0003a460: 2020 2020 2020 2020 4e6f 7465 730d 0a20          Notes.. 
-0003a470: 2020 2020 2020 202d 2d2d 2d2d 0d0a 2020         -----..  
-0003a480: 2020 2020 2020 6874 7470 733a 2f2f 6172        https://ar
-0003a490: 726f 772e 6170 6163 6865 2e6f 7267 2f64  row.apache.org/d
-0003a4a0: 6f63 732f 7079 7468 6f6e 2f65 7874 656e  ocs/python/exten
-0003a4b0: 6469 6e67 5f74 7970 6573 2e68 746d 6c23  ding_types.html#
-0003a4c0: 636f 6e74 726f 6c6c 696e 672d 636f 6e76  controlling-conv
-0003a4d0: 6572 7369 6f6e 2d74 6f2d 7079 6172 726f  ersion-to-pyarro
-0003a4e0: 772d 6172 7261 792d 7769 7468 2d74 6865  w-array-with-the
-0003a4f0: 2d61 7272 6f77 2d61 7272 6179 2d70 726f  -arrow-array-pro
-0003a500: 746f 636f 6c0d 0a20 2020 2020 2020 2022  tocol..        "
-0003a510: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-0003a520: 726e 2073 656c 662e 746f 5f61 7272 6f77  rn self.to_arrow
-0003a530: 2874 7970 653d 7479 7065 2c20 7072 6573  (type=type, pres
-0003a540: 6572 7665 5f66 6978 6564 5f62 7974 6573  erve_fixed_bytes
-0003a550: 3d46 616c 7365 2c20 656d 7074 795f 7374  =False, empty_st
-0003a560: 7269 6e67 735f 746f 5f6e 756c 6c3d 5472  rings_to_null=Tr
-0003a570: 7565 290d 0a0d 0a20 2020 2023 202d 2d2d  ue)....    # ---
+00038480: 2020 2020 2020 2243 616e 2774 2070 6572        "Can't per
+00038490: 666f 726d 2061 207a 6572 6f2d 636f 7079  form a zero-copy
+000384a0: 2063 6f6e 7665 7273 696f 6e20 6f66 2061   conversion of a
+000384b0: 2066 6978 6564 2d73 697a 6520 6269 6e61   fixed-size bina
+000384c0: 7279 2061 7272 6179 2074 6f20 7269 7074  ry array to ript
+000384d0: 6162 6c65 2077 6865 6e20 7468 6520 696e  able when the in
+000384e0: 7075 7420 6172 7261 7920 636f 6e74 6169  put array contai
+000384f0: 6e73 206e 756c 6c73 2e22 0d0a 2020 2020  ns nulls."..    
+00038500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00038510: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00038520: 2020 2020 2061 7272 203d 2061 7272 2e66       arr = arr.f
+00038530: 696c 6c5f 6e75 6c6c 280d 0a20 2020 2020  ill_null(..     
+00038540: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00038550: 225c 7830 3022 202a 2061 7272 2e74 7970  "\x00" * arr.typ
+00038560: 652e 6279 7465 5f77 6964 7468 0d0a 2020  e.byte_width..  
+00038570: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+00038580: 2023 2063 616e 2774 2066 696c 6c20 7769   # can't fill wi
+00038590: 7468 2062 2222 2c20 7369 6e63 6520 6222  th b"", since b"
+000385a0: 2220 6973 206e 6f74 2076 616c 6964 2066  " is not valid f
+000385b0: 6f72 2066 6978 6564 2077 6964 7468 2074  or fixed width t
+000385c0: 7970 650d 0a0d 0a20 2020 2020 2020 2020  ype....         
+000385d0: 2020 2023 2043 616c 6c69 6e67 2070 612e     # Calling pa.
+000385e0: 4172 7261 792e 746f 5f6e 756d 7079 2077  Array.to_numpy w
+000385f0: 6974 6820 7a65 726f 5f63 6f70 793d 5472  ith zero_copy=Tr
+00038600: 7565 2072 6169 7365 7320 616e 2065 7272  ue raises an err
+00038610: 6f72 2077 6974 6820 6669 7865 6420 7369  or with fixed si
+00038620: 7a65 6420 6269 6e61 7279 2074 7970 652e  zed binary type.
+00038630: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00038640: 4361 6c6c 696e 6720 7061 2e41 7272 6179  Calling pa.Array
+00038650: 2e74 6f5f 6e75 6d70 7920 7769 7468 207a  .to_numpy with z
+00038660: 6572 6f5f 636f 7079 3d46 616c 7365 2072  ero_copy=False r
+00038670: 6574 7572 6e73 2061 206e 756d 7079 2061  eturns a numpy a
+00038680: 7272 6179 2077 6865 7265 2074 7970 6573  rray where types
+00038690: 2061 7265 2070 7974 686f 6e20 6279 7465   are python byte
+000386a0: 7320 6f62 6a65 6374 732e 0d0a 2020 2020  s objects...    
+000386b0: 2020 2020 2020 2020 2320 576f 726b 6172          # Workar
+000386c0: 6f75 6e64 2062 656c 6f77 2063 7265 6174  ound below creat
+000386d0: 6573 2074 6865 206e 756d 7079 2062 7566  es the numpy buf
+000386e0: 6665 7220 6f66 2074 7970 6520 2253 2220  fer of type "S" 
+000386f0: 6d61 6e75 616c 6c79 2e0d 0a20 2020 2020  manually...     
+00038700: 2020 2020 2020 2062 7566 203d 206e 702e         buf = np.
+00038710: 6672 6f6d 6275 6666 6572 280d 0a20 2020  frombuffer(..   
+00038720: 2020 2020 2020 2020 2020 2020 2061 7272               arr
+00038730: 2e62 7566 6665 7273 2829 5b31 5d2c 0d0a  .buffers()[1],..
+00038740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00038750: 6474 7970 653d 2253 2220 2b20 7374 7228  dtype="S" + str(
+00038760: 6172 722e 7479 7065 2e62 7974 655f 7769  arr.type.byte_wi
+00038770: 6474 6829 2c0d 0a20 2020 2020 2020 2020  dth),..         
+00038780: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
+00038790: 2020 2020 6966 2077 7269 7461 626c 6520      if writable 
+000387a0: 616e 6420 6e75 6c6c 5f63 6f75 6e74 203d  and null_count =
+000387b0: 3d20 303a 2020 2320 616c 7265 6164 7920  = 0:  # already 
+000387c0: 6d61 6465 2061 2063 6f70 7920 6966 206e  made a copy if n
+000387d0: 756c 6c5f 636f 756e 7420 213d 2030 0d0a  ull_count != 0..
+000387e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000387f0: 7265 7375 6c74 203d 2046 6173 7441 7272  result = FastArr
+00038800: 6179 286e 702e 636f 7079 2862 7566 2929  ay(np.copy(buf))
+00038810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00038820: 2020 7265 7375 6c74 2e66 6c61 6773 2e77    result.flags.w
+00038830: 7269 7465 6162 6c65 203d 2077 7269 7461  riteable = writa
+00038840: 626c 650d 0a20 2020 2020 2020 2020 2020  ble..           
+00038850: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00038860: 6c74 0d0a 0d0a 2020 2020 2020 2020 2020  lt....          
+00038870: 2020 7265 7375 6c74 203d 2046 6173 7441    result = FastA
+00038880: 7272 6179 2862 7566 290d 0a20 2020 2020  rray(buf)..     
+00038890: 2020 2020 2020 2072 6573 756c 742e 666c         result.fl
+000388a0: 6167 732e 7772 6974 6561 626c 6520 3d20  ags.writeable = 
+000388b0: 7772 6974 6162 6c65 0d0a 2020 2020 2020  writable..      
+000388c0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000388d0: 756c 740d 0a0d 0a20 2020 2020 2020 2065  ult....        e
+000388e0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000388f0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00038900: 6f72 280d 0a20 2020 2020 2020 2020 2020  or(..           
+00038910: 2020 2020 2066 2246 6173 7441 7272 6179       f"FastArray
+00038920: 2063 616e 6e6f 7420 6265 2063 7265 6174   cannot be creat
+00038930: 6564 2066 726f 6d20 6120 7079 6172 726f  ed from a pyarro
+00038940: 7720 6172 7261 7920 6f66 2074 7970 6520  w array of type 
+00038950: 277b 6172 722e 7479 7065 7d27 2e20 596f  '{arr.type}'. Yo
+00038960: 7520 6d61 7920 6e65 6564 2074 6f20 6361  u may need to ca
+00038970: 6c6c 2074 6865 2060 6672 6f6d 5f61 7272  ll the `from_arr
+00038980: 6f77 6020 6d65 7468 6f64 206f 6e20 6f6e  ow` method on on
+00038990: 6520 6f66 2074 6865 2064 6572 6976 6564  e of the derived
+000389a0: 2073 7562 636c 6173 7365 7320 696e 7374   subclasses inst
+000389b0: 6561 642e 220d 0a20 2020 2020 2020 2020  ead."..         
+000389c0: 2020 2029 0d0a 0d0a 2020 2020 6465 6620     )....    def 
+000389d0: 746f 5f61 7272 6f77 280d 0a20 2020 2020  to_arrow(..     
+000389e0: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
+000389f0: 2020 7479 7065 3a20 4f70 7469 6f6e 616c    type: Optional
+00038a00: 5b22 7061 2e44 6174 6154 7970 6522 5d20  ["pa.DataType"] 
+00038a10: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+00038a20: 202a 2c0d 0a20 2020 2020 2020 2070 7265   *,..        pre
+00038a30: 7365 7276 655f 6669 7865 645f 6279 7465  serve_fixed_byte
+00038a40: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
+00038a50: 0d0a 2020 2020 2020 2020 656d 7074 795f  ..        empty_
+00038a60: 7374 7269 6e67 735f 746f 5f6e 756c 6c3a  strings_to_null:
+00038a70: 2062 6f6f 6c20 3d20 5472 7565 2c0d 0a20   bool = True,.. 
+00038a80: 2020 2029 202d 3e20 556e 696f 6e5b 2270     ) -> Union["p
+00038a90: 612e 4172 7261 7922 2c20 2270 612e 4368  a.Array", "pa.Ch
+00038aa0: 756e 6b65 6441 7272 6179 225d 3a0d 0a20  unkedArray"]:.. 
+00038ab0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00038ac0: 2020 2020 436f 6e76 6572 7420 7468 6973      Convert this
+00038ad0: 2060 4661 7374 4172 7261 7960 2074 6f20   `FastArray` to 
+00038ae0: 6120 6070 7961 7272 6f77 2e41 7272 6179  a `pyarrow.Array
+00038af0: 602e 0d0a 0d0a 2020 2020 2020 2020 5061  `.....        Pa
+00038b00: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
+00038b10: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
+00038b20: 2020 2020 2020 7479 7065 203a 2070 7961        type : pya
+00038b30: 7272 6f77 2e44 6174 6154 7970 652c 206f  rrow.DataType, o
+00038b40: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
+00038b50: 7320 746f 204e 6f6e 650d 0a20 2020 2020  s to None..     
+00038b60: 2020 2070 7265 7365 7276 655f 6669 7865     preserve_fixe
+00038b70: 645f 6279 7465 7320 3a20 626f 6f6c 2c20  d_bytes : bool, 
+00038b80: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
+00038b90: 7473 2074 6f20 4661 6c73 650d 0a20 2020  ts to False..   
+00038ba0: 2020 2020 2020 2020 2049 6620 7468 6973           If this
+00038bb0: 2060 4661 7374 4172 7261 7960 2069 7320   `FastArray` is 
+00038bc0: 616e 2041 5343 4949 2073 7472 696e 6720  an ASCII string 
+00038bd0: 6172 7261 7920 2864 7479 7065 2e6b 696e  array (dtype.kin
+00038be0: 6420 3d3d 2027 5327 292c 0d0a 2020 2020  d == 'S'),..    
+00038bf0: 2020 2020 2020 2020 7365 7420 7468 6973          set this
+00038c00: 2070 6172 616d 6574 6572 2074 6f20 5472   parameter to Tr
+00038c10: 7565 2074 6f20 7072 6f64 7563 6520 6120  ue to produce a 
+00038c20: 6669 7865 642d 6c65 6e67 7468 2062 696e  fixed-length bin
+00038c30: 6172 7920 6172 7261 790d 0a20 2020 2020  ary array..     
+00038c40: 2020 2020 2020 2069 6e73 7465 6164 206f         instead o
+00038c50: 6620 6120 7661 7269 6162 6c65 2d6c 656e  f a variable-len
+00038c60: 6774 6820 7374 7269 6e67 2061 7272 6179  gth string array
+00038c70: 2e0d 0a20 2020 2020 2020 2065 6d70 7479  ...        empty
+00038c80: 5f73 7472 696e 6773 5f74 6f5f 6e75 6c6c  _strings_to_null
+00038c90: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+00038ca0: 6c2c 2064 6566 6175 6c74 7320 546f 2054  l, defaults To T
+00038cb0: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
+00038cc0: 2049 6620 7468 6973 2060 4661 7374 4172   If this `FastAr
+00038cd0: 7261 7960 2069 7320 616e 2041 5343 4949  ray` is an ASCII
+00038ce0: 206f 7220 556e 6963 6f64 6520 7374 7269   or Unicode stri
+00038cf0: 6e67 2061 7272 6179 2c0d 0a20 2020 2020  ng array,..     
+00038d00: 2020 2020 2020 2073 7065 6369 6679 2054         specify T
+00038d10: 7275 6520 666f 7220 7468 6973 2070 6172  rue for this par
+00038d20: 616d 6574 6572 2074 6f20 636f 6e76 6572  ameter to conver
+00038d30: 7420 656d 7074 7920 7374 7269 6e67 7320  t empty strings 
+00038d40: 746f 206e 756c 6c73 2069 6e20 7468 6520  to nulls in the 
+00038d50: 6f75 7470 7574 2e0d 0a20 2020 2020 2020  output...       
+00038d60: 2020 2020 2072 6970 7461 626c 6520 696e       riptable in
+00038d70: 636f 6e73 6973 7465 6e74 6c79 2072 6563  consistently rec
+00038d80: 6f67 6e69 7a65 7320 7468 6520 656d 7074  ognizes the empt
+00038d90: 7920 7374 7269 6e67 2061 7320 616e 2027  y string as an '
+00038da0: 696e 7661 6c69 6427 2c0d 0a20 2020 2020  invalid',..     
+00038db0: 2020 2020 2020 2073 6f20 7468 6973 2070         so this p
+00038dc0: 6172 616d 6574 6572 2061 6c6c 6f77 7320  arameter allows 
+00038dd0: 7468 6520 6361 6c6c 6572 2074 6f20 7370  the caller to sp
+00038de0: 6563 6966 7920 7768 6963 6820 696e 7465  ecify which inte
+00038df0: 7270 7265 7461 7469 6f6e 0d0a 2020 2020  rpretation..    
+00038e00: 2020 2020 2020 2020 7468 6579 2077 616e          they wan
+00038e10: 742e 0d0a 0d0a 2020 2020 2020 2020 5265  t.....        Re
+00038e20: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
+00038e30: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00038e40: 7079 6172 726f 772e 4172 7261 7920 6f72  pyarrow.Array or
+00038e50: 2070 7961 7272 6f77 2e43 6875 6e6b 6564   pyarrow.Chunked
+00038e60: 4172 7261 790d 0a0d 0a20 2020 2020 2020  Array....       
+00038e70: 204e 6f74 6573 0d0a 2020 2020 2020 2020   Notes..        
+00038e80: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2054  -----..        T
+00038e90: 4f44 4f3a 2041 6464 2062 6f6f 6c20 7061  ODO: Add bool pa
+00038ea0: 7261 6d65 7465 7220 7768 6963 6820 6469  rameter which di
+00038eb0: 7265 6374 7320 7468 6520 636f 6e76 6572  rects the conver
+00038ec0: 7369 6f6e 2074 6f20 6368 6f6f 7365 2074  sion to choose t
+00038ed0: 6865 206d 6f73 742d 636f 6d70 6163 7420  he most-compact 
+00038ee0: 6f75 7470 7574 2074 7970 6520 706f 7373  output type poss
+00038ef0: 6962 6c65 3f0d 0a20 2020 2020 2020 2020  ible?..         
+00038f00: 2020 2020 2054 6869 7320 776f 756c 6420       This would 
+00038f10: 6265 2072 656c 6576 616e 7420 746f 2069  be relevant to i
+00038f20: 6e64 6963 6573 206f 6620 6361 7465 676f  ndices of catego
+00038f30: 7269 6361 6c2f 6469 6374 696f 6e61 7279  rical/dictionary
+00038f40: 2d65 6e63 6f64 6564 2061 7272 6179 732c  -encoded arrays,
+00038f50: 2062 7574 2063 6f75 6c64 2061 6c73 6f20   but could also 
+00038f60: 6d61 6b65 2073 656e 7365 0d0a 2020 2020  make sense..    
+00038f70: 2020 2020 2020 2020 2020 666f 7220 7265            for re
+00038f80: 6775 6c61 7220 4661 7374 4172 7261 7920  gular FastArray 
+00038f90: 7479 7065 7320 2865 2e67 2e20 746f 2075  types (e.g. to u
+00038fa0: 7365 2061 6e20 696e 7438 2069 6e73 7465  se an int8 inste
+00038fb0: 6164 206f 6620 616e 2069 6e74 3332 2077  ad of an int32 w
+00038fc0: 6865 6e20 6974 2764 2062 6520 6120 6c6f  hen it'd be a lo
+00038fd0: 7373 6c65 7373 2063 6f6e 7665 7273 696f  ssless conversio
+00038fe0: 6e29 2e0d 0a20 2020 2020 2020 2022 2222  n)...        """
+00038ff0: 0d0a 2020 2020 2020 2020 696d 706f 7274  ..        import
+00039000: 2062 7569 6c74 696e 730d 0a0d 0a20 2020   builtins....   
+00039010: 2020 2020 2069 6d70 6f72 7420 7079 6172       import pyar
+00039020: 726f 7720 6173 2070 610d 0a0d 0a20 2020  row as pa....   
+00039030: 2020 2020 2023 2044 6572 6976 6564 2061       # Derived a
+00039040: 7272 6179 2074 7970 6573 204d 5553 5420  rray types MUST 
+00039050: 696d 706c 656d 656e 7420 7468 6569 7220  implement their 
+00039060: 6f77 6e20 6f76 6572 6c6f 6164 206f 6620  own overload of 
+00039070: 7468 6973 2066 756e 6374 696f 6e0d 0a20  this function.. 
+00039080: 2020 2020 2020 2023 2066 6f72 2063 6f72         # for cor
+00039090: 7265 6374 6e65 7373 3b20 666f 7220 7468  rectness; for th
+000390a0: 6174 2072 6561 736f 6e2c 2072 6169 7365  at reason, raise
+000390b0: 2061 6e20 6572 726f 7220 6966 2073 6f6d   an error if som
+000390c0: 656f 6e65 2061 7474 656d 7074 7320 746f  eone attempts to
+000390d0: 0d0a 2020 2020 2020 2020 2320 6361 6c6c  ..        # call
+000390e0: 202a 7468 6973 2a20 696d 706c 656d 656e   *this* implemen
+000390f0: 7461 7469 6f6e 206f 6620 7468 6520 6d65  tation of the me
+00039100: 7468 6f64 2066 6f72 2061 2064 6572 6976  thod for a deriv
+00039110: 6564 2061 7272 6179 2074 7970 652e 0d0a  ed array type...
+00039120: 2020 2020 2020 2020 6966 2062 7569 6c74          if built
+00039130: 696e 732e 7479 7065 2873 656c 6629 2021  ins.type(self) !
+00039140: 3d20 4661 7374 4172 7261 793a 0d0a 2020  = FastArray:..  
+00039150: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00039160: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00039170: 726f 7228 0d0a 2020 2020 2020 2020 2020  ror(..          
+00039180: 2020 2020 2020 6622 5468 6520 607b 6275        f"The `{bu
+00039190: 696c 7469 6e73 2e74 7970 6528 7365 6c66  iltins.type(self
+000391a0: 292e 5f5f 7175 616c 6e61 6d65 5f5f 7d60  ).__qualname__}`
+000391b0: 2074 7970 6520 6d75 7374 2069 6d70 6c65   type must imple
+000391c0: 6d65 6e74 2069 7427 7320 6f77 6e20 6f76  ment it's own ov
+000391d0: 6572 7269 6465 206f 6620 7468 6520 6074  erride of the `t
+000391e0: 6f5f 6172 726f 7728 2960 206d 6574 686f  o_arrow()` metho
+000391f0: 642e 220d 0a20 2020 2020 2020 2020 2020  d."..           
+00039200: 2029 0d0a 0d0a 2020 2020 2020 2020 2320   )....        # 
+00039210: 7269 7074 6162 6c65 2028 6174 206c 6561  riptable (at lea
+00039220: 7374 2061 7320 6f66 2031 2e30 2e35 3629  st as of 1.0.56)
+00039230: 2064 6f65 7320 6e6f 7420 2a74 7275 6c79   does not *truly
+00039240: 2a20 7375 7070 6f72 7420 696e 7661 6c69  * support invali
+00039250: 642f 4e41 2076 616c 7565 730d 0a20 2020  d/NA values..   
+00039260: 2020 2020 2023 2069 6e20 626f 6f6c 206f       # in bool o
+00039270: 7220 6173 6369 692f 756e 6963 6f64 6520  r ascii/unicode 
+00039280: 7374 7269 6e67 2d74 7970 6564 2061 7272  string-typed arr
+00039290: 6179 732e 2048 616e 646c 6520 7468 6f73  ays. Handle thos
+000392a0: 6520 6474 7970 6573 2073 7065 6369 616c  e dtypes special
+000392b0: 6c79 2e0d 0a20 2020 2020 2020 2069 6620  ly...        if 
+000392c0: 6e70 2e69 7373 7562 6474 7970 6528 7365  np.issubdtype(se
+000392d0: 6c66 2e64 7479 7065 2c20 6e70 2e69 6e74  lf.dtype, np.int
+000392e0: 6567 6572 293a 0d0a 2020 2020 2020 2020  eger):..        
+000392f0: 2020 2020 2320 544f 444f 3a20 4966 2074      # TODO: If t
+00039300: 6869 7320 6172 7261 7920 6861 7320 2e6e  his array has .n
+00039310: 6469 6d73 203e 3d20 322c 206e 6565 6420  dims >= 2, need 
+00039320: 746f 2063 6f6e 7665 7274 2074 6f20 7079  to convert to py
+00039330: 6172 726f 7720 7573 696e 6720 7061 2e54  arrow using pa.T
+00039340: 656e 736f 722e 6672 6f6d 5f6e 756d 7079  ensor.from_numpy
+00039350: 282e 2e2e 292e 2054 6861 7420 646f 6573  (...). That does
+00039360: 6e27 7420 6861 6e64 6c65 206d 6173 6b73  n't handle masks
+00039370: 2061 7320 6f66 2070 7961 7272 6f77 2034   as of pyarrow 4
+00039380: 2e30 2e0d 0a0d 0a20 2020 2020 2020 2020  .0.....         
+00039390: 2020 2023 2047 6574 2061 206d 6173 6b20     # Get a mask 
+000393a0: 6f66 2069 6e76 616c 6964 732e 0d0a 2020  of invalids...  
+000393b0: 2020 2020 2020 2020 2020 696e 7661 6c69            invali
+000393c0: 6473 5f6d 6173 6b20 3d20 7365 6c66 2e69  ds_mask = self.i
+000393d0: 736e 616e 2829 0d0a 0d0a 2020 2020 2020  snan()....      
+000393e0: 2020 2020 2020 2320 4966 2061 6c6c 2076        # If all v
+000393f0: 616c 7565 7320 6172 6520 7661 6c69 642c  alues are valid,
+00039400: 2064 6f6e 2774 2062 6f74 6865 7220 6372   don't bother cr
+00039410: 6561 7469 6e67 2061 6e20 616c 6c2d 4661  eating an all-Fa
+00039420: 6c73 6520 6d61 736b 2c20 6974 2773 206a  lse mask, it's j
+00039430: 7573 7420 7761 7374 696e 6720 6d65 6d6f  ust wasting memo
+00039440: 7279 2e0d 0a20 2020 2020 2020 2020 2020  ry...           
+00039450: 2069 6620 6e6f 7420 696e 7661 6c69 6473   if not invalids
+00039460: 5f6d 6173 6b2e 616e 7928 293a 0d0a 2020  _mask.any():..  
+00039470: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00039480: 7661 6c69 6473 5f6d 6173 6b20 3d20 4e6f  valids_mask = No
+00039490: 6e65 0d0a 0d0a 2020 2020 2020 2020 2020  ne....          
+000394a0: 2020 2320 4372 6561 7465 2074 6865 2070    # Create the p
+000394b0: 7961 7272 6f77 2061 7272 6179 2066 726f  yarrow array fro
+000394c0: 6d20 6974 202b 2074 6869 7320 6172 7261  m it + this arra
+000394d0: 792e 0d0a 2020 2020 2020 2020 2020 2020  y...            
+000394e0: 7265 7475 726e 2070 612e 6172 7261 7928  return pa.array(
+000394f0: 7365 6c66 2e5f 6e70 2c20 6d61 736b 3d69  self._np, mask=i
+00039500: 6e76 616c 6964 735f 6d61 736b 2c20 7479  nvalids_mask, ty
+00039510: 7065 3d74 7970 6529 0d0a 0d0a 2020 2020  pe=type)....    
+00039520: 2020 2020 656c 6966 206e 702e 6973 7375      elif np.issu
+00039530: 6264 7479 7065 2873 656c 662e 6474 7970  bdtype(self.dtyp
+00039540: 652c 206e 702e 666c 6f61 7469 6e67 293a  e, np.floating):
+00039550: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00039560: 5573 696e 6720 666c 6f61 7469 6e67 2d70  Using floating-p
+00039570: 6f69 6e74 204e 614e 2074 6f20 7369 676e  oint NaN to sign
+00039580: 616c 2062 6f74 6820 4e61 4e20 616e 6420  al both NaN and 
+00039590: 4e41 2f6e 756c 6c20 696e 2072 6970 7461  NA/null in ripta
+000395a0: 626c 6520 6d65 616e 7320 7765 0d0a 2020  ble means we..  
+000395b0: 2020 2020 2020 2020 2020 2320 6e65 6564            # need
+000395c0: 2074 6f20 6d61 6b65 2061 2064 6563 6973   to make a decis
+000395d0: 696f 6e20 6865 7265 206f 6e20 7768 6574  ion here on whet
+000395e0: 6865 7220 746f 206d 6172 6b20 7468 6f73  her to mark thos
+000395f0: 6520 7661 6c75 6573 2061 7320 4e41 2f6e  e values as NA/n
+00039600: 756c 6c20 7661 6c75 6573 0d0a 2020 2020  ull values..    
+00039610: 2020 2020 2020 2020 2320 696e 2074 6865          # in the
+00039620: 2072 6574 7572 6e65 6420 7079 6172 726f   returned pyarro
+00039630: 7720 6172 7261 792e 0d0a 2020 2020 2020  w array...      
+00039640: 2020 2020 2020 2320 466f 7220 6e6f 772c        # For now,
+00039650: 2077 6520 646f 6e27 7420 2d2d 2077 6520   we don't -- we 
+00039660: 6a75 7374 2070 6173 7320 7468 6520 6461  just pass the da
+00039670: 7461 2061 6c6f 6e67 2064 6972 6563 746c  ta along directl
+00039680: 792c 2073 6f20 7468 6520 6361 6c6c 6572  y, so the caller
+00039690: 2063 616e 2064 6563 6964 650d 0a20 2020   can decide..   
+000396a0: 2020 2020 2020 2020 2023 206f 6e20 7768           # on wh
+000396b0: 6574 6865 7220 7468 6579 2077 616e 7420  ether they want 
+000396c0: 746f 2068 616e 646c 6520 7468 6174 2e20  to handle that. 
+000396d0: 2849 6465 616c 6c79 2c20 7765 2764 2068  (Ideally, we'd h
+000396e0: 6176 6520 6120 7761 7920 746f 2070 6172  ave a way to par
+000396f0: 616d 6574 6572 697a 6520 7468 6973 0d0a  ameterize this..
+00039700: 2020 2020 2020 2020 2020 2020 2320 6275              # bu
+00039710: 7420 7468 6520 7072 6f74 6f63 6f6c 2064  t the protocol d
+00039720: 6f65 736e 2774 2073 7570 706f 7274 2069  oesn't support i
+00039730: 7420 6173 206f 6620 7079 6172 726f 7720  t as of pyarrow 
+00039740: 342e 302e 2049 6e20 616e 7920 6361 7365  4.0. In any case
+00039750: 2c20 6f6e 6c79 2074 6865 2062 6974 6d61  , only the bitma
+00039760: 736b 0d0a 2020 2020 2020 2020 2020 2020  sk..            
+00039770: 2320 6e65 6564 7320 746f 2062 6520 7265  # needs to be re
+00039780: 2d63 7265 6174 6564 206c 6174 6572 2069  -created later i
+00039790: 6620 7468 6520 7573 6572 2077 616e 7473  f the user wants
+000397a0: 2074 6f20 636f 6e73 6964 6572 2074 6865   to consider the
+000397b0: 204e 614e 7320 6173 204e 412f 6e75 6c6c   NaNs as NA/null
+000397c0: 2076 616c 7565 732e 290d 0a20 2020 2020   values.)..     
+000397d0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+000397e0: 6469 6d20 3e3d 2032 3a0d 0a20 2020 2020  dim >= 2:..     
+000397f0: 2020 2020 2020 2020 2020 2023 204e 4f54             # NOT
+00039800: 453a 2041 7320 6f66 2070 7961 7272 6f77  E: As of pyarrow
+00039810: 2034 2e30 2c20 7468 6973 206d 6574 686f   4.0, this metho
+00039820: 6420 646f 6573 6e27 7420 7375 7070 6f72  d doesn't suppor
+00039830: 7420 6120 6074 7970 6560 2061 7267 756d  t a `type` argum
+00039840: 656e 742e 0d0a 2020 2020 2020 2020 2020  ent...          
+00039850: 2020 2020 2020 7265 7475 726e 2070 612e        return pa.
+00039860: 5465 6e73 6f72 2e66 726f 6d5f 6e75 6d70  Tensor.from_nump
+00039870: 7928 7365 6c66 2e5f 6e70 290d 0a20 2020  y(self._np)..   
+00039880: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00039890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000398a0: 7265 7475 726e 2070 612e 6172 7261 7928  return pa.array(
+000398b0: 7365 6c66 2e5f 6e70 2c20 7479 7065 3d74  self._np, type=t
+000398c0: 7970 6529 0d0a 0d0a 2020 2020 2020 2020  ype)....        
+000398d0: 656c 6966 206e 702e 6973 7375 6264 7479  elif np.issubdty
+000398e0: 7065 2873 656c 662e 6474 7970 652c 2062  pe(self.dtype, b
+000398f0: 6f6f 6c29 3a0d 0a20 2020 2020 2020 2020  ool):..         
+00039900: 2020 2069 6620 7365 6c66 2e6e 6469 6d20     if self.ndim 
+00039910: 3e3d 2032 3a0d 0a20 2020 2020 2020 2020  >= 2:..         
+00039920: 2020 2020 2020 2023 204e 4f54 453a 2041         # NOTE: A
+00039930: 7320 6f66 2070 7961 7272 6f77 2034 2e30  s of pyarrow 4.0
+00039940: 2c20 7468 6973 206d 6574 686f 6420 646f  , this method do
+00039950: 6573 6e27 7420 7375 7070 6f72 7420 6120  esn't support a 
+00039960: 6074 7970 6560 2061 7267 756d 656e 742e  `type` argument.
+00039970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00039980: 2020 7265 7475 726e 2070 612e 5465 6e73    return pa.Tens
+00039990: 6f72 2e66 726f 6d5f 6e75 6d70 7928 7365  or.from_numpy(se
+000399a0: 6c66 2e5f 6e70 290d 0a20 2020 2020 2020  lf._np)..       
+000399b0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+000399c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000399d0: 726e 2070 612e 6172 7261 7928 7365 6c66  rn pa.array(self
+000399e0: 2e5f 6e70 2c20 7479 7065 3d74 7970 6529  ._np, type=type)
+000399f0: 0d0a 0d0a 2020 2020 2020 2020 656c 6966  ....        elif
+00039a00: 206e 702e 6973 7375 6264 7479 7065 2873   np.issubdtype(s
+00039a10: 656c 662e 6474 7970 652c 2062 7974 6573  elf.dtype, bytes
+00039a20: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00039a30: 2320 4966 2074 6865 2063 616c 6c65 7220  # If the caller 
+00039a40: 7761 6e74 7320 746f 2063 6f6e 7665 7274  wants to convert
+00039a50: 2065 6d70 7479 2073 7472 696e 6773 2074   empty strings t
+00039a60: 6f20 6e75 6c6c 732c 2067 6574 2061 206d  o nulls, get a m
+00039a70: 6173 6b20 6f66 2069 6e76 616c 6964 732e  ask of invalids.
+00039a80: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00039a90: 2065 6d70 7479 5f73 7472 696e 6773 5f74   empty_strings_t
+00039aa0: 6f5f 6e75 6c6c 3a0d 0a20 2020 2020 2020  o_null:..       
+00039ab0: 2020 2020 2020 2020 2069 6e76 616c 6964           invalid
+00039ac0: 735f 6d61 736b 203d 2073 656c 6620 3d3d  s_mask = self ==
+00039ad0: 2073 656c 662e 696e 760d 0a0d 0a20 2020   self.inv....   
+00039ae0: 2020 2020 2020 2020 2020 2020 2023 2049               # I
+00039af0: 6620 616c 6c20 7661 6c75 6573 2061 7265  f all values are
+00039b00: 2076 616c 6964 2c20 646f 6e27 7420 626f   valid, don't bo
+00039b10: 7468 6572 2063 7265 6174 696e 6720 616e  ther creating an
+00039b20: 2061 6c6c 2d46 616c 7365 206d 6173 6b2c   all-False mask,
+00039b30: 2069 7427 7320 6a75 7374 2077 6173 7469   it's just wasti
+00039b40: 6e67 206d 656d 6f72 792e 0d0a 2020 2020  ng memory...    
+00039b50: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00039b60: 6f74 2069 6e76 616c 6964 735f 6d61 736b  ot invalids_mask
+00039b70: 2e61 6e79 2829 3a0d 0a20 2020 2020 2020  .any():..       
+00039b80: 2020 2020 2020 2020 2020 2020 2069 6e76               inv
+00039b90: 616c 6964 735f 6d61 736b 203d 204e 6f6e  alids_mask = Non
+00039ba0: 650d 0a20 2020 2020 2020 2020 2020 2065  e..            e
+00039bb0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00039bc0: 2020 2020 2020 696e 7661 6c69 6473 5f6d        invalids_m
+00039bd0: 6173 6b20 3d20 4e6f 6e65 0d0a 0d0a 2020  ask = None....  
+00039be0: 2020 2020 2020 2020 2020 2320 446f 6573            # Does
+00039bf0: 2074 6865 2063 616c 6c65 7220 7761 6e74   the caller want
+00039c00: 2074 6f20 7072 6573 6572 7665 2074 6865   to preserve the
+00039c10: 2066 6978 6564 2d6c 656e 6774 6820 6269   fixed-length bi
+00039c20: 6e61 7279 2064 6174 613f 0d0a 2020 2020  nary data?..    
+00039c30: 2020 2020 2020 2020 6966 2070 7265 7365          if prese
+00039c40: 7276 655f 6669 7865 645f 6279 7465 733a  rve_fixed_bytes:
+00039c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00039c60: 2020 2320 436f 6e76 6572 7420 746f 2061    # Convert to a
+00039c70: 2066 6978 6564 2d6c 656e 6774 6820 6269   fixed-length bi
+00039c80: 6e61 7279 2028 2762 7974 6573 2729 2074  nary ('bytes') t
+00039c90: 7970 652e 0d0a 2020 2020 2020 2020 2020  ype...          
+00039ca0: 2020 2020 2020 656c 656d 656e 745f 7374        element_st
+00039cb0: 725f 6c65 6e67 7468 203d 206e 702e 6474  r_length = np.dt
+00039cc0: 7970 6528 7365 6c66 2e64 7479 7065 292e  ype(self.dtype).
+00039cd0: 6974 656d 7369 7a65 0d0a 2020 2020 2020  itemsize..      
+00039ce0: 2020 2020 2020 2020 2020 6172 725f 7479            arr_ty
+00039cf0: 7065 203d 2070 612e 6269 6e61 7279 2865  pe = pa.binary(e
+00039d00: 6c65 6d65 6e74 5f73 7472 5f6c 656e 6774  lement_str_lengt
+00039d10: 6829 2069 6620 7479 7065 2069 7320 4e6f  h) if type is No
+00039d20: 6e65 2065 6c73 6520 7479 7065 0d0a 2020  ne else type..  
+00039d30: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00039d40: 7475 726e 2070 612e 6172 7261 7928 7365  turn pa.array(se
+00039d50: 6c66 2e5f 6e70 2c20 6d61 736b 3d69 6e76  lf._np, mask=inv
+00039d60: 616c 6964 735f 6d61 736b 2c20 7479 7065  alids_mask, type
+00039d70: 3d61 7272 5f74 7970 6529 0d0a 2020 2020  =arr_type)..    
+00039d80: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00039d90: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00039da0: 2043 6f6e 7665 7274 2074 6869 7320 6172   Convert this ar
+00039db0: 7261 7920 746f 2061 2070 7961 7272 6f77  ray to a pyarrow
+00039dc0: 2076 6172 6961 626c 652d 6c65 6e67 7468   variable-length
+00039dd0: 2073 7472 696e 6720 6172 7261 792e 0d0a   string array...
+00039de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00039df0: 6966 2074 7970 6520 6973 204e 6f6e 653a  if type is None:
+00039e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00039e10: 2020 2020 2020 7479 7065 203d 2070 612e        type = pa.
+00039e20: 7374 7269 6e67 2829 0d0a 2020 2020 2020  string()..      
+00039e30: 2020 2020 2020 2020 2020 2320 436f 6e76            # Conv
+00039e40: 6572 7420 6173 2055 6e69 636f 6465 206e  ert as Unicode n
+00039e50: 6461 7272 6179 2074 6f20 7374 7269 6e67  darray to string
+00039e60: 6172 7261 792c 2061 7320 6279 7465 7374  array, as bytest
+00039e70: 7269 6e67 2064 6f65 7320 6e6f 7420 7072  ring does not pr
+00039e80: 6573 6572 7665 2065 6c65 6d65 6e74 206c  eserve element l
+00039e90: 656e 6774 6820 2872 6970 7461 626c 6523  ength (riptable#
+00039ea0: 3234 3929 0d0a 2020 2020 2020 2020 2020  249)..          
+00039eb0: 2020 2020 2020 7265 7475 726e 2070 612e        return pa.
+00039ec0: 6172 7261 7928 6e70 2e61 7272 6179 2873  array(np.array(s
+00039ed0: 656c 662e 5f6e 702c 2064 7479 7065 3d22  elf._np, dtype="
+00039ee0: 5522 292c 206d 6173 6b3d 696e 7661 6c69  U"), mask=invali
+00039ef0: 6473 5f6d 6173 6b2c 2074 7970 653d 7479  ds_mask, type=ty
+00039f00: 7065 290d 0a0d 0a20 2020 2020 2020 2065  pe)....        e
+00039f10: 6c69 6620 6e70 2e69 7373 7562 6474 7970  lif np.issubdtyp
+00039f20: 6528 7365 6c66 2e64 7479 7065 2c20 7374  e(self.dtype, st
+00039f30: 7229 3a0d 0a20 2020 2020 2020 2020 2020  r):..           
+00039f40: 2023 2049 6620 7468 6520 6361 6c6c 6572   # If the caller
+00039f50: 2077 616e 7473 2074 6f20 636f 6e76 6572   wants to conver
+00039f60: 7420 656d 7074 7920 7374 7269 6e67 7320  t empty strings 
+00039f70: 746f 206e 756c 6c73 2c20 6765 7420 6120  to nulls, get a 
+00039f80: 6d61 736b 206f 6620 696e 7661 6c69 6473  mask of invalids
+00039f90: 2e0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+00039fa0: 6620 656d 7074 795f 7374 7269 6e67 735f  f empty_strings_
+00039fb0: 746f 5f6e 756c 6c3a 0d0a 2020 2020 2020  to_null:..      
+00039fc0: 2020 2020 2020 2020 2020 696e 7661 6c69            invali
+00039fd0: 6473 5f6d 6173 6b20 3d20 7365 6c66 203d  ds_mask = self =
+00039fe0: 3d20 7365 6c66 2e69 6e76 0d0a 0d0a 2020  = self.inv....  
+00039ff0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0003a000: 4966 2061 6c6c 2076 616c 7565 7320 6172  If all values ar
+0003a010: 6520 7661 6c69 642c 2064 6f6e 2774 2062  e valid, don't b
+0003a020: 6f74 6865 7220 6372 6561 7469 6e67 2061  other creating a
+0003a030: 6e20 616c 6c2d 4661 6c73 6520 6d61 736b  n all-False mask
+0003a040: 2c20 6974 2773 206a 7573 7420 7761 7374  , it's just wast
+0003a050: 696e 6720 6d65 6d6f 7279 2e0d 0a20 2020  ing memory...   
+0003a060: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0003a070: 6e6f 7420 696e 7661 6c69 6473 5f6d 6173  not invalids_mas
+0003a080: 6b2e 616e 7928 293a 0d0a 2020 2020 2020  k.any():..      
+0003a090: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0003a0a0: 7661 6c69 6473 5f6d 6173 6b20 3d20 4e6f  valids_mask = No
+0003a0b0: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
+0003a0c0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0003a0d0: 2020 2020 2020 2069 6e76 616c 6964 735f         invalids_
+0003a0e0: 6d61 736b 203d 204e 6f6e 650d 0a0d 0a20  mask = None.... 
+0003a0f0: 2020 2020 2020 2020 2020 2023 2070 7961             # pya
+0003a100: 7272 6f77 2028 6173 206f 6620 7634 2e30  rrow (as of v4.0
+0003a110: 2920 646f 6573 206e 6f74 2068 6176 6520  ) does not have 
+0003a120: 6120 6669 7865 642d 7369 7a65 2055 6e69  a fixed-size Uni
+0003a130: 636f 6465 2073 7472 696e 6720 6461 7461  code string data
+0003a140: 2074 7970 652c 2073 6f20 756e 6c69 6b65   type, so unlike
+0003a150: 2074 6865 2027 6279 7465 7327 0d0a 2020   the 'bytes'..  
+0003a160: 2020 2020 2020 2020 2020 2320 6861 6e64            # hand
+0003a170: 6c69 6e67 2061 626f 7665 2066 6f72 2041  ling above for A
+0003a180: 5343 4949 2073 7472 696e 6773 2c20 7765  SCII strings, we
+0003a190: 2068 6176 6520 746f 2075 7365 2074 6865   have to use the
+0003a1a0: 2076 6172 6961 626c 652d 6c65 6e67 7468   variable-length
+0003a1b0: 2073 7472 696e 6720 6172 7261 7920 7479   string array ty
+0003a1c0: 7065 2e0d 0a20 2020 2020 2020 2020 2020  pe...           
+0003a1d0: 2069 6620 7479 7065 2069 7320 4e6f 6e65   if type is None
+0003a1e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0003a1f0: 2020 2074 7970 6520 3d20 7061 2e73 7472     type = pa.str
+0003a200: 696e 6728 290d 0a20 2020 2020 2020 2020  ing()..         
+0003a210: 2020 2072 6574 7572 6e20 7061 2e61 7272     return pa.arr
+0003a220: 6179 2873 656c 662e 5f6e 702c 206d 6173  ay(self._np, mas
+0003a230: 6b3d 696e 7661 6c69 6473 5f6d 6173 6b2c  k=invalids_mask,
+0003a240: 2074 7970 653d 7479 7065 290d 0a0d 0a20   type=type).... 
+0003a250: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0003a260: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0003a270: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+0003a280: 726f 7228 6622 4661 7374 4172 7261 7920  ror(f"FastArray 
+0003a290: 7769 7468 2064 7479 7065 2027 7b6e 702e  with dtype '{np.
+0003a2a0: 6474 7970 6528 7365 6c66 2e64 7479 7065  dtype(self.dtype
+0003a2b0: 297d 2720 6973 206e 6f74 2073 7570 706f  )}' is not suppo
+0003a2c0: 7274 6564 2e22 290d 0a0d 0a20 2020 2064  rted.")....    d
+0003a2d0: 6566 205f 5f61 7272 6f77 5f61 7272 6179  ef __arrow_array
+0003a2e0: 5f5f 2873 656c 662c 2074 7970 653a 204f  __(self, type: O
+0003a2f0: 7074 696f 6e61 6c5b 2270 612e 4461 7461  ptional["pa.Data
+0003a300: 5479 7065 225d 203d 204e 6f6e 6529 202d  Type"] = None) -
+0003a310: 3e20 556e 696f 6e5b 2270 612e 4172 7261  > Union["pa.Arra
+0003a320: 7922 2c20 2270 612e 4368 756e 6b65 6441  y", "pa.ChunkedA
+0003a330: 7272 6179 225d 3a0d 0a20 2020 2020 2020  rray"]:..       
+0003a340: 2022 2222 0d0a 2020 2020 2020 2020 496d   """..        Im
+0003a350: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+0003a360: 7468 6520 6060 5f5f 6172 726f 775f 6172  the ``__arrow_ar
+0003a370: 7261 795f 5f60 6020 7072 6f74 6f63 6f6c  ray__`` protocol
+0003a380: 2066 6f72 2063 6f6e 7665 7273 696f 6e20   for conversion 
+0003a390: 746f 2061 2070 7961 7272 6f77 2061 7272  to a pyarrow arr
+0003a3a0: 6179 2e0d 0a0d 0a20 2020 2020 2020 2050  ay.....        P
+0003a3b0: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
+0003a3c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+0003a3d0: 2020 2020 2020 2074 7970 6520 3a20 7079         type : py
+0003a3e0: 6172 726f 772e 4461 7461 5479 7065 2c20  arrow.DataType, 
+0003a3f0: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
+0003a400: 7473 2074 6f20 4e6f 6e65 0d0a 0d0a 2020  ts to None....  
+0003a410: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
+0003a420: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
+0003a430: 2020 2020 2020 2020 7079 6172 726f 772e          pyarrow.
+0003a440: 4172 7261 7920 6f72 2070 7961 7272 6f77  Array or pyarrow
+0003a450: 2e43 6875 6e6b 6564 4172 7261 790d 0a0d  .ChunkedArray...
+0003a460: 0a20 2020 2020 2020 204e 6f74 6573 0d0a  .        Notes..
+0003a470: 2020 2020 2020 2020 2d2d 2d2d 2d0d 0a20          -----.. 
+0003a480: 2020 2020 2020 2068 7474 7073 3a2f 2f61         https://a
+0003a490: 7272 6f77 2e61 7061 6368 652e 6f72 672f  rrow.apache.org/
+0003a4a0: 646f 6373 2f70 7974 686f 6e2f 6578 7465  docs/python/exte
+0003a4b0: 6e64 696e 675f 7479 7065 732e 6874 6d6c  nding_types.html
+0003a4c0: 2363 6f6e 7472 6f6c 6c69 6e67 2d63 6f6e  #controlling-con
+0003a4d0: 7665 7273 696f 6e2d 746f 2d70 7961 7272  version-to-pyarr
+0003a4e0: 6f77 2d61 7272 6179 2d77 6974 682d 7468  ow-array-with-th
+0003a4f0: 652d 6172 726f 772d 6172 7261 792d 7072  e-arrow-array-pr
+0003a500: 6f74 6f63 6f6c 0d0a 2020 2020 2020 2020  otocol..        
+0003a510: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+0003a520: 7572 6e20 7365 6c66 2e74 6f5f 6172 726f  urn self.to_arro
+0003a530: 7728 7479 7065 3d74 7970 652c 2070 7265  w(type=type, pre
+0003a540: 7365 7276 655f 6669 7865 645f 6279 7465  serve_fixed_byte
+0003a550: 733d 4661 6c73 652c 2065 6d70 7479 5f73  s=False, empty_s
+0003a560: 7472 696e 6773 5f74 6f5f 6e75 6c6c 3d54  trings_to_null=T
+0003a570: 7275 6529 0d0a 0d0a 2020 2020 2320 2d2d  rue)....    # --
 0003a580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003a590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003a5a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0003a5b0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 4063  --------..    @c
-0003a5c0: 6c61 7373 6d65 7468 6f64 0d0a 2020 2020  lassmethod..    
-0003a5d0: 6465 6620 7265 6769 7374 6572 5f66 756e  def register_fun
-0003a5e0: 6374 696f 6e28 636c 732c 206e 616d 652c  ction(cls, name,
-0003a5f0: 2066 756e 6329 3a0d 0a20 2020 2020 2020   func):..       
-0003a600: 2022 2222 0d0a 2020 2020 2020 2020 5573   """..        Us
-0003a610: 6564 2074 6f20 7265 6769 7374 6572 2066  ed to register f
-0003a620: 756e 6374 696f 6e73 2074 6f20 4661 7374  unctions to Fast
-0003a630: 4172 7261 792e 0d0a 2020 2020 2020 2020  Array...        
-0003a640: 5573 6564 2062 7920 7274 5f66 6173 7461  Used by rt_fasta
-0003a650: 7272 6179 6e75 6d62 610d 0a20 2020 2020  rraynumba..     
-0003a660: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-0003a670: 7365 7461 7474 7228 636c 732c 206e 616d  setattr(cls, nam
-0003a680: 652c 2066 756e 6329 0d0a 0d0a 2020 2020  e, func)....    
-0003a690: 6465 6620 6170 706c 795f 7363 6865 6d61  def apply_schema
-0003a6a0: 2873 656c 662c 2073 6368 656d 6129 3a0d  (self, schema):.
-0003a6b0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0003a6c0: 2020 2020 2020 4170 706c 7920 6120 7363        Apply a sc
-0003a6d0: 6865 6d61 2063 6f6e 7461 696e 696e 6720  hema containing 
-0003a6e0: 6465 7363 7269 7074 6976 6520 696e 666f  descriptive info
-0003a6f0: 726d 6174 696f 6e20 746f 2074 6865 2046  rmation to the F
-0003a700: 6173 7441 7272 6179 0d0a 0d0a 2020 2020  astArray....    
-0003a710: 2020 2020 3a70 6172 616d 2073 6368 656d      :param schem
-0003a720: 613a 2064 6963 740d 0a20 2020 2020 2020  a: dict..       
-0003a730: 203a 7265 7475 726e 3a20 6469 6374 696f   :return: dictio
-0003a740: 6e61 7279 206f 6620 6465 7669 6174 696f  nary of deviatio
-0003a750: 6e73 2066 726f 6d20 7468 6520 7363 6865  ns from the sche
-0003a760: 6d61 0d0a 2020 2020 2020 2020 2222 220d  ma..        """.
-0003a770: 0a20 2020 2020 2020 2066 726f 6d20 2e72  .        from .r
-0003a780: 745f 6d65 7461 2069 6d70 6f72 7420 6170  t_meta import ap
-0003a790: 706c 795f 7363 6865 6d61 2061 7320 5f61  ply_schema as _a
-0003a7a0: 7070 6c79 5f73 6368 656d 610d 0a0d 0a20  pply_schema.... 
-0003a7b0: 2020 2020 2020 2072 6574 7572 6e20 5f61         return _a
-0003a7c0: 7070 6c79 5f73 6368 656d 6128 7365 6c66  pply_schema(self
-0003a7d0: 2c20 7363 6865 6d61 290d 0a0d 0a20 2020  , schema)....   
-0003a7e0: 2064 6566 2069 6e66 6f28 7365 6c66 2c20   def info(self, 
-0003a7f0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-0003a800: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-0003a810: 2052 6574 7572 6e20 6120 6465 7363 7269   Return a descri
-0003a820: 7074 696f 6e20 6f66 2074 6865 2069 6e70  ption of the inp
-0003a830: 7574 2061 7272 6179 2773 2063 6f6e 7465  ut array's conte
-0003a840: 6e74 732e 0d0a 0d0a 2020 2020 2020 2020  nts.....        
-0003a850: 5468 6973 2069 6e66 6f72 6d61 7469 6f6e  This information
-0003a860: 2069 7320 7365 7420 7573 696e 6720 6046   is set using `F
-0003a870: 6173 7441 7272 6179 2e61 7070 6c79 5f73  astArray.apply_s
-0003a880: 6368 656d 6160 2061 6e64 2069 6e63 6c75  chema` and inclu
-0003a890: 6465 7320 7468 6520 7374 6577 6172 640d  des the steward.
-0003a8a0: 0a20 2020 2020 2020 2061 6e64 2064 7479  .        and dty
-0003a8b0: 7065 2e0d 0a0d 0a20 2020 2020 2020 2050  pe.....        P
-0003a8c0: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-0003a8d0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-0003a8e0: 2020 2020 2020 202a 2a6b 7761 7267 7320         **kwargs 
-0003a8f0: 3a20 6f70 7469 6f6e 616c 0d0a 2020 2020  : optional..    
-0003a900: 2020 2020 2020 2020 4b65 7977 6f72 6420          Keyword 
-0003a910: 6172 6775 6d65 6e74 7320 7061 7373 6564  arguments passed
-0003a920: 2074 6f20 3a66 756e 633a 602e 7274 5f6d   to :func:`.rt_m
-0003a930: 6574 612e 696e 666f 602e 0d0a 0d0a 2020  eta.info`.....  
-0003a940: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
-0003a950: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
-0003a960: 2020 2020 2020 2020 3a63 6c61 7373 3a60          :class:`
-0003a970: 2e72 745f 6d65 7461 2e49 6e66 6f60 0d0a  .rt_meta.Info`..
-0003a980: 2020 2020 2020 2020 2020 2020 4120 6465              A de
-0003a990: 7363 7269 7074 696f 6e20 6f66 2074 6865  scription of the
-0003a9a0: 2069 6e70 7574 2061 7272 6179 2773 2063   input array's c
-0003a9b0: 6f6e 7465 6e74 732e 0d0a 0d0a 2020 2020  ontents.....    
-0003a9c0: 2020 2020 5365 6520 416c 736f 0d0a 2020      See Also..  
-0003a9d0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a        --------..
-0003a9e0: 2020 2020 2020 2020 4661 7374 4172 7261          FastArra
-0003a9f0: 792e 646f 6320 3a20 5265 7475 726e 2074  y.doc : Return t
-0003aa00: 6865 2060 2e44 6f63 6020 6f62 6a65 6374  he `.Doc` object
-0003aa10: 2066 6f72 2074 6865 2069 6e70 7574 2060   for the input `
-0003aa20: 4661 7374 4172 7261 7960 2e0d 0a20 2020  FastArray`...   
-0003aa30: 2020 2020 202e 4361 7465 676f 7269 6361       .Categorica
-0003aa40: 6c2e 696e 666f 203a 2044 6973 706c 6179  l.info : Display
-0003aa50: 2061 2064 6573 6372 6970 7469 6f6e 206f   a description o
-0003aa60: 6620 7468 6520 696e 7075 7420 602e 4361  f the input `.Ca
-0003aa70: 7465 676f 7269 6361 6c60 2e0d 0a20 2020  tegorical`...   
-0003aa80: 2020 2020 202e 5374 7275 6374 2e69 6e66       .Struct.inf
-0003aa90: 6f20 3a0d 0a20 2020 2020 2020 2020 2020  o :..           
-0003aaa0: 2052 6574 7572 6e20 616e 206f 626a 6563   Return an objec
-0003aab0: 7420 636f 6e74 6169 6e69 6e67 2061 2064  t containing a d
-0003aac0: 6573 6372 6970 7469 6f6e 206f 6620 7468  escription of th
-0003aad0: 6520 696e 7075 7420 7374 7275 6374 7572  e input structur
-0003aae0: 6527 7320 636f 6e74 656e 7473 2e0d 0a0d  e's contents....
-0003aaf0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-0003ab00: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-0003ab10: 2d2d 2d0d 0a20 2020 2020 2020 2052 6574  ---..        Ret
-0003ab20: 7572 6e20 7468 6520 6465 7363 7269 7074  urn the descript
-0003ab30: 696f 6e20 6f66 2074 6865 2069 6e70 7574  ion of the input
-0003ab40: 2061 7272 6179 2773 2063 6f6e 7465 6e74   array's content
-0003ab50: 733a 0d0a 0d0a 2020 2020 2020 2020 3e3e  s:....        >>
-0003ab60: 3e20 6120 3d20 7274 2e46 4128 5b31 2c20  > a = rt.FA([1, 
-0003ab70: 322c 2033 2c20 342c 2035 5d29 0d0a 2020  2, 3, 4, 5])..  
-0003ab80: 2020 2020 2020 3e3e 3e20 612e 696e 666f        >>> a.info
-0003ab90: 2829 0d0a 2020 2020 2020 2020 4465 7363  ()..        Desc
-0003aba0: 7269 7074 696f 6e3a 203c 6e6f 2064 6573  ription: <no des
-0003abb0: 6372 6970 7469 6f6e 3e0d 0a20 2020 2020  cription>..     
-0003abc0: 2020 2053 7465 7761 7264 3a20 3c6e 6f20     Steward: <no 
-0003abd0: 7374 6577 6172 643e 0d0a 2020 2020 2020  steward>..      
-0003abe0: 2020 5479 7065 3a20 696e 7433 320d 0a0d    Type: int32...
-0003abf0: 0a20 2020 2020 2020 2041 7070 6c79 2061  .        Apply a
-0003ac00: 2073 6368 656d 6120 616e 6420 7265 7475   schema and retu
-0003ac10: 726e 2074 6865 2064 6573 6372 6970 7469  rn the descripti
-0003ac20: 6f6e 206f 6620 7468 6520 696e 7075 7420  on of the input 
-0003ac30: 6172 7261 7927 7320 636f 6e74 656e 7473  array's contents
-0003ac40: 3a0d 0a0d 0a20 2020 2020 2020 203e 3e3e  :....        >>>
-0003ac50: 2073 6368 656d 6120 3d20 7b22 4465 7363   schema = {"Desc
-0003ac60: 7269 7074 696f 6e22 3a20 2254 6869 7320  ription": "This 
-0003ac70: 6973 2061 6e20 6172 7261 7922 2c20 2253  is an array", "S
-0003ac80: 7465 7761 7264 223a 2022 4272 6961 6e22  teward": "Brian"
-0003ac90: 7d0d 0a20 2020 2020 2020 203e 3e3e 2061  }..        >>> a
-0003aca0: 2e61 7070 6c79 5f73 6368 656d 6128 7363  .apply_schema(sc
-0003acb0: 6865 6d61 290d 0a20 2020 2020 2020 207b  hema)..        {
-0003acc0: 7d0d 0a20 2020 2020 2020 203e 3e3e 2061  }..        >>> a
-0003acd0: 2e69 6e66 6f28 290d 0a20 2020 2020 2020  .info()..       
-0003ace0: 2044 6573 6372 6970 7469 6f6e 3a20 5468   Description: Th
-0003acf0: 6973 2069 7320 616e 2061 7272 6179 0d0a  is is an array..
-0003ad00: 2020 2020 2020 2020 5374 6577 6172 643a          Steward:
-0003ad10: 2042 7269 616e 0d0a 2020 2020 2020 2020   Brian..        
-0003ad20: 5479 7065 3a20 696e 7433 320d 0a0d 0a20  Type: int32.... 
-0003ad30: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
-0003ad40: 6520 6465 7363 7269 7074 696f 6e20 6f66  e description of
-0003ad50: 2074 6865 2069 6e70 7574 2061 7272 6179   the input array
-0003ad60: 2773 2063 6f6e 7465 6e74 7320 7769 7468  's contents with
-0003ad70: 2061 2074 6974 6c65 3a0d 0a0d 0a20 2020   a title:....   
-0003ad80: 2020 2020 203e 3e3e 2061 2e69 6e66 6f28       >>> a.info(
-0003ad90: 7469 746c 653d 2254 6573 7422 290d 0a20  title="Test").. 
-0003ada0: 2020 2020 2020 2054 6573 740d 0a20 2020         Test..   
-0003adb0: 2020 2020 203d 3d3d 3d0d 0a20 2020 2020       ====..     
-0003adc0: 2020 2044 6573 6372 6970 7469 6f6e 3a20     Description: 
-0003add0: 5468 6973 2069 7320 616e 2061 7272 6179  This is an array
-0003ade0: 0d0a 2020 2020 2020 2020 5374 6577 6172  ..        Stewar
-0003adf0: 643a 2042 7269 616e 0d0a 2020 2020 2020  d: Brian..      
-0003ae00: 2020 5479 7065 3a20 696e 7433 320d 0a20    Type: int32.. 
-0003ae10: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-0003ae20: 2020 2020 6672 6f6d 202e 7274 5f6d 6574      from .rt_met
-0003ae30: 6120 696d 706f 7274 2069 6e66 6f20 6173  a import info as
-0003ae40: 205f 696e 666f 0d0a 0d0a 2020 2020 2020   _info....      
-0003ae50: 2020 7265 7475 726e 205f 696e 666f 2873    return _info(s
-0003ae60: 656c 662c 202a 2a6b 7761 7267 7329 0d0a  elf, **kwargs)..
-0003ae70: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-0003ae80: 0a20 2020 2064 6566 2064 6f63 2873 656c  .    def doc(sel
-0003ae90: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
-0003aea0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0003aeb0: 2074 6865 2060 2e44 6f63 6020 6f62 6a65   the `.Doc` obje
-0003aec0: 6374 2066 6f72 2074 6865 2069 6e70 7574  ct for the input
-0003aed0: 2060 4661 7374 4172 7261 7960 2e0d 0a0d   `FastArray`....
-0003aee0: 0a20 2020 2020 2020 2049 6620 6e6f 2060  .        If no `
-0003aef0: 2e44 6f63 6020 6f62 6a65 6374 2065 7869  .Doc` object exi
-0003af00: 7374 732c 2072 6574 7572 6e20 604e 6f6e  sts, return `Non
-0003af10: 6560 2e0d 0a0d 0a20 2020 2020 2020 2052  e`.....        R
-0003af20: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
-0003af30: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-0003af40: 2060 7e72 6970 7461 626c 652e 7274 5f6d   `~riptable.rt_m
-0003af50: 6574 612e 446f 6360 0d0a 2020 2020 2020  eta.Doc`..      
-0003af60: 2020 2020 2020 5468 6520 602e 446f 6360        The `.Doc`
-0003af70: 206f 626a 6563 7420 666f 7220 7468 6520   object for the 
-0003af80: 696e 7075 7420 6046 6173 7441 7272 6179  input `FastArray
-0003af90: 602e 2049 6620 6e6f 2060 2e44 6f63 6020  `. If no `.Doc` 
-0003afa0: 6f62 6a65 6374 0d0a 2020 2020 2020 2020  object..        
-0003afb0: 2020 2020 6578 6973 7473 2c20 7265 7475      exists, retu
-0003afc0: 726e 2060 4e6f 6e65 602e 0d0a 0d0a 2020  rn `None`.....  
-0003afd0: 2020 2020 2020 5365 6520 416c 736f 0d0a        See Also..
-0003afe0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-0003aff0: 0d0a 2020 2020 2020 2020 4661 7374 4172  ..        FastAr
-0003b000: 7261 792e 696e 666f 203a 2052 6574 7572  ray.info : Retur
-0003b010: 6e20 6120 6465 7363 7269 7074 696f 6e20  n a description 
-0003b020: 6f66 2074 6865 2069 6e70 7574 2061 7272  of the input arr
-0003b030: 6179 2773 2063 6f6e 7465 6e74 732e 0d0a  ay's contents...
-0003b040: 2020 2020 2020 2020 7e72 6970 7461 626c          ~riptabl
-0003b050: 652e 7274 5f6d 6574 612e 6170 706c 795f  e.rt_meta.apply_
-0003b060: 7363 6865 6d61 203a 2053 6574 2060 2e44  schema : Set `.D
-0003b070: 6f63 6020 6f62 6a65 6374 2076 616c 7565  oc` object value
-0003b080: 732e 0d0a 0d0a 2020 2020 2020 2020 4578  s.....        Ex
-0003b090: 616d 706c 6573 0d0a 2020 2020 2020 2020  amples..        
-0003b0a0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-0003b0b0: 2020 4e6f 2060 2e44 6f63 6020 6f62 6a65    No `.Doc` obje
-0003b0c0: 6374 2065 7869 7374 733a 0d0a 0d0a 2020  ct exists:....  
-0003b0d0: 2020 2020 2020 3e3e 3e20 6120 3d20 7274        >>> a = rt
-0003b0e0: 2e46 4128 5b31 2c20 322c 2033 2c20 342c  .FA([1, 2, 3, 4,
-0003b0f0: 2035 5d29 0d0a 2020 2020 2020 2020 3e3e   5])..        >>
-0003b100: 3e20 7072 696e 7428 612e 646f 6329 0d0a  > print(a.doc)..
-0003b110: 2020 2020 2020 2020 4e6f 6e65 0d0a 0d0a          None....
-0003b120: 2020 2020 2020 2020 4170 706c 7920 6120          Apply a 
-0003b130: 7363 6865 6d61 2061 6e64 2072 6574 7572  schema and retur
-0003b140: 6e20 7468 6520 602e 446f 6360 206f 626a  n the `.Doc` obj
-0003b150: 6563 743a 0d0a 0d0a 2020 2020 2020 2020  ect:....        
-0003b160: 3e3e 3e20 7363 6865 6d61 203d 207b 2244  >>> schema = {"D
-0003b170: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
-0003b180: 6973 2069 7320 616e 2061 7272 6179 222c  is is an array",
-0003b190: 2022 5374 6577 6172 6422 3a20 2242 7269   "Steward": "Bri
-0003b1a0: 616e 222c 2022 5479 7065 223a 2022 696e  an", "Type": "in
-0003b1b0: 7433 3222 7d0d 0a20 2020 2020 2020 203e  t32"}..        >
-0003b1c0: 3e3e 2061 2e61 7070 6c79 5f73 6368 656d  >> a.apply_schem
-0003b1d0: 6128 7363 6865 6d61 290d 0a20 2020 2020  a(schema)..     
-0003b1e0: 2020 207b 7d0d 0a20 2020 2020 2020 203e     {}..        >
-0003b1f0: 3e3e 2061 2e64 6f63 0d0a 2020 2020 2020  >> a.doc..      
-0003b200: 2020 4465 7363 7269 7074 696f 6e3a 2054    Description: T
-0003b210: 6869 7320 6973 2061 6e20 6172 7261 790d  his is an array.
-0003b220: 0a20 2020 2020 2020 2053 7465 7761 7264  .        Steward
-0003b230: 3a20 4272 6961 6e0d 0a20 2020 2020 2020  : Brian..       
-0003b240: 2054 7970 653a 2069 6e74 3332 0d0a 0d0a   Type: int32....
-0003b250: 2020 2020 2020 2020 5265 7475 726e 2073          Return s
-0003b260: 7065 6369 6669 6320 602e 446f 6360 206f  pecific `.Doc` o
-0003b270: 626a 6563 7420 696e 666f 726d 6174 696f  bject informatio
-0003b280: 6e3a 0d0a 0d0a 2020 2020 2020 2020 3e3e  n:....        >>
-0003b290: 3e20 612e 646f 632e 5f74 7970 650d 0a20  > a.doc._type.. 
-0003b2a0: 2020 2020 2020 2027 696e 7433 3227 0d0a         'int32'..
-0003b2b0: 2020 2020 2020 2020 3e3e 3e20 612e 646f          >>> a.do
-0003b2c0: 632e 5f64 6573 6372 6970 0d0a 2020 2020  c._descrip..    
-0003b2d0: 2020 2020 2754 6869 7320 6973 2061 6e20      'This is an 
-0003b2e0: 6172 7261 7927 0d0a 2020 2020 2020 2020  array'..        
-0003b2f0: 3e3e 3e20 612e 646f 632e 5f73 7465 7761  >>> a.doc._stewa
-0003b300: 7264 0d0a 2020 2020 2020 2020 2742 7269  rd..        'Bri
-0003b310: 616e 270d 0a20 2020 2020 2020 203e 3e3e  an'..        >>>
-0003b320: 2070 7269 6e74 2861 2e64 6f63 2e5f 6465   print(a.doc._de
-0003b330: 7461 696c 290d 0a20 2020 2020 2020 204e  tail)..        N
-0003b340: 6f6e 650d 0a20 2020 2020 2020 2022 2222  one..        """
-0003b350: 0d0a 2020 2020 2020 2020 6672 6f6d 202e  ..        from .
-0003b360: 7274 5f6d 6574 6120 696d 706f 7274 2064  rt_meta import d
-0003b370: 6f63 2061 7320 5f64 6f63 0d0a 0d0a 2020  oc as _doc....  
-0003b380: 2020 2020 2020 7265 7475 726e 205f 646f        return _do
-0003b390: 6328 7365 6c66 290d 0a0d 0a20 2020 2023  c(self)....    #
-0003b3a0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
-0003b3b0: 3d3d 3d3d 3d3d 3d20 454e 4420 4f46 2043  ======= END OF C
-0003b3c0: 4c41 5353 2044 4546 494e 4954 494f 4e20  LASS DEFINITION 
-0003b3d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0003b3e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d  ===============.
-0003b3f0: 0a0d 0a0d 0a23 202d 2d2d 2d2d 2d2d 2d2d  .....# ---------
+0003a5b0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2040  ---------..    @
+0003a5c0: 636c 6173 736d 6574 686f 640d 0a20 2020  classmethod..   
+0003a5d0: 2064 6566 2072 6567 6973 7465 725f 6675   def register_fu
+0003a5e0: 6e63 7469 6f6e 2863 6c73 2c20 6e61 6d65  nction(cls, name
+0003a5f0: 2c20 6675 6e63 293a 0d0a 2020 2020 2020  , func):..      
+0003a600: 2020 2222 220d 0a20 2020 2020 2020 2055    """..        U
+0003a610: 7365 6420 746f 2072 6567 6973 7465 7220  sed to register 
+0003a620: 6675 6e63 7469 6f6e 7320 746f 2046 6173  functions to Fas
+0003a630: 7441 7272 6179 2e0d 0a20 2020 2020 2020  tArray...       
+0003a640: 2055 7365 6420 6279 2072 745f 6661 7374   Used by rt_fast
+0003a650: 6172 7261 796e 756d 6261 0d0a 2020 2020  arraynumba..    
+0003a660: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0003a670: 2073 6574 6174 7472 2863 6c73 2c20 6e61   setattr(cls, na
+0003a680: 6d65 2c20 6675 6e63 290d 0a0d 0a20 2020  me, func)....   
+0003a690: 2064 6566 2061 7070 6c79 5f73 6368 656d   def apply_schem
+0003a6a0: 6128 7365 6c66 2c20 7363 6865 6d61 293a  a(self, schema):
+0003a6b0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0003a6c0: 2020 2020 2020 2041 7070 6c79 2061 2073         Apply a s
+0003a6d0: 6368 656d 6120 636f 6e74 6169 6e69 6e67  chema containing
+0003a6e0: 2064 6573 6372 6970 7469 7665 2069 6e66   descriptive inf
+0003a6f0: 6f72 6d61 7469 6f6e 2074 6f20 7468 6520  ormation to the 
+0003a700: 4661 7374 4172 7261 790d 0a0d 0a20 2020  FastArray....   
+0003a710: 2020 2020 203a 7061 7261 6d20 7363 6865       :param sche
+0003a720: 6d61 3a20 6469 6374 0d0a 2020 2020 2020  ma: dict..      
+0003a730: 2020 3a72 6574 7572 6e3a 2064 6963 7469    :return: dicti
+0003a740: 6f6e 6172 7920 6f66 2064 6576 6961 7469  onary of deviati
+0003a750: 6f6e 7320 6672 6f6d 2074 6865 2073 6368  ons from the sch
+0003a760: 656d 610d 0a20 2020 2020 2020 2022 2222  ema..        """
+0003a770: 0d0a 2020 2020 2020 2020 6672 6f6d 202e  ..        from .
+0003a780: 7274 5f6d 6574 6120 696d 706f 7274 2061  rt_meta import a
+0003a790: 7070 6c79 5f73 6368 656d 6120 6173 205f  pply_schema as _
+0003a7a0: 6170 706c 795f 7363 6865 6d61 0d0a 0d0a  apply_schema....
+0003a7b0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0003a7c0: 6170 706c 795f 7363 6865 6d61 2873 656c  apply_schema(sel
+0003a7d0: 662c 2073 6368 656d 6129 0d0a 0d0a 2020  f, schema)....  
+0003a7e0: 2020 6465 6620 696e 666f 2873 656c 662c    def info(self,
+0003a7f0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
+0003a800: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+0003a810: 2020 5265 7475 726e 2061 2064 6573 6372    Return a descr
+0003a820: 6970 7469 6f6e 206f 6620 7468 6520 696e  iption of the in
+0003a830: 7075 7420 6172 7261 7927 7320 636f 6e74  put array's cont
+0003a840: 656e 7473 2e0d 0a0d 0a20 2020 2020 2020  ents.....       
+0003a850: 2054 6869 7320 696e 666f 726d 6174 696f   This informatio
+0003a860: 6e20 6973 2073 6574 2075 7369 6e67 2060  n is set using `
+0003a870: 4661 7374 4172 7261 792e 6170 706c 795f  FastArray.apply_
+0003a880: 7363 6865 6d61 6020 616e 6420 696e 636c  schema` and incl
+0003a890: 7564 6573 2074 6865 2073 7465 7761 7264  udes the steward
+0003a8a0: 0d0a 2020 2020 2020 2020 616e 6420 6474  ..        and dt
+0003a8b0: 7970 652e 0d0a 0d0a 2020 2020 2020 2020  ype.....        
+0003a8c0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+0003a8d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+0003a8e0: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+0003a8f0: 203a 206f 7074 696f 6e61 6c0d 0a20 2020   : optional..   
+0003a900: 2020 2020 2020 2020 204b 6579 776f 7264           Keyword
+0003a910: 2061 7267 756d 656e 7473 2070 6173 7365   arguments passe
+0003a920: 6420 746f 203a 6675 6e63 3a60 2e72 745f  d to :func:`.rt_
+0003a930: 6d65 7461 2e69 6e66 6f60 2e0d 0a0d 0a20  meta.info`..... 
+0003a940: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
+0003a950: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
+0003a960: 0a20 2020 2020 2020 203a 636c 6173 733a  .        :class:
+0003a970: 602e 7274 5f6d 6574 612e 496e 666f 600d  `.rt_meta.Info`.
+0003a980: 0a20 2020 2020 2020 2020 2020 2041 2064  .            A d
+0003a990: 6573 6372 6970 7469 6f6e 206f 6620 7468  escription of th
+0003a9a0: 6520 696e 7075 7420 6172 7261 7927 7320  e input array's 
+0003a9b0: 636f 6e74 656e 7473 2e0d 0a0d 0a20 2020  contents.....   
+0003a9c0: 2020 2020 2053 6565 2041 6c73 6f0d 0a20       See Also.. 
+0003a9d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0d         --------.
+0003a9e0: 0a20 2020 2020 2020 2046 6173 7441 7272  .        FastArr
+0003a9f0: 6179 2e64 6f63 203a 2052 6574 7572 6e20  ay.doc : Return 
+0003aa00: 7468 6520 602e 446f 6360 206f 626a 6563  the `.Doc` objec
+0003aa10: 7420 666f 7220 7468 6520 696e 7075 7420  t for the input 
+0003aa20: 6046 6173 7441 7272 6179 602e 0d0a 2020  `FastArray`...  
+0003aa30: 2020 2020 2020 2e43 6174 6567 6f72 6963        .Categoric
+0003aa40: 616c 2e69 6e66 6f20 3a20 4469 7370 6c61  al.info : Displa
+0003aa50: 7920 6120 6465 7363 7269 7074 696f 6e20  y a description 
+0003aa60: 6f66 2074 6865 2069 6e70 7574 2060 2e43  of the input `.C
+0003aa70: 6174 6567 6f72 6963 616c 602e 0d0a 2020  ategorical`...  
+0003aa80: 2020 2020 2020 2e53 7472 7563 742e 696e        .Struct.in
+0003aa90: 666f 203a 0d0a 2020 2020 2020 2020 2020  fo :..          
+0003aaa0: 2020 5265 7475 726e 2061 6e20 6f62 6a65    Return an obje
+0003aab0: 6374 2063 6f6e 7461 696e 696e 6720 6120  ct containing a 
+0003aac0: 6465 7363 7269 7074 696f 6e20 6f66 2074  description of t
+0003aad0: 6865 2069 6e70 7574 2073 7472 7563 7475  he input structu
+0003aae0: 7265 2773 2063 6f6e 7465 6e74 732e 0d0a  re's contents...
+0003aaf0: 0d0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
+0003ab00: 6573 0d0a 2020 2020 2020 2020 2d2d 2d2d  es..        ----
+0003ab10: 2d2d 2d2d 0d0a 2020 2020 2020 2020 5265  ----..        Re
+0003ab20: 7475 726e 2074 6865 2064 6573 6372 6970  turn the descrip
+0003ab30: 7469 6f6e 206f 6620 7468 6520 696e 7075  tion of the inpu
+0003ab40: 7420 6172 7261 7927 7320 636f 6e74 656e  t array's conten
+0003ab50: 7473 3a0d 0a0d 0a20 2020 2020 2020 203e  ts:....        >
+0003ab60: 3e3e 2061 203d 2072 742e 4641 285b 312c  >> a = rt.FA([1,
+0003ab70: 2032 2c20 332c 2034 2c20 355d 290d 0a20   2, 3, 4, 5]).. 
+0003ab80: 2020 2020 2020 203e 3e3e 2061 2e69 6e66         >>> a.inf
+0003ab90: 6f28 290d 0a20 2020 2020 2020 2044 6573  o()..        Des
+0003aba0: 6372 6970 7469 6f6e 3a20 3c6e 6f20 6465  cription: <no de
+0003abb0: 7363 7269 7074 696f 6e3e 0d0a 2020 2020  scription>..    
+0003abc0: 2020 2020 5374 6577 6172 643a 203c 6e6f      Steward: <no
+0003abd0: 2073 7465 7761 7264 3e0d 0a20 2020 2020   steward>..     
+0003abe0: 2020 2054 7970 653a 2069 6e74 3332 0d0a     Type: int32..
+0003abf0: 0d0a 2020 2020 2020 2020 4170 706c 7920  ..        Apply 
+0003ac00: 6120 7363 6865 6d61 2061 6e64 2072 6574  a schema and ret
+0003ac10: 7572 6e20 7468 6520 6465 7363 7269 7074  urn the descript
+0003ac20: 696f 6e20 6f66 2074 6865 2069 6e70 7574  ion of the input
+0003ac30: 2061 7272 6179 2773 2063 6f6e 7465 6e74   array's content
+0003ac40: 733a 0d0a 0d0a 2020 2020 2020 2020 3e3e  s:....        >>
+0003ac50: 3e20 7363 6865 6d61 203d 207b 2244 6573  > schema = {"Des
+0003ac60: 6372 6970 7469 6f6e 223a 2022 5468 6973  cription": "This
+0003ac70: 2069 7320 616e 2061 7272 6179 222c 2022   is an array", "
+0003ac80: 5374 6577 6172 6422 3a20 2242 7269 616e  Steward": "Brian
+0003ac90: 227d 0d0a 2020 2020 2020 2020 3e3e 3e20  "}..        >>> 
+0003aca0: 612e 6170 706c 795f 7363 6865 6d61 2873  a.apply_schema(s
+0003acb0: 6368 656d 6129 0d0a 2020 2020 2020 2020  chema)..        
+0003acc0: 7b7d 0d0a 2020 2020 2020 2020 3e3e 3e20  {}..        >>> 
+0003acd0: 612e 696e 666f 2829 0d0a 2020 2020 2020  a.info()..      
+0003ace0: 2020 4465 7363 7269 7074 696f 6e3a 2054    Description: T
+0003acf0: 6869 7320 6973 2061 6e20 6172 7261 790d  his is an array.
+0003ad00: 0a20 2020 2020 2020 2053 7465 7761 7264  .        Steward
+0003ad10: 3a20 4272 6961 6e0d 0a20 2020 2020 2020  : Brian..       
+0003ad20: 2054 7970 653a 2069 6e74 3332 0d0a 0d0a   Type: int32....
+0003ad30: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
+0003ad40: 6865 2064 6573 6372 6970 7469 6f6e 206f  he description o
+0003ad50: 6620 7468 6520 696e 7075 7420 6172 7261  f the input arra
+0003ad60: 7927 7320 636f 6e74 656e 7473 2077 6974  y's contents wit
+0003ad70: 6820 6120 7469 746c 653a 0d0a 0d0a 2020  h a title:....  
+0003ad80: 2020 2020 2020 3e3e 3e20 612e 696e 666f        >>> a.info
+0003ad90: 2874 6974 6c65 3d22 5465 7374 2229 0d0a  (title="Test")..
+0003ada0: 2020 2020 2020 2020 5465 7374 0d0a 2020          Test..  
+0003adb0: 2020 2020 2020 3d3d 3d3d 0d0a 2020 2020        ====..    
+0003adc0: 2020 2020 4465 7363 7269 7074 696f 6e3a      Description:
+0003add0: 2054 6869 7320 6973 2061 6e20 6172 7261   This is an arra
+0003ade0: 790d 0a20 2020 2020 2020 2053 7465 7761  y..        Stewa
+0003adf0: 7264 3a20 4272 6961 6e0d 0a20 2020 2020  rd: Brian..     
+0003ae00: 2020 2054 7970 653a 2069 6e74 3332 0d0a     Type: int32..
+0003ae10: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+0003ae20: 2020 2020 2066 726f 6d20 2e72 745f 6d65       from .rt_me
+0003ae30: 7461 2069 6d70 6f72 7420 696e 666f 2061  ta import info a
+0003ae40: 7320 5f69 6e66 6f0d 0a0d 0a20 2020 2020  s _info....     
+0003ae50: 2020 2072 6574 7572 6e20 5f69 6e66 6f28     return _info(
+0003ae60: 7365 6c66 2c20 2a2a 6b77 6172 6773 290d  self, **kwargs).
+0003ae70: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+0003ae80: 0d0a 2020 2020 6465 6620 646f 6328 7365  ..    def doc(se
+0003ae90: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
+0003aea0: 220d 0a20 2020 2020 2020 2052 6574 7572  "..        Retur
+0003aeb0: 6e20 7468 6520 602e 446f 6360 206f 626a  n the `.Doc` obj
+0003aec0: 6563 7420 666f 7220 7468 6520 696e 7075  ect for the inpu
+0003aed0: 7420 6046 6173 7441 7272 6179 602e 0d0a  t `FastArray`...
+0003aee0: 0d0a 2020 2020 2020 2020 4966 206e 6f20  ..        If no 
+0003aef0: 602e 446f 6360 206f 626a 6563 7420 6578  `.Doc` object ex
+0003af00: 6973 7473 2c20 7265 7475 726e 2060 4e6f  ists, return `No
+0003af10: 6e65 602e 0d0a 0d0a 2020 2020 2020 2020  ne`.....        
+0003af20: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
+0003af30: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020   -------..      
+0003af40: 2020 607e 7269 7074 6162 6c65 2e72 745f    `~riptable.rt_
+0003af50: 6d65 7461 2e44 6f63 600d 0a20 2020 2020  meta.Doc`..     
+0003af60: 2020 2020 2020 2054 6865 2060 2e44 6f63         The `.Doc
+0003af70: 6020 6f62 6a65 6374 2066 6f72 2074 6865  ` object for the
+0003af80: 2069 6e70 7574 2060 4661 7374 4172 7261   input `FastArra
+0003af90: 7960 2e20 4966 206e 6f20 602e 446f 6360  y`. If no `.Doc`
+0003afa0: 206f 626a 6563 740d 0a20 2020 2020 2020   object..       
+0003afb0: 2020 2020 2065 7869 7374 732c 2072 6574       exists, ret
+0003afc0: 7572 6e20 604e 6f6e 6560 2e0d 0a0d 0a20  urn `None`..... 
+0003afd0: 2020 2020 2020 2053 6565 2041 6c73 6f0d         See Also.
+0003afe0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0003aff0: 2d0d 0a20 2020 2020 2020 2046 6173 7441  -..        FastA
+0003b000: 7272 6179 2e69 6e66 6f20 3a20 5265 7475  rray.info : Retu
+0003b010: 726e 2061 2064 6573 6372 6970 7469 6f6e  rn a description
+0003b020: 206f 6620 7468 6520 696e 7075 7420 6172   of the input ar
+0003b030: 7261 7927 7320 636f 6e74 656e 7473 2e0d  ray's contents..
+0003b040: 0a20 2020 2020 2020 207e 7269 7074 6162  .        ~riptab
+0003b050: 6c65 2e72 745f 6d65 7461 2e61 7070 6c79  le.rt_meta.apply
+0003b060: 5f73 6368 656d 6120 3a20 5365 7420 602e  _schema : Set `.
+0003b070: 446f 6360 206f 626a 6563 7420 7661 6c75  Doc` object valu
+0003b080: 6573 2e0d 0a0d 0a20 2020 2020 2020 2045  es.....        E
+0003b090: 7861 6d70 6c65 730d 0a20 2020 2020 2020  xamples..       
+0003b0a0: 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020   --------..     
+0003b0b0: 2020 204e 6f20 602e 446f 6360 206f 626a     No `.Doc` obj
+0003b0c0: 6563 7420 6578 6973 7473 3a0d 0a0d 0a20  ect exists:.... 
+0003b0d0: 2020 2020 2020 203e 3e3e 2061 203d 2072         >>> a = r
+0003b0e0: 742e 4641 285b 312c 2032 2c20 332c 2034  t.FA([1, 2, 3, 4
+0003b0f0: 2c20 355d 290d 0a20 2020 2020 2020 203e  , 5])..        >
+0003b100: 3e3e 2070 7269 6e74 2861 2e64 6f63 290d  >> print(a.doc).
+0003b110: 0a20 2020 2020 2020 204e 6f6e 650d 0a0d  .        None...
+0003b120: 0a20 2020 2020 2020 2041 7070 6c79 2061  .        Apply a
+0003b130: 2073 6368 656d 6120 616e 6420 7265 7475   schema and retu
+0003b140: 726e 2074 6865 2060 2e44 6f63 6020 6f62  rn the `.Doc` ob
+0003b150: 6a65 6374 3a0d 0a0d 0a20 2020 2020 2020  ject:....       
+0003b160: 203e 3e3e 2073 6368 656d 6120 3d20 7b22   >>> schema = {"
+0003b170: 4465 7363 7269 7074 696f 6e22 3a20 2254  Description": "T
+0003b180: 6869 7320 6973 2061 6e20 6172 7261 7922  his is an array"
+0003b190: 2c20 2253 7465 7761 7264 223a 2022 4272  , "Steward": "Br
+0003b1a0: 6961 6e22 2c20 2254 7970 6522 3a20 2269  ian", "Type": "i
+0003b1b0: 6e74 3332 227d 0d0a 2020 2020 2020 2020  nt32"}..        
+0003b1c0: 3e3e 3e20 612e 6170 706c 795f 7363 6865  >>> a.apply_sche
+0003b1d0: 6d61 2873 6368 656d 6129 0d0a 2020 2020  ma(schema)..    
+0003b1e0: 2020 2020 7b7d 0d0a 2020 2020 2020 2020      {}..        
+0003b1f0: 3e3e 3e20 612e 646f 630d 0a20 2020 2020  >>> a.doc..     
+0003b200: 2020 2044 6573 6372 6970 7469 6f6e 3a20     Description: 
+0003b210: 5468 6973 2069 7320 616e 2061 7272 6179  This is an array
+0003b220: 0d0a 2020 2020 2020 2020 5374 6577 6172  ..        Stewar
+0003b230: 643a 2042 7269 616e 0d0a 2020 2020 2020  d: Brian..      
+0003b240: 2020 5479 7065 3a20 696e 7433 320d 0a0d    Type: int32...
+0003b250: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
+0003b260: 7370 6563 6966 6963 2060 2e44 6f63 6020  specific `.Doc` 
+0003b270: 6f62 6a65 6374 2069 6e66 6f72 6d61 7469  object informati
+0003b280: 6f6e 3a0d 0a0d 0a20 2020 2020 2020 203e  on:....        >
+0003b290: 3e3e 2061 2e64 6f63 2e5f 7479 7065 0d0a  >> a.doc._type..
+0003b2a0: 2020 2020 2020 2020 2769 6e74 3332 270d          'int32'.
+0003b2b0: 0a20 2020 2020 2020 203e 3e3e 2061 2e64  .        >>> a.d
+0003b2c0: 6f63 2e5f 6465 7363 7269 700d 0a20 2020  oc._descrip..   
+0003b2d0: 2020 2020 2027 5468 6973 2069 7320 616e       'This is an
+0003b2e0: 2061 7272 6179 270d 0a20 2020 2020 2020   array'..       
+0003b2f0: 203e 3e3e 2061 2e64 6f63 2e5f 7374 6577   >>> a.doc._stew
+0003b300: 6172 640d 0a20 2020 2020 2020 2027 4272  ard..        'Br
+0003b310: 6961 6e27 0d0a 2020 2020 2020 2020 3e3e  ian'..        >>
+0003b320: 3e20 7072 696e 7428 612e 646f 632e 5f64  > print(a.doc._d
+0003b330: 6574 6169 6c29 0d0a 2020 2020 2020 2020  etail)..        
+0003b340: 4e6f 6e65 0d0a 2020 2020 2020 2020 2222  None..        ""
+0003b350: 220d 0a20 2020 2020 2020 2066 726f 6d20  "..        from 
+0003b360: 2e72 745f 6d65 7461 2069 6d70 6f72 7420  .rt_meta import 
+0003b370: 646f 6320 6173 205f 646f 630d 0a0d 0a20  doc as _doc.... 
+0003b380: 2020 2020 2020 2072 6574 7572 6e20 5f64         return _d
+0003b390: 6f63 2873 656c 6629 0d0a 0d0a 2020 2020  oc(self)....    
+0003b3a0: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
+0003b3b0: 3d3d 3d3d 3d3d 3d3d 2045 4e44 204f 4620  ======== END OF 
+0003b3c0: 434c 4153 5320 4445 4649 4e49 5449 4f4e  CLASS DEFINITION
+0003b3d0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+0003b3e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0003b3f0: 0d0a 0d0a 0d0a 2320 2d2d 2d2d 2d2d 2d2d  ......# --------
 0003b400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003b410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003b420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0003b430: 2d2d 0d0a 6465 6620 5f73 6574 6661 7374  --..def _setfast
-0003b440: 6172 7261 7976 6965 7728 6172 7229 3a0d  arrayview(arr):.
-0003b450: 0a20 2020 2022 2222 0d0a 2020 2020 4361  .    """..    Ca
-0003b460: 6c6c 2066 726f 6d20 4350 5020 696e 746f  ll from CPP into
-0003b470: 2070 7974 686f 6e20 746f 2066 6c69 7020   python to flip 
-0003b480: 6172 7261 7920 7669 6577 0d0a 2020 2020  array view..    
-0003b490: 2222 220d 0a20 2020 2069 6620 6973 696e  """..    if isin
-0003b4a0: 7374 616e 6365 2861 7272 2c20 4661 7374  stance(arr, Fast
-0003b4b0: 4172 7261 7929 3a0d 0a20 2020 2020 2020  Array):..       
-0003b4c0: 2069 6620 4661 7374 4172 7261 792e 5665   if FastArray.Ve
-0003b4d0: 7262 6f73 6520 3e20 323a 0d0a 2020 2020  rbose > 2:..    
-0003b4e0: 2020 2020 2020 2020 7072 696e 7428 226e          print("n
-0003b4f0: 6f20 6e65 6564 2074 6f20 7365 7466 6173  o need to setfas
-0003b500: 7461 7272 6179 7669 6577 222c 2061 7272  tarrayview", arr
-0003b510: 2e64 7479 7065 2c20 6c65 6e28 6172 7229  .dtype, len(arr)
-0003b520: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0003b530: 6e20 6172 720d 0a0d 0a20 2020 2069 6620  n arr....    if 
-0003b540: 4661 7374 4172 7261 792e 5665 7262 6f73  FastArray.Verbos
-0003b550: 6520 3e20 323a 0d0a 2020 2020 2020 2020  e > 2:..        
-0003b560: 7072 696e 7428 2273 6574 6661 7374 6172  print("setfastar
-0003b570: 7261 7976 6965 7722 2c20 6172 722e 6474  rayview", arr.dt
-0003b580: 7970 652c 206c 656e 2861 7272 2929 0d0a  ype, len(arr))..
-0003b590: 0d0a 2020 2020 7265 7475 726e 2061 7272  ..    return arr
-0003b5a0: 2e76 6965 7728 4661 7374 4172 7261 7929  .view(FastArray)
-0003b5b0: 0d0a 0d0a 0d0a 2320 2d2d 2d2d 2d2d 2d2d  ......# --------
+0003b430: 2d2d 2d0d 0a64 6566 205f 7365 7466 6173  ---..def _setfas
+0003b440: 7461 7272 6179 7669 6577 2861 7272 293a  tarrayview(arr):
+0003b450: 0d0a 2020 2020 2222 220d 0a20 2020 2043  ..    """..    C
+0003b460: 616c 6c20 6672 6f6d 2043 5050 2069 6e74  all from CPP int
+0003b470: 6f20 7079 7468 6f6e 2074 6f20 666c 6970  o python to flip
+0003b480: 2061 7272 6179 2076 6965 770d 0a20 2020   array view..   
+0003b490: 2022 2222 0d0a 2020 2020 6966 2069 7369   """..    if isi
+0003b4a0: 6e73 7461 6e63 6528 6172 722c 2046 6173  nstance(arr, Fas
+0003b4b0: 7441 7272 6179 293a 0d0a 2020 2020 2020  tArray):..      
+0003b4c0: 2020 6966 2046 6173 7441 7272 6179 2e56    if FastArray.V
+0003b4d0: 6572 626f 7365 203e 2032 3a0d 0a20 2020  erbose > 2:..   
+0003b4e0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+0003b4f0: 6e6f 206e 6565 6420 746f 2073 6574 6661  no need to setfa
+0003b500: 7374 6172 7261 7976 6965 7722 2c20 6172  starrayview", ar
+0003b510: 722e 6474 7970 652c 206c 656e 2861 7272  r.dtype, len(arr
+0003b520: 2929 0d0a 2020 2020 2020 2020 7265 7475  ))..        retu
+0003b530: 726e 2061 7272 0d0a 0d0a 2020 2020 6966  rn arr....    if
+0003b540: 2046 6173 7441 7272 6179 2e56 6572 626f   FastArray.Verbo
+0003b550: 7365 203e 2032 3a0d 0a20 2020 2020 2020  se > 2:..       
+0003b560: 2070 7269 6e74 2822 7365 7466 6173 7461   print("setfasta
+0003b570: 7272 6179 7669 6577 222c 2061 7272 2e64  rrayview", arr.d
+0003b580: 7479 7065 2c20 6c65 6e28 6172 7229 290d  type, len(arr)).
+0003b590: 0a0d 0a20 2020 2072 6574 7572 6e20 6172  ...    return ar
+0003b5a0: 722e 7669 6577 2846 6173 7441 7272 6179  r.view(FastArray
+0003b5b0: 290d 0a0d 0a0d 0a23 202d 2d2d 2d2d 2d2d  )......# -------
 0003b5c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003b5d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003b5e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0003b5f0: 2d2d 2d0d 0a64 6566 205f 7365 7466 6173  ---..def _setfas
-0003b600: 7461 7272 6179 7479 7065 2829 3a0d 0a20  tarraytype():.. 
-0003b610: 2020 2023 202d 2d2d 2d2d 2d2d 2d2d 2d2d     # -----------
+0003b5f0: 2d2d 2d2d 0d0a 6465 6620 5f73 6574 6661  ----..def _setfa
+0003b600: 7374 6172 7261 7974 7970 6528 293a 0d0a  starraytype():..
+0003b610: 2020 2020 2320 2d2d 2d2d 2d2d 2d2d 2d2d      # ----------
 0003b620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003b630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003b640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0003b650: 0d0a 2020 2020 2320 6361 6c6c 696e 6720  ..    # calling 
-0003b660: 7468 6973 2066 756e 6374 696f 6e20 7769  this function wi
-0003b670: 6c6c 2066 6f72 6365 2066 6d20 746f 2072  ll force fm to r
-0003b680: 6574 7572 6e20 4661 7374 4172 7261 7920  eturn FastArray 
-0003b690: 7375 6263 6c61 7373 0d0a 2020 2020 2320  subclass..    # 
-0003b6a0: 7263 2e42 6173 6963 4d61 7468 486f 6f6b  rc.BasicMathHook
-0003b6b0: 2846 6173 7441 7272 6179 2c20 6e70 2e6e  (FastArray, np.n
-0003b6c0: 6461 7272 6179 290d 0a20 2020 2023 2043  darray)..    # C
-0003b6d0: 6f6d 696e 6720 6e65 7874 2062 7569 6c64  oming next build
-0003b6e0: 0d0a 2020 2020 6661 203d 206e 702e 6172  ..    fa = np.ar
-0003b6f0: 616e 6765 2831 292e 7669 6577 2846 6173  ange(1).view(Fas
-0003b700: 7441 7272 6179 290d 0a20 2020 2072 632e  tArray)..    rc.
-0003b710: 5365 7446 6173 7441 7272 6179 5479 7065  SetFastArrayType
-0003b720: 2866 612c 205f 7365 7466 6173 7461 7272  (fa, _setfastarr
-0003b730: 6179 7669 6577 290d 0a20 2020 2072 632e  ayview)..    rc.
-0003b740: 4261 7369 634d 6174 6848 6f6f 6b28 6661  BasicMathHook(fa
-0003b750: 2c20 6661 2e5f 6e70 290d 0a0d 0a0d 0a23  , fa._np)......#
-0003b760: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0003b650: 2d0d 0a20 2020 2023 2063 616c 6c69 6e67  -..    # calling
+0003b660: 2074 6869 7320 6675 6e63 7469 6f6e 2077   this function w
+0003b670: 696c 6c20 666f 7263 6520 666d 2074 6f20  ill force fm to 
+0003b680: 7265 7475 726e 2046 6173 7441 7272 6179  return FastArray
+0003b690: 2073 7562 636c 6173 730d 0a20 2020 2023   subclass..    #
+0003b6a0: 2072 632e 4261 7369 634d 6174 6848 6f6f   rc.BasicMathHoo
+0003b6b0: 6b28 4661 7374 4172 7261 792c 206e 702e  k(FastArray, np.
+0003b6c0: 6e64 6172 7261 7929 0d0a 2020 2020 2320  ndarray)..    # 
+0003b6d0: 436f 6d69 6e67 206e 6578 7420 6275 696c  Coming next buil
+0003b6e0: 640d 0a20 2020 2066 6120 3d20 6e70 2e61  d..    fa = np.a
+0003b6f0: 7261 6e67 6528 3129 2e76 6965 7728 4661  range(1).view(Fa
+0003b700: 7374 4172 7261 7929 0d0a 2020 2020 7263  stArray)..    rc
+0003b710: 2e53 6574 4661 7374 4172 7261 7954 7970  .SetFastArrayTyp
+0003b720: 6528 6661 2c20 5f73 6574 6661 7374 6172  e(fa, _setfastar
+0003b730: 7261 7976 6965 7729 0d0a 2020 2020 7263  rayview)..    rc
+0003b740: 2e42 6173 6963 4d61 7468 486f 6f6b 2866  .BasicMathHook(f
+0003b750: 612c 2066 612e 5f6e 7029 0d0a 0d0a 0d0a  a, fa._np)......
+0003b760: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  # --------------
 0003b770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003b780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0003b790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 6465  ------------..de
-0003b7a0: 6620 5f46 6978 7570 446f 6353 7472 696e  f _FixupDocStrin
-0003b7b0: 6773 2829 3a0d 0a20 2020 2022 2222 0d0a  gs():..    """..
-0003b7c0: 2020 2020 4c6f 6164 2061 6c6c 2074 6865      Load all the
-0003b7d0: 206d 656d 6265 7220 6675 6e63 7469 6f6e   member function
-0003b7e0: 206f 6620 7468 6973 206d 6f64 756c 650d   of this module.
-0003b7f0: 0a20 2020 204c 6f61 6420 616c 6c20 7468  .    Load all th
-0003b800: 6520 6d65 6d62 6572 2066 756e 6374 696f  e member functio
-0003b810: 6e73 206f 6620 7468 6520 6e70 206d 6f64  ns of the np mod
-0003b820: 756c 650d 0a20 2020 2049 6620 7765 2066  ule..    If we f
-0003b830: 696e 6420 6120 6d61 7463 682c 2063 6f70  ind a match, cop
-0003b840: 7920 6f76 6572 2074 6865 2064 6f63 2073  y over the doc s
-0003b850: 7472 696e 6773 0d0a 2020 2020 2222 220d  trings..    """.
-0003b860: 0a20 2020 2069 6d70 6f72 7420 696e 7370  .    import insp
-0003b870: 6563 740d 0a20 2020 2069 6d70 6f72 7420  ect..    import 
-0003b880: 7379 730d 0a0d 0a20 2020 206d 796d 6f64  sys....    mymod
-0003b890: 756c 6520 3d20 7379 732e 6d6f 6475 6c65  ule = sys.module
-0003b8a0: 735b 5f5f 6e61 6d65 5f5f 5d0d 0a20 2020  s[__name__]..   
-0003b8b0: 2061 6c6c 5f6d 7966 756e 6374 696f 6e73   all_myfunctions
-0003b8c0: 203d 2069 6e73 7065 6374 2e67 6574 6d65   = inspect.getme
-0003b8d0: 6d62 6572 7328 4661 7374 4172 7261 792c  mbers(FastArray,
-0003b8e0: 2069 6e73 7065 6374 2e69 7366 756e 6374   inspect.isfunct
-0003b8f0: 696f 6e29 0d0a 0d0a 2020 2020 7472 793a  ion)....    try:
-0003b900: 0d0a 2020 2020 2020 2020 2320 626f 7474  ..        # bott
-0003b910: 6c65 6e65 636b 2069 7320 6f70 7469 6f6e  leneck is option
-0003b920: 616c 0d0a 2020 2020 2020 2020 616c 6c5f  al..        all_
-0003b930: 626e 6675 6e63 7469 6f6e 7320 3d20 696e  bnfunctions = in
-0003b940: 7370 6563 742e 6765 746d 656d 6265 7273  spect.getmembers
-0003b950: 2862 6e2c 2069 6e73 7065 6374 2e69 7366  (bn, inspect.isf
-0003b960: 756e 6374 696f 6e29 0d0a 2020 2020 2020  unction)..      
-0003b970: 2020 616c 6c5f 626e 6675 6e63 7469 6f6e    all_bnfunction
-0003b980: 7320 2b3d 2069 6e73 7065 6374 2e67 6574  s += inspect.get
-0003b990: 6d65 6d62 6572 7328 626e 2c20 696e 7370  members(bn, insp
-0003b9a0: 6563 742e 6973 6275 696c 7469 6e29 0d0a  ect.isbuiltin)..
-0003b9b0: 0d0a 2020 2020 2020 2020 2320 6275 696c  ..        # buil
-0003b9c0: 6420 6469 6374 696f 6e61 7279 206f 6620  d dictionary of 
-0003b9d0: 626f 7474 6c65 6e65 636b 2064 6f63 730d  bottleneck docs.
-0003b9e0: 0a20 2020 2020 2020 2062 6e64 6963 7420  .        bndict 
-0003b9f0: 3d20 7b7d 0d0a 2020 2020 2020 2020 666f  = {}..        fo
-0003ba00: 7220 6675 6e63 7320 696e 2061 6c6c 5f62  r funcs in all_b
-0003ba10: 6e66 756e 6374 696f 6e73 3a0d 0a20 2020  nfunctions:..   
-0003ba20: 2020 2020 2020 2020 2062 6e64 6963 745b           bndict[
-0003ba30: 6675 6e63 735b 305d 5d20 3d20 6675 6e63  funcs[0]] = func
-0003ba40: 735b 315d 0d0a 0d0a 2020 2020 2020 2020  s[1]....        
-0003ba50: 2320 6e6f 7720 666f 7220 6561 6368 2066  # now for each f
-0003ba60: 756e 6374 696f 6e20 7468 6174 2068 6173  unction that has
-0003ba70: 2061 6e20 626e 2066 6c61 766f 722c 2063   an bn flavor, c
-0003ba80: 6f70 7920 6f76 6572 2074 6865 2064 6f63  opy over the doc
-0003ba90: 2073 7472 696e 6773 0d0a 2020 2020 2020   strings..      
-0003baa0: 2020 666f 7220 6675 6e63 7320 696e 2061    for funcs in a
-0003bab0: 6c6c 5f6d 7966 756e 6374 696f 6e73 3a0d  ll_myfunctions:.
-0003bac0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0003bad0: 2866 756e 6373 5b30 5d20 696e 2062 6e64  (funcs[0] in bnd
-0003bae0: 6963 7429 2061 6e64 2028 6675 6e63 735b  ict) and (funcs[
-0003baf0: 315d 2e5f 5f64 6f63 5f5f 2069 7320 4e6f  1].__doc__ is No
-0003bb00: 6e65 293a 0d0a 2020 2020 2020 2020 2020  ne):..          
-0003bb10: 2020 2020 2020 6675 6e63 735b 315d 2e5f        funcs[1]._
-0003bb20: 5f64 6f63 5f5f 203d 2062 6e64 6963 745b  _doc__ = bndict[
-0003bb30: 6675 6e63 735b 305d 5d2e 5f5f 646f 635f  funcs[0]].__doc_
-0003bb40: 5f0d 0a20 2020 2065 7863 6570 7420 4578  _..    except Ex
-0003bb50: 6365 7074 696f 6e3a 0d0a 2020 2020 2020  ception:..      
-0003bb60: 2020 7061 7373 0d0a 0d0a 2020 2020 616c    pass....    al
-0003bb70: 6c5f 6e70 6675 6e63 7469 6f6e 7320 3d20  l_npfunctions = 
-0003bb80: 5b66 756e 6320 666f 7220 6675 6e63 2069  [func for func i
-0003bb90: 6e20 696e 7370 6563 742e 6765 746d 656d  n inspect.getmem
-0003bba0: 6265 7273 286e 702e 6e64 6172 7261 7929  bers(np.ndarray)
-0003bbb0: 2069 6620 6e6f 7420 6675 6e63 5b30 5d2e   if not func[0].
-0003bbc0: 7374 6172 7473 7769 7468 2822 5f22 295d  startswith("_")]
-0003bbd0: 0d0a 0d0a 2020 2020 2320 6275 696c 6420  ....    # build 
-0003bbe0: 6469 6374 696f 6e61 7279 206f 6620 6e70  dictionary of np
-0003bbf0: 2e6e 6461 7272 6179 2064 6f63 730d 0a20  .ndarray docs.. 
-0003bc00: 2020 206e 7064 6963 7420 3d20 7b7d 0d0a     npdict = {}..
-0003bc10: 2020 2020 666f 7220 6675 6e63 7320 696e      for funcs in
-0003bc20: 2061 6c6c 5f6e 7066 756e 6374 696f 6e73   all_npfunctions
-0003bc30: 3a0d 0a20 2020 2020 2020 206e 7064 6963  :..        npdic
-0003bc40: 745b 6675 6e63 735b 305d 5d20 3d20 6675  t[funcs[0]] = fu
-0003bc50: 6e63 735b 315d 0d0a 0d0a 2020 2020 2320  ncs[1]....    # 
-0003bc60: 6e6f 7720 666f 7220 6561 6368 2066 756e  now for each fun
-0003bc70: 6374 696f 6e20 7468 6174 2068 6173 2061  ction that has a
-0003bc80: 6e20 6e70 2066 6c61 766f 722c 2063 6f70  n np flavor, cop
-0003bc90: 7920 6f76 6572 2074 6865 2064 6f63 2073  y over the doc s
-0003bca0: 7472 696e 6773 0d0a 2020 2020 666f 7220  trings..    for 
-0003bcb0: 6675 6e63 7320 696e 2061 6c6c 5f6d 7966  funcs in all_myf
-0003bcc0: 756e 6374 696f 6e73 3a0d 0a20 2020 2020  unctions:..     
-0003bcd0: 2020 2069 6620 2866 756e 6373 5b30 5d20     if (funcs[0] 
-0003bce0: 696e 206e 7064 6963 7429 2061 6e64 2028  in npdict) and (
-0003bcf0: 6675 6e63 735b 315d 2e5f 5f64 6f63 5f5f  funcs[1].__doc__
-0003bd00: 2069 7320 4e6f 6e65 293a 0d0a 2020 2020   is None):..    
-0003bd10: 2020 2020 2020 2020 6675 6e63 735b 315d          funcs[1]
-0003bd20: 2e5f 5f64 6f63 5f5f 203d 206e 7064 6963  .__doc__ = npdic
-0003bd30: 745b 6675 6e63 735b 305d 5d2e 5f5f 646f  t[funcs[0]].__do
-0003bd40: 635f 5f0d 0a0d 0a20 2020 2023 206e 6f77  c__....    # now
-0003bd50: 2064 6f20 6a75 7374 2070 6c61 696e 206e   do just plain n
-0003bd60: 700d 0a20 2020 2061 6c6c 5f6e 7066 756e  p..    all_npfun
-0003bd70: 6374 696f 6e73 203d 205b 6675 6e63 2066  ctions = [func f
-0003bd80: 6f72 2066 756e 6320 696e 2069 6e73 7065  or func in inspe
-0003bd90: 6374 2e67 6574 6d65 6d62 6572 7328 6e70  ct.getmembers(np
-0003bda0: 2920 6966 2022 5f5f 2220 6e6f 7420 696e  ) if "__" not in
-0003bdb0: 2066 756e 6373 5b30 5d5d 0d0a 0d0a 2020   funcs[0]]....  
-0003bdc0: 2020 2320 6275 696c 6420 6469 6374 696f    # build dictio
-0003bdd0: 6e61 7279 206f 6620 6e70 2064 6f63 730d  nary of np docs.
-0003bde0: 0a20 2020 206e 7064 6963 7420 3d20 7b7d  .    npdict = {}
-0003bdf0: 0d0a 2020 2020 666f 7220 6675 6e63 7320  ..    for funcs 
-0003be00: 696e 2061 6c6c 5f6e 7066 756e 6374 696f  in all_npfunctio
-0003be10: 6e73 3a0d 0a20 2020 2020 2020 2023 2070  ns:..        # p
-0003be20: 7269 6e74 2822 6765 7474 696e 6720 646f  rint("getting do
-0003be30: 6320 7374 7269 6e67 2066 6f72 2022 2c20  c string for ", 
-0003be40: 6675 6e63 735b 305d 290d 0a20 2020 2020  funcs[0])..     
-0003be50: 2020 206e 7064 6963 745b 6675 6e63 735b     npdict[funcs[
-0003be60: 305d 5d20 3d20 6675 6e63 735b 315d 0d0a  0]] = funcs[1]..
-0003be70: 0d0a 2020 2020 2320 6e6f 7720 666f 7220  ..    # now for 
-0003be80: 6561 6368 2066 756e 6374 696f 6e20 7468  each function th
-0003be90: 6174 2068 6173 2061 6e20 6e70 2066 6c61  at has an np fla
-0003bea0: 766f 722c 2063 6f70 7920 6f76 6572 2074  vor, copy over t
-0003beb0: 6865 2064 6f63 2073 7472 696e 6773 0d0a  he doc strings..
-0003bec0: 2020 2020 666f 7220 6675 6e63 7320 696e      for funcs in
-0003bed0: 2061 6c6c 5f6d 7966 756e 6374 696f 6e73   all_myfunctions
-0003bee0: 3a0d 0a20 2020 2020 2020 2069 6620 2866  :..        if (f
-0003bef0: 756e 6373 5b30 5d20 696e 206e 7064 6963  uncs[0] in npdic
-0003bf00: 7429 2061 6e64 2028 6675 6e63 735b 315d  t) and (funcs[1]
-0003bf10: 2e5f 5f64 6f63 5f5f 2069 7320 4e6f 6e65  .__doc__ is None
-0003bf20: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0003bf30: 6675 6e63 735b 315d 2e5f 5f64 6f63 5f5f  funcs[1].__doc__
-0003bf40: 203d 206e 7064 6963 745b 6675 6e63 735b   = npdict[funcs[
-0003bf50: 305d 5d2e 5f5f 646f 635f 5f0d 0a0d 0a0d  0]].__doc__.....
-0003bf60: 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .# -------------
+0003b790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a64  -------------..d
+0003b7a0: 6566 205f 4669 7875 7044 6f63 5374 7269  ef _FixupDocStri
+0003b7b0: 6e67 7328 293a 0d0a 2020 2020 2222 220d  ngs():..    """.
+0003b7c0: 0a20 2020 204c 6f61 6420 616c 6c20 7468  .    Load all th
+0003b7d0: 6520 6d65 6d62 6572 2066 756e 6374 696f  e member functio
+0003b7e0: 6e20 6f66 2074 6869 7320 6d6f 6475 6c65  n of this module
+0003b7f0: 0d0a 2020 2020 4c6f 6164 2061 6c6c 2074  ..    Load all t
+0003b800: 6865 206d 656d 6265 7220 6675 6e63 7469  he member functi
+0003b810: 6f6e 7320 6f66 2074 6865 206e 7020 6d6f  ons of the np mo
+0003b820: 6475 6c65 0d0a 2020 2020 4966 2077 6520  dule..    If we 
+0003b830: 6669 6e64 2061 206d 6174 6368 2c20 636f  find a match, co
+0003b840: 7079 206f 7665 7220 7468 6520 646f 6320  py over the doc 
+0003b850: 7374 7269 6e67 730d 0a20 2020 2022 2222  strings..    """
+0003b860: 0d0a 2020 2020 696d 706f 7274 2069 6e73  ..    import ins
+0003b870: 7065 6374 0d0a 2020 2020 696d 706f 7274  pect..    import
+0003b880: 2073 7973 0d0a 0d0a 2020 2020 6d79 6d6f   sys....    mymo
+0003b890: 6475 6c65 203d 2073 7973 2e6d 6f64 756c  dule = sys.modul
+0003b8a0: 6573 5b5f 5f6e 616d 655f 5f5d 0d0a 2020  es[__name__]..  
+0003b8b0: 2020 616c 6c5f 6d79 6675 6e63 7469 6f6e    all_myfunction
+0003b8c0: 7320 3d20 696e 7370 6563 742e 6765 746d  s = inspect.getm
+0003b8d0: 656d 6265 7273 2846 6173 7441 7272 6179  embers(FastArray
+0003b8e0: 2c20 696e 7370 6563 742e 6973 6675 6e63  , inspect.isfunc
+0003b8f0: 7469 6f6e 290d 0a0d 0a20 2020 2074 7279  tion)....    try
+0003b900: 3a0d 0a20 2020 2020 2020 2023 2062 6f74  :..        # bot
+0003b910: 746c 656e 6563 6b20 6973 206f 7074 696f  tleneck is optio
+0003b920: 6e61 6c0d 0a20 2020 2020 2020 2061 6c6c  nal..        all
+0003b930: 5f62 6e66 756e 6374 696f 6e73 203d 2069  _bnfunctions = i
+0003b940: 6e73 7065 6374 2e67 6574 6d65 6d62 6572  nspect.getmember
+0003b950: 7328 626e 2c20 696e 7370 6563 742e 6973  s(bn, inspect.is
+0003b960: 6675 6e63 7469 6f6e 290d 0a20 2020 2020  function)..     
+0003b970: 2020 2061 6c6c 5f62 6e66 756e 6374 696f     all_bnfunctio
+0003b980: 6e73 202b 3d20 696e 7370 6563 742e 6765  ns += inspect.ge
+0003b990: 746d 656d 6265 7273 2862 6e2c 2069 6e73  tmembers(bn, ins
+0003b9a0: 7065 6374 2e69 7362 7569 6c74 696e 290d  pect.isbuiltin).
+0003b9b0: 0a0d 0a20 2020 2020 2020 2023 2062 7569  ...        # bui
+0003b9c0: 6c64 2064 6963 7469 6f6e 6172 7920 6f66  ld dictionary of
+0003b9d0: 2062 6f74 746c 656e 6563 6b20 646f 6373   bottleneck docs
+0003b9e0: 0d0a 2020 2020 2020 2020 626e 6469 6374  ..        bndict
+0003b9f0: 203d 207b 7d0d 0a20 2020 2020 2020 2066   = {}..        f
+0003ba00: 6f72 2066 756e 6373 2069 6e20 616c 6c5f  or funcs in all_
+0003ba10: 626e 6675 6e63 7469 6f6e 733a 0d0a 2020  bnfunctions:..  
+0003ba20: 2020 2020 2020 2020 2020 626e 6469 6374            bndict
+0003ba30: 5b66 756e 6373 5b30 5d5d 203d 2066 756e  [funcs[0]] = fun
+0003ba40: 6373 5b31 5d0d 0a0d 0a20 2020 2020 2020  cs[1]....       
+0003ba50: 2023 206e 6f77 2066 6f72 2065 6163 6820   # now for each 
+0003ba60: 6675 6e63 7469 6f6e 2074 6861 7420 6861  function that ha
+0003ba70: 7320 616e 2062 6e20 666c 6176 6f72 2c20  s an bn flavor, 
+0003ba80: 636f 7079 206f 7665 7220 7468 6520 646f  copy over the do
+0003ba90: 6320 7374 7269 6e67 730d 0a20 2020 2020  c strings..     
+0003baa0: 2020 2066 6f72 2066 756e 6373 2069 6e20     for funcs in 
+0003bab0: 616c 6c5f 6d79 6675 6e63 7469 6f6e 733a  all_myfunctions:
+0003bac0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0003bad0: 2028 6675 6e63 735b 305d 2069 6e20 626e   (funcs[0] in bn
+0003bae0: 6469 6374 2920 616e 6420 2866 756e 6373  dict) and (funcs
+0003baf0: 5b31 5d2e 5f5f 646f 635f 5f20 6973 204e  [1].__doc__ is N
+0003bb00: 6f6e 6529 3a0d 0a20 2020 2020 2020 2020  one):..         
+0003bb10: 2020 2020 2020 2066 756e 6373 5b31 5d2e         funcs[1].
+0003bb20: 5f5f 646f 635f 5f20 3d20 626e 6469 6374  __doc__ = bndict
+0003bb30: 5b66 756e 6373 5b30 5d5d 2e5f 5f64 6f63  [funcs[0]].__doc
+0003bb40: 5f5f 0d0a 2020 2020 6578 6365 7074 2045  __..    except E
+0003bb50: 7863 6570 7469 6f6e 3a0d 0a20 2020 2020  xception:..     
+0003bb60: 2020 2070 6173 730d 0a0d 0a20 2020 2061     pass....    a
+0003bb70: 6c6c 5f6e 7066 756e 6374 696f 6e73 203d  ll_npfunctions =
+0003bb80: 205b 6675 6e63 2066 6f72 2066 756e 6320   [func for func 
+0003bb90: 696e 2069 6e73 7065 6374 2e67 6574 6d65  in inspect.getme
+0003bba0: 6d62 6572 7328 6e70 2e6e 6461 7272 6179  mbers(np.ndarray
+0003bbb0: 2920 6966 206e 6f74 2066 756e 635b 305d  ) if not func[0]
+0003bbc0: 2e73 7461 7274 7377 6974 6828 225f 2229  .startswith("_")
+0003bbd0: 5d0d 0a0d 0a20 2020 2023 2062 7569 6c64  ]....    # build
+0003bbe0: 2064 6963 7469 6f6e 6172 7920 6f66 206e   dictionary of n
+0003bbf0: 702e 6e64 6172 7261 7920 646f 6373 0d0a  p.ndarray docs..
+0003bc00: 2020 2020 6e70 6469 6374 203d 207b 7d0d      npdict = {}.
+0003bc10: 0a20 2020 2066 6f72 2066 756e 6373 2069  .    for funcs i
+0003bc20: 6e20 616c 6c5f 6e70 6675 6e63 7469 6f6e  n all_npfunction
+0003bc30: 733a 0d0a 2020 2020 2020 2020 6e70 6469  s:..        npdi
+0003bc40: 6374 5b66 756e 6373 5b30 5d5d 203d 2066  ct[funcs[0]] = f
+0003bc50: 756e 6373 5b31 5d0d 0a0d 0a20 2020 2023  uncs[1]....    #
+0003bc60: 206e 6f77 2066 6f72 2065 6163 6820 6675   now for each fu
+0003bc70: 6e63 7469 6f6e 2074 6861 7420 6861 7320  nction that has 
+0003bc80: 616e 206e 7020 666c 6176 6f72 2c20 636f  an np flavor, co
+0003bc90: 7079 206f 7665 7220 7468 6520 646f 6320  py over the doc 
+0003bca0: 7374 7269 6e67 730d 0a20 2020 2066 6f72  strings..    for
+0003bcb0: 2066 756e 6373 2069 6e20 616c 6c5f 6d79   funcs in all_my
+0003bcc0: 6675 6e63 7469 6f6e 733a 0d0a 2020 2020  functions:..    
+0003bcd0: 2020 2020 6966 2028 6675 6e63 735b 305d      if (funcs[0]
+0003bce0: 2069 6e20 6e70 6469 6374 2920 616e 6420   in npdict) and 
+0003bcf0: 2866 756e 6373 5b31 5d2e 5f5f 646f 635f  (funcs[1].__doc_
+0003bd00: 5f20 6973 204e 6f6e 6529 3a0d 0a20 2020  _ is None):..   
+0003bd10: 2020 2020 2020 2020 2066 756e 6373 5b31           funcs[1
+0003bd20: 5d2e 5f5f 646f 635f 5f20 3d20 6e70 6469  ].__doc__ = npdi
+0003bd30: 6374 5b66 756e 6373 5b30 5d5d 2e5f 5f64  ct[funcs[0]].__d
+0003bd40: 6f63 5f5f 0d0a 0d0a 2020 2020 2320 6e6f  oc__....    # no
+0003bd50: 7720 646f 206a 7573 7420 706c 6169 6e20  w do just plain 
+0003bd60: 6e70 0d0a 2020 2020 616c 6c5f 6e70 6675  np..    all_npfu
+0003bd70: 6e63 7469 6f6e 7320 3d20 5b66 756e 6320  nctions = [func 
+0003bd80: 666f 7220 6675 6e63 2069 6e20 696e 7370  for func in insp
+0003bd90: 6563 742e 6765 746d 656d 6265 7273 286e  ect.getmembers(n
+0003bda0: 7029 2069 6620 225f 5f22 206e 6f74 2069  p) if "__" not i
+0003bdb0: 6e20 6675 6e63 735b 305d 5d0d 0a0d 0a20  n funcs[0]].... 
+0003bdc0: 2020 2023 2062 7569 6c64 2064 6963 7469     # build dicti
+0003bdd0: 6f6e 6172 7920 6f66 206e 7020 646f 6373  onary of np docs
+0003bde0: 0d0a 2020 2020 6e70 6469 6374 203d 207b  ..    npdict = {
+0003bdf0: 7d0d 0a20 2020 2066 6f72 2066 756e 6373  }..    for funcs
+0003be00: 2069 6e20 616c 6c5f 6e70 6675 6e63 7469   in all_npfuncti
+0003be10: 6f6e 733a 0d0a 2020 2020 2020 2020 2320  ons:..        # 
+0003be20: 7072 696e 7428 2267 6574 7469 6e67 2064  print("getting d
+0003be30: 6f63 2073 7472 696e 6720 666f 7220 222c  oc string for ",
+0003be40: 2066 756e 6373 5b30 5d29 0d0a 2020 2020   funcs[0])..    
+0003be50: 2020 2020 6e70 6469 6374 5b66 756e 6373      npdict[funcs
+0003be60: 5b30 5d5d 203d 2066 756e 6373 5b31 5d0d  [0]] = funcs[1].
+0003be70: 0a0d 0a20 2020 2023 206e 6f77 2066 6f72  ...    # now for
+0003be80: 2065 6163 6820 6675 6e63 7469 6f6e 2074   each function t
+0003be90: 6861 7420 6861 7320 616e 206e 7020 666c  hat has an np fl
+0003bea0: 6176 6f72 2c20 636f 7079 206f 7665 7220  avor, copy over 
+0003beb0: 7468 6520 646f 6320 7374 7269 6e67 730d  the doc strings.
+0003bec0: 0a20 2020 2066 6f72 2066 756e 6373 2069  .    for funcs i
+0003bed0: 6e20 616c 6c5f 6d79 6675 6e63 7469 6f6e  n all_myfunction
+0003bee0: 733a 0d0a 2020 2020 2020 2020 6966 2028  s:..        if (
+0003bef0: 6675 6e63 735b 305d 2069 6e20 6e70 6469  funcs[0] in npdi
+0003bf00: 6374 2920 616e 6420 2866 756e 6373 5b31  ct) and (funcs[1
+0003bf10: 5d2e 5f5f 646f 635f 5f20 6973 204e 6f6e  ].__doc__ is Non
+0003bf20: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+0003bf30: 2066 756e 6373 5b31 5d2e 5f5f 646f 635f   funcs[1].__doc_
+0003bf40: 5f20 3d20 6e70 6469 6374 5b66 756e 6373  _ = npdict[funcs
+0003bf50: 5b30 5d5d 2e5f 5f64 6f63 5f5f 0d0a 0d0a  [0]].__doc__....
+0003bf60: 0d0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..# ------------
 0003bf70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003bf80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0003bf90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a63  -------------..c
-0003bfa0: 6c61 7373 2054 6872 6561 6469 6e67 3a0d  lass Threading:.
-0003bfb0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-0003bfc0: 6f64 0d0a 2020 2020 6465 6620 6f6e 2829  od..    def on()
-0003bfd0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-0003bfe0: 2020 2020 2020 2020 5475 726e 2072 6970          Turn rip
-0003bff0: 7461 626c 6520 7468 7265 6164 696e 6720  table threading 
-0003c000: 6f6e 2e0d 0a20 2020 2020 2020 2055 7365  on...        Use
-0003c010: 6420 6f6e 6c79 2077 6865 6e20 7269 7074  d only when ript
-0003c020: 6162 6c65 2074 6872 6561 6469 6e67 2077  able threading w
-0003c030: 6173 2074 7572 6e65 6420 6f66 662e 0d0a  as turned off...
-0003c040: 0d0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-0003c050: 650d 0a20 2020 2020 2020 202d 2d2d 2d2d  e..        -----
-0003c060: 2d2d 0d0a 2020 2020 2020 2020 613d 7274  --..        a=rt
-0003c070: 2e61 7261 6e67 6528 315f 3030 305f 3030  .arange(1_000_00
-0003c080: 290d 0a20 2020 2020 2020 2054 6872 6561  )..        Threa
-0003c090: 6469 6e67 2e6f 6666 2829 0d0a 2020 2020  ding.off()..    
-0003c0a0: 2020 2020 2574 696d 6520 612b 3d31 0d0a      %time a+=1..
-0003c0b0: 2020 2020 2020 2020 5468 7265 6164 696e          Threadin
-0003c0c0: 672e 6f6e 2829 0d0a 2020 2020 2020 2020  g.on()..        
-0003c0d0: 2574 696d 6520 612b 3d31 0d0a 0d0a 2020  %time a+=1....  
-0003c0e0: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
-0003c0f0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
-0003c100: 2020 2020 2020 2020 5072 6576 696f 7573          Previous
-0003c110: 6c79 2077 6865 7468 6572 2074 6872 6561  ly whether threa
-0003c120: 6469 6e67 2077 6173 206f 6e20 6f72 206e  ding was on or n
-0003c130: 6f74 2e20 3020 6f72 2031 2e20 303d 7468  ot. 0 or 1. 0=th
-0003c140: 7265 6164 696e 6720 7761 7320 6f66 6620  reading was off 
-0003c150: 6265 666f 7265 2e0d 0a0d 0a20 2020 2020  before.....     
-0003c160: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-0003c170: 7265 7475 726e 2046 6173 7441 7272 6179  return FastArray
-0003c180: 2e5f 544f 4e28 290d 0a0d 0a20 2020 2040  ._TON()....    @
-0003c190: 7374 6174 6963 6d65 7468 6f64 0d0a 2020  staticmethod..  
-0003c1a0: 2020 6465 6620 6f66 6628 293a 0d0a 2020    def off():..  
-0003c1b0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-0003c1c0: 2020 2054 7572 6e20 7269 7074 6162 6c65     Turn riptable
-0003c1d0: 2074 6872 6561 6469 6e67 206f 6666 2e0d   threading off..
-0003c1e0: 0a20 2020 2020 2020 2055 7365 6675 6c20  .        Useful 
-0003c1f0: 666f 7220 7768 656e 2074 6865 2073 7973  for when the sys
-0003c200: 7465 6d20 6861 7320 6f74 6865 7220 7072  tem has other pr
-0003c210: 6f63 6573 7365 7320 7573 696e 6720 6f74  ocesses using ot
-0003c220: 6865 7220 7468 7265 6164 730d 0a20 2020  her threads..   
-0003c230: 2020 2020 206f 7220 746f 206c 696d 6974       or to limit
-0003c240: 2074 6872 6561 6469 6e67 2072 6573 6f75   threading resou
-0003c250: 7263 6573 2e0d 0a0d 0a20 2020 2020 2020  rces.....       
-0003c260: 2045 7861 6d70 6c65 0d0a 2020 2020 2020   Example..      
-0003c270: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-0003c280: 2020 2061 3d72 742e 6172 616e 6765 2831     a=rt.arange(1
-0003c290: 5f30 3030 5f30 3029 0d0a 2020 2020 2020  _000_00)..      
-0003c2a0: 2020 5468 7265 6164 696e 672e 6f66 6628    Threading.off(
-0003c2b0: 290d 0a20 2020 2020 2020 2025 7469 6d65  )..        %time
-0003c2c0: 2061 2b3d 310d 0a20 2020 2020 2020 2054   a+=1..        T
-0003c2d0: 6872 6561 6469 6e67 2e6f 6e28 290d 0a20  hreading.on().. 
-0003c2e0: 2020 2020 2020 2025 7469 6d65 2061 2b3d         %time a+=
-0003c2f0: 310d 0a0d 0a20 2020 2020 2020 2052 6574  1....        Ret
-0003c300: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
-0003c310: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2050  -----..        P
-0003c320: 7265 7669 6f75 736c 7920 7768 6574 6865  reviously whethe
-0003c330: 7220 7468 7265 6164 696e 6720 7761 7320  r threading was 
-0003c340: 6f6e 206f 7220 6e6f 742e 2030 206f 7220  on or not. 0 or 
-0003c350: 312e 2030 3d74 6872 6561 6469 6e67 2077  1. 0=threading w
-0003c360: 6173 206f 6666 2062 6566 6f72 652e 0d0a  as off before...
-0003c370: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0003c380: 2020 2020 2072 6574 7572 6e20 4661 7374       return Fast
-0003c390: 4172 7261 792e 5f54 4f46 4628 290d 0a0d  Array._TOFF()...
-0003c3a0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-0003c3b0: 6f64 0d0a 2020 2020 6465 6620 7468 7265  od..    def thre
-0003c3c0: 6164 7328 7468 7265 6164 636f 756e 7429  ads(threadcount)
-0003c3d0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-0003c3e0: 2020 2020 2020 2020 5365 7420 686f 7720          Set how 
-0003c3f0: 6d61 6e79 2077 6f72 6b65 7220 7468 7265  many worker thre
-0003c400: 6164 7320 7269 7074 6162 6c65 2063 616e  ads riptable can
-0003c410: 2075 7365 2e0d 0a20 2020 2020 2020 204f   use...        O
-0003c420: 6674 656e 2064 6566 6175 6c74 7320 746f  ften defaults to
-0003c430: 2031 3220 616e 6420 6361 6e6e 6f74 2062   12 and cannot b
-0003c440: 6520 7365 7420 6265 6c6f 7720 3120 6f72  e set below 1 or
-0003c450: 203e 2033 312e 0d0a 0d0a 2020 2020 2020   > 31.....      
-0003c460: 2020 546f 2074 7572 6e20 7269 7074 6162    To turn riptab
-0003c470: 6c65 2074 6872 6561 6469 6e67 206f 6666  le threading off
-0003c480: 2063 6f6d 706c 6574 656c 7920 7573 6520   completely use 
-0003c490: 5468 7265 6164 696e 672e 6f66 6628 290d  Threading.off().
-0003c4a0: 0a20 2020 2020 2020 2055 7365 6675 6c20  .        Useful 
-0003c4b0: 666f 7220 7768 656e 2074 6865 2073 7973  for when the sys
-0003c4c0: 7465 6d20 6861 7320 6f74 6865 7220 7072  tem has other pr
-0003c4d0: 6f63 6573 7365 7320 7573 696e 6720 6f74  ocesses using ot
-0003c4e0: 6865 7220 7468 7265 6164 730d 0a20 2020  her threads..   
-0003c4f0: 2020 2020 206f 7220 746f 206c 696d 6974       or to limit
-0003c500: 2074 6872 6561 6469 6e67 2072 6573 6f75   threading resou
-0003c510: 7263 6573 2e0d 0a0d 0a20 2020 2020 2020  rces.....       
-0003c520: 2045 7861 6d70 6c65 0d0a 2020 2020 2020   Example..      
-0003c530: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-0003c540: 2020 2054 6872 6561 6469 6e67 2e74 6872     Threading.thr
-0003c550: 6561 6473 2838 290d 0a0d 0a20 2020 2020  eads(8)....     
-0003c560: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-0003c570: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-0003c580: 2020 2020 206e 756d 6265 7220 6f66 2074       number of t
-0003c590: 6872 6561 6473 2070 7265 7669 6f75 736c  hreads previousl
-0003c5a0: 7920 7573 6564 0d0a 2020 2020 2020 2020  y used..        
-0003c5b0: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
-0003c5c0: 7572 6e20 7263 2e53 6574 5468 7265 6164  urn rc.SetThread
-0003c5d0: 5761 6b65 5570 2874 6872 6561 6463 6f75  WakeUp(threadcou
-0003c5e0: 6e74 290d 0a0d 0a0d 0a23 202d 2d2d 2d2d  nt)......# -----
+0003bf90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
+0003bfa0: 636c 6173 7320 5468 7265 6164 696e 673a  class Threading:
+0003bfb0: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+0003bfc0: 686f 640d 0a20 2020 2064 6566 206f 6e28  hod..    def on(
+0003bfd0: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+0003bfe0: 0a20 2020 2020 2020 2054 7572 6e20 7269  .        Turn ri
+0003bff0: 7074 6162 6c65 2074 6872 6561 6469 6e67  ptable threading
+0003c000: 206f 6e2e 0d0a 2020 2020 2020 2020 5573   on...        Us
+0003c010: 6564 206f 6e6c 7920 7768 656e 2072 6970  ed only when rip
+0003c020: 7461 626c 6520 7468 7265 6164 696e 6720  table threading 
+0003c030: 7761 7320 7475 726e 6564 206f 6666 2e0d  was turned off..
+0003c040: 0a0d 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+0003c050: 6c65 0d0a 2020 2020 2020 2020 2d2d 2d2d  le..        ----
+0003c060: 2d2d 2d0d 0a20 2020 2020 2020 2061 3d72  ---..        a=r
+0003c070: 742e 6172 616e 6765 2831 5f30 3030 5f30  t.arange(1_000_0
+0003c080: 3029 0d0a 2020 2020 2020 2020 5468 7265  0)..        Thre
+0003c090: 6164 696e 672e 6f66 6628 290d 0a20 2020  ading.off()..   
+0003c0a0: 2020 2020 2025 7469 6d65 2061 2b3d 310d       %time a+=1.
+0003c0b0: 0a20 2020 2020 2020 2054 6872 6561 6469  .        Threadi
+0003c0c0: 6e67 2e6f 6e28 290d 0a20 2020 2020 2020  ng.on()..       
+0003c0d0: 2025 7469 6d65 2061 2b3d 310d 0a0d 0a20   %time a+=1.... 
+0003c0e0: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
+0003c0f0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
+0003c100: 0a20 2020 2020 2020 2050 7265 7669 6f75  .        Previou
+0003c110: 736c 7920 7768 6574 6865 7220 7468 7265  sly whether thre
+0003c120: 6164 696e 6720 7761 7320 6f6e 206f 7220  ading was on or 
+0003c130: 6e6f 742e 2030 206f 7220 312e 2030 3d74  not. 0 or 1. 0=t
+0003c140: 6872 6561 6469 6e67 2077 6173 206f 6666  hreading was off
+0003c150: 2062 6566 6f72 652e 0d0a 0d0a 2020 2020   before.....    
+0003c160: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0003c170: 2072 6574 7572 6e20 4661 7374 4172 7261   return FastArra
+0003c180: 792e 5f54 4f4e 2829 0d0a 0d0a 2020 2020  y._TON()....    
+0003c190: 4073 7461 7469 636d 6574 686f 640d 0a20  @staticmethod.. 
+0003c1a0: 2020 2064 6566 206f 6666 2829 3a0d 0a20     def off():.. 
+0003c1b0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0003c1c0: 2020 2020 5475 726e 2072 6970 7461 626c      Turn riptabl
+0003c1d0: 6520 7468 7265 6164 696e 6720 6f66 662e  e threading off.
+0003c1e0: 0d0a 2020 2020 2020 2020 5573 6566 756c  ..        Useful
+0003c1f0: 2066 6f72 2077 6865 6e20 7468 6520 7379   for when the sy
+0003c200: 7374 656d 2068 6173 206f 7468 6572 2070  stem has other p
+0003c210: 726f 6365 7373 6573 2075 7369 6e67 206f  rocesses using o
+0003c220: 7468 6572 2074 6872 6561 6473 0d0a 2020  ther threads..  
+0003c230: 2020 2020 2020 6f72 2074 6f20 6c69 6d69        or to limi
+0003c240: 7420 7468 7265 6164 696e 6720 7265 736f  t threading reso
+0003c250: 7572 6365 732e 0d0a 0d0a 2020 2020 2020  urces.....      
+0003c260: 2020 4578 616d 706c 650d 0a20 2020 2020    Example..     
+0003c270: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
+0003c280: 2020 2020 613d 7274 2e61 7261 6e67 6528      a=rt.arange(
+0003c290: 315f 3030 305f 3030 290d 0a20 2020 2020  1_000_00)..     
+0003c2a0: 2020 2054 6872 6561 6469 6e67 2e6f 6666     Threading.off
+0003c2b0: 2829 0d0a 2020 2020 2020 2020 2574 696d  ()..        %tim
+0003c2c0: 6520 612b 3d31 0d0a 2020 2020 2020 2020  e a+=1..        
+0003c2d0: 5468 7265 6164 696e 672e 6f6e 2829 0d0a  Threading.on()..
+0003c2e0: 2020 2020 2020 2020 2574 696d 6520 612b          %time a+
+0003c2f0: 3d31 0d0a 0d0a 2020 2020 2020 2020 5265  =1....        Re
+0003c300: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
+0003c310: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+0003c320: 5072 6576 696f 7573 6c79 2077 6865 7468  Previously wheth
+0003c330: 6572 2074 6872 6561 6469 6e67 2077 6173  er threading was
+0003c340: 206f 6e20 6f72 206e 6f74 2e20 3020 6f72   on or not. 0 or
+0003c350: 2031 2e20 303d 7468 7265 6164 696e 6720   1. 0=threading 
+0003c360: 7761 7320 6f66 6620 6265 666f 7265 2e0d  was off before..
+0003c370: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0003c380: 2020 2020 2020 7265 7475 726e 2046 6173        return Fas
+0003c390: 7441 7272 6179 2e5f 544f 4646 2829 0d0a  tArray._TOFF()..
+0003c3a0: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+0003c3b0: 686f 640d 0a20 2020 2064 6566 2074 6872  hod..    def thr
+0003c3c0: 6561 6473 2874 6872 6561 6463 6f75 6e74  eads(threadcount
+0003c3d0: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+0003c3e0: 0a20 2020 2020 2020 2053 6574 2068 6f77  .        Set how
+0003c3f0: 206d 616e 7920 776f 726b 6572 2074 6872   many worker thr
+0003c400: 6561 6473 2072 6970 7461 626c 6520 6361  eads riptable ca
+0003c410: 6e20 7573 652e 0d0a 2020 2020 2020 2020  n use...        
+0003c420: 4f66 7465 6e20 6465 6661 756c 7473 2074  Often defaults t
+0003c430: 6f20 3132 2061 6e64 2063 616e 6e6f 7420  o 12 and cannot 
+0003c440: 6265 2073 6574 2062 656c 6f77 2031 206f  be set below 1 o
+0003c450: 7220 3e20 3331 2e0d 0a0d 0a20 2020 2020  r > 31.....     
+0003c460: 2020 2054 6f20 7475 726e 2072 6970 7461     To turn ripta
+0003c470: 626c 6520 7468 7265 6164 696e 6720 6f66  ble threading of
+0003c480: 6620 636f 6d70 6c65 7465 6c79 2075 7365  f completely use
+0003c490: 2054 6872 6561 6469 6e67 2e6f 6666 2829   Threading.off()
+0003c4a0: 0d0a 2020 2020 2020 2020 5573 6566 756c  ..        Useful
+0003c4b0: 2066 6f72 2077 6865 6e20 7468 6520 7379   for when the sy
+0003c4c0: 7374 656d 2068 6173 206f 7468 6572 2070  stem has other p
+0003c4d0: 726f 6365 7373 6573 2075 7369 6e67 206f  rocesses using o
+0003c4e0: 7468 6572 2074 6872 6561 6473 0d0a 2020  ther threads..  
+0003c4f0: 2020 2020 2020 6f72 2074 6f20 6c69 6d69        or to limi
+0003c500: 7420 7468 7265 6164 696e 6720 7265 736f  t threading reso
+0003c510: 7572 6365 732e 0d0a 0d0a 2020 2020 2020  urces.....      
+0003c520: 2020 4578 616d 706c 650d 0a20 2020 2020    Example..     
+0003c530: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
+0003c540: 2020 2020 5468 7265 6164 696e 672e 7468      Threading.th
+0003c550: 7265 6164 7328 3829 0d0a 0d0a 2020 2020  reads(8)....    
+0003c560: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
+0003c570: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
+0003c580: 2020 2020 2020 6e75 6d62 6572 206f 6620        number of 
+0003c590: 7468 7265 6164 7320 7072 6576 696f 7573  threads previous
+0003c5a0: 6c79 2075 7365 640d 0a20 2020 2020 2020  ly used..       
+0003c5b0: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+0003c5c0: 7475 726e 2072 632e 5365 7454 6872 6561  turn rc.SetThrea
+0003c5d0: 6457 616b 6555 7028 7468 7265 6164 636f  dWakeUp(threadco
+0003c5e0: 756e 7429 0d0a 0d0a 0d0a 2320 2d2d 2d2d  unt)......# ----
 0003c5f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003c600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003c610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0003c620: 2d2d 2d2d 2d0d 0a63 6c61 7373 2052 6563  -----..class Rec
-0003c630: 7963 6c65 3a0d 0a20 2020 2040 7374 6174  ycle:..    @stat
-0003c640: 6963 6d65 7468 6f64 0d0a 2020 2020 6465  icmethod..    de
-0003c650: 6620 6f6e 2829 3a0d 0a20 2020 2020 2020  f on():..       
-0003c660: 2022 2222 0d0a 2020 2020 2020 2020 5475   """..        Tu
-0003c670: 726e 2072 6970 7461 626c 6520 7265 6379  rn riptable recy
-0003c680: 636c 696e 6720 6f6e 2e0d 0a20 2020 2020  cling on...     
-0003c690: 2020 2055 7365 6420 6f6e 6c79 2077 6865     Used only whe
-0003c6a0: 6e20 7269 7074 6162 6c65 2072 6563 7963  n riptable recyc
-0003c6b0: 6c69 6e67 2077 6173 2074 7572 6e65 6420  ling was turned 
-0003c6c0: 6f66 662e 0d0a 0d0a 2020 2020 2020 2020  off.....        
-0003c6d0: 4578 616d 706c 650d 0a20 2020 2020 2020  Example..       
-0003c6e0: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020   -------..      
-0003c6f0: 2020 613d 6172 616e 6765 2831 5f30 3030    a=arange(1_000
-0003c700: 5f30 3029 0d0a 2020 2020 2020 2020 5265  _00)..        Re
-0003c710: 6379 636c 652e 6f66 6628 290d 0a20 2020  cycle.off()..   
-0003c720: 2020 2020 2025 7469 6d65 6974 2061 3d61       %timeit a=a
-0003c730: 202b 2031 0d0a 2020 2020 2020 2020 5265   + 1..        Re
-0003c740: 6379 636c 652e 6f6e 2829 0d0a 2020 2020  cycle.on()..    
-0003c750: 2020 2020 2574 696d 6569 7420 613d 6120      %timeit a=a 
-0003c760: 2b20 310d 0a0d 0a20 2020 2020 2020 2022  + 1....        "
-0003c770: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-0003c780: 726e 2046 6173 7441 7272 6179 2e5f 524f  rn FastArray._RO
-0003c790: 4e28 290d 0a0d 0a20 2020 2040 7374 6174  N()....    @stat
-0003c7a0: 6963 6d65 7468 6f64 0d0a 2020 2020 6465  icmethod..    de
-0003c7b0: 6620 6f66 6628 293a 0d0a 2020 2020 2020  f off():..      
-0003c7c0: 2020 7265 7475 726e 2046 6173 7441 7272    return FastArr
-0003c7d0: 6179 2e5f 524f 4646 2829 0d0a 0d0a 2020  ay._ROFF()....  
-0003c7e0: 2020 4073 7461 7469 636d 6574 686f 640d    @staticmethod.
-0003c7f0: 0a20 2020 2064 6566 206e 6f77 2874 696d  .    def now(tim
-0003c800: 656f 7574 3a20 696e 7420 3d20 3029 3a0d  eout: int = 0):.
-0003c810: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0003c820: 2020 2020 2020 5061 7373 2074 6865 2067        Pass the g
-0003c830: 6172 6261 6765 2063 6f6c 6c65 6374 6f72  arbage collector
-0003c840: 2074 696d 656f 7574 2076 616c 7565 2074   timeout value t
-0003c850: 6f20 636c 6561 6e75 702e 0d0a 2020 2020  o cleanup...    
-0003c860: 2020 2020 416c 736f 2063 616c 6c73 2074      Also calls t
-0003c870: 6865 2070 7974 686f 6e20 6761 7262 6167  he python garbag
-0003c880: 6520 636f 6c6c 6563 746f 722e 0d0a 0d0a  e collector.....
-0003c890: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0003c8a0: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
-0003c8b0: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-0003c8c0: 7469 6d65 6f75 743a 2064 6566 6175 6c74  timeout: default
-0003c8d0: 2074 6f20 302e 2020 3020 7769 6c6c 206e   to 0.  0 will n
-0003c8e0: 6f74 2073 6574 2061 2074 696d 656f 7574  ot set a timeout
-0003c8f0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-0003c900: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
-0003c910: 2d2d 2d2d 0d0a 2020 2020 2020 2020 746f  ----..        to
-0003c920: 7461 6c20 6172 7261 7973 2064 656c 6574  tal arrays delet
-0003c930: 6564 0d0a 2020 2020 2020 2020 2222 220d  ed..        """.
-0003c940: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-0003c950: 6763 0d0a 0d0a 2020 2020 2020 2020 6763  gc....        gc
-0003c960: 2e63 6f6c 6c65 6374 2829 0d0a 2020 2020  .collect()..    
-0003c970: 2020 2020 7265 7375 6c74 203d 2072 632e      result = rc.
-0003c980: 5265 6379 636c 6547 6172 6261 6765 436f  RecycleGarbageCo
-0003c990: 6c6c 6563 744e 6f77 2874 696d 656f 7574  llectNow(timeout
-0003c9a0: 295b 2254 6f74 616c 4465 6c65 7465 6422  )["TotalDeleted"
-0003c9b0: 5d0d 0a20 2020 2020 2020 2069 6620 7265  ]..        if re
-0003c9c0: 7375 6c74 203e 2030 3a0d 0a20 2020 2020  sult > 0:..     
-0003c9d0: 2020 2020 2020 2072 632e 5265 6379 636c         rc.Recycl
-0003c9e0: 6547 6172 6261 6765 436f 6c6c 6563 744e  eGarbageCollectN
-0003c9f0: 6f77 2874 696d 656f 7574 290d 0a20 2020  ow(timeout)..   
-0003ca00: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0003ca10: 6c74 0d0a 0d0a 2020 2020 4073 7461 7469  lt....    @stati
-0003ca20: 636d 6574 686f 640d 0a20 2020 2064 6566  cmethod..    def
-0003ca30: 2074 696d 656f 7574 2874 696d 656f 7574   timeout(timeout
-0003ca40: 3a20 696e 7420 3d20 3130 3029 3a0d 0a20  : int = 100):.. 
-0003ca50: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-0003ca60: 2020 2020 5061 7373 2074 6865 2067 6172      Pass the gar
-0003ca70: 6261 6765 2063 6f6c 6c65 6374 6f72 2074  bage collector t
-0003ca80: 696d 656f 7574 2076 616c 7565 2074 6f20  imeout value to 
-0003ca90: 6578 7069 7265 2e0d 0a20 2020 2020 2020  expire...       
-0003caa0: 2054 6865 2074 696d 656f 7574 2076 616c   The timeout val
-0003cab0: 7565 2069 7320 726f 7567 686c 7920 696e  ue is roughly in
-0003cac0: 2032 2f35 2073 6563 732e 0d0a 2020 2020   2/5 secs...    
-0003cad0: 2020 2020 4120 7661 6c75 6520 6f66 2031      A value of 1
-0003cae0: 3030 2069 7320 7573 7561 6c6c 7920 6162  00 is usually ab
-0003caf0: 6f75 7420 3430 2073 6563 6f6e 6473 2e0d  out 40 seconds..
-0003cb00: 0a20 2020 2020 2020 2049 6620 616e 2061  .        If an a
-0003cb10: 7272 6179 2068 6173 206e 6f74 2062 6565  rray has not bee
-0003cb20: 6e20 7265 7573 6564 2062 7920 7468 6520  n reused by the 
-0003cb30: 7469 6d65 6f75 742c 2069 7420 6973 2070  timeout, it is p
-0003cb40: 6572 6d61 6e65 6e74 6c79 2064 656c 6574  ermanently delet
-0003cb50: 6564 2e0d 0a0d 0a20 2020 2020 2020 2052  ed.....        R
-0003cb60: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
-0003cb70: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-0003cb80: 2070 7265 7669 6f75 7320 7469 6d65 7370   previous timesp
-0003cb90: 616e 0d0a 2020 2020 2020 2020 2222 220d  an..        """.
-0003cba0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0003cbb0: 7263 2e52 6563 7963 6c65 5365 7447 6172  rc.RecycleSetGar
-0003cbc0: 6261 6765 436f 6c6c 6563 7454 696d 656f  bageCollectTimeo
-0003cbd0: 7574 2874 696d 656f 7574 290d 0a0d 0a0d  ut(timeout).....
-0003cbe0: 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .# -------------
+0003c620: 2d2d 2d2d 2d2d 0d0a 636c 6173 7320 5265  ------..class Re
+0003c630: 6379 636c 653a 0d0a 2020 2020 4073 7461  cycle:..    @sta
+0003c640: 7469 636d 6574 686f 640d 0a20 2020 2064  ticmethod..    d
+0003c650: 6566 206f 6e28 293a 0d0a 2020 2020 2020  ef on():..      
+0003c660: 2020 2222 220d 0a20 2020 2020 2020 2054    """..        T
+0003c670: 7572 6e20 7269 7074 6162 6c65 2072 6563  urn riptable rec
+0003c680: 7963 6c69 6e67 206f 6e2e 0d0a 2020 2020  ycling on...    
+0003c690: 2020 2020 5573 6564 206f 6e6c 7920 7768      Used only wh
+0003c6a0: 656e 2072 6970 7461 626c 6520 7265 6379  en riptable recy
+0003c6b0: 636c 696e 6720 7761 7320 7475 726e 6564  cling was turned
+0003c6c0: 206f 6666 2e0d 0a0d 0a20 2020 2020 2020   off.....       
+0003c6d0: 2045 7861 6d70 6c65 0d0a 2020 2020 2020   Example..      
+0003c6e0: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
+0003c6f0: 2020 2061 3d61 7261 6e67 6528 315f 3030     a=arange(1_00
+0003c700: 305f 3030 290d 0a20 2020 2020 2020 2052  0_00)..        R
+0003c710: 6563 7963 6c65 2e6f 6666 2829 0d0a 2020  ecycle.off()..  
+0003c720: 2020 2020 2020 2574 696d 6569 7420 613d        %timeit a=
+0003c730: 6120 2b20 310d 0a20 2020 2020 2020 2052  a + 1..        R
+0003c740: 6563 7963 6c65 2e6f 6e28 290d 0a20 2020  ecycle.on()..   
+0003c750: 2020 2020 2025 7469 6d65 6974 2061 3d61       %timeit a=a
+0003c760: 202b 2031 0d0a 0d0a 2020 2020 2020 2020   + 1....        
+0003c770: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+0003c780: 7572 6e20 4661 7374 4172 7261 792e 5f52  urn FastArray._R
+0003c790: 4f4e 2829 0d0a 0d0a 2020 2020 4073 7461  ON()....    @sta
+0003c7a0: 7469 636d 6574 686f 640d 0a20 2020 2064  ticmethod..    d
+0003c7b0: 6566 206f 6666 2829 3a0d 0a20 2020 2020  ef off():..     
+0003c7c0: 2020 2072 6574 7572 6e20 4661 7374 4172     return FastAr
+0003c7d0: 7261 792e 5f52 4f46 4628 290d 0a0d 0a20  ray._ROFF().... 
+0003c7e0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+0003c7f0: 0d0a 2020 2020 6465 6620 6e6f 7728 7469  ..    def now(ti
+0003c800: 6d65 6f75 743a 2069 6e74 203d 2030 293a  meout: int = 0):
+0003c810: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0003c820: 2020 2020 2020 2050 6173 7320 7468 6520         Pass the 
+0003c830: 6761 7262 6167 6520 636f 6c6c 6563 746f  garbage collecto
+0003c840: 7220 7469 6d65 6f75 7420 7661 6c75 6520  r timeout value 
+0003c850: 746f 2063 6c65 616e 7570 2e0d 0a20 2020  to cleanup...   
+0003c860: 2020 2020 2041 6c73 6f20 6361 6c6c 7320       Also calls 
+0003c870: 7468 6520 7079 7468 6f6e 2067 6172 6261  the python garba
+0003c880: 6765 2063 6f6c 6c65 6374 6f72 2e0d 0a0d  ge collector....
+0003c890: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0003c8a0: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
+0003c8b0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+0003c8c0: 2074 696d 656f 7574 3a20 6465 6661 756c   timeout: defaul
+0003c8d0: 7420 746f 2030 2e20 2030 2077 696c 6c20  t to 0.  0 will 
+0003c8e0: 6e6f 7420 7365 7420 6120 7469 6d65 6f75  not set a timeou
+0003c8f0: 740d 0a0d 0a20 2020 2020 2020 2052 6574  t....        Ret
+0003c900: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
+0003c910: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2074  -----..        t
+0003c920: 6f74 616c 2061 7272 6179 7320 6465 6c65  otal arrays dele
+0003c930: 7465 640d 0a20 2020 2020 2020 2022 2222  ted..        """
+0003c940: 0d0a 2020 2020 2020 2020 696d 706f 7274  ..        import
+0003c950: 2067 630d 0a0d 0a20 2020 2020 2020 2067   gc....        g
+0003c960: 632e 636f 6c6c 6563 7428 290d 0a20 2020  c.collect()..   
+0003c970: 2020 2020 2072 6573 756c 7420 3d20 7263       result = rc
+0003c980: 2e52 6563 7963 6c65 4761 7262 6167 6543  .RecycleGarbageC
+0003c990: 6f6c 6c65 6374 4e6f 7728 7469 6d65 6f75  ollectNow(timeou
+0003c9a0: 7429 5b22 546f 7461 6c44 656c 6574 6564  t)["TotalDeleted
+0003c9b0: 225d 0d0a 2020 2020 2020 2020 6966 2072  "]..        if r
+0003c9c0: 6573 756c 7420 3e20 303a 0d0a 2020 2020  esult > 0:..    
+0003c9d0: 2020 2020 2020 2020 7263 2e52 6563 7963          rc.Recyc
+0003c9e0: 6c65 4761 7262 6167 6543 6f6c 6c65 6374  leGarbageCollect
+0003c9f0: 4e6f 7728 7469 6d65 6f75 7429 0d0a 2020  Now(timeout)..  
+0003ca00: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0003ca10: 756c 740d 0a0d 0a20 2020 2040 7374 6174  ult....    @stat
+0003ca20: 6963 6d65 7468 6f64 0d0a 2020 2020 6465  icmethod..    de
+0003ca30: 6620 7469 6d65 6f75 7428 7469 6d65 6f75  f timeout(timeou
+0003ca40: 743a 2069 6e74 203d 2031 3030 293a 0d0a  t: int = 100):..
+0003ca50: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+0003ca60: 2020 2020 2050 6173 7320 7468 6520 6761       Pass the ga
+0003ca70: 7262 6167 6520 636f 6c6c 6563 746f 7220  rbage collector 
+0003ca80: 7469 6d65 6f75 7420 7661 6c75 6520 746f  timeout value to
+0003ca90: 2065 7870 6972 652e 0d0a 2020 2020 2020   expire...      
+0003caa0: 2020 5468 6520 7469 6d65 6f75 7420 7661    The timeout va
+0003cab0: 6c75 6520 6973 2072 6f75 6768 6c79 2069  lue is roughly i
+0003cac0: 6e20 322f 3520 7365 6373 2e0d 0a20 2020  n 2/5 secs...   
+0003cad0: 2020 2020 2041 2076 616c 7565 206f 6620       A value of 
+0003cae0: 3130 3020 6973 2075 7375 616c 6c79 2061  100 is usually a
+0003caf0: 626f 7574 2034 3020 7365 636f 6e64 732e  bout 40 seconds.
+0003cb00: 0d0a 2020 2020 2020 2020 4966 2061 6e20  ..        If an 
+0003cb10: 6172 7261 7920 6861 7320 6e6f 7420 6265  array has not be
+0003cb20: 656e 2072 6575 7365 6420 6279 2074 6865  en reused by the
+0003cb30: 2074 696d 656f 7574 2c20 6974 2069 7320   timeout, it is 
+0003cb40: 7065 726d 616e 656e 746c 7920 6465 6c65  permanently dele
+0003cb50: 7465 642e 0d0a 0d0a 2020 2020 2020 2020  ted.....        
+0003cb60: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
+0003cb70: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020   -------..      
+0003cb80: 2020 7072 6576 696f 7573 2074 696d 6573    previous times
+0003cb90: 7061 6e0d 0a20 2020 2020 2020 2022 2222  pan..        """
+0003cba0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0003cbb0: 2072 632e 5265 6379 636c 6553 6574 4761   rc.RecycleSetGa
+0003cbc0: 7262 6167 6543 6f6c 6c65 6374 5469 6d65  rbageCollectTime
+0003cbd0: 6f75 7428 7469 6d65 6f75 7429 0d0a 0d0a  out(timeout)....
+0003cbe0: 0d0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..# ------------
 0003cbf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003cc00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0003cc10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a63  -------------..c
-0003cc20: 6c61 7373 204c 6564 6765 723a 0d0a 2020  lass Ledger:..  
-0003cc30: 2020 4073 7461 7469 636d 6574 686f 640d    @staticmethod.
-0003cc40: 0a20 2020 2064 6566 206f 6e28 293a 0d0a  .    def on():..
-0003cc50: 2020 2020 2020 2020 2222 2254 7572 6e20          """Turn 
-0003cc60: 7468 6520 6d61 7468 206c 6564 6765 7220  the math ledger 
-0003cc70: 6f6e 2074 6f20 7265 636f 7264 2061 6c6c  on to record all
-0003cc80: 2061 7272 6179 206d 6174 6820 726f 7574   array math rout
-0003cc90: 696e 6573 2222 220d 0a20 2020 2020 2020  ines"""..       
-0003cca0: 2072 6574 7572 6e20 5479 7065 5265 6769   return TypeRegi
-0003ccb0: 7374 6572 2e4d 6174 684c 6564 6765 722e  ster.MathLedger.
-0003ccc0: 5f4c 6564 6765 724f 6e28 290d 0a0d 0a20  _LedgerOn().... 
-0003ccd0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-0003cce0: 0d0a 2020 2020 6465 6620 6f66 6628 293a  ..    def off():
-0003ccf0: 0d0a 2020 2020 2020 2020 2222 2254 7572  ..        """Tur
-0003cd00: 6e20 7468 6520 6d61 7468 206c 6564 6765  n the math ledge
-0003cd10: 7220 6f66 6622 2222 0d0a 2020 2020 2020  r off"""..      
-0003cd20: 2020 7265 7475 726e 2054 7970 6552 6567    return TypeReg
-0003cd30: 6973 7465 722e 4d61 7468 4c65 6467 6572  ister.MathLedger
-0003cd40: 2e5f 4c65 6467 6572 4f66 6628 290d 0a0d  ._LedgerOff()...
-0003cd50: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-0003cd60: 6f64 0d0a 2020 2020 6465 6620 6475 6d70  od..    def dump
-0003cd70: 2864 6174 6173 6574 3d54 7275 6529 3a0d  (dataset=True):.
-0003cd80: 0a20 2020 2020 2020 2022 2222 5072 696e  .        """Prin
-0003cd90: 7420 6f75 7420 7468 6520 6d61 7468 206c  t out the math l
-0003cda0: 6564 6765 7222 2222 0d0a 2020 2020 2020  edger"""..      
-0003cdb0: 2020 7265 7475 726e 2054 7970 6552 6567    return TypeReg
-0003cdc0: 6973 7465 722e 4d61 7468 4c65 6467 6572  ister.MathLedger
-0003cdd0: 2e5f 4c65 6467 6572 4475 6d70 2864 6174  ._LedgerDump(dat
-0003cde0: 6173 6574 3d64 6174 6173 6574 290d 0a0d  aset=dataset)...
-0003cdf0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-0003ce00: 6f64 0d0a 2020 2020 6465 6620 746f 5f66  od..    def to_f
-0003ce10: 696c 6528 6669 6c65 6e61 6d65 293a 0d0a  ile(filename):..
-0003ce20: 2020 2020 2020 2020 2222 2253 6176 6520          """Save 
-0003ce30: 7468 6520 6d61 7468 206c 6564 6765 7220  the math ledger 
-0003ce40: 746f 2061 2066 696c 6522 2222 0d0a 2020  to a file"""..  
-0003ce50: 2020 2020 2020 7265 7475 726e 2054 7970        return Typ
-0003ce60: 6552 6567 6973 7465 722e 4d61 7468 4c65  eRegister.MathLe
-0003ce70: 6467 6572 2e5f 4c65 6467 6572 4475 6d70  dger._LedgerDump
-0003ce80: 4669 6c65 2866 696c 656e 616d 6529 0d0a  File(filename)..
-0003ce90: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-0003cea0: 686f 640d 0a20 2020 2064 6566 2063 6c65  hod..    def cle
-0003ceb0: 6172 2829 3a0d 0a20 2020 2020 2020 2022  ar():..        "
-0003cec0: 2222 436c 6561 7220 616c 6c20 7468 6520  ""Clear all the 
-0003ced0: 656e 7472 6965 7320 696e 2074 6865 206d  entries in the m
-0003cee0: 6174 6820 6c65 6467 6572 2222 220d 0a20  ath ledger""".. 
-0003cef0: 2020 2020 2020 2072 6574 7572 6e20 5479         return Ty
-0003cf00: 7065 5265 6769 7374 6572 2e4d 6174 684c  peRegister.MathL
-0003cf10: 6564 6765 722e 5f4c 6564 6765 7243 6c65  edger._LedgerCle
-0003cf20: 6172 2829 0d0a 0d0a 0d0a 2320 2d2d 2d2d  ar()......# ----
+0003cc10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
+0003cc20: 636c 6173 7320 4c65 6467 6572 3a0d 0a20  class Ledger:.. 
+0003cc30: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+0003cc40: 0d0a 2020 2020 6465 6620 6f6e 2829 3a0d  ..    def on():.
+0003cc50: 0a20 2020 2020 2020 2022 2222 5475 726e  .        """Turn
+0003cc60: 2074 6865 206d 6174 6820 6c65 6467 6572   the math ledger
+0003cc70: 206f 6e20 746f 2072 6563 6f72 6420 616c   on to record al
+0003cc80: 6c20 6172 7261 7920 6d61 7468 2072 6f75  l array math rou
+0003cc90: 7469 6e65 7322 2222 0d0a 2020 2020 2020  tines"""..      
+0003cca0: 2020 7265 7475 726e 2054 7970 6552 6567    return TypeReg
+0003ccb0: 6973 7465 722e 4d61 7468 4c65 6467 6572  ister.MathLedger
+0003ccc0: 2e5f 4c65 6467 6572 4f6e 2829 0d0a 0d0a  ._LedgerOn()....
+0003ccd0: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
+0003cce0: 640d 0a20 2020 2064 6566 206f 6666 2829  d..    def off()
+0003ccf0: 3a0d 0a20 2020 2020 2020 2022 2222 5475  :..        """Tu
+0003cd00: 726e 2074 6865 206d 6174 6820 6c65 6467  rn the math ledg
+0003cd10: 6572 206f 6666 2222 220d 0a20 2020 2020  er off"""..     
+0003cd20: 2020 2072 6574 7572 6e20 5479 7065 5265     return TypeRe
+0003cd30: 6769 7374 6572 2e4d 6174 684c 6564 6765  gister.MathLedge
+0003cd40: 722e 5f4c 6564 6765 724f 6666 2829 0d0a  r._LedgerOff()..
+0003cd50: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+0003cd60: 686f 640d 0a20 2020 2064 6566 2064 756d  hod..    def dum
+0003cd70: 7028 6461 7461 7365 743d 5472 7565 293a  p(dataset=True):
+0003cd80: 0d0a 2020 2020 2020 2020 2222 2250 7269  ..        """Pri
+0003cd90: 6e74 206f 7574 2074 6865 206d 6174 6820  nt out the math 
+0003cda0: 6c65 6467 6572 2222 220d 0a20 2020 2020  ledger"""..     
+0003cdb0: 2020 2072 6574 7572 6e20 5479 7065 5265     return TypeRe
+0003cdc0: 6769 7374 6572 2e4d 6174 684c 6564 6765  gister.MathLedge
+0003cdd0: 722e 5f4c 6564 6765 7244 756d 7028 6461  r._LedgerDump(da
+0003cde0: 7461 7365 743d 6461 7461 7365 7429 0d0a  taset=dataset)..
+0003cdf0: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+0003ce00: 686f 640d 0a20 2020 2064 6566 2074 6f5f  hod..    def to_
+0003ce10: 6669 6c65 2866 696c 656e 616d 6529 3a0d  file(filename):.
+0003ce20: 0a20 2020 2020 2020 2022 2222 5361 7665  .        """Save
+0003ce30: 2074 6865 206d 6174 6820 6c65 6467 6572   the math ledger
+0003ce40: 2074 6f20 6120 6669 6c65 2222 220d 0a20   to a file""".. 
+0003ce50: 2020 2020 2020 2072 6574 7572 6e20 5479         return Ty
+0003ce60: 7065 5265 6769 7374 6572 2e4d 6174 684c  peRegister.MathL
+0003ce70: 6564 6765 722e 5f4c 6564 6765 7244 756d  edger._LedgerDum
+0003ce80: 7046 696c 6528 6669 6c65 6e61 6d65 290d  pFile(filename).
+0003ce90: 0a0d 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
+0003cea0: 7468 6f64 0d0a 2020 2020 6465 6620 636c  thod..    def cl
+0003ceb0: 6561 7228 293a 0d0a 2020 2020 2020 2020  ear():..        
+0003cec0: 2222 2243 6c65 6172 2061 6c6c 2074 6865  """Clear all the
+0003ced0: 2065 6e74 7269 6573 2069 6e20 7468 6520   entries in the 
+0003cee0: 6d61 7468 206c 6564 6765 7222 2222 0d0a  math ledger"""..
+0003cef0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+0003cf00: 7970 6552 6567 6973 7465 722e 4d61 7468  ypeRegister.Math
+0003cf10: 4c65 6467 6572 2e5f 4c65 6467 6572 436c  Ledger._LedgerCl
+0003cf20: 6561 7228 290d 0a0d 0a0d 0a23 202d 2d2d  ear()......# ---
 0003cf30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003cf40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003cf50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0003cf60: 2d2d 2d2d 2d2d 0d0a 2320 7468 6973 2069  ------..# this i
-0003cf70: 7320 6361 6c6c 6564 2077 6865 6e20 7468  s called when th
-0003cf80: 6520 6d6f 6475 6c65 2069 7320 6c6f 6164  e module is load
-0003cf90: 6564 0d0a 5f46 6978 7570 446f 6353 7472  ed.._FixupDocStr
-0003cfa0: 696e 6773 2829 0d0a 0d0a 2320 4e4f 5445  ings()....# NOTE
-0003cfb0: 3a20 4b65 6570 2074 6869 7320 6174 2074  : Keep this at t
-0003cfc0: 6865 2065 6e64 206f 6620 7468 6520 6669  he end of the fi
-0003cfd0: 6c65 0d0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  le..# ----------
+0003cf60: 2d2d 2d2d 2d2d 2d0d 0a23 2074 6869 7320  -------..# this 
+0003cf70: 6973 2063 616c 6c65 6420 7768 656e 2074  is called when t
+0003cf80: 6865 206d 6f64 756c 6520 6973 206c 6f61  he module is loa
+0003cf90: 6465 640d 0a5f 4669 7875 7044 6f63 5374  ded.._FixupDocSt
+0003cfa0: 7269 6e67 7328 290d 0a0d 0a23 204e 4f54  rings()....# NOT
+0003cfb0: 453a 204b 6565 7020 7468 6973 2061 7420  E: Keep this at 
+0003cfc0: 7468 6520 656e 6420 6f66 2074 6865 2066  the end of the f
+0003cfd0: 696c 650d 0a23 202d 2d2d 2d2d 2d2d 2d2d  ile..# ---------
 0003cfe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003cff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0003d000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0003d010: 2d0d 0a23 2063 616c 6c69 6e67 2074 6869  -..# calling thi
-0003d020: 7320 6675 6e63 7469 6f6e 2077 696c 6c20  s function will 
-0003d030: 666f 7263 6520 666d 2074 6f20 7265 7475  force fm to retu
-0003d040: 726e 2046 6173 7441 7272 6179 2073 7562  rn FastArray sub
-0003d050: 636c 6173 730d 0a5f 7365 7466 6173 7461  class.._setfasta
-0003d060: 7272 6179 7479 7065 2829 0d0a 0d0a 5479  rraytype()....Ty
-0003d070: 7065 5265 6769 7374 6572 2e46 6173 7441  peRegister.FastA
-0003d080: 7272 6179 203d 2046 6173 7441 7272 6179  rray = FastArray
-0003d090: 0d0a 0d0a 4661 7374 4172 7261 792e 7265  ....FastArray.re
-0003d0a0: 6769 7374 6572 5f66 756e 6374 696f 6e28  gister_function(
-0003d0b0: 2264 6573 6372 6962 6522 2c20 6465 7363  "describe", desc
-0003d0c0: 7269 6265 290d 0a                        ribe)..
+0003d010: 2d2d 0d0a 2320 6361 6c6c 696e 6720 7468  --..# calling th
+0003d020: 6973 2066 756e 6374 696f 6e20 7769 6c6c  is function will
+0003d030: 2066 6f72 6365 2066 6d20 746f 2072 6574   force fm to ret
+0003d040: 7572 6e20 4661 7374 4172 7261 7920 7375  urn FastArray su
+0003d050: 6263 6c61 7373 0d0a 5f73 6574 6661 7374  bclass.._setfast
+0003d060: 6172 7261 7974 7970 6528 290d 0a0d 0a54  arraytype()....T
+0003d070: 7970 6552 6567 6973 7465 722e 4661 7374  ypeRegister.Fast
+0003d080: 4172 7261 7920 3d20 4661 7374 4172 7261  Array = FastArra
+0003d090: 790d 0a0d 0a46 6173 7441 7272 6179 2e72  y....FastArray.r
+0003d0a0: 6567 6973 7465 725f 6675 6e63 7469 6f6e  egister_function
+0003d0b0: 2822 6465 7363 7269 6265 222c 2064 6573  ("describe", des
+0003d0c0: 6372 6962 6529 0d0a                      cribe)..
```

### Comparing `riptable-1.9.1/riptable/rt_fastarraynumba.py` & `riptable-1.9.2/riptable/rt_fastarraynumba.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_groupby.py` & `riptable-1.9.2/riptable/rt_groupby.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_groupbykeys.py` & `riptable-1.9.2/riptable/rt_groupbykeys.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_groupbynumba.py` & `riptable-1.9.2/riptable/rt_groupbynumba.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_groupbyops.py` & `riptable-1.9.2/riptable/rt_groupbyops.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_grouping.py` & `riptable-1.9.2/riptable/rt_grouping.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_hstack.py` & `riptable-1.9.2/riptable/rt_hstack.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_imatrix.py` & `riptable-1.9.2/riptable/rt_imatrix.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_io.py` & `riptable-1.9.2/riptable/rt_io.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_itemcontainer.py` & `riptable-1.9.2/riptable/rt_itemcontainer.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_ledger.py` & `riptable-1.9.2/riptable/rt_ledger.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_matplotlib.py` & `riptable-1.9.2/riptable/rt_matplotlib.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_merge.py` & `riptable-1.9.2/riptable/rt_merge.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_merge_asof.py` & `riptable-1.9.2/riptable/rt_merge_asof.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_meta.py` & `riptable-1.9.2/riptable/rt_meta.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_misc.py` & `riptable-1.9.2/riptable/rt_misc.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_mlutils.py` & `riptable-1.9.2/riptable/rt_mlutils.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_multiset.py` & `riptable-1.9.2/riptable/rt_multiset.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_numpy.py` & `riptable-1.9.2/riptable/rt_numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -4583,15 +4583,15 @@
 def logical(a):
     if isinstance(a, np.ndarray):
         if a.dtype == np.bool_:
             return a
         return a.astype(np.bool_)
     # TODO: Check for scalar here? Then we can be maybe use np.asanyarray(..., dtype=bool).view(TypeRegister.FastArray)
     #       to replace the use of the deprecated `np.bool`.
-    return np.bool(a).view(TypeRegister.FastArray)
+    return np.bool_(a).view(TypeRegister.FastArray)
 
 
 ##-------------------------------------------------------
 # not allowed
 # class bool(np.bool):
 #    pass
```

### Comparing `riptable-1.9.1/riptable/rt_pdataset.py` & `riptable-1.9.2/riptable/rt_pdataset.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_pgroupby.py` & `riptable-1.9.2/riptable/rt_pgroupby.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_sds.py` & `riptable-1.9.2/riptable/rt_sds.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_sharedmemory.py` & `riptable-1.9.2/riptable/rt_sharedmemory.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_sort_cache.py` & `riptable-1.9.2/riptable/rt_sort_cache.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_stats.py` & `riptable-1.9.2/riptable/rt_stats.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_str.py` & `riptable-1.9.2/riptable/rt_str.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_struct.py` & `riptable-1.9.2/riptable/rt_struct.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_timers.py` & `riptable-1.9.2/riptable/rt_timers.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_timezone.py` & `riptable-1.9.2/riptable/rt_timezone.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/rt_utils.py` & `riptable-1.9.2/riptable/rt_utils.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/test_tooling_integration/ipykernel_integration_test.py` & `riptable-1.9.2/riptable/test_tooling_integration/ipykernel_integration_test.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/test_tooling_integration/ipython_compatibility_test.py` & `riptable-1.9.2/riptable/test_tooling_integration/ipython_compatibility_test.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/test_tooling_integration/ipython_integration_test.py` & `riptable-1.9.2/riptable/test_tooling_integration/ipython_integration_test.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/test_tooling_integration/run.py` & `riptable-1.9.2/riptable/test_tooling_integration/run.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/test_tooling_integration/test_display/test_display.py` & `riptable-1.9.2/riptable/test_tooling_integration/test_display/test_display.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/test_tooling_integration/test_display/vnu_checker.py` & `riptable-1.9.2/riptable/test_tooling_integration/test_display/vnu_checker.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/testing/array_assert.py` & `riptable-1.9.2/riptable/testing/array_assert.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/testing/randgen.py` & `riptable-1.9.2/riptable/testing/randgen.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/generator_categorical_unit_test.py` & `riptable-1.9.2/riptable/tests/generator_categorical_unit_test.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/generator_groupby_unit_test.py` & `riptable-1.9.2/riptable/tests/generator_groupby_unit_test.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/groupby_categorical_unit_test_parameters.py` & `riptable-1.9.2/riptable/tests/groupby_categorical_unit_test_parameters.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/groupby_unit_test_parameters.py` & `riptable-1.9.2/riptable/tests/groupby_unit_test_parameters.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/run.py` & `riptable-1.9.2/riptable/tests/run.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/runall.py` & `riptable-1.9.2/riptable/tests/runall.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_accum2.py` & `riptable-1.9.2/riptable/tests/test_accum2.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_accumtable.py` & `riptable-1.9.2/riptable/tests/test_accumtable.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_apply.py` & `riptable-1.9.2/riptable/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_base_function.py` & `riptable-1.9.2/riptable/tests/test_base_function.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_bitcount.py` & `riptable-1.9.2/riptable/tests/test_bitcount.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical.py` & `riptable-1.9.2/riptable/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical_autotest_aggregated_functions.py` & `riptable-1.9.2/riptable/tests/test_categorical_autotest_aggregated_functions.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical_base_index.py` & `riptable-1.9.2/riptable/tests/test_categorical_base_index.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical_dtype.py` & `riptable-1.9.2/riptable/tests/test_categorical_dtype.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical_filter_invalid.py` & `riptable-1.9.2/riptable/tests/test_categorical_filter_invalid.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical_functions.py` & `riptable-1.9.2/riptable/tests/test_categorical_functions.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical_groupby.py` & `riptable-1.9.2/riptable/tests/test_categorical_groupby.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical_keywords.py` & `riptable-1.9.2/riptable/tests/test_categorical_keywords.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical_modify.py` & `riptable-1.9.2/riptable/tests/test_categorical_modify.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical_ordered.py` & `riptable-1.9.2/riptable/tests/test_categorical_ordered.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical_setitem.py` & `riptable-1.9.2/riptable/tests/test_categorical_setitem.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical_sort_order.py` & `riptable-1.9.2/riptable/tests/test_categorical_sort_order.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_categorical_values.py` & `riptable-1.9.2/riptable/tests/test_categorical_values.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_conversion_utils.py` & `riptable-1.9.2/riptable/tests/test_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_csv.py` & `riptable-1.9.2/riptable/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_cut.py` & `riptable-1.9.2/riptable/tests/test_cut.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_dataset.py` & `riptable-1.9.2/riptable/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_dataset_slicing.py` & `riptable-1.9.2/riptable/tests/test_dataset_slicing.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_date.py` & `riptable-1.9.2/riptable/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_datetime.py` & `riptable-1.9.2/riptable/tests/test_datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,38 @@
     return bool(np.all(a == b))
 
 
 def arr_all(a):
     return bool(np.all(a))
 
 
+def test_dtn_start_date_array():
+    # For the DTN constructor, this tests how a Date array for start_date
+    # is applied to arr.
+    arr = ["08:00", "13:00"]  # String arr is parsed as TimeSpan.
+
+    # If len(start_date) == 1, the Date should be broadcast to arr.
+    start_date = Date("20230601")
+    dtn = DateTimeNano(arr, from_tz="UTC", to_tz="UTC", start_date=start_date)
+    assert (Date(dtn) == start_date).all(), "start_date wasn't properly broadcast to arr."
+
+    # If len(start_date) == len(arr), the start_date values should be applied elementwise to arr.
+    days = len(arr)
+    start_date = Date.range("20230601", days=days)
+    dtn = DateTimeNano(arr, from_tz="UTC", to_tz="UTC", start_date=start_date)
+    assert (Date(dtn) == start_date).all(), "start_date wasn't properly applied elementwise to arr."
+
+    # Otherwise, if len(start_date) != len(arr), an error should be raised.
+    days = len(arr) + 1
+    start_date = Date.range("20230601", days=days)
+    msg = "start_date Date array must be either length 1 or the same length as arr."
+    with pytest.raises(ValueError, match=msg):
+        DateTimeNano(arr, from_tz="UTC", to_tz="UTC", start_date=start_date)
+
+
 def test_dtn_from_matlab():
     # Test that the output matches what the code should be generating.
     arr = [737426, 738583.75]
     from_tz = "NYC"
     to_tz = "NYC"
     _timezone = TimeZone(from_tz=from_tz, to_tz=to_tz)
     obj = DateTimeNano(arr, from_matlab=True, from_tz=from_tz)
```

### Comparing `riptable-1.9.1/riptable/tests/test_datetime_math.py` & `riptable-1.9.2/riptable/tests/test_datetime_math.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_fastarray.py` & `riptable-1.9.2/riptable/tests/test_fastarray.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_fastarray_bn.py` & `riptable-1.9.2/riptable/tests/test_fastarray_bn.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_fastarray_constructor.py` & `riptable-1.9.2/riptable/tests/test_fastarray_constructor.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_fastarray_functions.py` & `riptable-1.9.2/riptable/tests/test_fastarray_functions.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_files/groupby1_ex3.pickle` & `riptable-1.9.2/riptable/tests/test_files/groupby1_ex3.pickle`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_files/unicode_ex1.csv` & `riptable-1.9.2/riptable/tests/test_files/unicode_ex1.csv`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_files/unicode_ex2.csv` & `riptable-1.9.2/riptable/tests/test_files/unicode_ex2.csv`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_files/unicode_ex3.csv` & `riptable-1.9.2/riptable/tests/test_files/unicode_ex3.csv`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_flatten.py` & `riptable-1.9.2/riptable/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_groupby.py` & `riptable-1.9.2/riptable/tests/test_groupby.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_groupby_autotest_aggregated_functions.py` & `riptable-1.9.2/riptable/tests/test_groupby_autotest_aggregated_functions.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_groupby_functions.py` & `riptable-1.9.2/riptable/tests/test_groupby_functions.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_groupby_simple_multikey.py` & `riptable-1.9.2/riptable/tests/test_groupby_simple_multikey.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_groupbyops.py` & `riptable-1.9.2/riptable/tests/test_groupbyops.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_grouping.py` & `riptable-1.9.2/riptable/tests/test_grouping.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_interop_pyarrow.py` & `riptable-1.9.2/riptable/tests/test_interop_pyarrow.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_ismember.py` & `riptable-1.9.2/riptable/tests/test_ismember.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_lexsort.py` & `riptable-1.9.2/riptable/tests/test_lexsort.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_merge.py` & `riptable-1.9.2/riptable/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_merge_asof.py` & `riptable-1.9.2/riptable/tests/test_merge_asof.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_meta.py` & `riptable-1.9.2/riptable/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_multiset.py` & `riptable-1.9.2/riptable/tests/test_multiset.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_pandas_utils.py` & `riptable-1.9.2/riptable/tests/test_pandas_utils.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_pdataset.py` & `riptable-1.9.2/riptable/tests/test_pdataset.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_pgroupby.py` & `riptable-1.9.2/riptable/tests/test_pgroupby.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_restore_subclass.py` & `riptable-1.9.2/riptable/tests/test_restore_subclass.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_riptide_cpp.py` & `riptable-1.9.2/riptable/tests/test_riptide_cpp.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_rtnumpy.py` & `riptable-1.9.2/riptable/tests/test_rtnumpy.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_rtutils.py` & `riptable-1.9.2/riptable/tests/test_rtutils.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_saveload.py` & `riptable-1.9.2/riptable/tests/test_saveload.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_scalar.py` & `riptable-1.9.2/riptable/tests/test_scalar.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_sds.py` & `riptable-1.9.2/riptable/tests/test_sds.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_sprint_fastarray.py` & `riptable-1.9.2/riptable/tests/test_sprint_fastarray.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_str.py` & `riptable-1.9.2/riptable/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_struct.py` & `riptable-1.9.2/riptable/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_timewindow.py` & `riptable-1.9.2/riptable/tests/test_timewindow.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_ufunc2.py` & `riptable-1.9.2/riptable/tests/test_ufunc2.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_unique.py` & `riptable-1.9.2/riptable/tests/test_unique.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/test_utils.py` & `riptable-1.9.2/riptable/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable/tests/utils.py` & `riptable-1.9.2/riptable/tests/utils.py`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/riptable.egg-info/PKG-INFO` & `riptable-1.9.2/riptable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riptable
-Version: 1.9.1
+Version: 1.9.2
 Summary: Python Package for riptable studies framework
 Home-page: https://github.com/rtosholdings/riptable
 Author: RTOS Holdings
 Author-email: rtosholdings-bot@sig.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `riptable-1.9.1/riptable.egg-info/SOURCES.txt` & `riptable-1.9.2/riptable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `riptable-1.9.1/setup.py` & `riptable-1.9.2/setup.py`

 * *Files identical despite different names*

