# Comparing `tmp/holobench-0.0.5.tar.gz` & `tmp/holobench-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holobench-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "holobench-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `holobench-0.0.5.tar` & `holobench-0.0.6.tar`

### file list

```diff
@@ -1,87 +1,88 @@
--rw-r--r--   0        0        0      338 2023-07-22 13:39:33.630996 holobench-0.0.5/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1459 2023-07-22 13:46:18.085296 holobench-0.0.5/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      502 2023-07-16 12:36:45.474978 holobench-0.0.5/.github/dependabot.yml
--rw-r--r--   0        0        0     1264 2023-07-16 12:36:45.474978 holobench-0.0.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3208 2023-07-20 18:29:05.424632 holobench-0.0.5/.gitignore
--rw-r--r--   0        0        0      381 2023-07-16 12:36:45.474978 holobench-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      209 2023-07-16 12:36:45.474978 holobench-0.0.5/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      379 2023-07-16 12:36:45.474978 holobench-0.0.5/.pylintrc
--rw-r--r--   0        0        0      187 2023-07-16 12:36:45.474978 holobench-0.0.5/.vscode/settings.json
--rw-r--r--   0        0        0      885 2023-07-22 13:41:19.523506 holobench-0.0.5/.vscode/tasks.json
--rw-r--r--   0        0        0     1065 2023-07-16 12:36:45.474978 holobench-0.0.5/LICENSE
--rw-r--r--   0        0        0     2720 2023-07-16 12:36:45.474978 holobench-0.0.5/README.md
--rw-r--r--   0        0        0      789 2023-07-22 12:02:54.862576 holobench-0.0.5/bencher/__init__.py
--rw-r--r--   0        0        0    25862 2023-07-22 09:13:13.899071 holobench-0.0.5/bencher/bench_cfg.py
--rw-r--r--   0        0        0     3858 2023-07-16 12:36:45.474978 holobench-0.0.5/bencher/bench_plot_server.py
--rw-r--r--   0        0        0    24828 2023-07-22 09:13:13.899071 holobench-0.0.5/bencher/bench_vars.py
--rw-r--r--   0        0        0    27767 2023-07-22 13:39:33.630996 holobench-0.0.5/bencher/bencher.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.474978 holobench-0.0.5/bencher/example/__init__.py
--rw-r--r--   0        0        0     4168 2023-07-22 13:39:33.630996 holobench-0.0.5/bencher/example/benchmark_data.py
--rw-r--r--   0        0        0     3745 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_categorical.py
--rw-r--r--   0        0        0     1901 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_custom_sweep.py
--rw-r--r--   0        0        0     3197 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_float2D_scatter.py
--rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_float3D.py
--rw-r--r--   0        0        0     2817 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_float3D_cone.py
--rw-r--r--   0        0        0     3562 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_float_cat.py
--rw-r--r--   0        0        0     4348 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_floats.py
--rw-r--r--   0        0        0     4018 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_floats2D.py
--rw-r--r--   0        0        0     4101 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/example/example_holosweep.py
--rw-r--r--   0        0        0     1805 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/example/example_hvplot_explorer.py
--rw-r--r--   0        0        0     2619 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/example/example_interactive.py
--rw-r--r--   0        0        0     2416 2023-07-22 12:02:54.862576 holobench-0.0.5/bencher/example/example_kwargs.py
--rw-r--r--   0        0        0     2431 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_pareto.py
--rw-r--r--   0        0        0     3438 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_persistent.py
--rw-r--r--   0        0        0     2540 2023-07-20 18:29:05.428632 holobench-0.0.5/bencher/example/example_plot_library.py
--rw-r--r--   0        0        0     4027 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_sample_cache.py
--rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_sample_cache_context.py
--rw-r--r--   0        0        0    11711 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_simple.py
--rw-r--r--   0        0        0     1525 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/example/example_simple_bool.py
--rw-r--r--   0        0        0     1473 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_simple_cat.py
--rw-r--r--   0        0        0     1393 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_simple_float.py
--rw-r--r--   0        0        0     1172 2023-07-20 18:29:05.428632 holobench-0.0.5/bencher/example/example_template.py
--rw-r--r--   0        0        0     1951 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_time_event.py
--rw-r--r--   0        0        0     2990 2023-07-20 19:07:32.744938 holobench-0.0.5/bencher/example/example_vector.py
--rw-r--r--   0        0        0     6718 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/example/example_workflow.py
--rw-r--r--   0        0        0     2261 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/example/hv_bool_bug.py
--rw-r--r--   0        0        0    10946 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/optuna_conversions.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/plotting/__init__.py
--rw-r--r--   0        0        0     5436 2023-07-20 18:29:05.428632 holobench-0.0.5/bencher/plotting/plot_collection.py
--rw-r--r--   0        0        0     4705 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/plotting/plot_filter.py
--rw-r--r--   0        0        0     3579 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/plotting/plot_library.py
--rw-r--r--   0        0        0     1197 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/plotting/plot_types.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/plotting/plots/__init__.py
--rw-r--r--   0        0        0     2539 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/plotting/plots/catplot.py
--rw-r--r--   0        0        0     3754 2023-07-20 18:29:05.428632 holobench-0.0.5/bencher/plotting/plots/heatmap.py
--rw-r--r--   0        0        0     3821 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/plotting/plots/hv_interactive.py
--rw-r--r--   0        0        0     6359 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/plotting/plots/lineplot.py
--rw-r--r--   0        0        0      618 2023-07-20 18:29:05.432632 holobench-0.0.5/bencher/plotting/plots/plot_base.py
--rw-r--r--   0        0        0     1616 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/plotting/plots/scatterplot.py
--rw-r--r--   0        0        0     3830 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/plotting/plots/surface.py
--rw-r--r--   0        0        0     1194 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/plotting/plots/tables.py
--rw-r--r--   0        0        0     5971 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/plotting/plots/volume.py
--rw-r--r--   0        0        0    10787 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/plotting_functions.py
--rw-r--r--   0        0        0    14109 2023-07-22 09:13:13.903071 holobench-0.0.5/bencher/plt_cfg.py
--rw-r--r--   0        0        0     2339 2023-07-16 12:36:45.478978 holobench-0.0.5/bencher/utils.py
--rw-r--r--   0        0        0      423 2023-07-16 12:36:45.478978 holobench-0.0.5/dependencies.yaml
--rw-r--r--   0        0        0     1045 2023-07-16 12:36:45.478978 holobench-0.0.5/package.xml
--rw-r--r--   0        0        0     1473 2023-07-22 13:40:20.687222 holobench-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      227 2023-07-20 18:29:05.432632 holobench-0.0.5/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.5/resource/bencher
--rw-r--r--   0        0        0       83 2023-07-16 12:36:45.478978 holobench-0.0.5/setup.cfg
--rw-r--r--   0        0        0      628 2023-07-16 12:36:45.478978 holobench-0.0.5/setup.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.5/test/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.5/test/plots/__init__.py
--rw-r--r--   0        0        0      973 2023-07-16 12:36:45.478978 holobench-0.0.5/test/plots/test_catplot.py
--rw-r--r--   0        0        0     1330 2023-07-16 12:36:45.478978 holobench-0.0.5/test/plots/test_plots_common.py
--rw-r--r--   0        0        0     1089 2023-07-16 12:36:45.478978 holobench-0.0.5/test/plots/test_tables.py
--rw-r--r--   0        0        0     3497 2023-07-20 19:19:06.224197 holobench-0.0.5/test/test_bench_examples.py
--rw-r--r--   0        0        0    16047 2023-07-16 12:36:45.478978 holobench-0.0.5/test/test_bencher.py
--rw-r--r--   0        0        0     6150 2023-07-16 12:36:45.478978 holobench-0.0.5/test/test_combinations.py
--rw-r--r--   0        0        0     3534 2023-07-16 12:36:45.478978 holobench-0.0.5/test/test_plot_collection.py
--rw-r--r--   0        0        0     2772 2023-07-16 12:36:45.478978 holobench-0.0.5/test/test_plot_filter.py
--rw-r--r--   0        0        0     1788 2023-07-16 12:36:45.478978 holobench-0.0.5/test/test_plot_library.py
--rw-r--r--   0        0        0     5671 2023-07-16 12:36:45.478978 holobench-0.0.5/test/test_sample_cache.py
--rw-r--r--   0        0        0     1972 2023-07-16 12:36:45.478978 holobench-0.0.5/test/test_sweep_vars.py
--rw-r--r--   0        0        0     1207 2023-07-16 12:36:45.478978 holobench-0.0.5/test/test_utils.py
--rw-r--r--   0        0        0     2439 2023-07-16 12:36:45.478978 holobench-0.0.5/test/test_vars.py
--rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 holobench-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      338 2023-07-22 13:39:33.630996 holobench-0.0.6/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1482 2023-07-24 17:38:19.734638 holobench-0.0.6/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      502 2023-07-16 12:36:45.474978 holobench-0.0.6/.github/dependabot.yml
+-rw-r--r--   0        0        0     1264 2023-07-16 12:36:45.474978 holobench-0.0.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3208 2023-07-20 18:29:05.424632 holobench-0.0.6/.gitignore
+-rw-r--r--   0        0        0      381 2023-07-16 12:36:45.474978 holobench-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      209 2023-07-16 12:36:45.474978 holobench-0.0.6/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      379 2023-07-16 12:36:45.474978 holobench-0.0.6/.pylintrc
+-rw-r--r--   0        0        0      187 2023-07-16 12:36:45.474978 holobench-0.0.6/.vscode/settings.json
+-rw-r--r--   0        0        0      895 2023-07-24 17:38:19.734638 holobench-0.0.6/.vscode/tasks.json
+-rw-r--r--   0        0        0     1065 2023-07-16 12:36:45.474978 holobench-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2720 2023-07-16 12:36:45.474978 holobench-0.0.6/README.md
+-rw-r--r--   0        0        0      789 2023-07-22 12:02:54.862576 holobench-0.0.6/bencher/__init__.py
+-rw-r--r--   0        0        0    26273 2023-07-24 17:38:19.734638 holobench-0.0.6/bencher/bench_cfg.py
+-rw-r--r--   0        0        0     3858 2023-07-16 12:36:45.474978 holobench-0.0.6/bencher/bench_plot_server.py
+-rw-r--r--   0        0        0    24828 2023-07-22 09:13:13.899071 holobench-0.0.6/bencher/bench_vars.py
+-rw-r--r--   0        0        0    27768 2023-07-24 17:38:19.738638 holobench-0.0.6/bencher/bencher.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.474978 holobench-0.0.6/bencher/example/__init__.py
+-rw-r--r--   0        0        0     4168 2023-07-22 13:39:33.630996 holobench-0.0.6/bencher/example/benchmark_data.py
+-rw-r--r--   0        0        0      923 2023-07-24 17:38:19.738638 holobench-0.0.6/bencher/example/example_bokeh_plotly.py
+-rw-r--r--   0        0        0     3745 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_categorical.py
+-rw-r--r--   0        0        0     1901 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_custom_sweep.py
+-rw-r--r--   0        0        0     3197 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_float2D_scatter.py
+-rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_float3D.py
+-rw-r--r--   0        0        0     2817 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_float3D_cone.py
+-rw-r--r--   0        0        0     3562 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_float_cat.py
+-rw-r--r--   0        0        0     4348 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_floats.py
+-rw-r--r--   0        0        0     4018 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_floats2D.py
+-rw-r--r--   0        0        0     5136 2023-07-24 17:38:19.738638 holobench-0.0.6/bencher/example/example_holosweep.py
+-rw-r--r--   0        0        0     1805 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/example/example_hvplot_explorer.py
+-rw-r--r--   0        0        0     2619 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/example/example_interactive.py
+-rw-r--r--   0        0        0     2416 2023-07-22 12:02:54.862576 holobench-0.0.6/bencher/example/example_kwargs.py
+-rw-r--r--   0        0        0     2431 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_pareto.py
+-rw-r--r--   0        0        0     3438 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_persistent.py
+-rw-r--r--   0        0        0     2540 2023-07-20 18:29:05.428632 holobench-0.0.6/bencher/example/example_plot_library.py
+-rw-r--r--   0        0        0     4027 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_sample_cache.py
+-rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_sample_cache_context.py
+-rw-r--r--   0        0        0    11711 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_simple.py
+-rw-r--r--   0        0        0     1525 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/example/example_simple_bool.py
+-rw-r--r--   0        0        0     1473 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_simple_cat.py
+-rw-r--r--   0        0        0     1393 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_simple_float.py
+-rw-r--r--   0        0        0     1172 2023-07-20 18:29:05.428632 holobench-0.0.6/bencher/example/example_template.py
+-rw-r--r--   0        0        0     1951 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_time_event.py
+-rw-r--r--   0        0        0     2990 2023-07-20 19:07:32.744938 holobench-0.0.6/bencher/example/example_vector.py
+-rw-r--r--   0        0        0     6718 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/example/example_workflow.py
+-rw-r--r--   0        0        0     2261 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/example/hv_bool_bug.py
+-rw-r--r--   0        0        0    10946 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/optuna_conversions.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/plotting/__init__.py
+-rw-r--r--   0        0        0     5436 2023-07-20 18:29:05.428632 holobench-0.0.6/bencher/plotting/plot_collection.py
+-rw-r--r--   0        0        0     4705 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/plotting/plot_filter.py
+-rw-r--r--   0        0        0     3579 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plotting/plot_library.py
+-rw-r--r--   0        0        0     1197 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plotting/plot_types.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/plotting/plots/__init__.py
+-rw-r--r--   0        0        0     2539 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/plotting/plots/catplot.py
+-rw-r--r--   0        0        0     3754 2023-07-20 18:29:05.428632 holobench-0.0.6/bencher/plotting/plots/heatmap.py
+-rw-r--r--   0        0        0     3821 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plotting/plots/hv_interactive.py
+-rw-r--r--   0        0        0     6359 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plotting/plots/lineplot.py
+-rw-r--r--   0        0        0      618 2023-07-20 18:29:05.432632 holobench-0.0.6/bencher/plotting/plots/plot_base.py
+-rw-r--r--   0        0        0     1616 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/plotting/plots/scatterplot.py
+-rw-r--r--   0        0        0     3830 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plotting/plots/surface.py
+-rw-r--r--   0        0        0     1194 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/plotting/plots/tables.py
+-rw-r--r--   0        0        0     5971 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plotting/plots/volume.py
+-rw-r--r--   0        0        0    11572 2023-07-24 17:38:19.738638 holobench-0.0.6/bencher/plotting_functions.py
+-rw-r--r--   0        0        0    14109 2023-07-22 09:13:13.903071 holobench-0.0.6/bencher/plt_cfg.py
+-rw-r--r--   0        0        0     2339 2023-07-16 12:36:45.478978 holobench-0.0.6/bencher/utils.py
+-rw-r--r--   0        0        0      423 2023-07-16 12:36:45.478978 holobench-0.0.6/dependencies.yaml
+-rw-r--r--   0        0        0     1045 2023-07-16 12:36:45.478978 holobench-0.0.6/package.xml
+-rw-r--r--   0        0        0     1473 2023-07-24 17:39:14.150854 holobench-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      227 2023-07-20 18:29:05.432632 holobench-0.0.6/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.6/resource/bencher
+-rw-r--r--   0        0        0       83 2023-07-16 12:36:45.478978 holobench-0.0.6/setup.cfg
+-rw-r--r--   0        0        0      628 2023-07-16 12:36:45.478978 holobench-0.0.6/setup.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.6/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.6/test/plots/__init__.py
+-rw-r--r--   0        0        0      973 2023-07-16 12:36:45.478978 holobench-0.0.6/test/plots/test_catplot.py
+-rw-r--r--   0        0        0     1330 2023-07-16 12:36:45.478978 holobench-0.0.6/test/plots/test_plots_common.py
+-rw-r--r--   0        0        0     1089 2023-07-16 12:36:45.478978 holobench-0.0.6/test/plots/test_tables.py
+-rw-r--r--   0        0        0     3497 2023-07-20 19:19:06.224197 holobench-0.0.6/test/test_bench_examples.py
+-rw-r--r--   0        0        0    16047 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_bencher.py
+-rw-r--r--   0        0        0     6150 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_combinations.py
+-rw-r--r--   0        0        0     3534 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_plot_collection.py
+-rw-r--r--   0        0        0     2772 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_plot_filter.py
+-rw-r--r--   0        0        0     1788 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_plot_library.py
+-rw-r--r--   0        0        0     5671 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_sample_cache.py
+-rw-r--r--   0        0        0     1972 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_sweep_vars.py
+-rw-r--r--   0        0        0     1207 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_utils.py
+-rw-r--r--   0        0        0     2439 2023-07-16 12:36:45.478978 holobench-0.0.6/test/test_vars.py
+-rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 holobench-0.0.6/PKG-INFO
```

### Comparing `holobench-0.0.5/.devcontainer/devcontainer.json` & `holobench-0.0.6/.devcontainer/devcontainer.json`

 * *Files 6% similar despite different names*

```diff
@@ -31,13 +31,14 @@
 			"extensions": [
 				"ms-python.python",
 				"ms-python.vscode-pylance",
 				"ms-python.pylint",
 				"njpwerner.autodocstring",
 				"charliermarsh.ruff",
 				"mhutchie.git-graph",
-				"bungcip.better-toml"
+				"bungcip.better-toml",
+				"eamodio.gitlens"
 			]
 		}
 	},
 	// "onCreateCommand": "pre-commit install-hooks"
 }
```

### Comparing `holobench-0.0.5/.github/workflows/ci.yml` & `holobench-0.0.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/.gitignore` & `holobench-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/.vscode/tasks.json` & `holobench-0.0.6/.vscode/tasks.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'tasks'": "{1: {'command': 'flit install --symlink'}}"}*

```diff
@@ -2,15 +2,15 @@
     "tasks": [
         {
             "command": "ruff . --fix && black .",
             "label": "autoformat",
             "type": "shell"
         },
         {
-            "command": "flit install",
+            "command": "flit install --symlink",
             "label": "flit install",
             "type": "shell"
         },
         {
             "command": "flit publish",
             "label": "flit publish",
             "type": "shell"
```

### Comparing `holobench-0.0.5/LICENSE` & `holobench-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/README.md` & `holobench-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/__init__.py` & `holobench-0.0.6/bencher/__init__.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/bench_cfg.py` & `holobench-0.0.6/bencher/bench_cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -544,18 +544,30 @@
         ds = self.get_hv_dataset(reduce)
         pt = ds.to(hv.Bars)
         if reduce:
             pt *= ds.to(hv.ErrorBars)
         return pt
 
     def to_nd_layout(self) -> hv.NdLayout:
-        return hv.NdLayout(self.hmap, kdims=self.hmap_kdims)
+        return hv.NdLayout(self.hmap, kdims=self.hmap_kdims).opts(
+            shared_axes=False, shared_datasource=False
+        )
 
     def to_holomap(self) -> hv.HoloMap:
-        return hv.HoloMap(self.to_nd_layout())
+        # return hv.HoloMap(self.hmap, self.hmap_kdims)
+        return hv.HoloMap(self.to_nd_layout()).opts(shared_axes=False)
+
+    def to_grid(self):
+        inputs = self.inputs_as_str()
+        if len(inputs) > 2:
+            inputs = inputs[:2]
+        return self.to_holomap().grid(inputs)
+
+    def inputs_as_str(self) -> List[str]:
+        return [i.name for i in self.input_vars]
 
 
 def describe_benchmark(bench_cfg: BenchCfg) -> str:
     """Generate a string summary of the inputs and results from a BenchCfg
 
     Args:
         bench_cfg (BenchCfg): BenchCfg to generate a summary of
```

### Comparing `holobench-0.0.5/bencher/bench_plot_server.py` & `holobench-0.0.6/bencher/bench_plot_server.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/bench_vars.py` & `holobench-0.0.6/bencher/bench_vars.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/bencher.py` & `holobench-0.0.6/bencher/bencher.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,24 +487,25 @@
             function_input_vars (List): list of function inputs as dicts
             dims_name (List[str]): names of the n-d dimension
             constant_inputs (dict): input values to keep constant
         """
         self.worker_wrapper_call_count += 1
         function_input = dict(zip(dims_name, function_input_vars))
 
+        fn_inp_with_rep = tuple(function_input.values())
+
         if constant_inputs is not None:
             function_input |= constant_inputs
 
         if bench_cfg.print_bench_inputs:
             logging.info("Bench Inputs:")
             for k, v in function_input.items():
                 logging.info(f"\t {k}:{v}")
 
         # store a tuple of the inputs as keys for a holomap
-        fn_inp_with_rep = tuple(function_input.values())
         if bench_cfg.use_sample_cache:
             # the signature is the hash of the inputs to to the function + meta variables such as repeat and time + the hash of the benchmark sweep as a whole (without the repeats hash)
             fn_inputs_sorted = list(SortedDict(function_input).items())
             function_input_signature_pure = hash_sha1((fn_inputs_sorted, bench_cfg.tag))
 
             function_input_signature_benchmark_context = hash_sha1(
                 (function_input_signature_pure, bench_cfg_sample_hash)
```

### Comparing `holobench-0.0.5/bencher/example/benchmark_data.py` & `holobench-0.0.6/bencher/example/benchmark_data.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_categorical.py` & `holobench-0.0.6/bencher/example/example_categorical.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_custom_sweep.py` & `holobench-0.0.6/bencher/example/example_custom_sweep.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_float2D_scatter.py` & `holobench-0.0.6/bencher/example/example_float2D_scatter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_float3D.py` & `holobench-0.0.6/bencher/example/example_float3D.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_float3D_cone.py` & `holobench-0.0.6/bencher/example/example_float3D_cone.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_float_cat.py` & `holobench-0.0.6/bencher/example/example_float_cat.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_floats.py` & `holobench-0.0.6/bencher/example/example_floats.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_floats2D.py` & `holobench-0.0.6/bencher/example/example_floats2D.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_holosweep.py` & `holobench-0.0.6/bencher/example/example_holosweep.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,29 +8,40 @@
 import random
 import numpy as np
 from holoviews import opts
 import panel as pn
 import holoviews as hv
 
 
+from strenum import StrEnum
+from enum import auto
+
+
+class Function(StrEnum):
+    fn_cos = auto()
+    fn_sin = auto()
+
+
 class Waves(bch.ParametrizedSweep):
     phase = bch.FloatSweep(
-        default=0, bounds=[0, math.pi], doc="Input angle", units="rad", samples=5
+        default=0, bounds=[0, math.pi], doc="Input angle", units="rad", samples=2
     )
 
-    freq = bch.FloatSweep(default=0, bounds=[0, math.pi], doc="Input angle", units="rad", samples=4)
+    freq = bch.FloatSweep(default=0, bounds=[0, math.pi], doc="Input angle", units="rad", samples=2)
 
     theta = bch.FloatSweep(
         default=0, bounds=[0, math.pi], doc="Input angle", units="rad", samples=10
     )
 
+    compute_fn = bch.EnumSweep(Function)
+
     noisy = bch.BoolSweep(default=True)
 
     out_sin = bch.ResultVar(units="v", doc="sin of theta with some noise")
-    out_cos = bch.ResultVar(units="v", doc="cos of theta with some noise")
+    # out_cos = bch.ResultVar(units="v", doc="cos of theta with some noise")
 
     out_sum = bch.ResultVar(units="v", doc="The sum")
 
     def calc(self, phase=0.0, freq=1.0, theta=0.0, noisy=True) -> dict:
         if noisy:
             noise = 1.0
         else:
@@ -43,56 +54,81 @@
 
         pt = hv.Text(0, 0, f"{phase}\n{freq}\n {theta}")
         pt *= hv.Ellipse(0, 0, 1)
         pt = hv.Points([theta, self.out_sin])
 
         return self.get_results_values_as_dict(holomap=pt)
 
-    def calc_vec(self, phase=0.0, freq=1.0, noisy=True) -> dict:
+    def calc_vec(
+        self, phase=0.0, freq=1.0, noisy=True, compute_fn: Function = Function.fn_sin
+    ) -> dict:
         if noisy:
             noise = 1.0
         else:
             noise = 0.0
 
         theta = np.arange(0, 6, 0.1)
-        dat = np.sin(phase + freq * theta) + random.uniform(0, noise)
+
+        match compute_fn:
+            case Function.fn_sin:
+                dat = np.sin(phase + freq * theta) + random.uniform(0, noise)
+            case Function.fn_cos:
+                dat = np.cos(phase + freq * theta) + random.uniform(0, noise)
 
         self.out_sum = sum(dat)
         hmap = hv.Curve((theta, dat), "theta", "voltage")
-        return self.get_results_values_as_dict(holomap=hmap)
+
+        pt = hv.Text(0, 0, f"{compute_fn}\n{phase}\n{freq}")
+        pt *= hv.Ellipse(0, 0, 1)
+
+        # pt = hv.Image(np.ones([100, 100]) * freq * phase * 100)
+        # pt = hv.Points([theta, self.out_sin])
+
+        return self.get_results_values_as_dict(holomap=pt)
 
 
 if __name__ == "__main__":
-    opts.defaults(
-        # opts.NdLayout(shared_axes=False, shared_datasource=False, width=500),
-        opts.Overlay(width=500, legend_position="right"),
-    )
+    # opts.defaults(
+    #     # opts.NdLayout(shared_axes=False, shared_datasource=False, width=500),
+    #     opts.Overlay(width=500, legend_position="right"),
+    # )
     wv = Waves()
 
+    # hv.extension("plotly", "bokeh")
+
     bch_wv = bch.Bench("waves", wv.calc, plot_lib=None)
 
-    res = bch_wv.plot_sweep(
-        "phase",
-        # input_vars=[wv.param.theta, wv.param.freq, wv.param.phase, wv.param.noisy],
-        input_vars=[wv.param.theta, wv.param.freq, wv.param.phase],
-        result_vars=[wv.param.out_sin],
-        run_cfg=bch.BenchRunCfg(repeats=3),
-    )
+    # res = bch_wv.plot_sweep(
+    #     "phase",
+    #     # input_vars=[wv.param.theta, wv.param.freq, wv.param.phase, wv.param.noisy],
+    #     input_vars=[wv.param.theta, wv.param.freq, wv.param.phase],
+    #     result_vars=[wv.param.out_sin],
+    #     run_cfg=bch.BenchRunCfg(repeats=3),
+    # )
 
-    bch_wv.append(res.to_curve().layout("freq"))
+    # bch_wv.append(res.to_curve().layout("freq"))
 
     bch_wv.worker = wv.calc_vec
     res = bch_wv.plot_sweep(
         "holo",
-        input_vars=[wv.param.freq, wv.param.phase],
+        input_vars=[wv.param.freq, wv.param.phase, wv.param.compute_fn],
         result_vars=[wv.param.out_sum],
-        run_cfg=bch.BenchRunCfg(repeats=3),
+        run_cfg=bch.BenchRunCfg(repeats=3, auto_plot=False),
     )
 
-    bch_wv.append(res.to_holomap())
+    # hv.extension("bokeh")
+
+    # bch_wv.append(res.to_holomap().opts(backend="bokeh"))
+
+    # bch_wv.append(hv.HoloMap(res.hmap, res.hmap_kdims).opts(backend="bokeh"))
+    # bch_wv.plots_instance.append(res.to_grid().opts(backend="bokeh"))
+    # bch_wv.append(res.to_holomap().layout().)
+
+    # bch_wv.append(res.to_holomap())
+    bch_wv.append(res.to_grid())
 
     # bch_wv.append(ndlay.grid("freq"))
     bch_wv.plot()
 
     # bch_wv.append(res.to_curve().layout())
 
     # res = bch_wv.plot_sweep(
```

### Comparing `holobench-0.0.5/bencher/example/example_hvplot_explorer.py` & `holobench-0.0.6/bencher/example/example_hvplot_explorer.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_interactive.py` & `holobench-0.0.6/bencher/example/example_interactive.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_kwargs.py` & `holobench-0.0.6/bencher/example/example_kwargs.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_pareto.py` & `holobench-0.0.6/bencher/example/example_pareto.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_persistent.py` & `holobench-0.0.6/bencher/example/example_persistent.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_plot_library.py` & `holobench-0.0.6/bencher/example/example_plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_sample_cache.py` & `holobench-0.0.6/bencher/example/example_sample_cache.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_sample_cache_context.py` & `holobench-0.0.6/bencher/example/example_sample_cache_context.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_simple.py` & `holobench-0.0.6/bencher/example/example_simple.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_simple_bool.py` & `holobench-0.0.6/bencher/example/example_simple_bool.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_simple_cat.py` & `holobench-0.0.6/bencher/example/example_simple_cat.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_simple_float.py` & `holobench-0.0.6/bencher/example/example_simple_float.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_template.py` & `holobench-0.0.6/bencher/example/example_template.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_time_event.py` & `holobench-0.0.6/bencher/example/example_time_event.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_vector.py` & `holobench-0.0.6/bencher/example/example_vector.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/example_workflow.py` & `holobench-0.0.6/bencher/example/example_workflow.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/example/hv_bool_bug.py` & `holobench-0.0.6/bencher/example/hv_bool_bug.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/optuna_conversions.py` & `holobench-0.0.6/bencher/optuna_conversions.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plot_collection.py` & `holobench-0.0.6/bencher/plotting/plot_collection.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plot_filter.py` & `holobench-0.0.6/bencher/plotting/plot_filter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plot_library.py` & `holobench-0.0.6/bencher/plotting/plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plot_types.py` & `holobench-0.0.6/bencher/plotting/plot_types.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plots/catplot.py` & `holobench-0.0.6/bencher/plotting/plots/catplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plots/heatmap.py` & `holobench-0.0.6/bencher/plotting/plots/heatmap.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plots/hv_interactive.py` & `holobench-0.0.6/bencher/plotting/plots/hv_interactive.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plots/lineplot.py` & `holobench-0.0.6/bencher/plotting/plots/lineplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plots/plot_base.py` & `holobench-0.0.6/bencher/plotting/plots/plot_base.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plots/scatterplot.py` & `holobench-0.0.6/bencher/plotting/plots/scatterplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plots/surface.py` & `holobench-0.0.6/bencher/plotting/plots/surface.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plots/tables.py` & `holobench-0.0.6/bencher/plotting/plots/tables.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting/plots/volume.py` & `holobench-0.0.6/bencher/plotting/plots/volume.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/plotting_functions.py` & `holobench-0.0.6/bencher/plotting_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 from holoviews import opts
 
 from bencher.bench_cfg import BenchCfg, PltCfgBase
 from bencher.bench_vars import ParametrizedSweep, ResultList, ResultVar, ResultVec
 import plotly.graph_objs as go
 
 
-hv.extension("plotly")
+# hv.extension("plotly")
+
+
+hv.extension("bokeh", "plotly")
 
 
 def wrap_long_time_labels(bench_cfg: BenchCfg) -> BenchCfg:
     """Takes a benchCfg and wraps any index labels that are too long to be plotted easily
 
     Args:
         bench_cfg (BenchCfg):
@@ -308,39 +311,61 @@
         bench_cfg (BenchCfg): description of benchmark
         rv (ParametrizedSweep): result variable to plot
         xr_cfg (PltCfgBase): config of x,y variables
     Returns:
         pn.pane.holoview: A 2d surface plot as a holoview in a pane
     """
 
-    hv.extension("plotly")
-
     bench_cfg = wrap_long_time_labels(bench_cfg)
 
     alpha = 0.3
 
     da = bench_cfg.ds[rv.name]
 
     mean = da.mean("repeat")
 
-    opts.defaults(
-        opts.Surface(
-            colorbar=True,
-            width=800,
-            height=800,
-            zlabel=xr_cfg.zlabel,
-            title=xr_cfg.title,
-            # image_rtol=0.002,
-        )
-    )
+    # opts.defaults(
+    #     opts.Surface(
+    #         backend=bke
+    #         # colorbar=True,
+    #         # width=800,
+    #         # height=800,
+    #         # zlabel=xr_cfg.zlabel,
+    #         # title=xr_cfg.title,
+    #         # image_rtol=0.002,
+    #     )
+    # )
     # TODO a warning suggests setting this parameter, but it does not seem to help as expected, leaving here to fix in the future
     # hv.config.image_rtol = 1.0
 
     ds = hv.Dataset(mean)
+    # return hv.output(ds.to(hv.Surface).opts(backend=bke), backend=bke)
     surface = ds.to(hv.Surface)
 
+    # if bench_cfg.repeats > 1:
+    #     std_dev = da.std("repeat")
+    #     upper = hv.Dataset(mean + std_dev).to(hv.Surface).opts(alpha=alpha, colorbar=False)
+    #     lower = hv.Dataset(mean - std_dev).to(hv.Surface).opts(alpha=alpha, colorbar=False)
+    #     return surface * upper * lower
+    # return surface
+
     if bench_cfg.repeats > 1:
         std_dev = da.std("repeat")
-        upper = hv.Dataset(mean + std_dev).to(hv.Surface).opts(alpha=alpha, colorbar=False)
-        lower = hv.Dataset(mean - std_dev).to(hv.Surface).opts(alpha=alpha, colorbar=False)
-        return surface * upper * lower
-    return surface
+        surface *= (
+            hv.Dataset(mean + std_dev)
+            .to(hv.Surface)
+            .opts(alpha=alpha, colorbar=False, backend="plotly")
+        )
+        surface *= (
+            hv.Dataset(mean - std_dev)
+            .to(hv.Surface)
+            .opts(alpha=alpha, colorbar=False, backend="plotly")
+        )
+    return pn.Column(
+        # surface
+        hv.render(
+            surface.opts(
+                width=800, height=800, zlabel=xr_cfg.zlabel, title=xr_cfg.title, backend="plotly"
+            ),
+            backend="plotly",
+        )
+    )
```

### Comparing `holobench-0.0.5/bencher/plt_cfg.py` & `holobench-0.0.6/bencher/plt_cfg.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/bencher/utils.py` & `holobench-0.0.6/bencher/utils.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/package.xml` & `holobench-0.0.6/package.xml`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/pyproject.toml` & `holobench-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name =  "holobench"
-version = "0.0.5"
+version = "0.0.6"
 
 authors = [
     {name = "Austin Gregg-Smith", email = "blooop@gmail.com"},
 ]
 description = "A package for benchmarking the performance of arbitrary functions"
 readme = "README.md"
```

### Comparing `holobench-0.0.5/setup.py` & `holobench-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/plots/test_catplot.py` & `holobench-0.0.6/test/plots/test_catplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/plots/test_plots_common.py` & `holobench-0.0.6/test/plots/test_plots_common.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/plots/test_tables.py` & `holobench-0.0.6/test/plots/test_tables.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/test_bench_examples.py` & `holobench-0.0.6/test/test_bench_examples.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/test_bencher.py` & `holobench-0.0.6/test/test_bencher.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/test_combinations.py` & `holobench-0.0.6/test/test_combinations.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/test_plot_collection.py` & `holobench-0.0.6/test/test_plot_collection.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/test_plot_filter.py` & `holobench-0.0.6/test/test_plot_filter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/test_plot_library.py` & `holobench-0.0.6/test/test_plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/test_sample_cache.py` & `holobench-0.0.6/test/test_sample_cache.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/test_sweep_vars.py` & `holobench-0.0.6/test/test_sweep_vars.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/test_utils.py` & `holobench-0.0.6/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/test/test_vars.py` & `holobench-0.0.6/test/test_vars.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.5/PKG-INFO` & `holobench-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holobench
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for benchmarking the performance of arbitrary functions
 Author-email: Austin Gregg-Smith <blooop@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: holoviews[reccomended]
 Requires-Dist: hvplot==0.8.4
 Requires-Dist: diskcache
```

