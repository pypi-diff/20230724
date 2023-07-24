# Comparing `tmp/plottoolbox-104.3.0.tar.gz` & `tmp/plottoolbox-104.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plottoolbox-104.3.0.tar", last modified: Fri May 12 04:06:22 2023, max compression
+gzip compressed data, was "plottoolbox-104.3.1.tar", last modified: Mon Jul 24 04:52:30 2023, max compression
```

## Comparing `plottoolbox-104.3.0.tar` & `plottoolbox-104.3.1.tar`

### file list

```diff
@@ -1,305 +1,306 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.135568 plottoolbox-104.3.0/
--rw-rw-r--   0 tim       (1000) tim       (1000)      102 2023-05-01 05:47:35.000000 plottoolbox-104.3.0/.deepsource.toml
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.059570 plottoolbox-104.3.0/.github/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.063570 plottoolbox-104.3.0/.github/workflows/
--rw-rw-r--   0 tim       (1000) tim       (1000)      505 2023-05-01 05:47:35.000000 plottoolbox-104.3.0/.github/workflows/clean-workflow-runs.yml
--rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-05-01 05:47:35.000000 plottoolbox-104.3.0/.github/workflows/python-package.yml
--rw-r--r--   0 tim       (1000) tim       (1000)      341 2023-03-05 18:49:44.000000 plottoolbox-104.3.0/.gitignore
--rw-rw-r--   0 tim       (1000) tim       (1000)      381 2023-03-26 20:12:03.000000 plottoolbox-104.3.0/.gitmodules
--rw-r--r--   0 tim       (1000) tim       (1000)       74 2020-09-26 07:35:12.000000 plottoolbox-104.3.0/.hgignore
--rw-rw-r--   0 tim       (1000) tim       (1000)     2736 2023-05-11 22:26:46.000000 plottoolbox-104.3.0/.pre-commit-config.yaml
--rw-r--r--   0 tim       (1000) tim       (1000)       50 2020-09-26 07:35:40.000000 plottoolbox-104.3.0/AUTHORS.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1038 2022-09-28 02:46:31.000000 plottoolbox-104.3.0/BADGES.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     2305 2023-05-12 03:55:34.000000 plottoolbox-104.3.0/CHANGELOG.md
--rw-r--r--   0 tim       (1000) tim       (1000)     3179 2021-06-20 01:30:38.000000 plottoolbox-104.3.0/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1488 2020-09-26 07:36:10.000000 plottoolbox-104.3.0/LICENSE.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      377 2023-03-14 12:58:47.000000 plottoolbox-104.3.0/MANIFEST.in
--rw-rw-r--   0 tim       (1000) tim       (1000)     6486 2023-05-12 04:06:22.135568 plottoolbox-104.3.0/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     5086 2022-09-30 03:05:15.000000 plottoolbox-104.3.0/README.rst
--rw-r--r--   0 tim       (1000) tim       (1000)        8 2023-05-12 03:55:34.000000 plottoolbox-104.3.0/VERSION
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.067570 plottoolbox-104.3.0/docs/
--rw-r--r--   0 tim       (1000) tim       (1000)     5712 2020-10-10 00:42:42.000000 plottoolbox-104.3.0/docs/Makefile
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.071570 plottoolbox-104.3.0/docs/_function_autosummary/
--rw-rw-r--   0 tim       (1000) tim       (1000)      131 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.about.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      161 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.autocorrelation.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      125 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.bar.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      151 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.bar_stacked.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      128 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.barh.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      154 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.barh_stacked.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      143 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.bootstrap.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      137 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.boxplot.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      151 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.double_mass.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      131 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.handh.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      137 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.heatmap.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      134 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.hexbin.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      143 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.histogram.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      125 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.kde.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      142 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.kde_time.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      142 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.lag_plot.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      157 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.lognorm_xaxis.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      157 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.lognorm_yaxis.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      148 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.norm_xaxis.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      148 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.norm_yaxis.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      175 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.probability_density.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      160 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.scatter_matrix.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      134 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.target.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      134 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.taylor.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      128 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.time.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      157 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.weibull_xaxis.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      157 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.weibull_yaxis.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      122 2023-04-30 02:55:55.000000 plottoolbox-104.3.0/docs/_function_autosummary/plottoolbox.plottoolbox.xy.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       55 2021-06-20 01:30:38.000000 plottoolbox-104.3.0/docs/authors.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     2446 2023-05-11 22:26:17.000000 plottoolbox-104.3.0/docs/command_line.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     9595 2023-01-22 03:38:20.000000 plottoolbox-104.3.0/docs/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)       60 2020-10-10 00:42:42.000000 plottoolbox-104.3.0/docs/contributing.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     1235 2023-05-03 00:50:09.000000 plottoolbox-104.3.0/docs/function_summary.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      450 2021-07-21 21:07:34.000000 plottoolbox-104.3.0/docs/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       79 2020-10-10 00:42:42.000000 plottoolbox-104.3.0/docs/license.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2021-12-16 18:37:10.000000 plottoolbox-104.3.0/docs/make.bat
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2021-06-20 01:30:38.000000 plottoolbox-104.3.0/docs/readme.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     2694 2023-05-12 03:55:35.000000 plottoolbox-104.3.0/pyproject.toml
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2020-09-26 07:36:10.000000 plottoolbox-104.3.0/pytest.ini
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-05-12 04:06:22.135568 plottoolbox-104.3.0/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      458 2023-03-01 15:41:43.000000 plottoolbox-104.3.0/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.059570 plottoolbox-104.3.0/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.075569 plottoolbox-104.3.0/src/plottoolbox/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.075569 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.075569 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/examples/
--rw-rw-r--   0 tim       (1000) tim       (1000)     9105 2023-03-12 15:02:27.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/examples/plot-examples.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.075569 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/
--rw-rw-r--   0 tim       (1000) tim       (1000)      958 2023-03-14 13:38:10.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/__init__.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.075569 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.079569 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/color/
--rw-rw-r--   0 tim       (1000) tim       (1000)      226 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/color/bright.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      193 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/color/high-contrast.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      237 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/color/high-vis.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      245 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/color/light.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      255 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/color/muted.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      135 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/color/retro.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      201 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/color/std-colors.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      227 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/color/vibrant.mplstyle
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.079569 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/journals/
--rw-rw-r--   0 tim       (1000) tim       (1000)      393 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/journals/ieee.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      906 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/journals/nature.mplstyle
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.079569 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/languages/
--rw-rw-r--   0 tim       (1000) tim       (1000)      144 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/languages/cjk-jp-font.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      142 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/languages/cjk-kr-font.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      154 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/languages/cjk-sc-font.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      155 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/languages/cjk-tc-font.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      197 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/languages/russian-font.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      224 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/languages/turkish-font.mplstyle
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.079569 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/misc/
--rw-rw-r--   0 tim       (1000) tim       (1000)      272 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/misc/grid.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      378 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/misc/latex-sans.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)       40 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/misc/no-latex.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      130 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/misc/pgf.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      364 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/misc/sans.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      643 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/notebook.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)      333 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/scatter.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)     1110 2023-03-08 03:08:47.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/science.mplstyle
--rw-rw-r--   0 tim       (1000) tim       (1000)     1348 2023-03-12 15:02:27.000000 plottoolbox-104.3.0/src/plottoolbox/SciencePlots/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.059570 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.087569 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/
--rw-rw-r--   0 tim       (1000) tim       (1000)     4674 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/Farmington_River_data.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5567 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/all_stats.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6386 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/convertMatFile.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5095 2023-03-14 13:39:52.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/get_time_series.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     4490 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/load_data.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2209 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/read_csv_data.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4177 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target1.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6106 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target10.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4275 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target2.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4654 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target3.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4791 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target4.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5152 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target5.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5248 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target6.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5615 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target7.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5673 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target8.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     8556 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target9.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      592 2023-03-14 13:39:52.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target_options.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5206 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor1.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5727 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor10.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4164 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor11.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5340 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor12.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6409 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor13.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    10510 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor14.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4998 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor2.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5253 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor3.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5690 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor4.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5765 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor5.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5704 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor6.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5811 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor7.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6634 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor8.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6465 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor9.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      592 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor_options.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.087569 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Test/
--rw-rw-r--   0 tim       (1000) tim       (1000)    10754 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Test/test_plots.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.099569 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1877 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/__init__.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     4527 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/add_legend.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      784 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/bias.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1679 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/brier_score.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1115 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/centered_rms_dev.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1837 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/check_duplicate_stats.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      980 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/check_on_off.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1821 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/check_taylor_stats.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3114 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/error_check_stats.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1760 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/get_axis_tick_label.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     1216 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/get_from_dict_or_default.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6092 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/get_target_diagram_axes.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    16209 2023-03-18 01:42:37.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/get_target_diagram_options.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2550 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/get_taylor_diagram_axes.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    21862 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/get_taylor_diagram_options.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3279 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/kling_gupta_eff09.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3324 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/kling_gupta_eff12.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2188 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/nash_sutcliffe_eff.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2815 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/overlay_target_diagram_circles.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     5211 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/overlay_taylor_diagram_circles.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3141 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/overlay_taylor_diagram_lines.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7970 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/plot_pattern_diagram_colorbar.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     7105 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/plot_pattern_diagram_markers.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3396 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/plot_target_axes.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)    11728 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/plot_taylor_axes.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2796 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/plot_taylor_obs.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      617 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/report_duplicate_stats.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      963 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/rmsd.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      925 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/save_figures.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1751 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/skill_score_brier.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1611 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/skill_score_murphy.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     9464 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/target_diagram.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2559 2023-03-18 01:29:59.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/target_statistics.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    13609 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/taylor_diagram.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2569 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/taylor_statistics.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      455 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/use_sci_notation.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      880 2023-03-14 13:39:53.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/utils.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4264 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/write_stats.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5316 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/write_target_stats.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5231 2023-03-14 13:39:58.000000 plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/write_taylor_stats.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1910 2023-03-26 22:07:58.000000 plottoolbox-104.3.0/src/plottoolbox/__init__.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.103569 plottoolbox-104.3.0/src/plottoolbox/_functions/
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2023-01-23 20:56:50.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3438 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/autocorrelation.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7190 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/bar.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7244 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/bar_stacked.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7080 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/barh.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7102 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/barh_stacked.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5041 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/bootstrap.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4944 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/boxplot.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6742 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/double_mass.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4968 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/handh.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5983 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/heatmap.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4472 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/hexbin.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5034 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/histogram.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5842 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/kde.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7182 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/kde_time.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5185 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/lag_plot.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7750 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/lognorm_xaxis.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7716 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/lognorm_yaxis.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7643 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/norm_xaxis.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7696 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/norm_yaxis.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5660 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/probability_density.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5107 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/scatter_matrix.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4405 2023-05-11 22:53:05.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/target.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3864 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/taylor.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5879 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/time.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5095 2023-05-11 22:26:18.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/waterfall.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7589 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/weibull_xaxis.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7693 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/weibull_yaxis.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7537 2023-05-12 03:44:04.000000 plottoolbox-104.3.0/src/plottoolbox/_functions/xy.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    27577 2023-05-02 00:24:02.000000 plottoolbox-104.3.0/src/plottoolbox/_plotutils.py
--rw-r--r--   0 tim       (1000) tim       (1000)    72738 2023-03-26 22:10:15.000000 plottoolbox-104.3.0/src/plottoolbox/plottoolbox.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.103569 plottoolbox-104.3.0/src/plottoolbox/waterfall_ax/
--rw-rw-r--   0 tim       (1000) tim       (1000)      657 2023-03-26 22:10:22.000000 plottoolbox-104.3.0/src/plottoolbox/waterfall_ax/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.103569 plottoolbox-104.3.0/src/plottoolbox/waterfall_ax/waterfall_ax/
--rw-rw-r--   0 tim       (1000) tim       (1000)       41 2023-03-26 22:10:22.000000 plottoolbox-104.3.0/src/plottoolbox/waterfall_ax/waterfall_ax/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    10001 2023-04-03 02:20:00.000000 plottoolbox-104.3.0/src/plottoolbox/waterfall_ax/waterfall_ax/waterfall_ax.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.075569 plottoolbox-104.3.0/src/plottoolbox.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     6486 2023-05-12 04:06:21.000000 plottoolbox-104.3.0/src/plottoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)    12747 2023-05-12 04:06:22.000000 plottoolbox-104.3.0/src/plottoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-05-12 04:06:21.000000 plottoolbox-104.3.0/src/plottoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       62 2023-05-12 04:06:21.000000 plottoolbox-104.3.0/src/plottoolbox.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      236 2023-05-12 04:06:21.000000 plottoolbox-104.3.0/src/plottoolbox.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       12 2023-05-12 04:06:21.000000 plottoolbox-104.3.0/src/plottoolbox.egg-info/top_level.txt
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.127568 plottoolbox-104.3.0/tests/
--rw-r--r--   0 tim       (1000) tim       (1000)  5411566 2021-03-19 23:27:40.000000 plottoolbox-104.3.0/tests/02234500_65_65.csv
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2023-01-22 03:38:20.000000 plottoolbox-104.3.0/tests/__init__.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-05-12 04:06:22.135568 plottoolbox-104.3.0/tests/baseline/
--rw-r--r--   0 tim       (1000) tim       (1000)    37406 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_autocorrelation.png
--rw-r--r--   0 tim       (1000) tim       (1000)    31916 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_bar.png
--rw-r--r--   0 tim       (1000) tim       (1000)    35045 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_bar_stacked.png
--rw-r--r--   0 tim       (1000) tim       (1000)    30663 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_barh.png
--rw-r--r--   0 tim       (1000) tim       (1000)    34581 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_barh_stacked.png
--rw-r--r--   0 tim       (1000) tim       (1000)    24015 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_boxplot.png
--rw-r--r--   0 tim       (1000) tim       (1000)    30921 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_double_mass.png
--rw-r--r--   0 tim       (1000) tim       (1000)    36999 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_double_mass_marker.png
--rw-r--r--   0 tim       (1000) tim       (1000)    42100 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_double_mass_mult.png
--rw-r--r--   0 tim       (1000) tim       (1000)   150426 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_heatmap.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    72201 2023-03-01 21:16:24.000000 plottoolbox-104.3.0/tests/baseline/test_hexbin.png
--rw-r--r--   0 tim       (1000) tim       (1000)    33878 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_histogram.png
--rw-r--r--   0 tim       (1000) tim       (1000)    58166 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_kde_time.png
--rw-r--r--   0 tim       (1000) tim       (1000)    64489 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_kde_time_multiple_traces.png
--rw-r--r--   0 tim       (1000) tim       (1000)    33169 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_lag_plot.png
--rw-r--r--   0 tim       (1000) tim       (1000)    30939 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_lognorm_xaxis.png
--rw-r--r--   0 tim       (1000) tim       (1000)    28815 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_lognorm_yaxis.png
--rw-r--r--   0 tim       (1000) tim       (1000)    31655 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_norm_xaxis.png
--rw-r--r--   0 tim       (1000) tim       (1000)    28921 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_norm_yaxis.png
--rw-r--r--   0 tim       (1000) tim       (1000)    23921 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_probability_density.png
--rw-r--r--   0 tim       (1000) tim       (1000)    87625 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_scatter_matrix.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    41249 2023-03-18 01:43:59.000000 plottoolbox-104.3.0/tests/baseline/test_target.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    82456 2023-03-13 02:41:16.000000 plottoolbox-104.3.0/tests/baseline/test_taylor.png
--rw-r--r--   0 tim       (1000) tim       (1000)    39301 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_time_markers.png
--rw-r--r--   0 tim       (1000) tim       (1000)   112833 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_time_multiple_traces_new_style_plot.png
--rw-r--r--   0 tim       (1000) tim       (1000)   112134 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_time_multiple_traces_plot.png
--rw-r--r--   0 tim       (1000) tim       (1000)    58721 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_time_multiple_traces_style_plot.png
--rw-r--r--   0 tim       (1000) tim       (1000)    50929 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_time_plot.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    32889 2023-05-12 03:34:58.000000 plottoolbox-104.3.0/tests/baseline/test_waterfall.png
--rw-r--r--   0 tim       (1000) tim       (1000)    32214 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_weibull_xaxis.png
--rw-r--r--   0 tim       (1000) tim       (1000)    29194 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_weibull_yaxis.png
--rw-r--r--   0 tim       (1000) tim       (1000)    87205 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_xy.png
--rw-r--r--   0 tim       (1000) tim       (1000)    46025 2022-07-18 15:27:42.000000 plottoolbox-104.3.0/tests/baseline/test_xy_multiple_traces.png
--rw-r--r--   0 tim       (1000) tim       (1000)    71428 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_xy_multiple_traces_logx.png
--rw-r--r--   0 tim       (1000) tim       (1000)    77455 2022-07-18 15:28:12.000000 plottoolbox-104.3.0/tests/baseline/test_xy_multiple_traces_logy.png
--rw-r--r--   0 tim       (1000) tim       (1000)    37598 2020-09-26 07:35:10.000000 plottoolbox-104.3.0/tests/baseline/test_xy_multiple_traces_markers.png
--rw-r--r--   0 tim       (1000) tim       (1000)      394 2023-01-22 03:38:20.000000 plottoolbox-104.3.0/tests/capture.py
--rw-r--r--   0 tim       (1000) tim       (1000)    40960 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data.wdm
--rw-r--r--   0 tim       (1000) tim       (1000)    89620 2022-07-18 00:44:27.000000 plottoolbox-104.3.0/tests/data_02325000_flow.csv
--rw-r--r--   0 tim       (1000) tim       (1000)       84 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_bi_daily.csv
--rw-r--r--   0 tim       (1000) tim       (1000)    75863 2022-07-18 00:42:28.000000 plottoolbox-104.3.0/tests/data_daily.csv
--rw-r--r--   0 tim       (1000) tim       (1000)   122972 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_daily_sample.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      829 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_dirty_index.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      188 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_empty_cols.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      241 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_fill_from.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      697 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_filter_fft_lowpass.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      825 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_filter_flat.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      862 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_filter_hanning.csv
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_filter_transform.csv
--rw-r--r--   0 tim       (1000) tim       (1000)     1164 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_flat.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      611 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_flat_01.csv
--rw-r--r--   0 tim       (1000) tim       (1000)   549278 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_flow_stage.xlsx
--rw-r--r--   0 tim       (1000) tim       (1000)   172784 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_gainesville_daily_precip.csv
--rw-r--r--   0 tim       (1000) tim       (1000)   120195 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_gainesville_daily_precip_index.csv
--rw-r--r--   0 tim       (1000) tim       (1000)  9677288 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_gainesville_hourly_precip.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      463 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_missing.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      149 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_multiple_cols.csv
--rw-r--r--   0 tim       (1000) tim       (1000)     1189 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_read_append.csv
--rw-r--r--   0 tim       (1000) tim       (1000)     1165 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_read_append_header.csv
--rw-r--r--   0 tim       (1000) tim       (1000)     1515 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_read_append_header_cols.csv
--rw-r--r--   0 tim       (1000) tim       (1000)     1165 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_read_append_header_duplicate.csv
--rw-r--r--   0 tim       (1000) tim       (1000)       44 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_simple.csv
--rw-r--r--   0 tim       (1000) tim       (1000)       81 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_simple_extra_rows.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      140 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_simple_extra_rows_sparse.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      684 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_sine.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      209 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_spaces.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      141 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_stacked.csv
--rw-r--r--   0 tim       (1000) tim       (1000)      183 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_stacked_1.csv
--rw-r--r--   0 tim       (1000) tim       (1000)    30254 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_sunspot.csv
--rw-r--r--   0 tim       (1000) tim       (1000)    53259 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_sunspot_EST.csv
--rw-r--r--   0 tim       (1000) tim       (1000)    17446 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_sunspot_index.csv
--rw-r--r--   0 tim       (1000) tim       (1000)    34163 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_sunspot_normalized_0_to_1.csv
--rw-r--r--   0 tim       (1000) tim       (1000)    31517 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_sunspot_normalized_10_to_20.csv
--rw-r--r--   0 tim       (1000) tim       (1000)    36205 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_sunspot_normalized_pct_rank.csv
--rw-r--r--   0 tim       (1000) tim       (1000)    36871 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_sunspot_normalized_zscore.csv
--rw-r--r--   0 tim       (1000) tim       (1000)       91 2021-06-29 23:02:12.000000 plottoolbox-104.3.0/tests/data_unstacked.csv
--rw-r--r--   0 tim       (1000) tim       (1000)     3488 2023-03-01 04:59:34.000000 plottoolbox-104.3.0/tests/test_plot_1.py
--rw-r--r--   0 tim       (1000) tim       (1000)     3557 2023-01-22 03:38:20.000000 plottoolbox-104.3.0/tests/test_plot_2.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4410 2023-03-27 02:30:00.000000 plottoolbox-104.3.0/tests/test_plot_3.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.257004 plottoolbox-104.3.1/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      102 2023-06-17 22:11:59.000000 plottoolbox-104.3.1/.deepsource.toml
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.217003 plottoolbox-104.3.1/.github/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.221003 plottoolbox-104.3.1/.github/workflows/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      501 2023-06-17 22:11:59.000000 plottoolbox-104.3.1/.github/workflows/clean-workflow-runs.yml
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-06-17 22:11:59.000000 plottoolbox-104.3.1/.github/workflows/python-package.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)      341 2023-03-05 18:49:44.000000 plottoolbox-104.3.1/.gitignore
+-rw-rw-r--   0 tim       (1000) tim       (1000)      381 2023-03-26 20:12:03.000000 plottoolbox-104.3.1/.gitmodules
+-rw-r--r--   0 tim       (1000) tim       (1000)       74 2020-09-26 07:35:12.000000 plottoolbox-104.3.1/.hgignore
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2651 2023-07-24 04:27:51.000000 plottoolbox-104.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 tim       (1000) tim       (1000)       50 2020-09-26 07:35:40.000000 plottoolbox-104.3.1/AUTHORS.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1038 2022-09-28 02:46:31.000000 plottoolbox-104.3.1/BADGES.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     2386 2023-07-24 04:52:20.000000 plottoolbox-104.3.1/CHANGELOG.md
+-rw-r--r--   0 tim       (1000) tim       (1000)     3179 2021-06-20 01:30:38.000000 plottoolbox-104.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1488 2020-09-26 07:36:10.000000 plottoolbox-104.3.1/LICENSE.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      377 2023-03-14 12:58:47.000000 plottoolbox-104.3.1/MANIFEST.in
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6351 2023-07-24 04:52:30.257004 plottoolbox-104.3.1/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4951 2023-06-10 05:29:49.000000 plottoolbox-104.3.1/README.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)        8 2023-07-24 04:52:20.000000 plottoolbox-104.3.1/VERSION
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.221003 plottoolbox-104.3.1/docs/
+-rw-r--r--   0 tim       (1000) tim       (1000)     5712 2020-10-10 00:42:42.000000 plottoolbox-104.3.1/docs/Makefile
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.225003 plottoolbox-104.3.1/docs/_function_autosummary/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      131 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.about.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      161 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.autocorrelation.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      125 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.bar.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      151 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.bar_stacked.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      128 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.barh.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      154 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.barh_stacked.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      143 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.bootstrap.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      137 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.boxplot.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      151 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.double_mass.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      131 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.handh.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      137 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.heatmap.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      134 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.hexbin.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      143 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.histogram.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      125 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.kde.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      142 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.kde_time.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      142 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.lag_plot.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      157 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.lognorm_xaxis.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      157 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.lognorm_yaxis.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      148 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.norm_xaxis.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      148 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.norm_yaxis.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      175 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.probability_density.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      160 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.scatter_matrix.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      134 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.target.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      134 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.taylor.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      128 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.time.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      143 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.waterfall.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      157 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.weibull_xaxis.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      157 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.weibull_yaxis.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      122 2023-06-19 14:23:38.000000 plottoolbox-104.3.1/docs/_function_autosummary/plottoolbox.plottoolbox.xy.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       55 2021-06-20 01:30:38.000000 plottoolbox-104.3.1/docs/authors.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2446 2023-05-13 04:19:53.000000 plottoolbox-104.3.1/docs/command_line.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     9595 2023-01-22 03:38:20.000000 plottoolbox-104.3.1/docs/conf.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       60 2020-10-10 00:42:42.000000 plottoolbox-104.3.1/docs/contributing.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1235 2023-05-13 04:12:35.000000 plottoolbox-104.3.1/docs/function_summary.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      450 2021-07-21 21:07:34.000000 plottoolbox-104.3.1/docs/index.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       79 2020-10-10 00:42:42.000000 plottoolbox-104.3.1/docs/license.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2021-12-16 18:37:10.000000 plottoolbox-104.3.1/docs/make.bat
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2021-06-20 01:30:38.000000 plottoolbox-104.3.1/docs/readme.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2712 2023-07-24 04:52:21.000000 plottoolbox-104.3.1/pyproject.toml
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2020-09-26 07:36:10.000000 plottoolbox-104.3.1/pytest.ini
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-07-24 04:52:30.257004 plottoolbox-104.3.1/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      458 2023-03-01 15:41:43.000000 plottoolbox-104.3.1/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.217003 plottoolbox-104.3.1/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.225003 plottoolbox-104.3.1/src/plottoolbox/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.225003 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.225003 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/examples/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     9105 2023-03-12 15:02:27.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/examples/plot-examples.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.225003 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      958 2023-03-14 13:38:10.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/__init__.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.225003 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.225003 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/color/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      226 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/color/bright.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      193 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/color/high-contrast.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      237 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/color/high-vis.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      245 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/color/light.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      255 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/color/muted.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      135 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/color/retro.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      201 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/color/std-colors.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      227 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/color/vibrant.mplstyle
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.225003 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/journals/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      393 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/journals/ieee.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      906 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/journals/nature.mplstyle
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.225003 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/languages/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      144 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/languages/cjk-jp-font.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      142 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/languages/cjk-kr-font.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      154 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/languages/cjk-sc-font.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      155 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/languages/cjk-tc-font.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      197 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/languages/russian-font.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      224 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/languages/turkish-font.mplstyle
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.229003 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/misc/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      272 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/misc/grid.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      378 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/misc/latex-sans.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)       40 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/misc/no-latex.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      130 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/misc/pgf.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      364 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/misc/sans.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      643 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/notebook.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)      333 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/scatter.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1110 2023-03-08 03:08:47.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/science.mplstyle
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1348 2023-03-12 15:02:27.000000 plottoolbox-104.3.1/src/plottoolbox/SciencePlots/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.221003 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.229003 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4674 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/Farmington_River_data.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5567 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/all_stats.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6386 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/convertMatFile.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5095 2023-03-14 13:39:52.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/get_time_series.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     4490 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/load_data.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2209 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/read_csv_data.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4177 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target1.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6106 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target10.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4275 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target2.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4654 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target3.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4791 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target4.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5152 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target5.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5248 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target6.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5615 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target7.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5673 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target8.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     8556 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target9.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      592 2023-03-14 13:39:52.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target_options.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5206 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor1.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5727 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor10.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4164 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor11.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5340 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor12.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6409 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor13.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    10510 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor14.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4998 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor2.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5253 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor3.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5690 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor4.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5765 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor5.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5704 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor6.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5811 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor7.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6634 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor8.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6465 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor9.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      592 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor_options.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.229003 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Test/
+-rw-rw-r--   0 tim       (1000) tim       (1000)    10754 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Test/test_plots.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.233003 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1877 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/__init__.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     4527 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/add_legend.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      784 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/bias.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1679 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/brier_score.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1115 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/centered_rms_dev.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1837 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/check_duplicate_stats.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      980 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/check_on_off.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1821 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/check_taylor_stats.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3114 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/error_check_stats.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1760 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/get_axis_tick_label.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     1216 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/get_from_dict_or_default.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6092 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/get_target_diagram_axes.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    16209 2023-03-18 01:42:37.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/get_target_diagram_options.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2550 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/get_taylor_diagram_axes.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    21862 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/get_taylor_diagram_options.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3279 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/kling_gupta_eff09.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3324 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/kling_gupta_eff12.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2188 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/nash_sutcliffe_eff.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2815 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/overlay_target_diagram_circles.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     5211 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/overlay_taylor_diagram_circles.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3141 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/overlay_taylor_diagram_lines.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7970 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/plot_pattern_diagram_colorbar.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     7105 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/plot_pattern_diagram_markers.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3396 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/plot_target_axes.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)    11728 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/plot_taylor_axes.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2796 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/plot_taylor_obs.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      617 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/report_duplicate_stats.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      963 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/rmsd.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      925 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/save_figures.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1751 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/skill_score_brier.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1611 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/skill_score_murphy.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     9464 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/target_diagram.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2559 2023-03-18 01:29:59.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/target_statistics.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    13609 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/taylor_diagram.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2569 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/taylor_statistics.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      455 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/use_sci_notation.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      880 2023-03-14 13:39:53.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/utils.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4264 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/write_stats.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5316 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/write_target_stats.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5231 2023-03-14 13:39:58.000000 plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/write_taylor_stats.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1910 2023-03-26 22:07:58.000000 plottoolbox-104.3.1/src/plottoolbox/__init__.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.237003 plottoolbox-104.3.1/src/plottoolbox/_functions/
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2023-01-23 20:56:50.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3438 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/autocorrelation.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7190 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/bar.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7244 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/bar_stacked.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7080 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/barh.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7102 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/barh_stacked.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5041 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/bootstrap.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4944 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/boxplot.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6742 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/double_mass.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4968 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/handh.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5983 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/heatmap.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4472 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/hexbin.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5034 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/histogram.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5842 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/kde.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7182 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/kde_time.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5185 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/lag_plot.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7754 2023-06-17 18:54:18.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/lognorm_xaxis.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7716 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/lognorm_yaxis.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7643 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/norm_xaxis.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7696 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/norm_yaxis.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5660 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/probability_density.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5107 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/scatter_matrix.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4405 2023-05-11 22:53:05.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/target.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3864 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/taylor.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6053 2023-07-24 04:27:35.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/time.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5095 2023-05-11 22:26:18.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/waterfall.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7589 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/weibull_xaxis.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7693 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/weibull_yaxis.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7537 2023-05-12 03:44:04.000000 plottoolbox-104.3.1/src/plottoolbox/_functions/xy.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    27577 2023-05-02 00:24:02.000000 plottoolbox-104.3.1/src/plottoolbox/_plotutils.py
+-rw-r--r--   0 tim       (1000) tim       (1000)    72737 2023-07-13 03:20:24.000000 plottoolbox-104.3.1/src/plottoolbox/plottoolbox.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.237003 plottoolbox-104.3.1/src/plottoolbox/waterfall_ax/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      657 2023-03-26 22:10:22.000000 plottoolbox-104.3.1/src/plottoolbox/waterfall_ax/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.237003 plottoolbox-104.3.1/src/plottoolbox/waterfall_ax/waterfall_ax/
+-rw-rw-r--   0 tim       (1000) tim       (1000)       41 2023-03-26 22:10:22.000000 plottoolbox-104.3.1/src/plottoolbox/waterfall_ax/waterfall_ax/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    10001 2023-04-03 02:20:00.000000 plottoolbox-104.3.1/src/plottoolbox/waterfall_ax/waterfall_ax/waterfall_ax.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.225003 plottoolbox-104.3.1/src/plottoolbox.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6351 2023-07-24 04:52:30.000000 plottoolbox-104.3.1/src/plottoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)    12812 2023-07-24 04:52:30.000000 plottoolbox-104.3.1/src/plottoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-07-24 04:52:30.000000 plottoolbox-104.3.1/src/plottoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       62 2023-07-24 04:52:30.000000 plottoolbox-104.3.1/src/plottoolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      247 2023-07-24 04:52:30.000000 plottoolbox-104.3.1/src/plottoolbox.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       12 2023-07-24 04:52:30.000000 plottoolbox-104.3.1/src/plottoolbox.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.253004 plottoolbox-104.3.1/tests/
+-rw-r--r--   0 tim       (1000) tim       (1000)  5411566 2021-03-19 23:27:40.000000 plottoolbox-104.3.1/tests/02234500_65_65.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2023-01-22 03:38:20.000000 plottoolbox-104.3.1/tests/__init__.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 04:52:30.257004 plottoolbox-104.3.1/tests/baseline/
+-rw-r--r--   0 tim       (1000) tim       (1000)    37406 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_autocorrelation.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    31916 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_bar.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    35045 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_bar_stacked.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    30663 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_barh.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    34581 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_barh_stacked.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    24015 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_boxplot.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    30921 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_double_mass.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    36999 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_double_mass_marker.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    42100 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_double_mass_mult.png
+-rw-r--r--   0 tim       (1000) tim       (1000)   150426 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_heatmap.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    72201 2023-03-01 21:16:24.000000 plottoolbox-104.3.1/tests/baseline/test_hexbin.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    33878 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_histogram.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    58166 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_kde_time.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    64489 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_kde_time_multiple_traces.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    33169 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_lag_plot.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    30939 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_lognorm_xaxis.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    28815 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_lognorm_yaxis.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    31655 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_norm_xaxis.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    28921 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_norm_yaxis.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    23921 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_probability_density.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    87625 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_scatter_matrix.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    41249 2023-03-18 01:43:59.000000 plottoolbox-104.3.1/tests/baseline/test_target.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    82456 2023-03-13 02:41:16.000000 plottoolbox-104.3.1/tests/baseline/test_taylor.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    39301 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_time_markers.png
+-rw-r--r--   0 tim       (1000) tim       (1000)   112833 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_time_multiple_traces_new_style_plot.png
+-rw-r--r--   0 tim       (1000) tim       (1000)   112134 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_time_multiple_traces_plot.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    58721 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_time_multiple_traces_style_plot.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    50929 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_time_plot.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    32889 2023-05-12 03:34:58.000000 plottoolbox-104.3.1/tests/baseline/test_waterfall.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    32214 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_weibull_xaxis.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    29194 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_weibull_yaxis.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    87205 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_xy.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    46025 2022-07-18 15:27:42.000000 plottoolbox-104.3.1/tests/baseline/test_xy_multiple_traces.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    71428 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_xy_multiple_traces_logx.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    77455 2022-07-18 15:28:12.000000 plottoolbox-104.3.1/tests/baseline/test_xy_multiple_traces_logy.png
+-rw-r--r--   0 tim       (1000) tim       (1000)    37598 2020-09-26 07:35:10.000000 plottoolbox-104.3.1/tests/baseline/test_xy_multiple_traces_markers.png
+-rw-r--r--   0 tim       (1000) tim       (1000)      394 2023-01-22 03:38:20.000000 plottoolbox-104.3.1/tests/capture.py
+-rw-r--r--   0 tim       (1000) tim       (1000)    40960 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data.wdm
+-rw-r--r--   0 tim       (1000) tim       (1000)    89620 2022-07-18 00:44:27.000000 plottoolbox-104.3.1/tests/data_02325000_flow.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)       84 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_bi_daily.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)    75863 2022-07-18 00:42:28.000000 plottoolbox-104.3.1/tests/data_daily.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)   122972 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_daily_sample.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      829 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_dirty_index.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      188 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_empty_cols.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      241 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_fill_from.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      697 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_filter_fft_lowpass.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      825 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_filter_flat.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      862 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_filter_hanning.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_filter_transform.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)     1164 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_flat.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      611 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_flat_01.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)   549278 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_flow_stage.xlsx
+-rw-r--r--   0 tim       (1000) tim       (1000)   172784 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_gainesville_daily_precip.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)   120195 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_gainesville_daily_precip_index.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)  9677288 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_gainesville_hourly_precip.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      463 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_missing.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      149 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_multiple_cols.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)     1189 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_read_append.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)     1165 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_read_append_header.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)     1515 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_read_append_header_cols.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)     1165 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_read_append_header_duplicate.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)       44 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_simple.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)       81 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_simple_extra_rows.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      140 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_simple_extra_rows_sparse.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      684 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_sine.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      209 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_spaces.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      141 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_stacked.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)      183 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_stacked_1.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)    30254 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_sunspot.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)    53259 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_sunspot_EST.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)    17446 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_sunspot_index.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)    34163 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_sunspot_normalized_0_to_1.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)    31517 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_sunspot_normalized_10_to_20.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)    36205 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_sunspot_normalized_pct_rank.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)    36871 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_sunspot_normalized_zscore.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)       91 2021-06-29 23:02:12.000000 plottoolbox-104.3.1/tests/data_unstacked.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)     3488 2023-03-01 04:59:34.000000 plottoolbox-104.3.1/tests/test_plot_1.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     3557 2023-01-22 03:38:20.000000 plottoolbox-104.3.1/tests/test_plot_2.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4410 2023-03-27 02:30:00.000000 plottoolbox-104.3.1/tests/test_plot_3.py
```

### Comparing `plottoolbox-104.3.0/.github/workflows/python-package.yml` & `plottoolbox-104.3.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/.pre-commit-config.yaml` & `plottoolbox-104.3.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -19,27 +19,27 @@
           - id: fix-encoding-pragma
             args: [--remove]
           - id: mixed-line-ending
           - id: trailing-whitespace
             exclude: notebooks/tstoolbox_plot_bash.sh
 
     - repo: https://github.com/pappasam/toml-sort
-      rev: v0.23.0
+      rev: v0.23.1
       hooks:
           - id: toml-sort-fix
             args: [--in-place, --spaces-indent-inline-array, '4']
 
     - repo: https://github.com/adrienverge/yamllint.git
-      rev: v1.31.0
+      rev: v1.32.0
       hooks:
           - id: yamllint
             args: [--format, parsable, --strict]
 
     - repo: https://github.com/jumanjihouse/pre-commit-hook-yamlfmt
-      rev: 0.2.2
+      rev: 0.2.3
       hooks:
           - id: yamlfmt
 
     - repo: https://github.com/jumanjihouse/pre-commit-hooks
       rev: 3.0.0
       hooks:
           - id: shellcheck
@@ -48,17 +48,18 @@
     - repo: https://github.com/lovesegfault/beautysh
       rev: v6.2.1
       hooks:
           - id: beautysh
             args: [--indent-size, '4']
 
     - repo: https://github.com/psf/black
-      rev: 23.3.0
+      rev: 23.7.0
       hooks:
           - id: black
+          - id: black-jupyter
 
     - repo: https://github.com/pycqa/isort
       rev: 5.12.0
       hooks:
           - id: isort
             name: isort (python)
             args: [--profile, black, --filter-files]
@@ -67,33 +68,28 @@
             types: [cython]
             args: [--profile, black, --filter-files]
           - id: isort
             name: isort (pyi)
             types: [pyi]
             args: [--profile, black, --filter-files]
 
-    - repo: https://github.com/dfm/black_nbconvert
-      rev: v0.4.0
-      hooks:
-          - id: black_nbconvert
-
     - repo: https://github.com/asottile/blacken-docs
-      rev: 1.13.0
+      rev: 1.15.0
       hooks:
           - id: blacken-docs
 
     - repo: https://github.com/asottile/pyupgrade
-      rev: v3.3.2
+      rev: v3.9.0
       hooks:
           - id: pyupgrade
 
     - repo: https://github.com/commitizen-tools/commitizen
-      rev: 3.1.1
+      rev: 3.5.3
       hooks:
           - id: commitizen
             stages: [commit-msg]
 
     - repo: https://github.com/mwouts/jupytext
-      rev: v1.14.5
+      rev: v1.14.7
       hooks:
           - id: jupytext
             args: [--from, ipynb, --to, auto:percent, --sync]
```

### Comparing `plottoolbox-104.3.0/BADGES.rst` & `plottoolbox-104.3.1/BADGES.rst`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/CHANGELOG.md` & `plottoolbox-104.3.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v104.3.1 (2023-07-24)
+
+### Fix
+
+- fixed secondary_y option for the time plot
+
 ## v104.3.0 (2023-05-11)
 
 ### Feat
 
 - added dropna option to all plots
 - **waterfall**: added new waterfall plot but not particularly impressed - WIP
```

### Comparing `plottoolbox-104.3.0/CONTRIBUTING.rst` & `plottoolbox-104.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/LICENSE.txt` & `plottoolbox-104.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/PKG-INFO` & `plottoolbox-104.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plottoolbox
-Version: 104.3.0
+Version: 104.3.1
 Summary: Command line script and Python library to make plots from data files.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/plottoolbox/docs/index.html#plottoolbox-documentation
 Project-URL: github, https://github.com/timcera/plottoolbox
 Project-URL: bitbucket, https://bitbucket.org/timcera/plottoolbox/src/main/
 Keywords: time-series,cli-app,aggregate,fill,filter
@@ -67,18 +67,26 @@
 Requirements
 ------------
 * pandas - on Windows this is part scientific Python distributions like
   Python(x,y), Anaconda, or Enthought.
 
 Installation
 ------------
-Should be as easy as running ``pip install plottoolbox`` or ``easy_install
-plottoolbox`` at any command line.  Not sure on Windows whether this will bring
-in pandas, but as mentioned above, if you start with scientific Python
-distribution then you shouldn't have a problem.
+pip
+~~~
+.. code-block:: bash
+
+    pip install plottoolbox
+
+conda
+~~~~~
+.. code-block:: bash
+
+    conda install -c conda-forge plottoolbox
+
 
 Usage - Command Line
 --------------------
 Just run 'plottoolbox --help' to get a list of subcommands::
 
     usage: plottoolbox [-h]
                        {autocorrelation, bar, bar_stacked, barh, barh_stacked,
```

### Comparing `plottoolbox-104.3.0/README.rst` & `plottoolbox-104.3.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -37,18 +37,26 @@
 Requirements
 ------------
 * pandas - on Windows this is part scientific Python distributions like
   Python(x,y), Anaconda, or Enthought.
 
 Installation
 ------------
-Should be as easy as running ``pip install plottoolbox`` or ``easy_install
-plottoolbox`` at any command line.  Not sure on Windows whether this will bring
-in pandas, but as mentioned above, if you start with scientific Python
-distribution then you shouldn't have a problem.
+pip
+~~~
+.. code-block:: bash
+
+    pip install plottoolbox
+
+conda
+~~~~~
+.. code-block:: bash
+
+    conda install -c conda-forge plottoolbox
+
 
 Usage - Command Line
 --------------------
 Just run 'plottoolbox --help' to get a list of subcommands::
 
     usage: plottoolbox [-h]
                        {autocorrelation, bar, bar_stacked, barh, barh_stacked,
```

### Comparing `plottoolbox-104.3.0/docs/Makefile` & `plottoolbox-104.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/docs/command_line.rst` & `plottoolbox-104.3.1/docs/command_line.rst`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/docs/conf.py` & `plottoolbox-104.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/docs/function_summary.rst` & `plottoolbox-104.3.1/docs/function_summary.rst`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/docs/make.bat` & `plottoolbox-104.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/pyproject.toml` & `plottoolbox-104.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 description = "Command line script and Python library to make plots from data files."
 dependencies = [
     "cltoolbox >= 1.0.0",
     "numpy",
     "scipy",
     "pandas",
     "pydantic",
-    "toolbox_utils >= 3.0.0, < 4.0.0",
-    "matplotlib"
+    "toolbox_utils >= 5.0.0, < 6.0.0",
+    "matplotlib",
+    "xlsxwriter"
 ]
 license = {text = "BSD-3-Clause"}
 authors = [
     {name = "Tim Cera", email = "tim@cerazone.net"}
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -83,15 +84,15 @@
 [tool.check-manifest]
 ignore = [".travis.yml", "docs/_function_autosummary/*"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "104.3.0"
+version = "104.3.1"
 version_files = ["VERSION"]
 
 [tool.isort]
 profile = "black"
 
 [tool.setuptools]
 license-files = ["LICENSE.txt"]
```

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SciencePlots/examples/plot-examples.py` & `plottoolbox-104.3.1/src/plottoolbox/SciencePlots/examples/plot-examples.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/__init__.py` & `plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/__init__.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/journals/nature.mplstyle` & `plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/journals/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/notebook.mplstyle` & `plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/notebook.mplstyle`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SciencePlots/scienceplots/styles/science.mplstyle` & `plottoolbox-104.3.1/src/plottoolbox/SciencePlots/scienceplots/styles/science.mplstyle`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SciencePlots/setup.py` & `plottoolbox-104.3.1/src/plottoolbox/SciencePlots/setup.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/Farmington_River_data.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/Farmington_River_data.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/all_stats.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/all_stats.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/convertMatFile.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/convertMatFile.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/get_time_series.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/get_time_series.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/load_data.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/load_data.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/read_csv_data.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/read_csv_data.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target1.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target1.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target10.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target10.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target2.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target2.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target3.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target3.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target4.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target4.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target5.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target5.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target6.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target6.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target7.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target7.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target8.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target8.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target9.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target9.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/target_options.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/target_options.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor1.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor1.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor10.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor10.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor11.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor11.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor12.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor12.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor13.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor13.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor14.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor14.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor2.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor2.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor3.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor3.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor4.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor4.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor5.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor5.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor6.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor6.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor7.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor7.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor8.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor8.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor9.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor9.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Examples/taylor_options.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Examples/taylor_options.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/Test/test_plots.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/Test/test_plots.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/__init__.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/add_legend.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/add_legend.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/bias.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/bias.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/brier_score.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/brier_score.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/centered_rms_dev.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/centered_rms_dev.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/check_duplicate_stats.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/check_duplicate_stats.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/check_on_off.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/check_on_off.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/check_taylor_stats.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/check_taylor_stats.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/error_check_stats.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/error_check_stats.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/get_axis_tick_label.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/get_axis_tick_label.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/get_from_dict_or_default.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/get_from_dict_or_default.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/get_target_diagram_axes.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/get_target_diagram_axes.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/get_target_diagram_options.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/get_target_diagram_options.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/get_taylor_diagram_axes.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/get_taylor_diagram_axes.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/get_taylor_diagram_options.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/get_taylor_diagram_options.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/kling_gupta_eff09.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/kling_gupta_eff09.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/kling_gupta_eff12.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/kling_gupta_eff12.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/nash_sutcliffe_eff.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/nash_sutcliffe_eff.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/overlay_target_diagram_circles.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/overlay_target_diagram_circles.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/overlay_taylor_diagram_circles.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/overlay_taylor_diagram_circles.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/overlay_taylor_diagram_lines.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/overlay_taylor_diagram_lines.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/plot_pattern_diagram_colorbar.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/plot_pattern_diagram_colorbar.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/plot_pattern_diagram_markers.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/plot_pattern_diagram_markers.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/plot_target_axes.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/plot_target_axes.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/plot_taylor_axes.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/plot_taylor_axes.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/plot_taylor_obs.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/plot_taylor_obs.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/report_duplicate_stats.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/report_duplicate_stats.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/rmsd.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/rmsd.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/save_figures.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/save_figures.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/skill_score_brier.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/skill_score_brier.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/skill_score_murphy.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/skill_score_murphy.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/target_diagram.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/target_diagram.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/target_statistics.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/target_statistics.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/taylor_diagram.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/taylor_diagram.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/taylor_statistics.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/taylor_statistics.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/utils.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/write_stats.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/write_stats.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/write_target_stats.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/write_target_stats.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/SkillMetrics/skill_metrics/write_taylor_stats.py` & `plottoolbox-104.3.1/src/plottoolbox/SkillMetrics/skill_metrics/write_taylor_stats.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/__init__.py` & `plottoolbox-104.3.1/src/plottoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/autocorrelation.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/autocorrelation.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/bar.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/bar.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/bar_stacked.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/bar_stacked.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/barh.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/barh.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/barh_stacked.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/barh_stacked.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/bootstrap.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/bootstrap.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/boxplot.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/boxplot.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/double_mass.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/double_mass.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/handh.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/handh.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/heatmap.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/heatmap.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/hexbin.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/hexbin.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/histogram.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/histogram.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/kde.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/kde.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/kde_time.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/kde_time.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/lag_plot.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/lag_plot.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/lognorm_xaxis.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/lognorm_xaxis.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import scienceplots
 
 matplotlib.use("Agg")
 
 warnings.filterwarnings("ignore")
 
 
-@tsutils.doc(tsutils.docstrings)
+@tsutils.doc(_plotutils.ldocstrings)
 def lognorm_xaxis(
     input_ts="-",
     columns=None,
     start_date=None,
     end_date=None,
     clean=False,
     skiprows=None,
```

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/lognorm_yaxis.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/lognorm_yaxis.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/norm_xaxis.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/norm_xaxis.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/norm_yaxis.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/norm_yaxis.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/probability_density.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/probability_density.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/scatter_matrix.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/target.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/target.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/taylor.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/taylor.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/time.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Collection of functions for the manipulation of time series."""
 
 import sys
 import warnings
 from pathlib import Path
 
 import matplotlib
+import numpy as np
 import pandas as pd
 from toolbox_utils import tsutils
 
 from .. import _plotutils
 
 sys.path.append(str(Path(__file__).parent / ".." / "SciencePlots"))
 import scienceplots
@@ -41,15 +42,15 @@
     linestyles="auto",
     markerstyles=" ",
     style="auto",
     xaxis="arithmetic",
     yaxis="arithmetic",
     xlim=None,
     ylim=None,
-    secondary_y=False,
+    secondary_y=None,
     mark_right=True,
     grid=False,
     drawstyle="default",
     por=False,
     invert_xaxis=False,
     invert_yaxis=False,
     round_index=None,
@@ -189,14 +190,19 @@
 
     plot_styles = tsutils.make_list(plot_styles) + ["no-latex"]
     plt.style.use(plot_styles)
 
     figsize = tsutils.make_list(figsize, n=2)
     _, ax = plt.subplots(figsize=figsize)
 
+    if secondary_y is not None:
+        secondary_y = np.array(
+            tsd.columns[tsutils.make_iloc(tsd.columns, tsutils.make_list(secondary_y))]
+        )
+
     ax = tsd.plot(
         legend=legend,
         subplots=subplots,
         sharex=sharex,
         sharey=sharey,
         logx=logx,
         logy=logy,
@@ -216,29 +222,26 @@
         plt.setp(line, marker=m)
         plt.setp(line, linestyle=l)
 
     xtitle = xtitle or "Time"
     plt.xlabel(xtitle)
     plt.ylabel(ytitle)
 
-    if legend:
-        plt.legend(loc="best")
-
     plt = _plotutils.hv_lines(
         plt,
         hlines_y=hlines_y,
         hlines_xmin=hlines_xmin,
         hlines_xmax=hlines_xmax,
         hlines_colors=hlines_colors,
         hlines_linestyles=hlines_linestyles,
-        vlines_x=None,
-        vlines_ymin=None,
-        vlines_ymax=None,
-        vlines_colors=None,
-        vlines_linestyles=None,
+        vlines_x=vlines_x,
+        vlines_ymin=vlines_ymin,
+        vlines_ymax=vlines_ymax,
+        vlines_colors=vlines_colors,
+        vlines_linestyles=vlines_linestyles,
     )
 
     if invert_xaxis is True:
         plt.gca().invert_xaxis()
     if invert_yaxis is True:
         plt.gca().invert_yaxis()
```

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/waterfall.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/waterfall.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/weibull_xaxis.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/weibull_xaxis.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/weibull_yaxis.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/weibull_yaxis.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_functions/xy.py` & `plottoolbox-104.3.1/src/plottoolbox/_functions/xy.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/_plotutils.py` & `plottoolbox-104.3.1/src/plottoolbox/_plotutils.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/plottoolbox.py` & `plottoolbox-104.3.1/src/plottoolbox/plottoolbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -2076,15 +2076,15 @@
         linestyles="auto",
         markerstyles=" ",
         style="auto",
         xaxis="arithmetic",
         yaxis="arithmetic",
         xlim=None,
         ylim=None,
-        secondary_y=False,
+        secondary_y=None,
         mark_right=True,
         grid=False,
         drawstyle="default",
         por=False,
         invert_xaxis=False,
         invert_yaxis=False,
         round_index=None,
```

### Comparing `plottoolbox-104.3.0/src/plottoolbox/waterfall_ax/setup.py` & `plottoolbox-104.3.1/src/plottoolbox/waterfall_ax/setup.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox/waterfall_ax/waterfall_ax/waterfall_ax.py` & `plottoolbox-104.3.1/src/plottoolbox/waterfall_ax/waterfall_ax/waterfall_ax.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/src/plottoolbox.egg-info/PKG-INFO` & `plottoolbox-104.3.1/src/plottoolbox.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plottoolbox
-Version: 104.3.0
+Version: 104.3.1
 Summary: Command line script and Python library to make plots from data files.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/plottoolbox/docs/index.html#plottoolbox-documentation
 Project-URL: github, https://github.com/timcera/plottoolbox
 Project-URL: bitbucket, https://bitbucket.org/timcera/plottoolbox/src/main/
 Keywords: time-series,cli-app,aggregate,fill,filter
@@ -67,18 +67,26 @@
 Requirements
 ------------
 * pandas - on Windows this is part scientific Python distributions like
   Python(x,y), Anaconda, or Enthought.
 
 Installation
 ------------
-Should be as easy as running ``pip install plottoolbox`` or ``easy_install
-plottoolbox`` at any command line.  Not sure on Windows whether this will bring
-in pandas, but as mentioned above, if you start with scientific Python
-distribution then you shouldn't have a problem.
+pip
+~~~
+.. code-block:: bash
+
+    pip install plottoolbox
+
+conda
+~~~~~
+.. code-block:: bash
+
+    conda install -c conda-forge plottoolbox
+
 
 Usage - Command Line
 --------------------
 Just run 'plottoolbox --help' to get a list of subcommands::
 
     usage: plottoolbox [-h]
                        {autocorrelation, bar, bar_stacked, barh, barh_stacked,
```

### Comparing `plottoolbox-104.3.0/src/plottoolbox.egg-info/SOURCES.txt` & `plottoolbox-104.3.1/src/plottoolbox.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 docs/_function_autosummary/plottoolbox.plottoolbox.norm_xaxis.rst
 docs/_function_autosummary/plottoolbox.plottoolbox.norm_yaxis.rst
 docs/_function_autosummary/plottoolbox.plottoolbox.probability_density.rst
 docs/_function_autosummary/plottoolbox.plottoolbox.scatter_matrix.rst
 docs/_function_autosummary/plottoolbox.plottoolbox.target.rst
 docs/_function_autosummary/plottoolbox.plottoolbox.taylor.rst
 docs/_function_autosummary/plottoolbox.plottoolbox.time.rst
+docs/_function_autosummary/plottoolbox.plottoolbox.waterfall.rst
 docs/_function_autosummary/plottoolbox.plottoolbox.weibull_xaxis.rst
 docs/_function_autosummary/plottoolbox.plottoolbox.weibull_yaxis.rst
 docs/_function_autosummary/plottoolbox.plottoolbox.xy.rst
 src/plottoolbox/__init__.py
 src/plottoolbox/_plotutils.py
 src/plottoolbox/plottoolbox.py
 src/plottoolbox.egg-info/PKG-INFO
```

### Comparing `plottoolbox-104.3.0/tests/02234500_65_65.csv` & `plottoolbox-104.3.1/tests/02234500_65_65.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_autocorrelation.png` & `plottoolbox-104.3.1/tests/baseline/test_autocorrelation.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_bar.png` & `plottoolbox-104.3.1/tests/baseline/test_bar.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_bar_stacked.png` & `plottoolbox-104.3.1/tests/baseline/test_bar_stacked.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_barh.png` & `plottoolbox-104.3.1/tests/baseline/test_barh.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_barh_stacked.png` & `plottoolbox-104.3.1/tests/baseline/test_barh_stacked.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_boxplot.png` & `plottoolbox-104.3.1/tests/baseline/test_boxplot.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_double_mass.png` & `plottoolbox-104.3.1/tests/baseline/test_double_mass.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_double_mass_marker.png` & `plottoolbox-104.3.1/tests/baseline/test_double_mass_marker.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_double_mass_mult.png` & `plottoolbox-104.3.1/tests/baseline/test_double_mass_mult.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_heatmap.png` & `plottoolbox-104.3.1/tests/baseline/test_heatmap.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_hexbin.png` & `plottoolbox-104.3.1/tests/baseline/test_hexbin.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_histogram.png` & `plottoolbox-104.3.1/tests/baseline/test_histogram.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_kde_time.png` & `plottoolbox-104.3.1/tests/baseline/test_kde_time.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_kde_time_multiple_traces.png` & `plottoolbox-104.3.1/tests/baseline/test_kde_time_multiple_traces.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_lag_plot.png` & `plottoolbox-104.3.1/tests/baseline/test_lag_plot.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_lognorm_xaxis.png` & `plottoolbox-104.3.1/tests/baseline/test_lognorm_xaxis.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_lognorm_yaxis.png` & `plottoolbox-104.3.1/tests/baseline/test_lognorm_yaxis.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_norm_xaxis.png` & `plottoolbox-104.3.1/tests/baseline/test_norm_xaxis.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_norm_yaxis.png` & `plottoolbox-104.3.1/tests/baseline/test_norm_yaxis.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_probability_density.png` & `plottoolbox-104.3.1/tests/baseline/test_probability_density.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_scatter_matrix.png` & `plottoolbox-104.3.1/tests/baseline/test_scatter_matrix.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_target.png` & `plottoolbox-104.3.1/tests/baseline/test_target.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_taylor.png` & `plottoolbox-104.3.1/tests/baseline/test_taylor.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_time_markers.png` & `plottoolbox-104.3.1/tests/baseline/test_time_markers.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_time_multiple_traces_new_style_plot.png` & `plottoolbox-104.3.1/tests/baseline/test_time_multiple_traces_new_style_plot.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_time_multiple_traces_plot.png` & `plottoolbox-104.3.1/tests/baseline/test_time_multiple_traces_plot.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_time_multiple_traces_style_plot.png` & `plottoolbox-104.3.1/tests/baseline/test_time_multiple_traces_style_plot.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_time_plot.png` & `plottoolbox-104.3.1/tests/baseline/test_time_plot.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_waterfall.png` & `plottoolbox-104.3.1/tests/baseline/test_waterfall.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_weibull_xaxis.png` & `plottoolbox-104.3.1/tests/baseline/test_weibull_xaxis.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_weibull_yaxis.png` & `plottoolbox-104.3.1/tests/baseline/test_weibull_yaxis.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_xy.png` & `plottoolbox-104.3.1/tests/baseline/test_xy.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_xy_multiple_traces.png` & `plottoolbox-104.3.1/tests/baseline/test_xy_multiple_traces.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_xy_multiple_traces_logx.png` & `plottoolbox-104.3.1/tests/baseline/test_xy_multiple_traces_logx.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_xy_multiple_traces_logy.png` & `plottoolbox-104.3.1/tests/baseline/test_xy_multiple_traces_logy.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/baseline/test_xy_multiple_traces_markers.png` & `plottoolbox-104.3.1/tests/baseline/test_xy_multiple_traces_markers.png`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data.wdm` & `plottoolbox-104.3.1/tests/data.wdm`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_02325000_flow.csv` & `plottoolbox-104.3.1/tests/data_02325000_flow.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_daily.csv` & `plottoolbox-104.3.1/tests/data_daily.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_daily_sample.csv` & `plottoolbox-104.3.1/tests/data_daily_sample.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_dirty_index.csv` & `plottoolbox-104.3.1/tests/data_dirty_index.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_filter_fft_lowpass.csv` & `plottoolbox-104.3.1/tests/data_filter_fft_lowpass.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_filter_flat.csv` & `plottoolbox-104.3.1/tests/data_filter_flat.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_filter_hanning.csv` & `plottoolbox-104.3.1/tests/data_filter_hanning.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_flat.csv` & `plottoolbox-104.3.1/tests/data_flat.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_flat_01.csv` & `plottoolbox-104.3.1/tests/data_flat_01.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_flow_stage.xlsx` & `plottoolbox-104.3.1/tests/data_flow_stage.xlsx`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_gainesville_daily_precip.csv` & `plottoolbox-104.3.1/tests/data_gainesville_daily_precip.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_gainesville_daily_precip_index.csv` & `plottoolbox-104.3.1/tests/data_gainesville_daily_precip_index.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_gainesville_hourly_precip.csv` & `plottoolbox-104.3.1/tests/data_gainesville_hourly_precip.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_read_append.csv` & `plottoolbox-104.3.1/tests/data_read_append.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_read_append_header.csv` & `plottoolbox-104.3.1/tests/data_read_append_header.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_read_append_header_cols.csv` & `plottoolbox-104.3.1/tests/data_read_append_header_cols.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_read_append_header_duplicate.csv` & `plottoolbox-104.3.1/tests/data_read_append_header_duplicate.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_sine.csv` & `plottoolbox-104.3.1/tests/data_sine.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_sunspot.csv` & `plottoolbox-104.3.1/tests/data_sunspot.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_sunspot_EST.csv` & `plottoolbox-104.3.1/tests/data_sunspot_EST.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_sunspot_index.csv` & `plottoolbox-104.3.1/tests/data_sunspot_index.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_sunspot_normalized_0_to_1.csv` & `plottoolbox-104.3.1/tests/data_sunspot_normalized_0_to_1.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_sunspot_normalized_10_to_20.csv` & `plottoolbox-104.3.1/tests/data_sunspot_normalized_10_to_20.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_sunspot_normalized_pct_rank.csv` & `plottoolbox-104.3.1/tests/data_sunspot_normalized_pct_rank.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/data_sunspot_normalized_zscore.csv` & `plottoolbox-104.3.1/tests/data_sunspot_normalized_zscore.csv`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/test_plot_1.py` & `plottoolbox-104.3.1/tests/test_plot_1.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/test_plot_2.py` & `plottoolbox-104.3.1/tests/test_plot_2.py`

 * *Files identical despite different names*

### Comparing `plottoolbox-104.3.0/tests/test_plot_3.py` & `plottoolbox-104.3.1/tests/test_plot_3.py`

 * *Files identical despite different names*

