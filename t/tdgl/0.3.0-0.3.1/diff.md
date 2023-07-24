# Comparing `tmp/tdgl-0.3.0.tar.gz` & `tmp/tdgl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdgl-0.3.0.tar", last modified: Thu Jun  8 18:23:28 2023, max compression
+gzip compressed data, was "tdgl-0.3.1.tar", last modified: Mon Jul 24 16:14:49 2023, max compression
```

## Comparing `tdgl-0.3.0.tar` & `tdgl-0.3.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.258404 tdgl-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-08 18:23:10.000000 tdgl-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-08 18:23:28.258404 tdgl-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-08 18:23:10.000000 tdgl-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:23:28.258404 tdgl-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-08 18:23:10.000000 tdgl-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/about.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33522 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/device/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/device/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/device/meshing.py
--rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/device/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    14231 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/em.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl/finite_volume/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/finite_volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/finite_volume/edge_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/finite_volume/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/finite_volume/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/finite_volume/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/fluxoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl/solution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solution/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    24575 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solution/plot_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    42236 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solution/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl/solver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solver/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solver/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solver/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl/sources/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/sources/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/sources/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.258404 tdgl-0.3.0/tdgl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_about.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.258404 tdgl-0.3.0/tdgl/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/visualization/animate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/visualization/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/visualization/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/visualization/io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4332 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-08 18:23:28.000000 tdgl-0.3.0/tdgl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-08 18:23:28.000000 tdgl-0.3.0/tdgl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:23:28.000000 tdgl-0.3.0/tdgl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-08 18:23:28.000000 tdgl-0.3.0/tdgl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 18:23:28.000000 tdgl-0.3.0/tdgl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:49.363866 tdgl-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-24 16:14:30.000000 tdgl-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-24 16:14:49.363866 tdgl-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-24 16:14:30.000000 tdgl-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:14:49.363866 tdgl-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-07-24 16:14:30.000000 tdgl-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:49.359866 tdgl-0.3.1/tdgl/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/about.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:49.359866 tdgl-0.3.1/tdgl/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33522 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/device/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/device/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/device/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/device/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14231 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/em.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:49.359866 tdgl-0.3.1/tdgl/finite_volume/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/finite_volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/finite_volume/edge_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/finite_volume/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/finite_volume/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/finite_volume/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/fluxoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:49.359866 tdgl-0.3.1/tdgl/solution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/solution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/solution/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27000 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/solution/plot_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42236 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/solution/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:49.359866 tdgl-0.3.1/tdgl/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/solver/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/solver/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/solver/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:49.363866 tdgl-0.3.1/tdgl/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/sources/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/sources/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:49.363866 tdgl-0.3.1/tdgl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/test/test_about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/test/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/test/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/test/test_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/test/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/test/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/test/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/test/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/test/test_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:49.363866 tdgl-0.3.1/tdgl/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/visualization/animate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/visualization/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/visualization/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/visualization/io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4332 2023-07-24 16:14:30.000000 tdgl-0.3.1/tdgl/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:14:49.359866 tdgl-0.3.1/tdgl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-24 16:14:49.000000 tdgl-0.3.1/tdgl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-24 16:14:49.000000 tdgl-0.3.1/tdgl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:14:49.000000 tdgl-0.3.1/tdgl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-24 16:14:49.000000 tdgl-0.3.1/tdgl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-24 16:14:49.000000 tdgl-0.3.1/tdgl.egg-info/top_level.txt
```

### Comparing `tdgl-0.3.0/LICENSE` & `tdgl-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/PKG-INFO` & `tdgl-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdgl
-Version: 0.3.0
+Version: 0.3.1
 Summary: pyTDGL: Time-dependent Ginzburg-Landau in Python.
 Home-page: https://github.com/loganbvh/py-tdgl
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor vortex Ginzburg-Landau
 Platform: Linux
@@ -51,19 +51,49 @@
 
 ## Learn `pyTDGL`
 
 The documentation for `pyTDGL` can be found at [py-tdgl.readthedocs.io](https://py-tdgl.readthedocs.io/en/latest/).
 
 ## Try `pyTDGL`
 
-Click the badge below and navigate to `docs/notebooks/` to try `pyTDGL` interactively online via [Binder](https://mybinder.org/)
+Click the badge below to try `pyTDGL` interactively online via [Google Colab](https://colab.research.google.com/):
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/loganbvh/py-tdgl/HEAD)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/loganbvh/py-tdgl/blob/main/docs/notebooks/quickstart.ipynb)
 
-## Acknowledgments
+## About `pyTDGL`
 
-Parts of this package have been adapted from [`SuperDetectorPy`](https://github.com/afsa/super-detector-py), a GitHub repo authored by [Mattias Jönsson](https://github.com/afsa). Both `SuperDetectorPy` and `py-tdgl` are released under the open-source MIT License. If you use either package in an academic publication or similar, please consider citing the following:
+### Authors
+
+- Primary author and maintainer: [@loganbvh](https://github.com/loganbvh/).
+
+### Citing `pyTDGL`
+
+`pyTDGL` is described in the following paper:
+
+>*pyTDGL: Time-dependent Ginzburg-Landau in Python*, Computer Physics Communications **291**, 108799 (2023), DOI: [10.1016/j.cpc.2023.108799](https://doi.org/10.1016/j.cpc.2023.108799).
+
+If you use `pyTDGL` in your research, please cite the paper linked above.
+
+    % BibTeX citation
+    @article{
+        Bishop-Van_Horn2023-wr,
+        title    = "{pyTDGL}: Time-dependent {Ginzburg-Landau} in Python",
+        author   = "Bishop-Van Horn, Logan",
+        journal  = "Comput. Phys. Commun.",
+        volume   =  291,
+        pages    = "108799",
+        month    =  may,
+        year     =  2023,
+        url      = "http://dx.doi.org/10.1016/j.cpc.2023.108799",
+        issn     = "0010-4655",
+        doi      = "10.1016/j.cpc.2023.108799"
+    }
+
+
+### Acknowledgments
+
+Parts of this package have been adapted from [`SuperDetectorPy`](https://github.com/afsa/super-detector-py), a GitHub repo authored by [Mattias Jönsson](https://github.com/afsa). Both `SuperDetectorPy` and `py-tdgl` are released under the open-source MIT License. If you use either package in an academic publication or similar, please consider citing the following in addition to the `pyTDGL` paper:
 
 - Mattias Jönsson, Theory for superconducting few-photon detectors (Doctoral dissertation), KTH Royal Institute of Technology (2022) ([Link](http://urn.kb.se/resolve?urn=urn:nbn:se:kth:diva-312132))
 - Mattias Jönsson, Robert Vedin, Samuel Gyger, James A. Sutton, Stephan Steinhauer, Val Zwiller, Mats Wallin, Jack Lidmar, Current crowding in nanoscale superconductors within the Ginzburg-Landau model, Phys. Rev. Applied 17, 064046 (2022) ([Link](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.17.064046))
 
 The user interface is adapted from [`SuperScreen`](https://github.com/loganbvh/superscreen).
```

### Comparing `tdgl-0.3.0/README.md` & `tdgl-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 
 ## Learn `pyTDGL`
 
 The documentation for `pyTDGL` can be found at [py-tdgl.readthedocs.io](https://py-tdgl.readthedocs.io/en/latest/).
 
 ## Try `pyTDGL`
 
-Click the badge below and navigate to `docs/notebooks/` to try `pyTDGL` interactively online via [Binder](https://mybinder.org/)
+Click the badge below to try `pyTDGL` interactively online via [Google Colab](https://colab.research.google.com/):
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/loganbvh/py-tdgl/HEAD)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/loganbvh/py-tdgl/blob/main/docs/notebooks/quickstart.ipynb)
 
 ## Install `pyTDGL`
 
-`pyTDGL` requires `python` `3.8`, `3.9`, or `3.10`. We recommend installing `pyTDGL` in a [`conda` environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html), e.g.
+`pyTDGL` requires `python` `3.8`, `3.9`, `3.10`, or `3.11`. We recommend installing `pyTDGL` in a [`conda` environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html), e.g.
 
 ```bash
 conda create --name tdgl python="3.10"
 conda activate tdgl
 ```
 
 ### Install via `pip`
```

### Comparing `tdgl-0.3.0/setup.py` & `tdgl-0.3.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,21 +16,51 @@
 
 ## Learn `pyTDGL`
 
 The documentation for `pyTDGL` can be found at [py-tdgl.readthedocs.io](https://py-tdgl.readthedocs.io/en/latest/).
 
 ## Try `pyTDGL`
 
-Click the badge below and navigate to `docs/notebooks/` to try `pyTDGL` interactively online via [Binder](https://mybinder.org/)
+Click the badge below to try `pyTDGL` interactively online via [Google Colab](https://colab.research.google.com/):
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/loganbvh/py-tdgl/HEAD)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/loganbvh/py-tdgl/blob/main/docs/notebooks/quickstart.ipynb)
 
-## Acknowledgments
+## About `pyTDGL`
 
-Parts of this package have been adapted from [`SuperDetectorPy`](https://github.com/afsa/super-detector-py), a GitHub repo authored by [Mattias Jönsson](https://github.com/afsa). Both `SuperDetectorPy` and `py-tdgl` are released under the open-source MIT License. If you use either package in an academic publication or similar, please consider citing the following:
+### Authors
+
+- Primary author and maintainer: [@loganbvh](https://github.com/loganbvh/).
+
+### Citing `pyTDGL`
+
+`pyTDGL` is described in the following paper:
+
+>*pyTDGL: Time-dependent Ginzburg-Landau in Python*, Computer Physics Communications **291**, 108799 (2023), DOI: [10.1016/j.cpc.2023.108799](https://doi.org/10.1016/j.cpc.2023.108799).
+
+If you use `pyTDGL` in your research, please cite the paper linked above.
+
+    % BibTeX citation
+    @article{
+        Bishop-Van_Horn2023-wr,
+        title    = "{pyTDGL}: Time-dependent {Ginzburg-Landau} in Python",
+        author   = "Bishop-Van Horn, Logan",
+        journal  = "Comput. Phys. Commun.",
+        volume   =  291,
+        pages    = "108799",
+        month    =  may,
+        year     =  2023,
+        url      = "http://dx.doi.org/10.1016/j.cpc.2023.108799",
+        issn     = "0010-4655",
+        doi      = "10.1016/j.cpc.2023.108799"
+    }
+
+
+### Acknowledgments
+
+Parts of this package have been adapted from [`SuperDetectorPy`](https://github.com/afsa/super-detector-py), a GitHub repo authored by [Mattias Jönsson](https://github.com/afsa). Both `SuperDetectorPy` and `py-tdgl` are released under the open-source MIT License. If you use either package in an academic publication or similar, please consider citing the following in addition to the `pyTDGL` paper:
 
 - Mattias Jönsson, Theory for superconducting few-photon detectors (Doctoral dissertation), KTH Royal Institute of Technology (2022) ([Link](http://urn.kb.se/resolve?urn=urn:nbn:se:kth:diva-312132))
 - Mattias Jönsson, Robert Vedin, Samuel Gyger, James A. Sutton, Stephan Steinhauer, Val Zwiller, Mats Wallin, Jack Lidmar, Current crowding in nanoscale superconductors within the Ginzburg-Landau model, Phys. Rev. Applied 17, 064046 (2022) ([Link](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.17.064046))
 
 The user interface is adapted from [`SuperScreen`](https://github.com/loganbvh/superscreen).
 """
 
@@ -54,15 +84,15 @@
     "matplotlib",
     "meshpy",
     "numba",
     "numpy",
     "pint",
     "pytest",
     "pytest-cov",
-    "scipy",
+    "scipy<1.11",
     "shapely",
     "tqdm",
 ]
 
 EXTRAS_REQUIRE = {
     "dev": [
         "black",
```

### Comparing `tdgl-0.3.0/tdgl/about.py` & `tdgl-0.3.1/tdgl/about.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/device/device.py` & `tdgl-0.3.1/tdgl/device/device.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/device/layer.py` & `tdgl-0.3.1/tdgl/device/layer.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/device/meshing.py` & `tdgl-0.3.1/tdgl/device/meshing.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/device/polygon.py` & `tdgl-0.3.1/tdgl/device/polygon.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/distance.py` & `tdgl-0.3.1/tdgl/distance.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/em.py` & `tdgl-0.3.1/tdgl/em.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/finite_volume/edge_mesh.py` & `tdgl-0.3.1/tdgl/finite_volume/edge_mesh.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/finite_volume/mesh.py` & `tdgl-0.3.1/tdgl/finite_volume/mesh.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/finite_volume/operators.py` & `tdgl-0.3.1/tdgl/finite_volume/operators.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/finite_volume/util.py` & `tdgl-0.3.1/tdgl/finite_volume/util.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/fluxoid.py` & `tdgl-0.3.1/tdgl/fluxoid.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/geometry.py` & `tdgl-0.3.1/tdgl/geometry.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/parameter.py` & `tdgl-0.3.1/tdgl/parameter.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/solution/data.py` & `tdgl-0.3.1/tdgl/solution/data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import dataclasses
-from typing import Any, Dict, Sequence, Tuple, Union
+import os
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import h5py
 import matplotlib.pyplot as plt
 import numpy as np
+from scipy import interpolate
+from tqdm import tqdm
 
 from ..finite_volume.mesh import Mesh
+from ..geometry import path_vectors
 
 
 def get_data_range(h5file: h5py.File) -> Tuple[int, int]:
     """Returns the minimum and maximum solve steps in the file."""
     keys = np.asarray([int(key) for key in h5file["data"]])
     return np.min(keys), np.max(keys)
 
@@ -433,7 +437,115 @@
         if self.theta is not None:
             h5group["theta"] = self.theta
         if self.screening_iterations is not None:
             h5group["screening_iterations"] = self.screening_iterations
 
     def __eq__(self, other: Any) -> bool:
         return dataclass_equals(self, other)
+
+
+def get_current_through_paths(
+    solution_path: os.PathLike,
+    paths: Union[np.ndarray, List[np.ndarray]],
+    dataset: Optional[str] = None,
+    interp_method: str = "linear",
+    units: Optional[str] = None,
+    with_units: bool = True,
+    progress_bar: bool = True,
+) -> Tuple[np.ndarray, Union[np.ndarray, List[np.ndarray]]]:
+    """Calculates the current through one or more paths for each saved time step.
+
+    Args:
+        solution_path: Path to the solution HDF5 file.
+        paths: A list of ``(n, 2)`` arrays of ``(x, y)`` coordinates defining
+            the paths. A single ``(n, 2)`` array is also allowed.
+        dataset: ``None``, ``"supercurrent"``, or ``"normal_current"``.
+            ``None`` indicates the total current.
+        interp_method: Interpolation method: either "linear" or "cubic".
+        units: The current units to return.
+        with_units: Whether to return a :class:`pint.Quantity` with units attached.
+        progress_bar: Whether to display a progress bar.
+
+    Returns:
+        ``(times, currents)``, where ``currents`` is a list of arrays of the
+        time-dependent current through each path. If ``paths`` is given as a
+        single array, ``currents`` will be returned as a single array.
+    """
+    from .solution import Solution
+
+    solution = Solution.from_hdf5(solution_path)
+    device = solution.device
+    mesh = device.mesh
+    ureg = device.ureg
+
+    valid_methods = ("linear", "cubic")
+    if interp_method not in valid_methods:
+        raise ValueError(
+            f"Interpolation method must be one of {valid_methods} (got {interp_method})."
+        )
+    if interp_method == "linear":
+        interpolator = interpolate.LinearNDInterpolator
+        interp_kwargs = dict(fill_value=0)
+    else:  # "cubic"
+        interpolator = interpolate.CloughTocher2DInterpolator
+        interp_kwargs = dict(fill_value=0)
+
+    valid_datasets = ("supercurrent", "normal_current", None)
+    if dataset not in valid_datasets:
+        raise ValueError(
+            f"Dataset name must be one of {valid_datasets} (got {dataset})."
+        )
+
+    if units is None:
+        units = solution.current_units
+
+    length_units = ureg(device.length_units)
+
+    if isinstance(paths, np.ndarray):
+        paths = [paths]
+    paths = [np.asarray(p) for p in paths]
+    edge_positions = []
+    edge_lengths = []
+    unit_normals = []
+    in_device = []
+    for path in paths:
+        edge_positions.append((path[:-1] + path[1:]) / 2)
+        lengths, normals = path_vectors(path)
+        edge_lengths.append(lengths)
+        unit_normals.append(normals)
+        in_device.append(device.contains_points(edge_positions[-1]))
+
+    step_min, step_max = solution.data_range
+    times = solution.times
+    sites = device.points
+    raw_currents = [np.zeros_like(times) for _ in paths]
+    with h5py.File(solution_path, "r") as h5file:
+        for i in tqdm(
+            range(step_min, step_max + 1), desc="Time steps", disable=(not progress_bar)
+        ):
+            grp = h5file[f"data/{i}"]
+            if dataset is None:
+                K = np.array(grp["normal_current"]) + np.array(grp["supercurrent"])
+            else:
+                K = np.array(grp[dataset])
+            K = mesh.get_quantity_on_site(K)
+            K_interp = interpolator(sites, K, **interp_kwargs)
+            for j, (path, lengths, normals, ix) in enumerate(
+                zip(paths, edge_lengths, unit_normals, in_device)
+            ):
+                K_path = K_interp(path)
+                # Evaluate the sheet current at the edge centers
+                K_edge = (K_path[:-1] + K_path[1:]) / 2
+                K_dot_n = (K_edge * normals).sum(axis=1)
+                raw_currents[j][i] = np.trapz((K_dot_n * lengths)[ix])
+
+    currents = []
+    for current in raw_currents:
+        J = current * (device.K0 * length_units).to(units)
+        if not with_units:
+            J = J.magnitude
+        currents.append(J)
+
+    if len(currents) == 1:
+        currents = currents[0]
+
+    return times, currents
```

### Comparing `tdgl-0.3.0/tdgl/solution/plot_solution.py` & `tdgl-0.3.1/tdgl/solution/plot_solution.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import os
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 from mpl_toolkits.axes_grid1.axes_divider import make_axes_locatable
 from scipy import interpolate
 
 from ..visualization import auto_grid, auto_range_iqr
+from .data import get_current_through_paths
 from .solution import Solution
 
 
 def setup_color_limits(
     dict_of_arrays: Dict[str, np.ndarray],
     vmin: Union[float, None] = None,
     vmax: Union[float, None] = None,
@@ -631,14 +633,82 @@
     ax.set_ylabel(f"$y$ [${length_units:~L}$]")
     cbar.set_label("$\\mu/v_0$")
     ax.set_xlim(x.min(), x.max())
     ax.set_ylim(y.min(), y.max())
     return fig, ax
 
 
+def plot_current_through_paths(
+    solution_path: os.PathLike,
+    paths: Union[np.ndarray, List[np.ndarray]],
+    dataset: Optional[str] = None,
+    interp_method: str = "linear",
+    units: Optional[str] = None,
+    progress_bar: bool = True,
+    grid: bool = True,
+    labels: bool = True,
+    legend: bool = True,
+    **figure_kwargs,
+) -> Tuple[
+    Tuple[plt.Figure, plt.Axes], Tuple[np.ndarray, Union[np.ndarray, List[np.ndarray]]]
+]:
+    """Plots the current through one or more paths for each saved time step.
+
+    Args:
+        solution_path: Path to the solution HDF5 file.
+        paths: A list of ``(n, 2)`` arrays of ``(x, y)`` coordinates defining
+            the paths. A single ``(n, 2)`` array is also allowed.
+        dataset: ``None``, ``"supercurrent"``, or ``"normal_current"``.
+            ``None`` indicates the total current.
+        interp_method: Interpolation method: either "linear" or "cubic".
+        units: The current units to return.
+        with_units: Whether to return a :class:`pint.Quantity` with units attached.
+        progress_bar: Whether to display a progress bar.
+        grid: Whether to add grid lines to the plot.
+        labels: Whether to include axis labels.
+        legend: Whether to include a legend.
+
+    Returns:
+        ``(fig, ax), (times, currents)``, where ``currents`` is a list of arrays of
+        the time-dependent current through each path. If ``paths`` is given as a
+        single array, ``currents`` will be returned as a single array.
+    """
+    times, currents = get_current_through_paths(
+        solution_path,
+        paths,
+        dataset=dataset,
+        interp_method=interp_method,
+        units=units,
+        with_units=True,
+        progress_bar=progress_bar,
+    )
+    if isinstance(paths, np.ndarray):
+        currents = [currents]
+    current_units = currents[0].units
+
+    label = {
+        "supercurrent": "Supercurrent",
+        "normal_current": "Normal current",
+        None: "Total current",
+    }[dataset]
+
+    fig, ax = plt.subplots(**figure_kwargs)
+    ax.grid(grid)
+    for i, current in enumerate(currents):
+        ax.plot(times, current.magnitude, label=f"Path {i}")
+
+    if labels:
+        ax.set_ylabel(f"{label} [${current_units:~L}$]")
+        ax.set_xlabel("Time, $t$ [$\\tau_0$]")
+    if legend:
+        ax.legend(loc=0)
+
+    return (fig, ax), (times, currents)
+
+
 def _patch_docstring(func):
     other_func = getattr(Solution, func.__name__)
     other_func.__doc__ = (
         other_func.__doc__
         + "\n\n"
         + "\n".join(
             [line for line in func.__doc__.split("\n    ") if "solution:" not in line]
```

### Comparing `tdgl-0.3.0/tdgl/solution/solution.py` & `tdgl-0.3.1/tdgl/solution/solution.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/solver/options.py` & `tdgl-0.3.1/tdgl/solver/options.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/solver/runner.py` & `tdgl-0.3.1/tdgl/solver/runner.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/solver/solve.py` & `tdgl-0.3.1/tdgl/solver/solve.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/sources/constant.py` & `tdgl-0.3.1/tdgl/sources/constant.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/sources/loop.py` & `tdgl-0.3.1/tdgl/sources/loop.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/test/conftest.py` & `tdgl-0.3.1/tdgl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/test/test_device.py` & `tdgl-0.3.1/tdgl/test/test_device.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/test/test_distance.py` & `tdgl-0.3.1/tdgl/test/test_distance.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/test/test_em.py` & `tdgl-0.3.1/tdgl/test/test_em.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/test/test_parameter.py` & `tdgl-0.3.1/tdgl/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/test/test_solution.py` & `tdgl-0.3.1/tdgl/test/test_solution.py`

 * *Files 17% similar despite different names*

```diff
@@ -116,7 +116,43 @@
         loaded_dynamics = DynamicsData.from_hdf5(f["dynamics"])
 
     assert loaded_dynamics == dynamics
 
     time = solution.times
     assert len(time) == (solution.data_range[1] + 1)
     assert solution.closest_solve_step(0) == 0
+
+
+@pytest.mark.parametrize("dataset", [None, "supercurrent", "normal_current", "invalid"])
+@pytest.mark.parametrize("interp_method", ["linear", "cubic", "invalid"])
+def test_get_current_through_paths(solution: tdgl.Solution, dataset, interp_method):
+    ys = np.linspace(-2, 2, 101)
+    xs = 7.5 * np.ones_like(ys)
+    paths = [
+        np.array([+xs, ys]).T,
+        np.array([-xs, ys]).T,
+    ]
+
+    Isrc = solution.terminal_currents(0)["source"]
+
+    if dataset == "invalid" or interp_method == "invalid":
+        with pytest.raises(ValueError):
+            times, currents = tdgl.get_current_through_paths(
+                solution.path,
+                paths[0],
+                dataset=dataset,
+                interp_method=interp_method,
+            )
+    else:
+        (fig, ax), (times, currents) = tdgl.plot_current_through_paths(
+            solution.path,
+            paths[0],
+            dataset=dataset,
+            interp_method=interp_method,
+            progress_bar=False,
+        )
+        assert len(currents) == 1
+        assert len(times) == len(currents[0])
+        for cs in currents:
+            assert isinstance(cs[0], pint.Quantity)
+            if dataset is None:
+                assert np.allclose(cs.m[1:], Isrc, rtol=2e-2)
```

### Comparing `tdgl-0.3.0/tdgl/test/test_solve.py` & `tdgl-0.3.1/tdgl/test/test_solve.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/test/test_visualization.py` & `tdgl-0.3.1/tdgl/test/test_visualization.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/test/test_visualize.py` & `tdgl-0.3.1/tdgl/test/test_visualize.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/visualization/animate.py` & `tdgl-0.3.1/tdgl/visualization/animate.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/visualization/common.py` & `tdgl-0.3.1/tdgl/visualization/common.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/visualization/interactive.py` & `tdgl-0.3.1/tdgl/visualization/interactive.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/visualization/io.py` & `tdgl-0.3.1/tdgl/visualization/io.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl/visualize.py` & `tdgl-0.3.1/tdgl/visualize.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.3.0/tdgl.egg-info/PKG-INFO` & `tdgl-0.3.1/tdgl.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdgl
-Version: 0.3.0
+Version: 0.3.1
 Summary: pyTDGL: Time-dependent Ginzburg-Landau in Python.
 Home-page: https://github.com/loganbvh/py-tdgl
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor vortex Ginzburg-Landau
 Platform: Linux
@@ -51,19 +51,49 @@
 
 ## Learn `pyTDGL`
 
 The documentation for `pyTDGL` can be found at [py-tdgl.readthedocs.io](https://py-tdgl.readthedocs.io/en/latest/).
 
 ## Try `pyTDGL`
 
-Click the badge below and navigate to `docs/notebooks/` to try `pyTDGL` interactively online via [Binder](https://mybinder.org/)
+Click the badge below to try `pyTDGL` interactively online via [Google Colab](https://colab.research.google.com/):
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/loganbvh/py-tdgl/HEAD)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/loganbvh/py-tdgl/blob/main/docs/notebooks/quickstart.ipynb)
 
-## Acknowledgments
+## About `pyTDGL`
 
-Parts of this package have been adapted from [`SuperDetectorPy`](https://github.com/afsa/super-detector-py), a GitHub repo authored by [Mattias Jönsson](https://github.com/afsa). Both `SuperDetectorPy` and `py-tdgl` are released under the open-source MIT License. If you use either package in an academic publication or similar, please consider citing the following:
+### Authors
+
+- Primary author and maintainer: [@loganbvh](https://github.com/loganbvh/).
+
+### Citing `pyTDGL`
+
+`pyTDGL` is described in the following paper:
+
+>*pyTDGL: Time-dependent Ginzburg-Landau in Python*, Computer Physics Communications **291**, 108799 (2023), DOI: [10.1016/j.cpc.2023.108799](https://doi.org/10.1016/j.cpc.2023.108799).
+
+If you use `pyTDGL` in your research, please cite the paper linked above.
+
+    % BibTeX citation
+    @article{
+        Bishop-Van_Horn2023-wr,
+        title    = "{pyTDGL}: Time-dependent {Ginzburg-Landau} in Python",
+        author   = "Bishop-Van Horn, Logan",
+        journal  = "Comput. Phys. Commun.",
+        volume   =  291,
+        pages    = "108799",
+        month    =  may,
+        year     =  2023,
+        url      = "http://dx.doi.org/10.1016/j.cpc.2023.108799",
+        issn     = "0010-4655",
+        doi      = "10.1016/j.cpc.2023.108799"
+    }
+
+
+### Acknowledgments
+
+Parts of this package have been adapted from [`SuperDetectorPy`](https://github.com/afsa/super-detector-py), a GitHub repo authored by [Mattias Jönsson](https://github.com/afsa). Both `SuperDetectorPy` and `py-tdgl` are released under the open-source MIT License. If you use either package in an academic publication or similar, please consider citing the following in addition to the `pyTDGL` paper:
 
 - Mattias Jönsson, Theory for superconducting few-photon detectors (Doctoral dissertation), KTH Royal Institute of Technology (2022) ([Link](http://urn.kb.se/resolve?urn=urn:nbn:se:kth:diva-312132))
 - Mattias Jönsson, Robert Vedin, Samuel Gyger, James A. Sutton, Stephan Steinhauer, Val Zwiller, Mats Wallin, Jack Lidmar, Current crowding in nanoscale superconductors within the Ginzburg-Landau model, Phys. Rev. Applied 17, 064046 (2022) ([Link](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.17.064046))
 
 The user interface is adapted from [`SuperScreen`](https://github.com/loganbvh/superscreen).
```

### Comparing `tdgl-0.3.0/tdgl.egg-info/SOURCES.txt` & `tdgl-0.3.1/tdgl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

