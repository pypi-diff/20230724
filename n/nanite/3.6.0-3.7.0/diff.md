# Comparing `tmp/nanite-3.6.0.tar.gz` & `tmp/nanite-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanite-3.6.0.tar", last modified: Fri Jul 21 13:21:02 2023, max compression
+gzip compressed data, was "nanite-3.7.0.tar", last modified: Mon Jul 24 13:26:43 2023, max compression
```

## Comparing `nanite-3.6.0.tar` & `nanite-3.7.0.tar`

### file list

```diff
@@ -1,164 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.731015 nanite-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-21 13:20:46.000000 nanite-3.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-21 13:20:46.000000 nanite-3.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-07-21 13:20:46.000000 nanite-3.6.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 13:20:46.000000 nanite-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-21 13:20:46.000000 nanite-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-21 13:21:02.731015 nanite-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-21 13:20:46.000000 nanite-3.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.703014 nanite-3.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.703014 nanite-3.6.0/docs/data/
--rw-r--r--   0 runner    (1001) docker     (123)   131520 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/data/force-save-example.jpk-force
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.703014 nanite-3.6.0/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/extensions/fancy_include.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/extensions/nanite_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/extensions/nanite_preprocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/extensions/simple_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    28646 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/fitting_geometry.png
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/fitting_geometry.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.703014 nanite-3.6.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/img/nanite-fit-example.png
--rw-r--r--   0 runner    (1001) docker     (123)    86373 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/img/nanite-rate-example.png
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/nanite.bib
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_code_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_develop.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_fitting_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_rating_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_z_bib.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.703014 nanite-3.6.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.703014 nanite-3.6.0/examples/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)   159955 2023-07-21 13:20:46.000000 nanite-3.6.0/examples/data/zebrafish-head-section-gray-matter.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)    37788 2023-07-21 13:20:46.000000 nanite-3.6.0/examples/fit_and_rate.png
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-21 13:20:46.000000 nanite-3.6.0/examples/fit_and_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-21 13:20:46.000000 nanite-3.6.0/examples/generate_example_images.py
--rw-r--r--   0 runner    (1001) docker     (123)   104455 2023-07-21 13:20:46.000000 nanite-3.6.0/examples/model_spherical_indenter.png
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-21 13:20:46.000000 nanite-3.6.0/examples/model_spherical_indenter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.707014 nanite-3.6.0/nanite/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.707014 nanite-3.6.0/nanite/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/cli/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/cli/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/cli/rating.py
--rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/indent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.711014 nanite-3.6.0/nanite/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/model_conical_indenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/model_hertz_paraboloidal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/model_hertz_three_sided_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/model_sneddon_spherical.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/model_sneddon_spherical_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/residuals.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/weight.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/poc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/qmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.711014 nanite-3.6.0/nanite/rate/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/rater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/regressors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.715014 nanite-3.6.0/nanite/rate/ts_zef18/
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_bin_apr_spikes_count.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_bin_cp_position.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_bin_size.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_apr_flatness.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_apr_size.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_apr_sum.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_bln_slope.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_bln_variation.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_cp_curvature.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_cp_magnitude.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_maxima_75perc.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_monotony.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_spike_area.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_sum.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_sum_75perc.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.707014 nanite-3.6.0/nanite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-21 13:20:46.000000 nanite-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:21:02.731015 nanite-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-21 13:20:46.000000 nanite-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.719015 nanite-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.731015 nanite-3.6.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/cli-profile-1.7.8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/cli-profile-2.1.0.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    42815 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-afm-workshop-fd_single_2021-10-22_14.16.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    68411 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-cl_calibration_force-save-2015-02-04.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)   158553 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)   497346 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_map-data-reference-points.jpk-force-map
--rw-r--r--   0 runner    (1001) docker     (123)   407527 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_map0d_extracted.jpk-force-map
--rwxr-xr-x   0 runner    (1001) docker     (123)  1645418 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_map1d_2016-11-07.jpk-force-map
--rw-r--r--   0 runner    (1001) docker     (123)   953060 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_map2x2_extracted.jpk-force-map
--rw-r--r--   0 runner    (1001) docker     (123)   401583 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_1.jpk-force-map
--rw-r--r--   0 runner    (1001) docker     (123)   400957 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map
--rwxr-xr-x   0 runner    (1001) docker     (123)   193751 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_1.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)   101264 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_2.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)   101240 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)   103538 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)   101531 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)   311042 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)     6785 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)     6783 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)     6799 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)   596184 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_tilted-baseline-mitotic_2021-01-29.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_spot3-0192.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/model_external_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    93520 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/rate-export_1.7.8.h5
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_cli_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_cli_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_cli_rating.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_fit_ancillary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_fit_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_fit_emodulus_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_fit_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_fit_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_indent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_indent2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_hertz_cone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_hertz_parabol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_hertz_pyramid_three.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_sneddon_spherical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_sneddon_spherical_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_sneddon_spherical_invert_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_open_jpk_variation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_poc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_qmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_rate_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_rate_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_rate_training_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.675730 nanite-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-24 13:26:27.000000 nanite-3.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-24 13:26:27.000000 nanite-3.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-24 13:26:27.000000 nanite-3.7.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 13:26:27.000000 nanite-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 13:26:27.000000 nanite-3.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-24 13:26:43.675730 nanite-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-24 13:26:27.000000 nanite-3.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.647730 nanite-3.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.647730 nanite-3.7.0/docs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   131520 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/data/force-save-example.jpk-force
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.647730 nanite-3.7.0/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/extensions/fancy_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/extensions/nanite_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/extensions/nanite_preprocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/extensions/simple_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28646 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/fitting_geometry.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/fitting_geometry.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.647730 nanite-3.7.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/img/nanite-fit-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86373 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/img/nanite-rate-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/nanite.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_code_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_develop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_fitting_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_rating_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_z_bib.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.647730 nanite-3.7.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.647730 nanite-3.7.0/examples/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   159955 2023-07-24 13:26:27.000000 nanite-3.7.0/examples/data/zebrafish-head-section-gray-matter.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)    37788 2023-07-24 13:26:27.000000 nanite-3.7.0/examples/fit_and_rate.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-24 13:26:27.000000 nanite-3.7.0/examples/fit_and_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-24 13:26:27.000000 nanite-3.7.0/examples/generate_example_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104455 2023-07-24 13:26:27.000000 nanite-3.7.0/examples/model_spherical_indenter.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-24 13:26:27.000000 nanite-3.7.0/examples/model_spherical_indenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.651730 nanite-3.7.0/nanite/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.651730 nanite-3.7.0/nanite/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/cli/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/cli/rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/indent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.655730 nanite-3.7.0/nanite/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/model_conical_indenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/model_hertz_paraboloidal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/model_hertz_three_sided_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/model_sneddon_spherical.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/model_sneddon_spherical_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/residuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/poc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/qmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.655730 nanite-3.7.0/nanite/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/rater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/regressors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.659730 nanite-3.7.0/nanite/rate/ts_zef18/
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_bin_apr_spikes_count.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_bin_cp_position.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_bin_size.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_apr_flatness.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_apr_size.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_apr_sum.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_bln_slope.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_bln_variation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_cp_curvature.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_cp_magnitude.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_maxima_75perc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_monotony.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_spike_area.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_sum.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_sum_75perc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.651730 nanite-3.7.0/nanite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-24 13:26:27.000000 nanite-3.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:26:43.675730 nanite-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-24 13:26:27.000000 nanite-3.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.663730 nanite-3.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.675730 nanite-3.7.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/cli-profile-1.7.8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/cli-profile-2.1.0.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    42815 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-afm-workshop-fd_single_2021-10-22_14.16.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68411 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-cl_calibration_force-save-2015-02-04.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)   158553 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)   497346 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_map-data-reference-points.jpk-force-map
+-rw-r--r--   0 runner    (1001) docker     (123)   407527 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_map0d_extracted.jpk-force-map
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1645418 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_map1d_2016-11-07.jpk-force-map
+-rw-r--r--   0 runner    (1001) docker     (123)   953060 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_map2x2_extracted.jpk-force-map
+-rw-r--r--   0 runner    (1001) docker     (123)   401583 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_1.jpk-force-map
+-rw-r--r--   0 runner    (1001) docker     (123)   400957 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map
+-rwxr-xr-x   0 runner    (1001) docker     (123)   193751 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_1.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   101264 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_2.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   101240 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   103538 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   101531 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   311042 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6785 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6783 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6799 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)   596184 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_tilted-baseline-drift-mitotic_2021-01-29.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)   188079 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_tilted-baseline-shift-adyp_2023-06-26.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_spot3-0192.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/model_external_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93520 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/rate-export_1.7.8.h5
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_cli_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_cli_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_cli_rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_fit_ancillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_fit_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_fit_emodulus_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_fit_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_fit_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_indent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_indent2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_hertz_cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_hertz_parabol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_hertz_pyramid_three.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_sneddon_spherical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_sneddon_spherical_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_sneddon_spherical_invert_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_open_jpk_variation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_poc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_qmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_rate_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_rate_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_rate_training_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_smooth.py
```

### Comparing `nanite-3.6.0/.gitignore` & `nanite-3.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/CHANGELOG` & `nanite-3.7.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+3.7.0
+ - feat: subtract linear slope from indentation curve (#22)
+ - ref: return normalization reference type for details from POC and preproc
+ - setup: bump scipy to 1.10.0 due to memory leak vulnerability
 3.6.0
  - tests: make tests less strict and some cleanup
  - setup: drop support for Python 3.8 and 3.9
  - setup: bump h5py from 2.8.0 to 3.9.0
  - build: migrate to pyproject.toml
  - ci: use cibuildwheel for releases
 3.5.4
```

### Comparing `nanite-3.6.0/LICENSE` & `nanite-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/PKG-INFO` & `nanite-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanite
-Version: 3.6.0
+Version: 3.7.0
 Summary: Loading, fitting, and rating AFM force-distance data
 Author: Paul Müller, Shada Abuhattum
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL version 3
 Project-URL: source, https://github.com/AFM-Analysis/nanite
 Project-URL: tracker, https://github.com/AFM-Analysis/nanite/issues
 Project-URL: documentation, https://nanite.readthedocs.io/en/stable/
```

### Comparing `nanite-3.6.0/README.rst` & `nanite-3.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/conf.py` & `nanite-3.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/data/force-save-example.jpk-force` & `nanite-3.7.0/docs/data/force-save-example.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/extensions/fancy_include.py` & `nanite-3.7.0/docs/extensions/fancy_include.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/extensions/github_changelog.py` & `nanite-3.7.0/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/extensions/nanite_models.py` & `nanite-3.7.0/docs/extensions/nanite_models.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/extensions/nanite_preprocs.py` & `nanite-3.7.0/docs/extensions/nanite_preprocs.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/extensions/simple_argparse.py` & `nanite-3.7.0/docs/extensions/simple_argparse.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/fitting_geometry.png` & `nanite-3.7.0/docs/fitting_geometry.png`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/fitting_geometry.svg` & `nanite-3.7.0/docs/fitting_geometry.svg`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/img/nanite-fit-example.png` & `nanite-3.7.0/docs/img/nanite-fit-example.png`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/img/nanite-rate-example.png` & `nanite-3.7.0/docs/img/nanite-rate-example.png`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/index.rst` & `nanite-3.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/nanite.bib` & `nanite-3.7.0/docs/nanite.bib`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/sec_cli.rst` & `nanite-3.7.0/docs/sec_cli.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/sec_code_reference.rst` & `nanite-3.7.0/docs/sec_code_reference.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/sec_develop.rst` & `nanite-3.7.0/docs/sec_develop.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/sec_fitting_guide.rst` & `nanite-3.7.0/docs/sec_fitting_guide.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/sec_getting_started.rst` & `nanite-3.7.0/docs/sec_getting_started.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/docs/sec_rating_workflow.rst` & `nanite-3.7.0/docs/sec_rating_workflow.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/examples/data/zebrafish-head-section-gray-matter.jpk-force` & `nanite-3.7.0/examples/data/zebrafish-head-section-gray-matter.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/examples/fit_and_rate.png` & `nanite-3.7.0/examples/fit_and_rate.png`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/examples/fit_and_rate.py` & `nanite-3.7.0/examples/fit_and_rate.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/examples/generate_example_images.py` & `nanite-3.7.0/examples/generate_example_images.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/examples/model_spherical_indenter.png` & `nanite-3.7.0/examples/model_spherical_indenter.png`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/examples/model_spherical_indenter.py` & `nanite-3.7.0/examples/model_spherical_indenter.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/cli/plotting.py` & `nanite-3.7.0/nanite/cli/plotting.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/cli/profile.py` & `nanite-3.7.0/nanite/cli/profile.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/cli/rating.py` & `nanite-3.7.0/nanite/cli/rating.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/fit.py` & `nanite-3.7.0/nanite/fit.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/group.py` & `nanite-3.7.0/nanite/group.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/indent.py` & `nanite-3.7.0/nanite/indent.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/model/__init__.py` & `nanite-3.7.0/nanite/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/model/core.py` & `nanite-3.7.0/nanite/model/core.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/model/logic.py` & `nanite-3.7.0/nanite/model/logic.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/model/model_conical_indenter.py` & `nanite-3.7.0/nanite/model/model_conical_indenter.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/model/model_hertz_paraboloidal.py` & `nanite-3.7.0/nanite/model/model_hertz_paraboloidal.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/model/model_hertz_three_sided_pyramid.py` & `nanite-3.7.0/nanite/model/model_hertz_three_sided_pyramid.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/model/model_sneddon_spherical.pyx` & `nanite-3.7.0/nanite/model/model_sneddon_spherical.pyx`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/model/model_sneddon_spherical_approximation.py` & `nanite-3.7.0/nanite/model/model_sneddon_spherical_approximation.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/model/residuals.py` & `nanite-3.7.0/nanite/model/residuals.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/poc.py` & `nanite-3.7.0/nanite/poc.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,14 +122,15 @@
             x = [0, force.size-1]
             details["plot force"] = [np.arange(force.size), force]
             details["plot baseline mean"] = [x, [bl_avg, bl_avg]]
             details["plot baseline threshold"] = [x, [bl_avg + bl_rng,
                                                       bl_avg + bl_rng]]
             details["plot poc"] = [[cp, cp],
                                    [force.min(), force.max()]]
+            details["norm"] = "force"
 
     if ret_details:
         return cp, details
     else:
         return cp
 
 
@@ -160,38 +161,41 @@
         one = d
         two = m * (x - x0) + d
         return np.maximum(one, two)
 
     def residual(params, x, data):
         return data - model(params, x)
 
-    y = np.array(force, copy=True)
     cp = np.nan
     details = {}
-    if y.size > 4:  # 3 fit parameters
-        ymin, ymax = np.min(y), np.max(y)
-        y = (y - ymin) / (ymax - ymin)
+    if force.size > 4:  # 3 fit parameters
+        # normalize force
+        fmin = np.min(force)
+        fptp = np.max(force) - fmin
+        y = (force - fmin) / fptp
         x = np.arange(y.size)
+        # get estimate for cp
         x0 = poc_frechet_direct_path(force)
         if np.isnan(x0):
             x0 = y.size // 2
         params = lmfit.Parameters()
         params.add('d', value=np.mean(y[:10]))
         params.add('x0', value=x0)
         params.add('m', value=(1 - y[x0])/(x.size - x0))
 
         out = lmfit.minimize(residual, params, args=(x, y), method="nelder")
         if out.success:
             cp = int(out.params["x0"])
             if ret_details:
-                details["plot force"] = [x, y]
+                details["plot force"] = [x, force]
                 details["plot fit"] = [np.arange(force.size),
-                                       model(out.params, x)]
+                                       model(out.params, x) * fptp + fmin]
                 details["plot poc"] = [[cp, cp],
-                                       [y.min(), y.max()]]
+                                       [fmin, fmin + fptp]]
+                details["norm"] = "force"
 
     if ret_details:
         return cp, details
     else:
         return cp
 
 
@@ -240,20 +244,20 @@
         curve[x1 <= 0] = d
         return curve
 
     def residual(params, x, data):
         curve = model(params, x)
         return data - curve
 
-    y = np.array(force, copy=True)
     cp = np.nan
     details = {}
-    if y.size > 6:  # 5 fit parameters
-        ymin, ymax = np.min(y), np.max(y)
-        y = (y - ymin) / (ymax - ymin)
+    if force.size > 6:  # 5 fit parameters
+        fmin = np.min(force)
+        fptp = np.max(force) - fmin
+        y = (force - fmin) / fptp
         x = np.arange(y.size)
         x0 = poc_frechet_direct_path(force)
         if np.isnan(x0):
             x0 = y.size // 2
         params = lmfit.Parameters()
         params.add('d', value=np.mean(y[:10]))
         params.add('x0', value=x0)
@@ -269,19 +273,20 @@
         params.add('c', value=.5, min=1e-3)
 
         out = lmfit.minimize(residual, params, args=(x, y), method="nelder")
 
         if out.success:
             cp = int(out.params["x0"])
             if ret_details:
-                details["plot force"] = [x, y]
+                details["plot force"] = [x, force]
                 details["plot fit"] = [np.arange(force.size),
-                                       model(out.params, x)]
+                                       model(out.params, x) * fptp + fmin]
                 details["plot poc"] = [[cp, cp],
-                                       [y.min(), y.max()]]
+                                       [fmin, fmin + fptp]]
+                details["norm"] = "force"
 
     if ret_details:
         return cp, details
     else:
         return cp
 
 
@@ -339,20 +344,20 @@
         curve[x1 > 0] += x1[x1 > 0]**3 / (a*x1[x1 > 0]**2 + b*x1[x1 > 0] + c)
         return curve
 
     def residual(params, x, data):
         curve = model(params, x)
         return data - curve
 
-    y = np.array(force, copy=True)
     cp = np.nan
     details = {}
-    if y.size > 7:  # 6 fit parameters
-        ymin, ymax = np.min(y), np.max(y)
-        y = (y - ymin) / (ymax - ymin)
+    if force.size > 7:  # 6 fit parameters
+        fmin = np.min(force)
+        fptp = np.max(force) - fmin
+        y = (force - fmin) / fptp
         x = np.arange(y.size)
         x0 = poc_frechet_direct_path(force)
         if np.isnan(x0):
             x0 = y.size // 2
         params = lmfit.Parameters()
         params.add('d', value=np.mean(y[:10]))
         params.add('x0', value=x0)
@@ -370,20 +375,20 @@
         params.add('c', value=.5, min=1e-3)
 
         out = lmfit.minimize(residual, params, args=(x, y), method="nelder")
 
         if out.success:
             cp = int(out.params["x0"])
             if ret_details:
-                details["plot force"] = [x, y]
+                details["plot force"] = [x, force]
                 details["plot fit"] = [np.arange(force.size),
-                                       model(out.params, x)]
+                                       model(out.params, x) * fptp + fmin]
                 details["plot poc"] = [[cp, cp],
-                                       [y.min(), y.max()]]
-                print(cp, y.min(), y.max())
+                                       [fmin, fmin + fptp]]
+                details["norm"] = "force"
 
     if ret_details:
         return cp, details
     else:
         return cp
 
 
@@ -415,15 +420,17 @@
     yr = x * np.sin(alpha) + y * np.cos(alpha)
     cp = np.argmin(yr)
 
     if ret_details:
         details = {"plot normalized rotated force": [np.arange(len(force)),
                                                      yr],
                    "plot poc": [[cp, cp],
-                                [yr.min(), yr.max()]]}
+                                [yr.min(), yr.max()]],
+                   "norm": "force-rotated",
+                   }
         return cp, details
     else:
         return cp
 
 
 @poc(identifier="gradient_zero_crossing",
      name="Gradient zero-crossing of indentation part",
@@ -460,18 +467,20 @@
                 # Weight with two times "filtsize//2", because we actually
                 # want the rolling median filter from the edge and not at the
                 # center of the array (and two times, because we did two
                 # filter operations).
                 cp = y.size - np.where(gradpos[::-1])[0][0] - cutoff + filtsize
 
                 if ret_details:
+                    # scale the gradient so that it aligns with the force
                     x = np.arange(gradn.size)
                     details["plot force gradient"] = [x, gradn]
                     details["plot threshold"] = [[x[0], x[-1]],
                                                  [thresh, thresh]]
                     details["plot poc"] = [[cp, cp],
                                            [gradn.min(), gradn.max()]]
+                    details["norm"] = "force-gradient"
 
     if ret_details:
         return cp, details
     else:
         return cp
```

### Comparing `nanite-3.6.0/nanite/preproc.py` & `nanite-3.7.0/nanite/preproc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 import inspect
 import functools
 import warnings
 
+import lmfit
 import numpy as np
 
 from . import poc
 from .smooth import smooth_axis_monotone
 
 
 #: Available preprocessors
@@ -122,14 +123,42 @@
                 if rr in identifiers:
                     rio.append(identifiers.index(rr))
             if np.any(np.array(rio) > cix):
                 raise ValueError(
                     f"Wrong optional step order for {pid}: {identifiers}!")
 
 
+def find_turning_point(tip_position, force, contact_point_index):
+    """Compute the turning point for a force-indentation curve
+
+    The turning point is defined as the point that is farthest away
+    from the contact point in the direction of indentation. This
+    implementation normalizes tip position according to their
+    minimum and maximum values. This is necessary, because they
+    live on different orders of magnitudes/units.
+    """
+    x = np.copy(tip_position)
+    y = np.copy(force)
+    idp = contact_point_index
+
+    # Flip and normalize tip position so that maximum is at minimum
+    # z-position (set to 1) which coincides with maximum indentation.
+    x -= x[idp]
+    x /= x.min()
+    x[x < 0] = 0
+
+    # Flip and normalize force so that maximum force is set to 1.
+    y -= np.average(y[:idp])
+    y /= y.max()
+    y[y < np.std(y[:idp])] = 0
+
+    idturn = np.argmax(x ** 2 + y ** 2)
+    return idturn
+
+
 def get_func(identifier):
     """Return preprocessor function for identifier"""
     for func in PREPROCESSORS:
         if func.identifier == identifier:
             return func
     else:
         raise KeyError(f"Preprocessor '{identifier}' unknown!")
@@ -225,26 +254,139 @@
         if not has_sc:
             missing.append("missing metadata 'spring constant'")
         mt = ", ".join(missing)
         raise ValueError("Cannot compute tip position: {}".format(mt))
 
 
 @preprocessing_step(identifier="correct_force_offset",
-                    name="baseline correction")
+                    name="baseline offset correction",
+                    steps_optional=["correct_force_slope"]
+                    )
 def preproc_correct_force_offset(apret):
     """Correct the force offset with an average baseline value
     """
     idp = poc.compute_poc(force=apret["force"],
                           method="deviation_from_baseline")
     if idp:
         apret["force"] = apret["force"] - np.average(apret["force"][:idp])
     else:
         apret["force"] = apret["force"] - apret["force"][0]
 
 
+@preprocessing_step(identifier="correct_force_slope",
+                    name="baseline slope correction",
+                    steps_required=["correct_tip_offset"],
+                    options=[
+                        {"name": "region",
+                         "type": str,
+                         "choices": ["baseline", "approach", "all"],
+                         "choices_human_readable": [
+                             "Correct up until contact point",
+                             "Correct the approach part",
+                             "Correct the entire dataset"],
+                         },
+                        {"name": "strategy",
+                         "type": str,
+                         "choices": ["drift", "shift"],
+                         "choices_human_readable": [
+                             "Temporal drift correction",
+                             "Spatial shift correction"]
+                         }
+                    ])
+def preproc_correct_force_slope(apret, region="baseline", strategy="shift",
+                                ret_details=False):
+    """Subtract a linear slope from selected parts of the force curve
+
+    Slope correction is a debatable topic in AFM analysis. Many voices
+    are of the opinion that this falsifies data and should not be done.
+    But when data are scarce, slope correction can help to extract valuable
+    information.
+
+    Slope correction uses the baseline (the part of the curve before the POC)
+    to determine the slope that should be subtracted from the data. Note
+    that for tilted data, you should use a contact point estimate based
+    on a line and a polynomial.
+
+    There are three regions for curve correction:
+
+    - baseline: Only the data leading up to the contact point are modified.
+      This has the advantage that indentation data are not modified, but the
+      baseline can still be used (as weight) in the fitting scheme.
+    - appraoch: The slope is subtracted from the entire approach curve.
+      This makes sense when you know that the slope affects baseline and
+      indentation part of your dataset.
+    - all: The entire dataset is corrected. This makes sense if you would
+      like to extract information about e.g. viscosity from the area between
+      the approach and retract curves of your dataset.
+
+    In addition, there are two strategies available:
+
+    - The "drift" approach assumes that the there is a global drift in the
+      dataset (caused e.g. by a thermal drift). Since these things are
+      usually of temporal nature, the correction in done over the time axis.
+      Use this if the beggining of the approach part and the end of the
+      retract part of your dataset "stick out" in opposite directions when
+      plotting force over tip position.
+    - The "shift" approach assumes that there is a global shift that is a
+      function of the distance between sample and cantilever. Use this if
+      the beginning of the approach part and the end of the retract part
+      align when plotting force over tip position.
+    """
+    tip_position = apret["tip position"]
+    time_position = apret["time"]
+    force = apret["force"]
+
+    # Get the current contact point position computed by "correct_tip_offset".
+    idp = np.argmin(np.abs(tip_position))
+    # Determine whether we want to do temporal or spatial correction:
+    # Fit a linear slope to the baseline part (all data up until idp)
+    mod = lmfit.models.LinearModel()
+    if strategy == "shift":
+        abscissa = tip_position
+    elif strategy == "drift":
+        abscissa = time_position
+    else:
+        raise ValueError(f"Invalid strategy '{strategy}'!")
+    pars = mod.guess(force[:idp], x=abscissa[:idp])
+    out = mod.fit(force[:idp], pars, x=abscissa[:idp])
+
+    force_edit = np.copy(force)
+    # Subtract the linear slope from the region data.
+    if region == "baseline":
+        # Only subtract the force from data up until the contact point.
+        # Make sure that there is no offset/jump by pulling the last
+        # element of the best fit array to zero.
+        force_edit[:idp] -= out.best_fit - out.best_fit[-1]
+    elif region == "approach":
+        # Subtract the force from everything that is part of the
+        # indentation part.
+        idturn = find_turning_point(tip_position=tip_position,
+                                    force=force_edit,
+                                    contact_point_index=idp)
+        # Extend the best fit towards the turning point.
+        best_fit_approach = mod.eval(out.params, x=abscissa[:idturn])
+        force_edit[:idturn] -= best_fit_approach - best_fit_approach[-1]
+    elif region == "all":
+        # Use the same approach as above, but subtract from the entire
+        # curve.
+        best_fit_all = mod.eval(out.params, x=abscissa)
+        force_edit -= best_fit_all - best_fit_all[idp]
+    else:
+        raise ValueError(f"Invalid region '{region}'!")
+
+    # Override the force information
+    apret["force"] = force_edit
+
+    if ret_details:
+        return {
+            "plot slope data": [np.arange(idp), force[:idp]],
+            "plot slope fit": [np.arange(idp), out.best_fit],
+            "norm": "force"}
+
+
 @preprocessing_step(
     identifier="correct_tip_offset",
     name="contact point estimation",
     steps_required=["compute_tip_position"],
     options=[
         {"name": "method",
          "type": str,
@@ -269,47 +411,41 @@
     apret["tip position"] = (apret["tip position"]
                              - apret["tip position"][cpid])
     return details
 
 
 @preprocessing_step(identifier="correct_split_approach_retract",
                     name="segment discovery",
-                    steps_required=["compute_tip_position"])
+                    steps_required=["compute_tip_position"],
+                    steps_optional=["correct_force_slope"],
+                    )
 def preproc_correct_split_approach_retract(apret):
     """Split the approach and retract curves (farthest point method)
 
     Approach and retract curves are defined by the microscope. When the
     direction of piezo movement is flipped, the force at the sample tip
     is still increasing. This can be either due to a time lag in the AFM
     system or due to a residual force acting on the sample due to the
     bent cantilever.
 
     To repair this time lag, we append parts of the retract curve to the
     approach curve, such that the curves are split at the minimum height.
     """
-    x = np.array(apret["tip position"], copy=True)
-    y = np.array(apret["force"], copy=True)
+    force = apret["force"]
 
-    idp = poc.poc_deviation_from_baseline(y)
+    idp = poc.poc_deviation_from_baseline(force)
     if idp and not np.isnan(idp):
-        # Flip and normalize tip position so that maximum is at minimum
-        # z-position (set to 1) which coincides with maximum indentation.
-        x -= x[idp]
-        x /= x.min()
-        x[x < 0] = 0
-
-        # Flip and normalize force so that maximum force is set to 1.
-        y -= np.average(y[:idp])
-        y /= y.max()
-        y[y < np.std(y[:idp])] = 0
-
-        idmin = np.argmax(x ** 2 + y ** 2)
+        idturn = find_turning_point(
+            tip_position=apret["tip position"],
+            force=force,
+            contact_point_index=idp,
+        )
 
         segment = np.zeros(len(apret), dtype=np.uint8)
-        segment[idmin:] = 1
+        segment[idturn:] = 1
         apret["segment"] = segment
     else:
         msg = "Cannot correct splitting of approach and retract curve " + \
               "because the contact point position could not be estimated."
         warnings.warn(msg, CannotSplitWarning)
 
 
@@ -317,15 +453,18 @@
                     name="monotonic height data",
                     steps_optional=[
                         # Otherwise we lose the location of the point
                         # of deepest indentation:
                         "correct_split_approach_retract",
                         # Otherwise it might not be applied to
                         # "tip position":
-                        "compute_tip_position"])
+                        "compute_tip_position",
+                        # Slope subtraction should happen first:
+                        "correct_force_slope"
+                        ])
 def preproc_smooth_height(apret):
     """Make height data monotonic
 
     For the columns "height (measured)", "height (piezo), and
     "tip position", this method ensures that the approach and
     retract segments are monotonic.
     """
```

### Comparing `nanite-3.6.0/nanite/qmap.py` & `nanite-3.7.0/nanite/qmap.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/features.py` & `nanite-3.7.0/nanite/rate/features.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/io.py` & `nanite-3.7.0/nanite/rate/io.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/rater.py` & `nanite-3.7.0/nanite/rate/rater.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/regressors.py` & `nanite-3.7.0/nanite/rate/regressors.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_apr_flatness.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_apr_flatness.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_apr_size.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_apr_size.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_apr_sum.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_apr_sum.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_bln_slope.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_bln_slope.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_bln_variation.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_bln_variation.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_cp_curvature.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_cp_curvature.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_cp_magnitude.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_cp_magnitude.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_maxima_75perc.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_maxima_75perc.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_monotony.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_monotony.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_spike_area.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_spike_area.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_sum.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_sum.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_sum_75perc.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_sum_75perc.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/rate/ts_zef18/train_response.txt` & `nanite-3.7.0/nanite/rate/ts_zef18/train_response.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/read.py` & `nanite-3.7.0/nanite/read.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite/smooth.py` & `nanite-3.7.0/nanite/smooth.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/nanite.egg-info/PKG-INFO` & `nanite-3.7.0/nanite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanite
-Version: 3.6.0
+Version: 3.7.0
 Summary: Loading, fitting, and rating AFM force-distance data
 Author: Paul Müller, Shada Abuhattum
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL version 3
 Project-URL: source, https://github.com/AFM-Analysis/nanite
 Project-URL: tracker, https://github.com/AFM-Analysis/nanite/issues
 Project-URL: documentation, https://nanite.readthedocs.io/en/stable/
```

### Comparing `nanite-3.6.0/nanite.egg-info/SOURCES.txt` & `nanite-3.7.0/nanite.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -137,11 +137,12 @@
 tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force
 tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force
 tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force
 tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force
 tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force
 tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force
 tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force
-tests/data/fmt-jpk-fd_single_tilted-baseline-mitotic_2021-01-29.jpk-force
+tests/data/fmt-jpk-fd_single_tilted-baseline-drift-mitotic_2021-01-29.jpk-force
+tests/data/fmt-jpk-fd_single_tilted-baseline-shift-adyp_2023-06-26.jpk-force
 tests/data/fmt-jpk-fd_spot3-0192.jpk-force
 tests/data/model_external_basic.py
 tests/data/rate-export_1.7.8.h5
```

### Comparing `nanite-3.6.0/pyproject.toml` & `nanite-3.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 license = {text = "GPL version 3"}
 dependencies = [
     "afmformats>=0.16.4",
     "h5py>=3.9.0",
     "lmfit>=1",
     "numpy>=1.22.0",  # cython build
     "scikit-learn>=0.23.0",  # rating tests
-    "scipy",
+    "scipy>=1.10.0",  # scipy memory leak vulnerability
   ]
 dynamic = ["version"]
 [project.optional-dependencies]
 CLI = ["appdirs",
        "matplotlib>=2.2.2",
        "tifffile>=0.15.0",
     ]
```

### Comparing `nanite-3.6.0/tests/common.py` & `nanite-3.7.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/conftest.py` & `nanite-3.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-afm-workshop-fd_single_2021-10-22_14.16.csv` & `nanite-3.7.0/tests/data/fmt-afm-workshop-fd_single_2021-10-22_14.16.csv`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-cl_calibration_force-save-2015-02-04.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-cl_calibration_force-save-2015-02-04.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_map-data-reference-points.jpk-force-map` & `nanite-3.7.0/tests/data/fmt-jpk-fd_map-data-reference-points.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_map0d_extracted.jpk-force-map` & `nanite-3.7.0/tests/data/fmt-jpk-fd_map0d_extracted.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_map1d_2016-11-07.jpk-force-map` & `nanite-3.7.0/tests/data/fmt-jpk-fd_map1d_2016-11-07.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_map2x2_extracted.jpk-force-map` & `nanite-3.7.0/tests/data/fmt-jpk-fd_map2x2_extracted.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_1.jpk-force-map` & `nanite-3.7.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_1.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map` & `nanite-3.7.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_1.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_1.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_2.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_2.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_single_tilted-baseline-mitotic_2021-01-29.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-fd_single_tilted-baseline-drift-mitotic_2021-01-29.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/fmt-jpk-fd_spot3-0192.jpk-force` & `nanite-3.7.0/tests/data/fmt-jpk-fd_spot3-0192.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/model_external_basic.py` & `nanite-3.7.0/tests/data/model_external_basic.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/data/rate-export_1.7.8.h5` & `nanite-3.7.0/tests/data/rate-export_1.7.8.h5`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_cli_plotting.py` & `nanite-3.7.0/tests/test_cli_plotting.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_cli_profile.py` & `nanite-3.7.0/tests/test_cli_profile.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_cli_rating.py` & `nanite-3.7.0/tests/test_cli_rating.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_fit_ancillary.py` & `nanite-3.7.0/tests/test_fit_ancillary.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_fit_base.py` & `nanite-3.7.0/tests/test_fit_base.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_fit_emodulus_search.py` & `nanite-3.7.0/tests/test_fit_emodulus_search.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_fit_hash.py` & `nanite-3.7.0/tests/test_fit_hash.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_fit_properties.py` & `nanite-3.7.0/tests/test_fit_properties.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_group.py` & `nanite-3.7.0/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_indent.py` & `nanite-3.7.0/tests/test_indent.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_indent2.py` & `nanite-3.7.0/tests/test_indent2.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_model.py` & `nanite-3.7.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_model_core.py` & `nanite-3.7.0/tests/test_model_core.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_model_expr.py` & `nanite-3.7.0/tests/test_model_expr.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_model_hertz_cone.py` & `nanite-3.7.0/tests/test_model_hertz_cone.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_model_hertz_parabol.py` & `nanite-3.7.0/tests/test_model_hertz_parabol.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_model_hertz_pyramid_three.py` & `nanite-3.7.0/tests/test_model_hertz_pyramid_three.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_model_logic.py` & `nanite-3.7.0/tests/test_model_logic.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_model_sneddon_spherical.py` & `nanite-3.7.0/tests/test_model_sneddon_spherical.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_model_sneddon_spherical_approximation.py` & `nanite-3.7.0/tests/test_model_sneddon_spherical_approximation.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_model_style.py` & `nanite-3.7.0/tests/test_model_style.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_open_jpk_variation.py` & `nanite-3.7.0/tests/test_open_jpk_variation.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_poc.py` & `nanite-3.7.0/tests/test_poc.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,16 @@
         -7.573822405258677e-12,
         atol=0)
 
 
 def test_poc_details_fit_line_polynomial():
     fd = IndentationGroup(
         data_path
-        / "fmt-jpk-fd_single_tilted-baseline-mitotic_2021-01-29.jpk-force")[0]
+        / "fmt-jpk-fd_single_tilted-baseline-drift-"
+          "mitotic_2021-01-29.jpk-force")[0]
     details = fd.apply_preprocessing(
         ["compute_tip_position", "correct_tip_offset"],
         options={"correct_tip_offset": {"method": "fit_line_polynomial"}},
         ret_details=True)
     pocd = details["correct_tip_offset"]
     for key in ["plot force",
                 "plot fit",
```

### Comparing `nanite-3.6.0/tests/test_qmap.py` & `nanite-3.7.0/tests/test_qmap.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_rate_features.py` & `nanite-3.7.0/tests/test_rate_features.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_rate_io.py` & `nanite-3.7.0/tests/test_rate_io.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_rate_training_set.py` & `nanite-3.7.0/tests/test_rate_training_set.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_read.py` & `nanite-3.7.0/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `nanite-3.6.0/tests/test_smooth.py` & `nanite-3.7.0/tests/test_smooth.py`

 * *Files identical despite different names*

