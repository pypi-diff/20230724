# Comparing `tmp/sb-arch-opt-1.1.4.tar.gz` & `tmp/sb-arch-opt-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sb-arch-opt-1.1.4.tar", last modified: Sat Jul  8 19:24:10 2023, max compression
+gzip compressed data, was "sb-arch-opt-1.1.5.tar", last modified: Mon Jul 24 09:48:06 2023, max compression
```

## Comparing `sb-arch-opt-1.1.4.tar` & `sb-arch-opt-1.1.5.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.226050 sb-arch-opt-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-08 19:24:10.226050 sb-arch-opt-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.214050 sb-arch-opt-1.1.4/sb_arch_opt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt/algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/hc_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    33800 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/infill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt/algo/botorch_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/botorch_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/botorch_interface/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/botorch_interface/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt/algo/hebo_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/hebo_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/hebo_interface/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/hebo_interface/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/md_mating.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/random_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/storage_restart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt/algo/segomoe_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/segomoe_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/segomoe_interface/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/segomoe_interface/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.222050 sb-arch-opt-1.1.4/sb_arch_opt/algo/smarty_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/smarty_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/smarty_interface/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/smarty_interface/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.222050 sb-arch-opt-1.1.4/sb_arch_opt/algo/tpe_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/tpe_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/tpe_interface/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.222050 sb-arch-opt-1.1.4/sb_arch_opt/algo/trieste_interface/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/trieste_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17309 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/trieste_interface/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/algo/trieste_interface/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24809 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/design_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/design_space_explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/pareto_front.py
--rw-r--r--   0 runner    (1001) docker     (123)    17454 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.222050 sb-arch-opt-1.1.4/sb_arch_opt/problems/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/constrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/gnc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21192 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/hidden_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    48482 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/md_mo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/problems_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/problems/turbofan_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.222050 sb-arch-opt-1.1.4/sb_arch_opt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.226050 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_arch_sbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_hebo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_pymoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_segomoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_smarty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_tpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_trieste.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.226050 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_constrained.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_gnc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_hidden_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_md_mo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_turbofan_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/test_design_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/test_design_space_explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/tests/test_tutorials.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/sb_arch_opt/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:24:10.218050 sb-arch-opt-1.1.4/sb_arch_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-08 19:24:10.000000 sb-arch-opt-1.1.4/sb_arch_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-08 19:24:10.000000 sb-arch-opt-1.1.4/sb_arch_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 19:24:10.000000 sb-arch-opt-1.1.4/sb_arch_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-08 19:24:10.000000 sb-arch-opt-1.1.4/sb_arch_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-08 19:24:10.000000 sb-arch-opt-1.1.4/sb_arch_opt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 19:24:10.226050 sb-arch-opt-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-08 19:23:58.000000 sb-arch-opt-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.166455 sb-arch-opt-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-24 09:48:06.166455 sb-arch-opt-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.158455 sb-arch-opt-1.1.5/sb_arch_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.158455 sb-arch-opt-1.1.5/sb_arch_opt/algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.158455 sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/hc_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33800 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/infill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.158455 sb-arch-opt-1.1.5/sb_arch_opt/algo/botorch_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/botorch_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/botorch_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/botorch_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.158455 sb-arch-opt-1.1.5/sb_arch_opt/algo/hebo_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/hebo_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/hebo_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/hebo_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.158455 sb-arch-opt-1.1.5/sb_arch_opt/algo/pymoo_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/pymoo_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/pymoo_interface/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/pymoo_interface/md_mating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/pymoo_interface/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/pymoo_interface/random_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/pymoo_interface/storage_restart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.162455 sb-arch-opt-1.1.5/sb_arch_opt/algo/segomoe_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/segomoe_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/segomoe_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/segomoe_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.162455 sb-arch-opt-1.1.5/sb_arch_opt/algo/smarty_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/smarty_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/smarty_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/smarty_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.162455 sb-arch-opt-1.1.5/sb_arch_opt/algo/tpe_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/tpe_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/tpe_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.162455 sb-arch-opt-1.1.5/sb_arch_opt/algo/trieste_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/trieste_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/trieste_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/algo/trieste_interface/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24809 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/design_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18885 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/design_space_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/pareto_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17454 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.162455 sb-arch-opt-1.1.5/sb_arch_opt/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/problems/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/problems/constrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/problems/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/problems/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/problems/gnc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21192 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/problems/hidden_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48482 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/problems/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/problems/md_mo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/problems/problems_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/problems/turbofan_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.162455 sb-arch-opt-1.1.5/sb_arch_opt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.166455 sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_arch_sbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_hebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_pymoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_segomoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_smarty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_tpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_trieste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.166455 sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_constrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_gnc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_hidden_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_md_mo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_turbofan_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/test_design_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/test_design_space_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16236 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/tests/test_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/sb_arch_opt/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:48:06.158455 sb-arch-opt-1.1.5/sb_arch_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-24 09:48:06.000000 sb-arch-opt-1.1.5/sb_arch_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-24 09:48:06.000000 sb-arch-opt-1.1.5/sb_arch_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:48:06.000000 sb-arch-opt-1.1.5/sb_arch_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-24 09:48:06.000000 sb-arch-opt-1.1.5/sb_arch_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 09:48:06.000000 sb-arch-opt-1.1.5/sb_arch_opt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:48:06.166455 sb-arch-opt-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-24 09:47:54.000000 sb-arch-opt-1.1.5/setup.py
```

### Comparing `sb-arch-opt-1.1.4/LICENSE` & `sb-arch-opt-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/PKG-INFO` & `sb-arch-opt-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sb-arch-opt
-Version: 1.1.4
+Version: 1.1.5
 Summary: SBArchOpt: Surrogate-Based Architecture Optimization
 Author: Jasper Bussemaker
 Author-email: jasper.bussemaker@dlr.de
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sb-arch-opt-1.1.4/README.md` & `sb-arch-opt-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/algo.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/algo.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,19 +46,20 @@
 from pymoo.util.normalization import Normalization
 from pymoo.core.initialization import Initialization
 from pymoo.core.duplicate import DuplicateElimination
 from pymoo.termination.max_gen import MaximumGenerationTermination
 from pymoo.termination.default import DefaultMultiObjectiveTermination, DefaultSingleObjectiveTermination
 from pymoo.optimize import minimize
 
+from sb_arch_opt.algo.arch_sbo.infill import *
+from sb_arch_opt.algo.arch_sbo.models import *
+from sb_arch_opt.algo.arch_sbo.hc_strategy import *
+
 try:
     from smt.surrogate_models.surrogate_model import SurrogateModel
-    from sb_arch_opt.algo.arch_sbo.infill import *
-    from sb_arch_opt.algo.arch_sbo.models import *
-    from sb_arch_opt.algo.arch_sbo.hc_strategy import *
 except ImportError:
     pass
 
 __all__ = ['InfillAlgorithm', 'SBOInfill', 'SurrogateInfillCallback', 'SurrogateInfillOptimizationProblem']
 
 log = logging.getLogger('sb_arch_opt.sbo')
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/api.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/hc_strategy.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/hc_strategy.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/infill.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/infill.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/metrics.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/metrics.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/arch_sbo/models.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/arch_sbo/models.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/botorch_interface/algo.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/botorch_interface/algo.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     - https://ax.dev/tutorials/gpei_hartmann_service.html#Special-Cases
     """
 
     def __init__(self, problem: ArchOptProblemBase):
         check_dependencies()
         self._problem = problem
 
-    def get_optimization_loop(self, n_init: int, n_infill: int) -> 'OptimizationLoop':
+    def get_optimization_loop(self, n_init: int, n_infill: int, seed: int = None) -> 'OptimizationLoop':
         experiment = self.get_experiment()
         n_eval_total = n_init+n_infill
         generation_strategy = choose_generation_strategy(
             search_space=experiment.search_space,
             experiment=experiment,
             num_trials=n_eval_total,
             num_initialization_trials=n_init,
@@ -74,14 +74,15 @@
         )
 
         return OptimizationLoop(
             experiment=experiment,
             evaluation_function=self.evaluate,
             total_trials=n_eval_total,
             generation_strategy=generation_strategy,
+            random_seed=seed,
         )
 
     def get_search_space(self) -> 'SearchSpace':
         """Gets the search space as defined by the underlying problem"""
         parameters = []
         for i, var_def in enumerate(self._problem.des_vars):
             name = f'x{i}'
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/botorch_interface/api.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/botorch_interface/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/hebo_interface/algo.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/hebo_interface/algo.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,21 +52,25 @@
 
 
 class HEBOArchOptInterface:
     """
     Interface class to HEBO algorithm.
     """
 
-    def __init__(self, problem: ArchOptProblemBase, n_init: int):
+    def __init__(self, problem: ArchOptProblemBase, n_init: int, seed: int = None):
         check_dependencies()
         self._problem = problem
         self._n_init = n_init
         self._optimizer = None
         self._design_space = None
 
+        self._seed = seed
+        if seed is not None:
+            np.random.seed(seed)
+
     @property
     def problem(self):
         return self._problem
 
     @property
     def n_batch(self):
         n_batch = self._problem.get_n_batch_evaluate()
@@ -97,15 +101,16 @@
             self._design_space = DesignSpace().parse(hebo_var_defs)
         return self._design_space
 
     @property
     def optimizer(self) -> 'AbstractOptimizer':
         if self._optimizer is None:
             if self._problem.n_obj == 1 and self._problem.n_ieq_constr == 0:
-                self._optimizer = HEBO(self.design_space, model_name='gpy', rand_sample=self._n_init)
+                self._optimizer = HEBO(self.design_space, model_name='gpy', rand_sample=self._n_init,
+                                       scramble_seed=self._seed)
             else:
                 self._optimizer = GeneralBO(self.design_space, num_obj=self._problem.n_obj,
                                             num_constr=self._problem.n_ieq_constr, rand_sample=self._n_init,
                                             model_config={'num_epochs': 100})
         return self._optimizer
 
     @property
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/hebo_interface/api.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/hebo_interface/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,13 +25,13 @@
 from sb_arch_opt.problem import ArchOptProblemBase
 from sb_arch_opt.algo.hebo_interface.algo import *
 
 
 __all__ = ['get_hebo_optimizer', 'HAS_HEBO']
 
 
-def get_hebo_optimizer(problem: ArchOptProblemBase, n_init: int):
+def get_hebo_optimizer(problem: ArchOptProblemBase, n_init: int, seed: int = None):
     """
     Gets the main interface to HEBO. Use the `optimize` method to run the DOE and infill loops.
     """
     check_dependencies()
-    return HEBOArchOptInterface(problem, n_init)
+    return HEBOArchOptInterface(problem, n_init, seed=seed)
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/api.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/pymoo_interface/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/md_mating.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/pymoo_interface/md_mating.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/metrics.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/pymoo_interface/metrics.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/random_search.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/pymoo_interface/random_search.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/pymoo_interface/storage_restart.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/pymoo_interface/storage_restart.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/segomoe_interface/algo.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/segomoe_interface/algo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/segomoe_interface/api.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/segomoe_interface/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/smarty_interface/algo.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/smarty_interface/algo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/smarty_interface/api.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/smarty_interface/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/tpe_interface/api.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/tpe_interface/api.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/trieste_interface/algo.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/trieste_interface/algo.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     Constraints: https://secondmind-labs.github.io/trieste/1.0.0/notebooks/inequality_constraints.html
     Multi-objective: https://secondmind-labs.github.io/trieste/1.0.0/notebooks/multi_objective_ehvi.html
     Hidden constraints: https://secondmind-labs.github.io/trieste/1.0.0/notebooks/failure_ego.html
     Ask-tell: https://secondmind-labs.github.io/trieste/1.0.0/notebooks/ask_tell_optimization.html
     """
 
     def __init__(self, problem: ArchOptProblemBase, n_init: int, n_infill: int, pof=.5,
-                 rule: 'AcquisitionRule' = None):
+                 rule: 'AcquisitionRule' = None, seed: int = None):
         check_dependencies()
         self._problem = problem
         self.pof = pof
         self._rule = rule
         self.n_init = n_init
         self.n_infill = n_infill
         self.eval_might_fail = problem.might_have_hidden_constraints()
@@ -107,14 +107,18 @@
         super().__init__(observer, search_space)
 
         self._results_folder = None
         self._datasets = None
         self._models = None
         self._state = None
 
+        if seed is not None:
+            np.random.seed(seed)
+            tf.random.set_seed(seed)
+
     @property
     def search_space(self):
         return self._search_space
 
     @property
     def observer(self) -> 'MultiObserver':
         return self._observer
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/algo/trieste_interface/api.py` & `sb-arch-opt-1.1.5/sb_arch_opt/algo/trieste_interface/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,13 +25,13 @@
 from sb_arch_opt.problem import ArchOptProblemBase
 from sb_arch_opt.algo.trieste_interface.algo import *
 
 
 __all__ = ['get_trieste_optimizer', 'HAS_TRIESTE']
 
 
-def get_trieste_optimizer(problem: ArchOptProblemBase, n_init: int, n_infill: int, pof: float = .5):
+def get_trieste_optimizer(problem: ArchOptProblemBase, n_init: int, n_infill: int, pof: float = .5, seed: int = None):
     """
     Gets the main interface to Trieste. Use the `run_optimization` method to run the DOE and infill loops.
     """
     check_dependencies()
-    return ArchOptBayesianOptimizer(problem, n_init, n_infill, pof=pof)
+    return ArchOptBayesianOptimizer(problem, n_init, n_infill, pof=pof, seed=seed)
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/design_space.py` & `sb-arch-opt-1.1.5/sb_arch_opt/design_space.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/design_space_explicit.py` & `sb-arch-opt-1.1.5/sb_arch_opt/design_space_explicit.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import numpy as np
 from typing import *
 from sb_arch_opt.design_space import ArchDesignSpace
+from sb_arch_opt.util import get_np_random_singleton
 from pymoo.core.variable import Variable, Real, Integer, Choice
 
 from ConfigSpace.util import generate_grid, get_random_neighbor
 from ConfigSpace.exceptions import ForbiddenValueError
 from ConfigSpace.configuration_space import ConfigurationSpace, Configuration
 from ConfigSpace.hyperparameters import UniformFloatHyperparameter, UniformIntegerHyperparameter, \
     CategoricalHyperparameter
@@ -429,12 +430,18 @@
         # Integer values are normalized similarly to what we do in round_x_discrete
         x[:, is_int_mask] = np.round(x[:, is_int_mask]*(xu[is_int_mask]-xl[is_int_mask]+.9999)+xl[is_int_mask]-.49999)
 
 
 class NoDefaultConfigurationSpace(ConfigurationSpace):
     """ConfigurationSpace that supports no default configuration"""
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        if kwargs.get('seed') is None:
+            self.random = get_np_random_singleton()
+
     def get_default_configuration(self, *args, **kwargs):
         raise NotImplementedError
 
     def _check_default_configuration(self, *args, **kwargs):
         pass
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/pareto_front.py` & `sb-arch-opt-1.1.5/sb_arch_opt/pareto_front.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/problem.py` & `sb-arch-opt-1.1.5/sb_arch_opt/problem.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/problems/assignment.py` & `sb-arch-opt-1.1.5/sb_arch_opt/problems/assignment.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/problems/constrained.py` & `sb-arch-opt-1.1.5/sb_arch_opt/problems/constrained.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/problems/continuous.py` & `sb-arch-opt-1.1.5/sb_arch_opt/problems/continuous.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/problems/discrete.py` & `sb-arch-opt-1.1.5/sb_arch_opt/problems/discrete.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/problems/gnc.py` & `sb-arch-opt-1.1.5/sb_arch_opt/problems/gnc.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/problems/hidden_constraints.py` & `sb-arch-opt-1.1.5/sb_arch_opt/problems/hidden_constraints.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/problems/hierarchical.py` & `sb-arch-opt-1.1.5/sb_arch_opt/problems/hierarchical.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/problems/md_mo.py` & `sb-arch-opt-1.1.5/sb_arch_opt/problems/md_mo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/problems/problems_base.py` & `sb-arch-opt-1.1.5/sb_arch_opt/problems/problems_base.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/problems/turbofan_arch.py` & `sb-arch-opt-1.1.5/sb_arch_opt/problems/turbofan_arch.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/sampling.py` & `sb-arch-opt-1.1.5/sb_arch_opt/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from pymoo.core.sampling import Sampling
 from pymoo.core.initialization import Initialization
 from pymoo.operators.sampling.rnd import FloatRandomSampling
 from pymoo.core.duplicate import DefaultDuplicateElimination
 from pymoo.operators.sampling.lhs import sampling_lhs_unit
 
 from sb_arch_opt.problem import ArchOptProblemBase, ArchOptRepair
+from sb_arch_opt.util import get_np_random_singleton
 
 __all__ = ['HierarchicalExhaustiveSampling', 'HierarchicalSampling',
            'get_init_sampler', 'LargeDuplicateElimination', 'TrailRepairWarning']
 
 log = logging.getLogger('sb_arch_opt.sampling')
 
 
@@ -185,22 +186,26 @@
 
     The first way yields better results, as there is an even chance of selecting every valid discrete design vector,
     however it takes more memory and might be too much for very large design spaces.
     """
 
     _n_comb_gen_all_max = 100e3
 
-    def __init__(self, repair: Repair = None, sobol=True):
+    def __init__(self, repair: Repair = None, sobol=True, seed=None):
         if repair is None:
             repair = ArchOptRepair()
         self._repair = repair
         self.sobol = sobol
         self.n_iter = 10
         super().__init__()
 
+        # Simply set the seed on the global numpy instance
+        if seed is not None:
+            np.random.seed(seed)
+
     def _do(self, problem, n_samples, **kwargs):
         x_sampled, _ = self.sample_get_x(problem, n_samples)
         return x_sampled
 
     def sample_get_x(self, problem: ArchOptProblemBase, n_samples: int) -> Tuple[np.ndarray, np.ndarray]:
         """
         Sample design points using the hierarchical sampling algorithm and return is_active information.
@@ -419,15 +424,16 @@
         More info: https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.qmc.Sobol.html
         """
 
         # Get the power of 2 for generating samples (generating a power of 2 gives points with the lowest discrepancy)
         pow2 = int(np.ceil(np.log2(n_samples)))
 
         # Sample points and only return the amount needed
-        x = Sobol(d=n_dims or 1).random_base2(m=pow2)
+        global_rng = get_np_random_singleton()
+        x = Sobol(d=n_dims or 1, seed=global_rng).random_base2(m=pow2)
         x = x[:n_samples, :]
         return x[:, 0] if n_dims is None else x
 
     @classmethod
     def _choice(cls, n_choose, n_from, replace=True, sobol=False):
         if sobol:
             return cls._sobol_choice(n_choose, n_from, replace=replace)
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_arch_sbo.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_arch_sbo.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,24 @@
 
     sbo = get_arch_sbo_rbf(init_size=10)
     result = minimize(problem, sbo, termination=('n_eval', 12), verbose=True, progress=True)
     assert len(result.pop) == 12
 
 
 @check_dependency()
+def test_arch_sbo_rbf_seed(problem: ArchOptProblemBase):
+    result = minimize(problem, get_arch_sbo_rbf(init_size=10), termination=('n_eval', 12), seed=42)
+    x1 = result.pop.get('X')
+
+    result = minimize(problem, get_arch_sbo_rbf(init_size=10), termination=('n_eval', 12), seed=42)
+    x2 = result.pop.get('X')
+    assert np.all(x1 == x2)
+
+
+@check_dependency()
 def test_arch_sbo_rbf_termination(problem: ArchOptProblemBase):
     assert HAS_ARCH_SBO
 
     sbo = get_arch_sbo_rbf(init_size=10)
     termination = get_sbo_termination(n_max_infill=12, tol=1e-3)
     assert minimize(problem, sbo, termination=termination, verbose=True, progress=True)
 
@@ -129,14 +139,24 @@
 
     sbo = get_arch_sbo_gp(problem, init_size=10)
     result = minimize(problem, sbo, termination=('n_eval', 11))
     assert len(result.pop) == 11
 
 
 @check_dependency()
+def test_arch_sbo_gp_seed(problem: ArchOptProblemBase):
+    result = minimize(problem, get_arch_sbo_gp(problem, init_size=10), termination=('n_eval', 11), seed=42)
+    x1 = result.pop.get('X')
+
+    result = minimize(problem, get_arch_sbo_gp(problem, init_size=10), termination=('n_eval', 11), seed=42)
+    x2 = result.pop.get('X')
+    assert np.all(x1 == x2)
+
+
+@check_dependency()
 def test_arch_sbo_gp_pls():
     assert HAS_ARCH_SBO
 
     problem = HierarchicalGoldstein()
     sbo = get_arch_sbo_gp(problem, init_size=10, kpls_n_dim=3)
     result = minimize(problem, sbo, termination=('n_eval', 12))
     assert len(result.pop) == 12
@@ -183,14 +203,15 @@
             sbo.initialize_from_previous_results(problem, tmp_folder)
 
             n_eval = 10+(i+1)
             result = minimize(problem, sbo, termination=('n_eval', n_eval))
             assert len(result.pop) == 10+(i+1)
 
 
+@check_dependency()
 def test_partial_restart():
     with tempfile.TemporaryDirectory() as tmp_folder:
         for i in range(100):
             try:
                 problem = CrashingProblem()
                 pop = load_from_previous_results(problem, tmp_folder)
                 n_evaluated = 0
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_botorch.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_botorch.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 check_dependency = lambda: pytest.mark.skipif(not HAS_BOTORCH, reason='BoTorch/Ax dependencies not installed')
 
 
 @check_dependency()
 def test_simple(problem: ArchOptProblemBase):
     interface = get_botorch_interface(problem)
-    opt = interface.get_optimization_loop(n_init=10, n_infill=1)
+    opt = interface.get_optimization_loop(n_init=10, n_infill=1, seed=42)
     opt.full_run()
 
     pop = interface.get_population(opt)
     assert len(pop) == 11
 
 
 @check_dependency()
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_hebo.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_hebo.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 @check_dependency()
 def test_simple():
     assert HAS_HEBO
 
     n_init = 30
-    hebo = get_hebo_optimizer(MOZDT1(), n_init=30)
+    hebo = get_hebo_optimizer(MOZDT1(), n_init=30, seed=42)
     hebo.optimize(n_infill=2)
 
     pop = hebo.pop
     assert len(pop) == n_init+2
 
 
 @check_dependency()
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_pymoo.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_pymoo.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,24 @@
 
 
 def test_termination(problem: ArchOptProblemBase):
     nsga2 = get_nsga2(pop_size=100)
     assert minimize(problem, nsga2, get_default_termination(problem, tol=1e-4), verbose=True, progress=True)
 
 
+def test_seed(problem: ArchOptProblemBase):
+    nsga2 = get_nsga2(pop_size=100)
+    result1 = minimize(problem, nsga2, termination=('n_gen', 20), seed=42)
+
+    nsga2 = get_nsga2(pop_size=100)
+    result2 = minimize(problem, nsga2, termination=('n_gen', 20), seed=42)
+
+    assert np.all(result1.pop.get('X') == result2.pop.get('X'))
+
+
 def test_failing_evaluations(failing_problem: ArchOptProblemBase):
     nsga2 = get_nsga2(pop_size=100)
     assert minimize(failing_problem, nsga2, termination=('n_gen', 10), verbose=True, progress=True)
 
 
 class DummyResultSavingProblem(ArchOptProblemBase):
 
@@ -99,28 +109,28 @@
             assert isinstance(nsga2.callback, ResultsStorageCallback)
 
             if i > 2:
                 problem.provide_previous_results = False
             assert initialize_from_previous_results(nsga2, problem, tmp_folder) == (i > 0)
             if i > 0:
                 assert isinstance(nsga2.initialization.sampling, Population)
-                assert len(nsga2.initialization.sampling) - (100+2*100*i) < 20
+                assert len(nsga2.initialization.sampling) == 100+2*100*i
 
-            minimize(problem, nsga2, termination=('n_gen', 3), copy_algorithm=False)
+            minimize(problem, nsga2, termination=('n_gen', 3), copy_algorithm=False, seed=42)
             assert os.path.exists(os.path.join(tmp_folder, 'pymoo_results.pkl'))
             assert os.path.exists(os.path.join(tmp_folder, 'pymoo_population.pkl'))
             assert os.path.exists(os.path.join(tmp_folder, 'pymoo_population.csv'))
             assert os.path.exists(os.path.join(tmp_folder, 'pymoo_population_cumulative.pkl'))
             assert os.path.exists(os.path.join(tmp_folder, 'pymoo_population_cumulative.csv'))
 
             assert problem.n_eval == 3+2*i  # 3 for initial population, 2 for next because the first is a restart
             assert problem.n_stored == 6+5*i
 
             n_cumulative = load_from_previous_results(problem, tmp_folder)
-            assert abs(len(n_cumulative) - (100+2*100*(i+1))) < 20
+            assert len(n_cumulative) == 100+2*100*(i+1)
 
 
 def test_batch_storage_evaluator(problem: ArchOptProblemBase):
     with tempfile.TemporaryDirectory() as tmp_folder:
         pop = HierarchicalSampling().do(problem, 110)
         assert pop.get('F').shape == (110, 0)
 
@@ -151,14 +161,26 @@
         assert os.path.exists(os.path.join(tmp_folder, 'pymoo_population.csv'))
 
         pop_loaded = load_from_previous_results(problem, tmp_folder)
         assert pop_loaded.get('X').shape == pop.get('X').shape
         assert pop_loaded.get('F').shape == pop.get('F').shape
 
 
+def test_doe_algo_seed(problem: ArchOptProblemBase):
+    x_doe = []
+    for seed in [42, None, 42]:
+        doe_algo = get_doe_algo(doe_size=100)
+        doe_algo.setup(problem, seed=seed)
+        doe_algo.run()
+        x_doe.append(doe_algo.pop.get('X'))
+
+    assert np.any(x_doe[0] != x_doe[1])
+    assert np.all(x_doe[0] == x_doe[2])
+
+
 class CrashingProblem(DummyResultSavingProblem):
 
     def __init__(self, failed_evals=True):
         self.failed_evals = failed_evals
         super().__init__()
         self.i_eval = 0
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_segomoe.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_segomoe.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_smarty.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_smarty.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_tpe.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_tpe.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/algo/test_trieste.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/algo/test_trieste.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     assert search_space.dimension == problem.n_var
 
 
 @check_dependency()
 def test_simple(problem: ArchOptProblemBase):
     assert HAS_TRIESTE
 
-    opt = get_trieste_optimizer(problem, n_init=10, n_infill=1)
+    opt = get_trieste_optimizer(problem, n_init=10, n_infill=1, seed=42)
     assert repr(opt)
     result = opt.run_optimization()
 
     pop = opt.to_population(result.datasets)
     assert len(pop) == 11
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/conftest.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_assignment.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_assignment.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_constrained.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_constrained.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_gnc.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_gnc.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_hidden_constraints.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_hidden_constraints.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_hierarchical.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_hierarchical.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_md_mo.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_md_mo.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/problems/test_turbofan_arch.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/problems/test_turbofan_arch.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/test_design_space.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/test_design_space.py`

 * *Files 7% similar despite different names*

```diff
@@ -129,15 +129,25 @@
         assert np.all(~LargeDuplicateElimination.eliminate(x_discrete))
         ds.get_discrete_rates(show=True)
 
         x_discrete_trial, is_act_trail = ds.all_discrete_x_by_trial_and_imputation
         assert np.all(x_discrete_trial == x_discrete)
         assert np.all(is_active_discrete == is_act_trail)
 
+        np.random.seed(None)
         for _ in range(10):
             x_sampled, is_act_sampled = ds.quick_sample_discrete_x(20)
             assert x_sampled.shape == (20, ds.n_var)
             assert is_act_sampled.shape == (20, ds.n_var)
 
             x_sampled_, is_act_sampled_ = ds.correct_x(x_sampled)
             assert np.all(x_sampled_ == x_sampled)
             assert np.all(is_act_sampled_ == is_act_sampled)
+
+        np.random.seed(42)
+        x1, _ = ds.quick_sample_discrete_x(20)
+        x2, _ = ds.quick_sample_discrete_x(20)
+        assert np.any(x1 != x2)
+
+        np.random.seed(42)
+        x3, _ = ds.quick_sample_discrete_x(20)
+        assert np.all(x1 == x3)
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/test_design_space_explicit.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/test_design_space_explicit.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,23 @@
 
     x, is_active = HierarchicalSampling(sobol=False).randomly_sample(
         ArchOptProblemBase(ds), 100, ArchOptRepair(), x_all=None, is_act_all=None)
     assert x.shape == (6, 2)
     assert is_active.shape == x.shape
     assert np.all(is_active)
 
+    np.random.seed(42)
+    x1, _ = ds.quick_sample_discrete_x(20)
+    x2, _ = ds.quick_sample_discrete_x(20)
+    assert np.any(x1 != x2)
+
+    np.random.seed(42)
+    x3, _ = ds.quick_sample_discrete_x(20)
+    assert np.all(x1 == x3)
+
 
 def test_hierarchy():
     ds = ExplicitArchDesignSpace([
         CategoricalParam('a', options=['A', 'B', 'C']),
         CategoricalParam('b', options=['E', 'F']),
         IntegerParam('c', 0, 1),
         ContinuousParam('d', 0, 1),
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/test_problem.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/test_problem.py`

 * *Files 7% similar despite different names*

```diff
@@ -284,14 +284,23 @@
         assert len(i) == 5
         assert 0 <= np.min(i) <= np.max(i) < 10
         assert len(np.unique(i)) == len(i)
 
     with pytest.raises(ValueError):
         HierarchicalSampling._sobol_choice(10, 5, replace=False)
 
+    np.random.seed(42)
+    i1 = HierarchicalSampling._sobol_choice(5, 100)
+    i2 = HierarchicalSampling._sobol_choice(5, 100)
+    assert np.any(i1 != i2)
+
+    np.random.seed(42)
+    i3 = HierarchicalSampling._sobol_choice(5, 100)
+    assert np.all(i1 == i3)
+
 
 def test_hierarchical_random_sampling(problem: ArchOptProblemBase):
 
     sampling_values = HierarchicalExhaustiveSampling.get_exhaustive_sample_values(problem)
     assert len(sampling_values) == 5
     assert np.prod([len(values) for values in sampling_values]) == 12500
 
@@ -302,14 +311,26 @@
         assert x.shape == (1000, 5)
         assert np.unique(x, axis=0).shape[0] == 1000
         problem.evaluate(x)
 
         x_imp, _ = problem.correct_x(x)
         assert np.all(x_imp == x)
 
+        np.random.seed(42)
+        x1 = sampling.do(problem, 1000).get('X')
+        x2 = sampling.do(problem, 1000).get('X')
+        assert np.any(x1 != x2)
+
+        np.random.seed(42)
+        x3 = sampling.do(problem, 1000).get('X')
+        assert np.all(x1 == x3)
+
+        x4 = HierarchicalSampling(sobol=sobol, seed=42).do(problem, 1000).get('X')
+        assert np.all(x1 == x4)
+
 
 def test_hierarchical_random_sampling_discrete_hierarchical(discrete_problem: ArchOptProblemBase):
 
     sampling_values = HierarchicalExhaustiveSampling.get_exhaustive_sample_values(discrete_problem)
     assert len(sampling_values) == 2
     assert np.prod([len(values) for values in sampling_values]) == 100
 
@@ -341,14 +362,23 @@
         assert x.shape == (1000, 5)
         assert np.unique(x, axis=0).shape[0] == 1000
         problem.evaluate(x)
 
         x_imp, _ = problem.correct_x(x)
         assert np.all(x_imp == x)
 
+        np.random.seed(42)
+        x1 = sampling.do(problem, 1000).get('X')
+        x2 = sampling.do(problem, 1000).get('X')
+        assert np.any(x1 != x2)
+
+        np.random.seed(42)
+        x3 = sampling.do(problem, 1000).get('X')
+        assert np.all(x1 == x3)
+
     HierarchicalSampling._n_comb_gen_all_max = limit
 
 
 def test_cached_pareto_front_mixin(problem: ArchOptTestProblemBase, discrete_problem: ArchOptTestProblemBase):
     problem.reset_pf_cache()
     assert not os.path.exists(problem._pf_cache_path())
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/tests/test_tutorials.py` & `sb-arch-opt-1.1.5/sb_arch_opt/tests/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt/util.py` & `sb-arch-opt-1.1.5/sb_arch_opt/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,7 +34,12 @@
         'loggers': {
             'sb_arch_opt': {
                 'handlers': ['console'],
                 'level': level,
             },
         },
     })
+
+
+def get_np_random_singleton():
+    from scipy._lib._util import check_random_state
+    return check_random_state(seed=None)
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt.egg-info/PKG-INFO` & `sb-arch-opt-1.1.5/sb_arch_opt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sb-arch-opt
-Version: 1.1.4
+Version: 1.1.5
 Summary: SBArchOpt: Surrogate-Based Architecture Optimization
 Author: Jasper Bussemaker
 Author-email: jasper.bussemaker@dlr.de
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sb-arch-opt-1.1.4/sb_arch_opt.egg-info/SOURCES.txt` & `sb-arch-opt-1.1.5/sb_arch_opt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.4/setup.py` & `sb-arch-opt-1.1.5/setup.py`

 * *Files identical despite different names*

