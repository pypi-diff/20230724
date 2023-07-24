# Comparing `tmp/dynareadout-23.6.tar.gz` & `tmp/dynareadout-23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynareadout-23.6.tar", last modified: Mon Jun 26 09:18:13 2023, max compression
+gzip compressed data, was "dynareadout-23.7.tar", last modified: Mon Jul 24 10:29:04 2023, max compression
```

## Comparing `dynareadout-23.6.tar` & `dynareadout-23.7.tar`

### file list

```diff
@@ -1,109 +1,113 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.675493 dynareadout-23.6/
--rw-rw-rw-   0        0        0      878 2023-02-01 10:01:57.000000 dynareadout-23.6/LICENSE
--rw-rw-rw-   0        0        0      251 2023-02-01 10:03:35.000000 dynareadout-23.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5295 2023-06-26 09:18:13.675493 dynareadout-23.6/PKG-INFO
--rw-rw-rw-   0        0        0     4520 2023-05-08 11:43:26.000000 dynareadout-23.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.592892 dynareadout-23.6/lib/
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.591894 dynareadout-23.6/lib/dynareadout/
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.631789 dynareadout-23.6/lib/dynareadout/src/
--rw-rw-rw-   0        0        0    15215 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binary_search.c
--rw-rw-rw-   0        0        0     4052 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binary_search.h
--rw-rw-rw-   0        0        0    30254 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/binout.c
--rw-rw-rw-   0        0        0     5776 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/binout.h
--rw-rw-rw-   0        0        0     3252 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binout_defines.h
--rw-rw-rw-   0        0        0    11391 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binout_directory.c
--rw-rw-rw-   0        0        0     5670 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binout_directory.h
--rw-rw-rw-   0        0        0     3791 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binout_glob.c
--rw-rw-rw-   0        0        0     1784 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binout_glob.h
--rw-rw-rw-   0        0        0    13180 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/binout_read.c
--rw-rw-rw-   0        0        0     4794 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binout_read.h
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.640765 dynareadout-23.6/lib/dynareadout/src/cpp/
--rw-rw-rw-   0        0        0    11763 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/cpp/array.hpp
--rw-rw-rw-   0        0        0     8819 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/cpp/binout.cpp
--rw-rw-rw-   0        0        0     3521 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/cpp/binout.hpp
--rw-rw-rw-   0        0        0    18739 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/cpp/d3plot.cpp
--rw-rw-rw-   0        0        0     7831 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/cpp/d3plot.hpp
--rw-rw-rw-   0        0        0     7685 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_part.cpp
--rw-rw-rw-   0        0        0     4841 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_part.hpp
--rw-rw-rw-   0        0        0     4418 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_state.cpp
--rw-rw-rw-   0        0        0     2848 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_state.hpp
--rw-rw-rw-   0        0        0     7096 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/cpp/key.cpp
--rw-rw-rw-   0        0        0    16902 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/cpp/key.hpp
--rw-rw-rw-   0        0        0     2005 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/cpp/vec.hpp
--rw-rw-rw-   0        0        0    22780 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3_buffer.c
--rw-rw-rw-   0        0        0     4304 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3_buffer.h
--rw-rw-rw-   0        0        0     6785 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/d3_defines.h
--rw-rw-rw-   0        0        0    93920 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3plot.c
--rw-rw-rw-   0        0        0    18155 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3plot.h
--rw-rw-rw-   0        0        0    12437 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3plot_data.c
--rw-rw-rw-   0        0        0     4251 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3plot_error_macros.h
--rw-rw-rw-   0        0        0     6690 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/d3plot_part_nodes.c
--rw-rw-rw-   0        0        0     5034 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/d3plot_part_nodes.h
--rw-rw-rw-   0        0        0    12188 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3plot_state.c
--rw-rw-rw-   0        0        0     4550 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/extra_string.c
--rw-rw-rw-   0        0        0     2236 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/extra_string.h
--rw-rw-rw-   0        0        0    51337 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/key.c
--rw-rw-rw-   0        0        0    10852 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/key.h
--rw-rw-rw-   0        0        0     6492 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/multi_file.c
--rw-rw-rw-   0        0        0     3161 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/multi_file.h
--rw-rw-rw-   0        0        0     5980 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/path.c
--rw-rw-rw-   0        0        0     2671 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/path.h
--rw-rw-rw-   0        0        0     4143 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/path_view.c
--rw-rw-rw-   0        0        0     3545 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/path_view.h
--rw-rw-rw-   0        0        0    25367 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/pgni.h
--rw-rw-rw-   0        0        0     9855 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/profiling.c
--rw-rw-rw-   0        0        0     3589 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/profiling.h
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.645753 dynareadout-23.6/lib/dynareadout/src/python/
--rw-rw-rw-   0        0        0    17631 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/python/conversions.hpp
--rw-rw-rw-   0        0        0     5735 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/python/pybind11_binout.cpp
--rw-rw-rw-   0        0        0    19773 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/python/pybind11_d3plot.cpp
--rw-rw-rw-   0        0        0     4897 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/python/pybind11_key.cpp
--rw-rw-rw-   0        0        0     1786 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/python/pybind11_module.cpp
--rw-rw-rw-   0        0        0     3348 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/sync.c
--rw-rw-rw-   0        0        0     2158 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/sync.h
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.646750 dynareadout-23.6/lib/pybind11/
--rw-rw-rw-   0        0        0     1713 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.593890 dynareadout-23.6/lib/pybind11/include/
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.662709 dynareadout-23.6/lib/pybind11/include/pybind11/
--rw-rw-rw-   0        0        0    24657 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/attr.h
--rw-rw-rw-   0        0        0     7262 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/buffer_info.h
--rw-rw-rw-   0        0        0    67301 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/cast.h
--rw-rw-rw-   0        0        0     8683 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/chrono.h
--rw-rw-rw-   0        0        0      122 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/common.h
--rw-rw-rw-   0        0        0     2170 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/complex.h
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.668291 dynareadout-23.6/lib/pybind11/include/pybind11/detail/
--rw-rw-rw-   0        0        0    28986 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/class.h
--rw-rw-rw-   0        0        0    51557 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/common.h
--rw-rw-rw-   0        0        0     5649 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/descr.h
--rw-rw-rw-   0        0        0    18409 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/init.h
--rw-rw-rw-   0        0        0    25640 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/internals.h
--rw-rw-rw-   0        0        0    43276 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-rw-   0        0        0     1690 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/typeid.h
--rw-rw-rw-   0        0        0    32860 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/eigen.h
--rw-rw-rw-   0        0        0    12071 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/embed.h
--rw-rw-rw-   0        0        0     4887 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/eval.h
--rw-rw-rw-   0        0        0     4825 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/functional.h
--rw-rw-rw-   0        0        0     8501 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/gil.h
--rw-rw-rw-   0        0        0     9127 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/iostream.h
--rw-rw-rw-   0        0        0    81515 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/numpy.h
--rw-rw-rw-   0        0        0     9305 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/operators.h
--rw-rw-rw-   0        0        0     2257 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/options.h
--rw-rw-rw-   0        0        0   128619 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/pybind11.h
--rw-rw-rw-   0        0        0    96315 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/pytypes.h
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.669291 dynareadout-23.6/lib/pybind11/include/pybind11/stl/
--rw-rw-rw-   0        0        0     4301 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-rw-   0        0        0    15783 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/stl.h
--rw-rw-rw-   0        0        0    27798 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/stl_bind.h
--rw-rw-rw-   0        0        0      858 2023-06-26 09:13:20.000000 dynareadout-23.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 09:18:13.675493 dynareadout-23.6/setup.cfg
--rw-rw-rw-   0        0        0     2776 2023-06-26 09:13:08.000000 dynareadout-23.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.594888 dynareadout-23.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.670288 dynareadout-23.6/src/dynareadout/
--rw-rw-rw-   0        0        0     1858 2023-04-24 08:55:05.000000 dynareadout-23.6/src/dynareadout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.674495 dynareadout-23.6/src/dynareadout.egg-info/
--rw-rw-rw-   0        0        0     5295 2023-06-26 09:18:13.000000 dynareadout-23.6/src/dynareadout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3297 2023-06-26 09:18:13.000000 dynareadout-23.6/src/dynareadout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 09:18:13.000000 dynareadout-23.6/src/dynareadout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-01 09:15:58.000000 dynareadout-23.6/src/dynareadout.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-06-26 09:18:13.000000 dynareadout-23.6/src/dynareadout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-26 09:18:13.000000 dynareadout-23.6/src/dynareadout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.298045 dynareadout-23.7/
+-rw-rw-rw-   0        0        0      878 2023-02-10 08:49:54.000000 dynareadout-23.7/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-02-10 08:49:54.000000 dynareadout-23.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5094 2023-07-24 10:29:04.296979 dynareadout-23.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4292 2023-07-24 09:31:53.000000 dynareadout-23.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.015789 dynareadout-23.7/lib/
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.011261 dynareadout-23.7/lib/dynareadout/
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.135234 dynareadout-23.7/lib/dynareadout/src/
+-rw-rw-rw-   0        0        0    15215 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/binary_search.c
+-rw-rw-rw-   0        0        0     4052 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/binary_search.h
+-rw-rw-rw-   0        0        0    30254 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/binout.c
+-rw-rw-rw-   0        0        0     5776 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/binout.h
+-rw-rw-rw-   0        0        0     3252 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/binout_defines.h
+-rw-rw-rw-   0        0        0    11391 2023-02-10 08:50:17.000000 dynareadout-23.7/lib/dynareadout/src/binout_directory.c
+-rw-rw-rw-   0        0        0     5670 2023-02-10 08:50:17.000000 dynareadout-23.7/lib/dynareadout/src/binout_directory.h
+-rw-rw-rw-   0        0        0     3791 2023-02-10 08:50:17.000000 dynareadout-23.7/lib/dynareadout/src/binout_glob.c
+-rw-rw-rw-   0        0        0     1784 2023-02-10 08:50:17.000000 dynareadout-23.7/lib/dynareadout/src/binout_glob.h
+-rw-rw-rw-   0        0        0    16033 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/binout_read.c
+-rw-rw-rw-   0        0        0     6018 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/binout_read.h
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.170148 dynareadout-23.7/lib/dynareadout/src/cpp/
+-rw-rw-rw-   0        0        0    12414 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/cpp/array.hpp
+-rw-rw-rw-   0        0        0     9280 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/cpp/binout.cpp
+-rw-rw-rw-   0        0        0     3914 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/cpp/binout.hpp
+-rw-rw-rw-   0        0        0    19282 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/cpp/d3plot.cpp
+-rw-rw-rw-   0        0        0     8224 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/cpp/d3plot.hpp
+-rw-rw-rw-   0        0        0     7787 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/cpp/d3plot_part.cpp
+-rw-rw-rw-   0        0        0     4841 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/cpp/d3plot_part.hpp
+-rw-rw-rw-   0        0        0     4418 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/cpp/d3plot_state.cpp
+-rw-rw-rw-   0        0        0     3387 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/cpp/d3plot_state.hpp
+-rw-rw-rw-   0        0        0     7159 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/cpp/key.cpp
+-rw-rw-rw-   0        0        0    16619 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/cpp/key.hpp
+-rw-rw-rw-   0        0        0     2005 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/cpp/vec.hpp
+-rw-rw-rw-   0        0        0    22834 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/d3_buffer.c
+-rw-rw-rw-   0        0        0     4304 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/d3_buffer.h
+-rw-rw-rw-   0        0        0     7118 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/d3_defines.h
+-rw-rw-rw-   0        0        0    93312 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/d3plot.c
+-rw-rw-rw-   0        0        0    18155 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/d3plot.h
+-rw-rw-rw-   0        0        0    12437 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/d3plot_data.c
+-rw-rw-rw-   0        0        0     4251 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/d3plot_error_macros.h
+-rw-rw-rw-   0        0        0     6690 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/d3plot_part_nodes.c
+-rw-rw-rw-   0        0        0     5034 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/d3plot_part_nodes.h
+-rw-rw-rw-   0        0        0    12188 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/d3plot_state.c
+-rw-rw-rw-   0        0        0     4550 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/extra_string.c
+-rw-rw-rw-   0        0        0     2352 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/extra_string.h
+-rw-rw-rw-   0        0        0    48776 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/key.c
+-rw-rw-rw-   0        0        0    10852 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/key.h
+-rw-rw-rw-   0        0        0     3742 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/line.c
+-rw-rw-rw-   0        0        0     2695 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/line.h
+-rw-rw-rw-   0        0        0     6277 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/multi_file.c
+-rw-rw-rw-   0        0        0     3161 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/multi_file.h
+-rw-rw-rw-   0        0        0     5980 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/path.c
+-rw-rw-rw-   0        0        0     2671 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/path.h
+-rw-rw-rw-   0        0        0     4143 2023-02-10 08:50:17.000000 dynareadout-23.7/lib/dynareadout/src/path_view.c
+-rw-rw-rw-   0        0        0     3545 2023-02-10 08:50:17.000000 dynareadout-23.7/lib/dynareadout/src/path_view.h
+-rw-rw-rw-   0        0        0    25367 2023-02-10 08:50:17.000000 dynareadout-23.7/lib/dynareadout/src/pgni.h
+-rw-rw-rw-   0        0        0     9855 2023-02-10 08:50:17.000000 dynareadout-23.7/lib/dynareadout/src/profiling.c
+-rw-rw-rw-   0        0        0     3589 2023-02-10 08:50:17.000000 dynareadout-23.7/lib/dynareadout/src/profiling.h
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.185011 dynareadout-23.7/lib/dynareadout/src/python/
+-rw-rw-rw-   0        0        0    17631 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/python/conversions.hpp
+-rw-rw-rw-   0        0        0     7292 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/python/pybind11_binout.cpp
+-rw-rw-rw-   0        0        0    21203 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/python/pybind11_d3plot.cpp
+-rw-rw-rw-   0        0        0     6543 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/python/pybind11_key.cpp
+-rw-rw-rw-   0        0        0     1782 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/python/pybind11_module.cpp
+-rw-rw-rw-   0        0        0     3348 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/sync.c
+-rw-rw-rw-   0        0        0     2158 2023-07-24 09:32:42.000000 dynareadout-23.7/lib/dynareadout/src/sync.h
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.187700 dynareadout-23.7/lib/pybind11/
+-rw-rw-rw-   0        0        0     1713 2023-02-10 08:50:17.000000 dynareadout-23.7/lib/pybind11/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.016802 dynareadout-23.7/lib/pybind11/include/
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.241679 dynareadout-23.7/lib/pybind11/include/pybind11/
+-rw-rw-rw-   0        0        0    25024 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/attr.h
+-rw-rw-rw-   0        0        0     7958 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/buffer_info.h
+-rw-rw-rw-   0        0        0    69016 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/cast.h
+-rw-rw-rw-   0        0        0     8683 2023-02-10 08:50:18.000000 dynareadout-23.7/lib/pybind11/include/pybind11/chrono.h
+-rw-rw-rw-   0        0        0      122 2023-02-10 08:50:18.000000 dynareadout-23.7/lib/pybind11/include/pybind11/common.h
+-rw-rw-rw-   0        0        0     2170 2023-02-10 08:50:18.000000 dynareadout-23.7/lib/pybind11/include/pybind11/complex.h
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.259200 dynareadout-23.7/lib/pybind11/include/pybind11/detail/
+-rw-rw-rw-   0        0        0    29261 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/detail/class.h
+-rw-rw-rw-   0        0        0    54735 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/detail/common.h
+-rw-rw-rw-   0        0        0     6133 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/detail/descr.h
+-rw-rw-rw-   0        0        0    18293 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/detail/init.h
+-rw-rw-rw-   0        0        0    28877 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/detail/internals.h
+-rw-rw-rw-   0        0        0    49541 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-rw-   0        0        0     1690 2023-02-10 08:50:18.000000 dynareadout-23.7/lib/pybind11/include/pybind11/detail/typeid.h
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.267760 dynareadout-23.7/lib/pybind11/include/pybind11/eigen/
+-rw-rw-rw-   0        0        0      387 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/eigen/common.h
+-rw-rw-rw-   0        0        0    32849 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/eigen/matrix.h
+-rw-rw-rw-   0        0        0    18958 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/eigen/tensor.h
+-rw-rw-rw-   0        0        0      328 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/eigen.h
+-rw-rw-rw-   0        0        0    13775 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/embed.h
+-rw-rw-rw-   0        0        0     4887 2023-02-10 08:50:18.000000 dynareadout-23.7/lib/pybind11/include/pybind11/eval.h
+-rw-rw-rw-   0        0        0     5139 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/functional.h
+-rw-rw-rw-   0        0        0     8501 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/gil.h
+-rw-rw-rw-   0        0        0     9127 2023-02-10 08:50:18.000000 dynareadout-23.7/lib/pybind11/include/pybind11/iostream.h
+-rw-rw-rw-   0        0        0    81723 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/numpy.h
+-rw-rw-rw-   0        0        0     9305 2023-02-10 08:50:18.000000 dynareadout-23.7/lib/pybind11/include/pybind11/operators.h
+-rw-rw-rw-   0        0        0     2826 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/options.h
+-rw-rw-rw-   0        0        0   129596 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/pybind11.h
+-rw-rw-rw-   0        0        0   101012 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/pytypes.h
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.269925 dynareadout-23.7/lib/pybind11/include/pybind11/stl/
+-rw-rw-rw-   0        0        0     4301 2023-02-10 08:50:18.000000 dynareadout-23.7/lib/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-rw-   0        0        0    15924 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/stl.h
+-rw-rw-rw-   0        0        0    30748 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/stl_bind.h
+-rw-rw-rw-   0        0        0     1990 2023-07-24 09:32:56.000000 dynareadout-23.7/lib/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+-rw-rw-rw-   0        0        0      848 2023-07-24 09:31:53.000000 dynareadout-23.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 10:29:04.298045 dynareadout-23.7/setup.cfg
+-rw-rw-rw-   0        0        0     2827 2023-07-24 09:31:53.000000 dynareadout-23.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.021830 dynareadout-23.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 10:29:04.294189 dynareadout-23.7/src/dynareadout.egg-info/
+-rw-rw-rw-   0        0        0     5094 2023-07-24 10:29:03.000000 dynareadout-23.7/src/dynareadout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3477 2023-07-24 10:29:04.000000 dynareadout-23.7/src/dynareadout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 10:29:03.000000 dynareadout-23.7/src/dynareadout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-10 08:50:46.000000 dynareadout-23.7/src/dynareadout.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-07-24 10:29:03.000000 dynareadout-23.7/src/dynareadout.egg-info/top_level.txt
```

### Comparing `dynareadout-23.6/LICENSE` & `dynareadout-23.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/PKG-INFO` & `dynareadout-23.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dynareadout
-Version: 23.6
-Summary: Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
+Version: 23.7
+Summary: High-Performance and Thread-Safe library for parsing binary output files and key files of LS Dyna (d3plot, binout, input deck)
 Author-email: PucklaJ <jonaas.pucher000000@gmail.com>
 Project-URL: Homepage, https://github.com/PucklaJ/dynareadout
 Project-URL: Bug Trackers, https://github.com/PucklaJ/dynareadout/issues
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: zlib/libpng License
 Classifier: Operating System :: Microsoft :: Windows
@@ -14,64 +14,53 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dynareadout
 
-An Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
+High-Performance and Thread-Safe C/C++ library for parsing binary output files and key files of LS Dyna (d3plot, binout, input deck) with bindings for python.
 
 ## Documentation
 
 You can find a [Wiki](https://github.com/PucklaJ/dynareadout/wiki) with API Documentation for python.
 
 ## Examples
 
 ### Binout
 
 ```python
-from dynareadout import Binout, BinoutType
+from dynareadout import Binout
 
 bin_file = None
 try:
   # This library also supports opening multiple binout files at once by globing them
-  bin_file = Binout("simulation/binout*")
+  bin_file = Binout("path/to/your/binout*")
 except RuntimeError as e:
   print("Failed to open binout: {}".format(e))
   exit(1)
 
 # Print the children of the binout
 children = bin_file.read("/")
 for (i, child) in enumerate(children):
   print("Child {}: {}".format(i, child))
 
 # Read some data. This read method can read variables with different types, but
 # there are also read methods for particular types
 node_ids = bin_file.read("nodout/ids")
-for (i, nid) in enumerate(node_ids):
-  print("Node ID {}: {}".format(i, nid))
+for i in range(len(node_ids)):
+  print("Node ID {}: {}".format(i, node_ids[i]))
 
-# You can also read this variable with the read method of the particular type
-# First find out what the type is
-node_ids_type = bin_file.get_type_id("/nodout/metadata/ids")
-
-# Then read the data using the special read method.
-# If you already know the exact type and path of a variable
-# these methods can be a bit more performant,
-# since the library does not need the get the type and path first.
-if node_ids_type == BinoutType.Int32:
-  node_ids = bin_file.read_int32("/nodout/metadata/ids")
-elif node_ids_type == BinoutType.Int64:
-  node_ids = bin_file.read_int64("/nodout/metadata/ids")
-else:
-  print("The node ids are not 32-Bit or 64-Bit integers")
-  exit(1)
+# You can also find out if a variable exists
+node_ids_exist = bin_file.variable_exists("/nodout/metadata/ids")
 
-for (i, nid) in enumerate(node_ids):
-  print("Node ID {}: {}".format(i, nid))
+# Get the number of time steps in the binout
+nodout_timesteps = bin_file.get_num_timesteps("/nodout")
+# The time steps can vary inside the binout
+rcforc_timesteps = bin_file.get_num_timesteps("/rcforc")
 
 # If you want to read "timed" data (x_displacement, x_force, etc.) you can do so also with the read method
 x_displacement = bin_file.read("nodout/x_displacement")
 for (t, time_step) in enumerate(x_displacement):
   for (n, x_disp) in enumerate(time_step):
     print("X Displacement time_step={}, node_id={}: {}".format(t, node_ids[n], x_displacement[t][n]))
 ```
@@ -80,16 +69,16 @@
 
 ```python
 from dynareadout import D3plot
 
 plot_file = None
 try:
   # Just give it the first d3plot file and it opens all of them
-  plot_file = D3plot("simulation/d3plot")
-except e as RuntimeError:
+  plot_file = D3plot("path/to/your/d3plot")
+except RuntimeError as e:
   print("Failed to open: {}".format(e))
   exit(1)
 
 # Read the title
 title = plot_file.read_title()
 print("Title: {}".format(title))
 
@@ -106,27 +95,27 @@
 ```
 
 ### KeyFile
 
 ```python
 from dynareadout import key_file_parse
 
-keywords = key_file_parse("simulation/input.k")
+keywords = key_file_parse("path/to/your/input.k")
 
 # Parse all nodes
 node_keywords = keywords["NODE"]
 
+# Loop over all *NODE keywords
 for i in range(len(node_keywords)):
+  # Loop over all cards of each *NODE keyword
   for j in range(len(node_keywords[i])):
     node = node_keywords[i][j]
-    node_data = node.parse_whole([8, 16, 16, 16])
-    nid = node_data[0]
-    x = node_data[1]
-    y = node_data[2]
-    z = node_data[3]
+    # Then you can parse the variables of each card as integers and floats
+    # The list of integers holds all the widths of each variable in the card in characters
+    nid, x, y, z = node.parse_whole([8, 16, 16, 16])
 
     print(f"NODE {nid:d}: ({x:.3f}; {y:.3f}; {z:.3f})")
 ```
 
 ## Other languages
 
 This library is also available for C and C++ this version can be found [here](https://github.com/PucklaJ/dynareadout).
```

### Comparing `dynareadout-23.6/README.md` & `dynareadout-23.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,48 @@
 # dynareadout
 
-An Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
+High-Performance and Thread-Safe C/C++ library for parsing binary output files and key files of LS Dyna (d3plot, binout, input deck) with bindings for python.
 
 ## Documentation
 
 You can find a [Wiki](https://github.com/PucklaJ/dynareadout/wiki) with API Documentation for python.
 
 ## Examples
 
 ### Binout
 
 ```python
-from dynareadout import Binout, BinoutType
+from dynareadout import Binout
 
 bin_file = None
 try:
   # This library also supports opening multiple binout files at once by globing them
-  bin_file = Binout("simulation/binout*")
+  bin_file = Binout("path/to/your/binout*")
 except RuntimeError as e:
   print("Failed to open binout: {}".format(e))
   exit(1)
 
 # Print the children of the binout
 children = bin_file.read("/")
 for (i, child) in enumerate(children):
   print("Child {}: {}".format(i, child))
 
 # Read some data. This read method can read variables with different types, but
 # there are also read methods for particular types
 node_ids = bin_file.read("nodout/ids")
-for (i, nid) in enumerate(node_ids):
-  print("Node ID {}: {}".format(i, nid))
+for i in range(len(node_ids)):
+  print("Node ID {}: {}".format(i, node_ids[i]))
 
-# You can also read this variable with the read method of the particular type
-# First find out what the type is
-node_ids_type = bin_file.get_type_id("/nodout/metadata/ids")
-
-# Then read the data using the special read method.
-# If you already know the exact type and path of a variable
-# these methods can be a bit more performant,
-# since the library does not need the get the type and path first.
-if node_ids_type == BinoutType.Int32:
-  node_ids = bin_file.read_int32("/nodout/metadata/ids")
-elif node_ids_type == BinoutType.Int64:
-  node_ids = bin_file.read_int64("/nodout/metadata/ids")
-else:
-  print("The node ids are not 32-Bit or 64-Bit integers")
-  exit(1)
+# You can also find out if a variable exists
+node_ids_exist = bin_file.variable_exists("/nodout/metadata/ids")
 
-for (i, nid) in enumerate(node_ids):
-  print("Node ID {}: {}".format(i, nid))
+# Get the number of time steps in the binout
+nodout_timesteps = bin_file.get_num_timesteps("/nodout")
+# The time steps can vary inside the binout
+rcforc_timesteps = bin_file.get_num_timesteps("/rcforc")
 
 # If you want to read "timed" data (x_displacement, x_force, etc.) you can do so also with the read method
 x_displacement = bin_file.read("nodout/x_displacement")
 for (t, time_step) in enumerate(x_displacement):
   for (n, x_disp) in enumerate(time_step):
     print("X Displacement time_step={}, node_id={}: {}".format(t, node_ids[n], x_displacement[t][n]))
 ```
@@ -62,16 +51,16 @@
 
 ```python
 from dynareadout import D3plot
 
 plot_file = None
 try:
   # Just give it the first d3plot file and it opens all of them
-  plot_file = D3plot("simulation/d3plot")
-except e as RuntimeError:
+  plot_file = D3plot("path/to/your/d3plot")
+except RuntimeError as e:
   print("Failed to open: {}".format(e))
   exit(1)
 
 # Read the title
 title = plot_file.read_title()
 print("Title: {}".format(title))
 
@@ -88,27 +77,27 @@
 ```
 
 ### KeyFile
 
 ```python
 from dynareadout import key_file_parse
 
-keywords = key_file_parse("simulation/input.k")
+keywords = key_file_parse("path/to/your/input.k")
 
 # Parse all nodes
 node_keywords = keywords["NODE"]
 
+# Loop over all *NODE keywords
 for i in range(len(node_keywords)):
+  # Loop over all cards of each *NODE keyword
   for j in range(len(node_keywords[i])):
     node = node_keywords[i][j]
-    node_data = node.parse_whole([8, 16, 16, 16])
-    nid = node_data[0]
-    x = node_data[1]
-    y = node_data[2]
-    z = node_data[3]
+    # Then you can parse the variables of each card as integers and floats
+    # The list of integers holds all the widths of each variable in the card in characters
+    nid, x, y, z = node.parse_whole([8, 16, 16, 16])
 
     print(f"NODE {nid:d}: ({x:.3f}; {y:.3f}; {z:.3f})")
 ```
 
 ## Other languages
 
 This library is also available for C and C++ this version can be found [here](https://github.com/PucklaJ/dynareadout).
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/binary_search.c` & `dynareadout-23.7/lib/dynareadout/src/binary_search.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/binary_search.h` & `dynareadout-23.7/lib/dynareadout/src/binary_search.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/binout.c` & `dynareadout-23.7/lib/dynareadout/src/binout.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/binout.h` & `dynareadout-23.7/lib/dynareadout/src/binout.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/binout_defines.h` & `dynareadout-23.7/lib/dynareadout/src/binout_defines.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/binout_directory.c` & `dynareadout-23.7/lib/dynareadout/src/binout_directory.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/binout_directory.h` & `dynareadout-23.7/lib/dynareadout/src/binout_directory.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/binout_glob.c` & `dynareadout-23.7/lib/dynareadout/src/binout_glob.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/binout_glob.h` & `dynareadout-23.7/lib/dynareadout/src/binout_glob.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/binout_read.c` & `dynareadout-23.7/lib/dynareadout/src/binout_read.c`

 * *Files 21% similar despite different names*

```diff
@@ -364,14 +364,102 @@
   double *data = (double *)_binout_read(bin_file, path_to_variable, data_size,
                                         BINOUT_TYPE_FLOAT64);
 
   END_PROFILE_FUNC();
   return data;
 }
 
+int8_t *binout_read_timed_i8(binout_file *bin_file, const char *variable,
+                             size_t *num_values, size_t *num_timesteps) {
+  BEGIN_PROFILE_FUNC();
+
+  int8_t *data = (int8_t *)_binout_read_timed(bin_file, variable, num_values,
+                                              num_timesteps, BINOUT_TYPE_INT8);
+
+  END_PROFILE_FUNC();
+  return data;
+}
+
+int16_t *binout_read_timed_i16(binout_file *bin_file, const char *variable,
+                               size_t *num_values, size_t *num_timesteps) {
+  BEGIN_PROFILE_FUNC();
+
+  int16_t *data = (int16_t *)_binout_read_timed(
+      bin_file, variable, num_values, num_timesteps, BINOUT_TYPE_INT16);
+
+  END_PROFILE_FUNC();
+  return data;
+}
+
+int32_t *binout_read_timed_i32(binout_file *bin_file, const char *variable,
+                               size_t *num_values, size_t *num_timesteps) {
+  BEGIN_PROFILE_FUNC();
+
+  int32_t *data = (int32_t *)_binout_read_timed(
+      bin_file, variable, num_values, num_timesteps, BINOUT_TYPE_INT32);
+
+  END_PROFILE_FUNC();
+  return data;
+}
+
+int64_t *binout_read_timed_i64(binout_file *bin_file, const char *variable,
+                               size_t *num_values, size_t *num_timesteps) {
+  BEGIN_PROFILE_FUNC();
+
+  int64_t *data = (int64_t *)_binout_read_timed(
+      bin_file, variable, num_values, num_timesteps, BINOUT_TYPE_INT64);
+
+  END_PROFILE_FUNC();
+  return data;
+}
+
+uint8_t *binout_read_timed_u8(binout_file *bin_file, const char *variable,
+                              size_t *num_values, size_t *num_timesteps) {
+  BEGIN_PROFILE_FUNC();
+
+  uint8_t *data = (uint8_t *)_binout_read_timed(
+      bin_file, variable, num_values, num_timesteps, BINOUT_TYPE_UINT8);
+
+  END_PROFILE_FUNC();
+  return data;
+}
+
+uint16_t *binout_read_timed_u16(binout_file *bin_file, const char *variable,
+                                size_t *num_values, size_t *num_timesteps) {
+  BEGIN_PROFILE_FUNC();
+
+  uint16_t *data = (uint16_t *)_binout_read_timed(
+      bin_file, variable, num_values, num_timesteps, BINOUT_TYPE_UINT16);
+
+  END_PROFILE_FUNC();
+  return data;
+}
+
+uint32_t *binout_read_timed_u32(binout_file *bin_file, const char *variable,
+                                size_t *num_values, size_t *num_timesteps) {
+  BEGIN_PROFILE_FUNC();
+
+  uint32_t *data = (uint32_t *)_binout_read_timed(
+      bin_file, variable, num_values, num_timesteps, BINOUT_TYPE_UINT32);
+
+  END_PROFILE_FUNC();
+  return data;
+}
+
+uint64_t *binout_read_timed_u64(binout_file *bin_file, const char *variable,
+                                size_t *num_values, size_t *num_timesteps) {
+  BEGIN_PROFILE_FUNC();
+
+  uint64_t *data = (uint64_t *)_binout_read_timed(
+      bin_file, variable, num_values, num_timesteps, BINOUT_TYPE_UINT64);
+
+  END_PROFILE_FUNC();
+  return data;
+}
+
 float *binout_read_timed_f32(binout_file *bin_file, const char *variable,
                              size_t *num_values, size_t *num_timesteps) {
   BEGIN_PROFILE_FUNC();
 
   float *data = (float *)_binout_read_timed(bin_file, variable, num_values,
                                             num_timesteps, BINOUT_TYPE_FLOAT32);
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/binout_read.h` & `dynareadout-23.7/lib/dynareadout/src/binout_read.h`

 * *Files 22% similar despite different names*

```diff
@@ -80,14 +80,30 @@
 
 /* Read a variable under the dxxxxxx folders. This functions reads all timesteps
  * of a variable at once. If the actual variable is something like
  * "/nodout/d000000/x_displacement" then variable has to be
  * "/nodout/x_displacement". The shape of the array is num_timesteps *
  * num_values which means to get a value you need to index like [timestep *
  * num_values + value]*/
+int8_t *binout_read_timed_i8(binout_file *bin_file, const char *variable,
+                             size_t *num_values, size_t *num_timesteps);
+int16_t *binout_read_timed_i16(binout_file *bin_file, const char *variable,
+                               size_t *num_values, size_t *num_timesteps);
+int32_t *binout_read_timed_i32(binout_file *bin_file, const char *variable,
+                               size_t *num_values, size_t *num_timesteps);
+int64_t *binout_read_timed_i64(binout_file *bin_file, const char *variable,
+                               size_t *num_values, size_t *num_timesteps);
+uint8_t *binout_read_timed_u8(binout_file *bin_file, const char *variable,
+                              size_t *num_values, size_t *num_timesteps);
+uint16_t *binout_read_timed_u16(binout_file *bin_file, const char *variable,
+                                size_t *num_values, size_t *num_timesteps);
+uint32_t *binout_read_timed_u32(binout_file *bin_file, const char *variable,
+                                size_t *num_values, size_t *num_timesteps);
+uint64_t *binout_read_timed_u64(binout_file *bin_file, const char *variable,
+                                size_t *num_values, size_t *num_timesteps);
 float *binout_read_timed_f32(binout_file *bin_file, const char *variable,
                              size_t *num_values, size_t *num_timesteps);
 double *binout_read_timed_f64(binout_file *bin_file, const char *variable,
                               size_t *num_values, size_t *num_timesteps);
 
 #ifdef __cplusplus
 }
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/cpp/array.hpp` & `dynareadout-23.7/lib/dynareadout/src/cpp/array.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -127,16 +127,16 @@
   // delete_data .... Wether to free data in the destructor
   Array() noexcept;
   Array(T *data, size_t size, bool delete_data = true) noexcept;
   Array(Array<T> &&rhs) noexcept;
   Array(const Array<T> &rhs) = delete;
   virtual ~Array() noexcept;
 
-  inline T &operator[](size_t index);
-  inline const T &operator[](size_t index) const;
+  virtual inline T &operator[](size_t index);
+  virtual inline const T &operator[](size_t index) const;
   Array<T> &operator=(Array<T> &&rhs) noexcept;
   bool operator==(const char *str2) const noexcept;
   bool operator==(const std::string &str2) const noexcept;
   bool operator==(const Array<T> &rhs) const noexcept;
 
   T *data() noexcept { return m_data; }
   const T *data() const noexcept { return m_data; }
@@ -163,15 +163,16 @@
 };
 
 class String : public Array<char> {
 public:
   String(char *str, bool delete_data = true) noexcept
       : Array<char>(str, ~0, delete_data) {}
 
-  inline size_t size() const { return strlen(m_data); }
+  inline size_t size() const noexcept { return strlen(m_data); }
+  inline bool empty() const noexcept { return m_data[0] == '\0'; }
 
   std::string str() const noexcept { return std::string(m_data); }
 
   bool operator==(const char *other) const noexcept {
     size_t i = 0;
     for (; m_data[i] != '\0' && other[i] != '\0'; i++) {
       if (m_data[i] != other[i]) {
@@ -191,14 +192,17 @@
 
     return m_data[i] == '\0' && rhs.m_data[i] == '\0';
   }
 
   bool operator==(const std::string &rhs) const noexcept {
     return operator==(rhs.c_str());
   }
+
+  inline char &operator[](size_t index) override;
+  inline const char &operator[](size_t index) const override;
 };
 
 class SizedString : public Array<char> {
 public:
   SizedString(char *str, size_t size, bool delete_data = true) noexcept
       : Array<char>(str, size, delete_data) {}
 
@@ -241,21 +245,21 @@
   bool operator==(const std::string &rhs) const noexcept {
     return operator==(rhs.c_str());
   }
 };
 
 static bool operator==(const String &str1, const SizedString &str2) noexcept {
   size_t i = 0;
-  for (; i < str1[i] != '\0' && i < str2.size(); i++) {
+  for (; i < str1.data()[i] != '\0' && i < str2.size(); i++) {
     if (str1[i] != str2[i]) {
       return false;
     }
   }
 
-  return i == str2.size() && str1[i] == '\0';
+  return i == str2.size() && str1.data()[i] == '\0';
 }
 
 inline bool operator==(const SizedString &str2, const String &str1) noexcept {
   return str1 == str2;
 }
 
 static std::ostream &operator<<(std::ostream &stream, const String &str) {
@@ -335,14 +339,34 @@
   if (empty() || index > m_size - 1) {
     throw std::runtime_error("Index out of Range");
   }
 
   return m_data[index];
 }
 
+char &String::operator[](size_t index) {
+  for (size_t i = 0; m_data[i] != '\0'; i++) {
+    if (i == index) {
+      return m_data[i];
+    }
+  }
+
+  throw std::runtime_error("Index out of Range");
+}
+
+const char &String::operator[](size_t index) const {
+  for (size_t i = 0; m_data[i] != '\0'; i++) {
+    if (i == index) {
+      return m_data[i];
+    }
+  }
+
+  throw std::runtime_error("Index out of Range");
+}
+
 template <typename T> Array<T> &Array<T>::operator=(Array<T> &&rhs) noexcept {
   m_data = rhs.m_data;
   m_size = rhs.m_size;
   m_delete_data = rhs.m_delete_data;
   rhs.m_data = nullptr;
   rhs.m_size = 0;
   rhs.m_delete_data = false;
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/cpp/binout.cpp` & `dynareadout-23.7/lib/dynareadout/src/cpp/binout.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -21,41 +21,42 @@
  * misrepresented as being the original software.
  *
  * 3. This notice may not be removed or altered from any source distribution.
  ************************************************************************************/
 
 #include "binout.hpp"
 #include <cstring>
+#include <functional>
 
 namespace dro {
 
-Binout::Exception::Exception(String error_str) noexcept
+Binout::Exception::Exception(Binout::Exception::ErrorString error_str) noexcept
     : m_error_str(std::move(error_str)) {}
 
 const char *Binout::Exception::what() const noexcept {
   return m_error_str.data();
 }
 
 Binout::Binout(const std::filesystem::path &file_name) {
   m_handle = binout_open(file_name.string().c_str());
   char *open_error = binout_open_error(&m_handle);
   if (open_error) {
     // Call binout_close since the destructor is not getting called
     binout_close(&m_handle);
-    throw Exception(String(open_error));
+    throw Exception(Exception::ErrorString(open_error));
   }
 }
 
 Binout::~Binout() noexcept { binout_close(&m_handle); }
 
 BinoutType Binout::get_type_id(const std::string &path_to_variable) const {
   const BinoutType type_id{static_cast<BinoutType>(binout_get_type_id(
       const_cast<binout_file *>(&m_handle), path_to_variable.c_str()))};
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return type_id;
 }
 
 bool Binout::variable_exists(
     const std::string &path_to_variable) const noexcept {
@@ -68,15 +69,15 @@
   char **children = binout_get_children(const_cast<binout_file *>(&m_handle),
                                         path.c_str(), &num_children);
 
   // If the path does not exist
   if (children == nullptr && num_children == static_cast<size_t>(~0)) {
     char *msg = reinterpret_cast<char *>(malloc(256 + path.length()));
     sprintf(msg, "The path \"%s\" does not exist", path.c_str());
-    throw Exception(String(msg));
+    throw Exception(Exception::ErrorString(msg));
   }
 
   std::vector<String> children_vec;
   for (size_t i = 0; i < num_children; i++) {
     children_vec.emplace_back(children[i], false);
   }
 
@@ -84,178 +85,166 @@
   return children_vec;
 }
 
 size_t Binout::get_num_timesteps(const std::string &path) const {
   const size_t num_timesteps{binout_get_num_timesteps(&m_handle, path.c_str())};
 
   if (num_timesteps == (size_t)~0) {
-    throw Exception(String(
+    throw Exception(Exception::ErrorString(
         const_cast<char *>("The path does not exist or has files as children"),
         false));
   }
 
   return num_timesteps;
 }
 
-template <> Array<int8_t> Binout::read(const std::string &path_to_variable) {
-  size_t data_size;
-  int8_t *data =
-      binout_read_i8(&m_handle, path_to_variable.c_str(), &data_size);
-  if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+template <typename T>
+inline Array<T>
+Binout_read(Binout &bin_file,
+            std::function<T *(binout_file *handle, const char *path_to_variable,
+                              size_t *data_size)>
+                load_func,
+            const std::string &path_to_variable) {
+  size_t data_size;
+  T *data =
+      load_func(&bin_file.get_handle(), path_to_variable.c_str(), &data_size);
+  if (bin_file.get_handle().error_string) {
+    throw Binout::Exception(Binout::Exception::ErrorString(
+        bin_file.get_handle().error_string, false));
   }
 
-  return Array<int8_t>(data, data_size);
+  return Array<T>(data, data_size);
+}
+
+template <> Array<int8_t> Binout::read(const std::string &path_to_variable) {
+  return Binout_read<int8_t>(*this, binout_read_i8, path_to_variable);
 }
 
 template <> Array<int16_t> Binout::read(const std::string &path_to_variable) {
-  size_t data_size;
-  int16_t *data =
-      binout_read_i16(&m_handle, path_to_variable.c_str(), &data_size);
-  return Array<int16_t>(data, data_size);
+  return Binout_read<int16_t>(*this, binout_read_i16, path_to_variable);
 }
 
 template <> Array<int32_t> Binout::read(const std::string &path_to_variable) {
-  size_t data_size;
-  int32_t *data =
-      binout_read_i32(&m_handle, path_to_variable.c_str(), &data_size);
-  if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
-  }
-
-  return Array<int32_t>(data, data_size);
+  return Binout_read<int32_t>(*this, binout_read_i32, path_to_variable);
 }
 
 template <> Array<int64_t> Binout::read(const std::string &path_to_variable) {
-  size_t data_size;
-  int64_t *data =
-      binout_read_i64(&m_handle, path_to_variable.c_str(), &data_size);
-  if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
-  }
-
-  return Array<int64_t>(data, data_size);
+  return Binout_read<int64_t>(*this, binout_read_i64, path_to_variable);
 }
 
 template <> Array<uint8_t> Binout::read(const std::string &path_to_variable) {
-  size_t data_size;
-  uint8_t *data =
-      binout_read_u8(&m_handle, path_to_variable.c_str(), &data_size);
-  if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
-  }
-
-  return Array<uint8_t>(data, data_size);
+  return Binout_read<uint8_t>(*this, binout_read_u8, path_to_variable);
 }
 
 template <> Array<uint16_t> Binout::read(const std::string &path_to_variable) {
-  size_t data_size;
-  uint16_t *data =
-      binout_read_u16(&m_handle, path_to_variable.c_str(), &data_size);
-  if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
-  }
-
-  return Array<uint16_t>(data, data_size);
+  return Binout_read<uint16_t>(*this, binout_read_u16, path_to_variable);
 }
 
 template <> Array<uint32_t> Binout::read(const std::string &path_to_variable) {
-  size_t data_size;
-  uint32_t *data =
-      binout_read_u32(&m_handle, path_to_variable.c_str(), &data_size);
-  if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
-  }
-
-  return Array<uint32_t>(data, data_size);
+  return Binout_read<uint32_t>(*this, binout_read_u32, path_to_variable);
 }
 
 template <> Array<uint64_t> Binout::read(const std::string &path_to_variable) {
-  size_t data_size;
-  uint64_t *data =
-      binout_read_u64(&m_handle, path_to_variable.c_str(), &data_size);
-  if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
-  }
-
-  return Array<uint64_t>(data, data_size);
+  return Binout_read<uint64_t>(*this, binout_read_u64, path_to_variable);
 }
 
 template <> Array<float> Binout::read(const std::string &path_to_variable) {
-  size_t data_size;
-  float *data =
-      binout_read_f32(&m_handle, path_to_variable.c_str(), &data_size);
-  if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
-  }
-
-  return Array<float>(data, data_size);
+  return Binout_read<float>(*this, binout_read_f32, path_to_variable);
 }
 
 template <> Array<double> Binout::read(const std::string &path_to_variable) {
-  size_t data_size;
-  double *data =
-      binout_read_f64(&m_handle, path_to_variable.c_str(), &data_size);
-  if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
-  }
-
-  return Array<double>(data, data_size);
+  return Binout_read<double>(*this, binout_read_f64, path_to_variable);
 }
 
-template <>
-std::vector<Array<float>> Binout::read_timed(const std::string &variable) {
+template <typename T>
+inline std::vector<Array<T>>
+Binout_read_timed(Binout &bin_file,
+                  std::function<T *(binout_file *handle, const char *variable,
+                                    size_t *num_values, size_t *num_timesteps)>
+                      load_func,
+                  const std::string &variable) {
   size_t num_values, num_timesteps;
-  float *data = binout_read_timed_f32(&m_handle, variable.c_str(), &num_values,
-                                      &num_timesteps);
-  if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+  T *data = load_func(&bin_file.get_handle(), variable.c_str(), &num_values,
+                      &num_timesteps);
+  if (bin_file.get_handle().error_string) {
+    throw Binout::Exception(Binout::Exception::ErrorString(
+        bin_file.get_handle().error_string, false));
   }
 
-  std::vector<Array<float>> vec;
-  vec.resize(num_timesteps);
+  std::vector<Array<T>> vec(num_timesteps);
 
   for (size_t t = 0; t < num_timesteps; t++) {
-    vec[t] = Array<float>(&data[t * num_values], num_values, t == 0);
+    vec[t] = Array<T>(&data[t * num_values], num_values, t == 0);
   }
 
   return vec;
 }
 
 template <>
-std::vector<Array<double>> Binout::read_timed(const std::string &variable) {
-  size_t num_values, num_timesteps;
-  double *data = binout_read_timed_f64(&m_handle, variable.c_str(), &num_values,
-                                       &num_timesteps);
-  if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
-  }
+std::vector<Array<int8_t>> Binout::read_timed(const std::string &variable) {
+  return Binout_read_timed<int8_t>(*this, binout_read_timed_i8, variable);
+}
 
-  std::vector<Array<double>> vec;
-  vec.resize(num_timesteps);
+template <>
+std::vector<Array<int16_t>> Binout::read_timed(const std::string &variable) {
+  return Binout_read_timed<int16_t>(*this, binout_read_timed_i16, variable);
+}
 
-  for (size_t t = 0; t < num_timesteps; t++) {
-    vec[t] = Array<double>(&data[t * num_values], num_values, t == 0);
-  }
+template <>
+std::vector<Array<int32_t>> Binout::read_timed(const std::string &variable) {
+  return Binout_read_timed<int32_t>(*this, binout_read_timed_i32, variable);
+}
 
-  return vec;
+template <>
+std::vector<Array<int64_t>> Binout::read_timed(const std::string &variable) {
+  return Binout_read_timed<int64_t>(*this, binout_read_timed_i64, variable);
+}
+
+template <>
+std::vector<Array<uint8_t>> Binout::read_timed(const std::string &variable) {
+  return Binout_read_timed<uint8_t>(*this, binout_read_timed_u8, variable);
+}
+
+template <>
+std::vector<Array<uint16_t>> Binout::read_timed(const std::string &variable) {
+  return Binout_read_timed<uint16_t>(*this, binout_read_timed_u16, variable);
+}
+
+template <>
+std::vector<Array<uint32_t>> Binout::read_timed(const std::string &variable) {
+  return Binout_read_timed<uint32_t>(*this, binout_read_timed_u32, variable);
+}
+
+template <>
+std::vector<Array<uint64_t>> Binout::read_timed(const std::string &variable) {
+  return Binout_read_timed<uint64_t>(*this, binout_read_timed_u64, variable);
+}
+
+template <>
+std::vector<Array<float>> Binout::read_timed(const std::string &variable) {
+  return Binout_read_timed<float>(*this, binout_read_timed_f32, variable);
+}
+
+template <>
+std::vector<Array<double>> Binout::read_timed(const std::string &variable) {
+  return Binout_read_timed<double>(*this, binout_read_timed_f64, variable);
 }
 
 std::string Binout::simple_path_to_real(const std::string &simple,
                                         BinoutType &type_id,
                                         bool &timed) const {
   uint8_t type_id_c;
   int timed_c;
 
   char *real_path = binout_simple_path_to_real(&m_handle, simple.c_str(),
                                                &type_id_c, &timed_c);
   if (!real_path) {
     char *msg = reinterpret_cast<char *>(malloc(256 + simple.length()));
     sprintf(msg, "The simple path \"%s\" can not be found", simple.c_str());
-    throw Exception(String(msg));
+    throw Exception(Exception::ErrorString(msg));
   }
 
   type_id = static_cast<BinoutType>(type_id_c);
   timed = timed_c != 0;
 
   std::string str(real_path);
   free(real_path);
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/cpp/binout.hpp` & `dynareadout-23.7/lib/dynareadout/src/cpp/binout.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -48,20 +48,35 @@
 
 // This class is used to open and read data from a binout file (or multiple
 // files by globbing)
 class Binout {
 public:
   class Exception : public std::exception {
   public:
-    Exception(String error_str) noexcept;
+#ifdef _WIN32
+    // On windows python scripts crash when deallocated the memory of a thrown
+    // exception
+    class ErrorString : public std::string {
+    public:
+      ErrorString(char *str, bool delete_data = true) noexcept
+          : std::string(str) {
+        if (delete_data)
+          free(str);
+      }
+    };
+#else
+    using ErrorString = String;
+#endif
+
+    Exception(ErrorString error_str) noexcept;
 
     const char *what() const noexcept override;
 
   private:
-    const String m_error_str;
+    const ErrorString m_error_str;
   };
 
   // Open a binout file (or multiple files by globbing) and parse its records to
   // be ready to read data
   Binout(const std::filesystem::path &file_name);
   ~Binout() noexcept;
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/cpp/d3plot.cpp` & `dynareadout-23.7/lib/dynareadout/src/cpp/d3plot.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  ************************************************************************************/
 
 #include "d3plot.hpp"
 #include <ctime>
 
 namespace dro {
 
-D3plot::Exception::Exception(String error_str) noexcept
+D3plot::Exception::Exception(D3plot::Exception::ErrorString error_str) noexcept
     : m_error_str(std::move(error_str)) {}
 
 const char *D3plot::Exception::what() const noexcept {
   return m_error_str.data();
 }
 
 size_t D3plot::index_for_id(const Array<d3_word> &ids, d3_word id) {
@@ -44,95 +44,95 @@
   if (m_handle.error_string) {
     // Copy the error string and call d3plot_close since the destructor is not
     // getting called
     char *error_string = m_handle.error_string;
     m_handle.error_string = NULL;
     d3plot_close(&m_handle);
 
-    throw Exception(String(error_string));
+    throw Exception(Exception::ErrorString(error_string));
   }
 }
 
 D3plot::~D3plot() noexcept { d3plot_close(&m_handle); }
 
 Array<d3_word> D3plot::read_node_ids() {
   size_t num_ids;
   d3_word *ids = d3plot_read_node_ids(&m_handle, &num_ids);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3_word>(ids, num_ids);
 }
 
 Array<d3_word> D3plot::read_solid_element_ids() {
   size_t num_ids;
   d3_word *ids = d3plot_read_solid_element_ids(&m_handle, &num_ids);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3_word>(ids, num_ids);
 }
 
 Array<d3_word> D3plot::read_beam_element_ids() {
   size_t num_ids;
   d3_word *ids = d3plot_read_beam_element_ids(&m_handle, &num_ids);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3_word>(ids, num_ids);
 }
 
 Array<d3_word> D3plot::read_shell_element_ids() {
   size_t num_ids;
   d3_word *ids = d3plot_read_shell_element_ids(&m_handle, &num_ids);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3_word>(ids, num_ids);
 }
 
 Array<d3_word> D3plot::read_thick_shell_element_ids() {
   size_t num_ids;
   d3_word *ids = d3plot_read_thick_shell_element_ids(&m_handle, &num_ids);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3_word>(ids, num_ids);
 }
 
 Array<d3_word> D3plot::read_all_element_ids() {
   size_t num_ids;
   d3_word *ids = d3plot_read_all_element_ids(&m_handle, &num_ids);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3_word>(ids, num_ids);
 }
 
 Array<d3_word> D3plot::read_part_ids() {
   size_t num_ids;
   d3_word *ids = d3plot_read_part_ids(&m_handle, &num_ids);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3_word>(ids, num_ids);
 }
 
 std::vector<SizedString> D3plot::read_part_titles() {
   size_t num_parts;
   char **part_titles = d3plot_read_part_titles(&m_handle, &num_parts);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   std::vector<SizedString> vec;
   vec.reserve(num_parts);
   for (size_t i = 0; i < num_parts; i++) {
     // Trim part titles
     size_t j = 0;
@@ -148,326 +148,326 @@
 }
 
 Array<dVec3> D3plot::read_node_coordinates(size_t state) {
   size_t num_nodes;
   dVec3 *nodes = reinterpret_cast<dVec3 *>(
       d3plot_read_node_coordinates(&m_handle, state, &num_nodes));
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<dVec3>(nodes, num_nodes);
 }
 
 std::vector<Array<dVec3>> D3plot::read_all_node_coordinates() {
   size_t num_nodes, num_time_steps;
   dVec3 *nodes = reinterpret_cast<dVec3 *>(
       d3plot_read_all_node_coordinates(&m_handle, &num_nodes, &num_time_steps));
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   std::vector<Array<dVec3>> time_steps(num_time_steps);
   for (size_t t = 0; t < num_time_steps; t++) {
     time_steps[t] = Array<dVec3>(&nodes[t * num_nodes], num_nodes, t == 0);
   }
   return time_steps;
 }
 
 Array<dVec3> D3plot::read_node_velocity(size_t state) {
   size_t num_nodes;
   dVec3 *nodes = reinterpret_cast<dVec3 *>(
       d3plot_read_node_velocity(&m_handle, state, &num_nodes));
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<dVec3>(nodes, num_nodes);
 }
 
 std::vector<Array<dVec3>> D3plot::read_all_node_velocity() {
   size_t num_nodes, num_time_steps;
   dVec3 *nodes = reinterpret_cast<dVec3 *>(
       d3plot_read_all_node_velocity(&m_handle, &num_nodes, &num_time_steps));
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   std::vector<Array<dVec3>> time_steps(num_time_steps);
   for (size_t t = 0; t < num_time_steps; t++) {
     time_steps[t] = Array<dVec3>(&nodes[t * num_nodes], num_nodes, t == 0);
   }
   return time_steps;
 }
 
 Array<dVec3> D3plot::read_node_acceleration(size_t state) {
   size_t num_nodes;
   dVec3 *nodes = reinterpret_cast<dVec3 *>(
       d3plot_read_node_acceleration(&m_handle, state, &num_nodes));
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<dVec3>(nodes, num_nodes);
 }
 
 std::vector<Array<dVec3>> D3plot::read_all_node_acceleration() {
   size_t num_nodes, num_time_steps;
   dVec3 *nodes = reinterpret_cast<dVec3 *>(d3plot_read_all_node_acceleration(
       &m_handle, &num_nodes, &num_time_steps));
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   std::vector<Array<dVec3>> time_steps(num_time_steps);
   for (size_t t = 0; t < num_time_steps; t++) {
     time_steps[t] = Array<dVec3>(&nodes[t * num_nodes], num_nodes, t == 0);
   }
   return time_steps;
 }
 
 Array<fVec3> D3plot::read_node_coordinates_32(size_t state) {
   size_t num_nodes;
   fVec3 *nodes = reinterpret_cast<fVec3 *>(
       d3plot_read_node_coordinates_32(&m_handle, state, &num_nodes));
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<fVec3>(nodes, num_nodes);
 }
 
 std::vector<Array<fVec3>> D3plot::read_all_node_coordinates_32() {
   size_t num_nodes, num_time_steps;
   fVec3 *nodes = reinterpret_cast<fVec3 *>(d3plot_read_all_node_coordinates_32(
       &m_handle, &num_nodes, &num_time_steps));
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   std::vector<Array<fVec3>> time_steps(num_time_steps);
   for (size_t t = 0; t < num_time_steps; t++) {
     time_steps[t] = Array<fVec3>(&nodes[t * num_nodes], num_nodes, t == 0);
   }
   return time_steps;
 }
 
 Array<fVec3> D3plot::read_node_velocity_32(size_t state) {
   size_t num_nodes;
   fVec3 *nodes = reinterpret_cast<fVec3 *>(
       d3plot_read_node_velocity_32(&m_handle, state, &num_nodes));
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<fVec3>(nodes, num_nodes);
 }
 
 std::vector<Array<fVec3>> D3plot::read_all_node_velocity_32() {
   size_t num_nodes, num_time_steps;
   fVec3 *nodes = reinterpret_cast<fVec3 *>(
       d3plot_read_all_node_velocity_32(&m_handle, &num_nodes, &num_time_steps));
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   std::vector<Array<fVec3>> time_steps(num_time_steps);
   for (size_t t = 0; t < num_time_steps; t++) {
     time_steps[t] = Array<fVec3>(&nodes[t * num_nodes], num_nodes, t == 0);
   }
   return time_steps;
 }
 
 Array<fVec3> D3plot::read_node_acceleration_32(size_t state) {
   size_t num_nodes;
   fVec3 *nodes = reinterpret_cast<fVec3 *>(
       d3plot_read_node_acceleration_32(&m_handle, state, &num_nodes));
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<fVec3>(nodes, num_nodes);
 }
 
 std::vector<Array<fVec3>> D3plot::read_all_node_acceleration_32() {
   size_t num_nodes, num_time_steps;
   fVec3 *nodes = reinterpret_cast<fVec3 *>(d3plot_read_all_node_acceleration_32(
       &m_handle, &num_nodes, &num_time_steps));
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   std::vector<Array<fVec3>> time_steps(num_time_steps);
   for (size_t t = 0; t < num_time_steps; t++) {
     time_steps[t] = Array<fVec3>(&nodes[t * num_nodes], num_nodes, t == 0);
   }
   return time_steps;
 }
 
 double D3plot::read_time(size_t state) {
   double time{d3plot_read_time(&m_handle, state)};
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
   return time;
 }
 
 Array<double> D3plot::read_all_time() {
   size_t num_states;
   double *times = d3plot_read_all_time(&m_handle, &num_states);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
   return Array<double>(times, num_states);
 }
 
 float D3plot::read_time_32(size_t state) {
   float time{d3plot_read_time_32(&m_handle, state)};
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
   return time;
 }
 
 Array<float> D3plot::read_all_time_32() {
   size_t num_states;
   float *times = d3plot_read_all_time_32(&m_handle, &num_states);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
   return Array<float>(times, num_states);
 }
 
 Array<d3plot_solid> D3plot::read_solids_state(size_t state) {
   size_t num_elements;
   d3plot_solid *elements =
       d3plot_read_solids_state(&m_handle, state, &num_elements);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3plot_solid>(elements, num_elements);
 }
 
 D3plotThickShellsState D3plot::read_thick_shells_state(size_t state) {
   size_t num_elements;
   size_t num_history_variables;
   d3plot_thick_shell *elements = d3plot_read_thick_shells_state(
       &m_handle, state, &num_elements, &num_history_variables);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return D3plotThickShellsState(elements, num_elements, num_history_variables);
 }
 
 Array<d3plot_beam> D3plot::read_beams_state(size_t state) {
   size_t num_elements;
   d3plot_beam *elements =
       d3plot_read_beams_state(&m_handle, state, &num_elements);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3plot_beam>(elements, num_elements);
 }
 
 D3plotShellsState D3plot::read_shells_state(size_t state) {
   size_t num_elements;
   size_t num_history_variables;
   d3plot_shell *elements = d3plot_read_shells_state(
       &m_handle, state, &num_elements, &num_history_variables);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return D3plotShellsState(elements, num_elements, num_history_variables);
 }
 
 Array<d3plot_solid_con> D3plot::read_solid_elements() {
   size_t num_elements;
   d3plot_solid_con *elements =
       d3plot_read_solid_elements(&m_handle, &num_elements);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3plot_solid_con>(elements, num_elements);
 }
 
 Array<d3plot_thick_shell_con> D3plot::read_thick_shell_elements() {
   size_t num_elements;
   d3plot_thick_shell_con *elements =
       d3plot_read_thick_shell_elements(&m_handle, &num_elements);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3plot_thick_shell_con>(elements, num_elements);
 }
 
 Array<d3plot_beam_con> D3plot::read_beam_elements() {
   size_t num_elements;
   d3plot_beam_con *elements =
       d3plot_read_beam_elements(&m_handle, &num_elements);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3plot_beam_con>(elements, num_elements);
 }
 
 Array<d3plot_shell_con> D3plot::read_shell_elements() {
   size_t num_elements;
   d3plot_shell_con *elements =
       d3plot_read_shell_elements(&m_handle, &num_elements);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   return Array<d3plot_shell_con>(elements, num_elements);
 }
 
 SizedString D3plot::read_title() {
   char *title = d3plot_read_title(&m_handle);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
 
   // Trim whitespace
   size_t j = 0;
   while (title[j] != ' ') {
     j++;
   }
 
   return SizedString(title, j);
 }
 
 std::chrono::system_clock::time_point D3plot::read_run_time() {
   const time_t run_time = d3plot_read_epoch_run_time(&m_handle);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
   return std::chrono::system_clock::time_point{std::chrono::seconds{run_time}};
 }
 
 D3plotPart D3plot::read_part(size_t part_index) {
   d3plot_part part = d3plot_read_part(&m_handle, part_index);
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
   return D3plotPart(part);
 }
 
 D3plotPart D3plot::read_part_by_id(size_t part_id,
                                    const Array<d3_word> &part_ids) {
   d3plot_part part = d3plot_read_part_by_id(&m_handle, part_id, part_ids.data(),
                                             part_ids.size());
   if (m_handle.error_string) {
-    throw Exception(String(m_handle.error_string, false));
+    throw Exception(Exception::ErrorString(m_handle.error_string, false));
   }
   return D3plotPart(part);
 }
 
 } // namespace dro
 
 std::ostream &operator<<(std::ostream &stream, const d3plot_tensor &t) {
@@ -488,15 +488,14 @@
   return stream << "Stress: " << s.stress
                 << "; Effective Plastic Strain: " << s.effective_plastic_strain;
 }
 
 std::ostream &operator<<(std::ostream &stream, const d3plot_solid &s) {
   return stream << "Stress: " << s.stress
                 << "; Effective Plastic Strain: " << s.effective_plastic_strain
-                << "; Extra1: " << s.extra1 << "; Extra2: " << s.extra2
                 << "; Strain: " << s.strain;
 }
 
 std::ostream &operator<<(std::ostream &stream, const d3plot_thick_shell &ts) {
   return stream << "Mid: " << ts.mid << "; Inner: " << ts.inner
                 << "; Outer: " << ts.outer
                 << "; Inner Strain: " << ts.inner_strain
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/cpp/d3plot.hpp` & `dynareadout-23.7/lib/dynareadout/src/cpp/d3plot.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,35 @@
 namespace dro {
 
 // This holds all data needed to read d3plot files
 class D3plot {
 public:
   class Exception : public std::exception {
   public:
-    Exception(String error_str) noexcept;
+#ifdef _WIN32
+    // On windows python scripts crash when deallocated the memory of a thrown
+    // exception
+    class ErrorString : public std::string {
+    public:
+      ErrorString(char *str, bool delete_data = true) noexcept
+          : std::string(str) {
+        if (delete_data)
+          free(str);
+      }
+    };
+#else
+    using ErrorString = String;
+#endif
+
+    Exception(ErrorString error_str) noexcept;
 
     const char *what() const noexcept override;
 
   private:
-    const String m_error_str;
+    const ErrorString m_error_str;
   };
 
   static size_t index_for_id(const Array<d3_word> &ids, d3_word id);
 
   // Open a d3plot file family by giving the root file name
   // Example: d3plot of d3plot01, d3plot02, d3plot03, etc.
   D3plot(const std::filesystem::path &root_file_name);
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_part.cpp` & `dynareadout-23.7/lib/dynareadout/src/cpp/d3plot_part.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -111,15 +111,16 @@
       thick_shell_ids ? thick_shell_ids->data() : NULL,
       thick_shell_ids ? thick_shell_ids->size() : 0,
       thick_shell_cons ? thick_shell_cons->data() : NULL,
       beam_cons ? beam_cons->data() : NULL,
       shell_cons ? shell_cons->data() : NULL,
       thick_shell_cons ? thick_shell_cons->data() : NULL);
   if (plot_file.get_handle().error_string) {
-    throw D3plot::Exception(String(plot_file.get_handle().error_string, false));
+    throw D3plot::Exception(D3plot::Exception::ErrorString(
+        plot_file.get_handle().error_string, false));
   }
 
   return Array<d3_word>(part_node_ids, num_part_node_ids);
 }
 
 Array<d3_word> D3plotPart::get_node_indices(
     D3plot &plot_file, const Array<d3_word> *solid_ids,
@@ -138,15 +139,16 @@
       thick_shell_ids ? thick_shell_ids->data() : NULL,
       thick_shell_ids ? thick_shell_ids->size() : 0,
       thick_shell_cons ? thick_shell_cons->data() : NULL,
       beam_cons ? beam_cons->data() : NULL,
       shell_cons ? shell_cons->data() : NULL,
       thick_shell_cons ? thick_shell_cons->data() : NULL);
   if (plot_file.get_handle().error_string) {
-    throw D3plot::Exception(String(plot_file.get_handle().error_string, false));
+    throw D3plot::Exception(D3plot::Exception::ErrorString(
+        plot_file.get_handle().error_string, false));
   }
 
   return Array<d3_word>(part_node_indices, num_part_node_indices);
 }
 
 size_t D3plotPart::get_num_nodes(
     D3plot &plot_file, const Array<d3_word> *solid_ids,
@@ -164,15 +166,16 @@
       thick_shell_ids ? thick_shell_ids->data() : NULL,
       thick_shell_ids ? thick_shell_ids->size() : 0,
       thick_shell_cons ? thick_shell_cons->data() : NULL,
       beam_cons ? beam_cons->data() : NULL,
       shell_cons ? shell_cons->data() : NULL,
       thick_shell_cons ? thick_shell_cons->data() : NULL);
   if (plot_file.get_handle().error_string) {
-    throw D3plot::Exception(String(plot_file.get_handle().error_string, false));
+    throw D3plot::Exception(D3plot::Exception::ErrorString(
+        plot_file.get_handle().error_string, false));
   }
 
   return num_nodes;
 }
 
 size_t D3plotPart::get_num_elements() const {
   return d3plot_part_get_num_elements(&m_part);
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_part.hpp` & `dynareadout-23.7/lib/dynareadout/src/cpp/d3plot_part.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_state.cpp` & `dynareadout-23.7/lib/dynareadout/src/cpp/d3plot_state.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_state.hpp` & `dynareadout-23.7/lib/dynareadout/src/cpp/d3plot_state.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -38,16 +38,21 @@
   D3plotShellsState(D3plotShellsState &&rhs) noexcept;
   ~D3plotShellsState() noexcept override;
 
   inline size_t get_num_history_variables() const noexcept {
     return m_num_history_variables;
   }
 
+  // Returns the history variables for the mid surface of the shell under index
   const Array<double> get_mid_history_variables(size_t index) const;
+  // Returns the history variables for the inner surface of the shell under
+  // index
   const Array<double> get_inner_history_variables(size_t index) const;
+  // Returns the history variables for the outer surface of the shell under
+  // index
   const Array<double> get_outer_history_variables(size_t index) const;
 
 private:
   size_t m_num_history_variables;
 };
 
 class D3plotThickShellsState : public Array<d3plot_thick_shell> {
@@ -58,16 +63,22 @@
   D3plotThickShellsState(D3plotThickShellsState &&rhs) noexcept;
   ~D3plotThickShellsState() noexcept override;
 
   inline size_t get_num_history_variables() const noexcept {
     return m_num_history_variables;
   }
 
+  // Returns the history variables of the mid surface of the thick shell under
+  // index
   const Array<double> get_mid_history_variables(size_t index) const;
+  // Returns the history variables of the inner surface of the thick shell under
+  // index
   const Array<double> get_inner_history_variables(size_t index) const;
+  // Returns the history variables of the outer surface of the thick shell under
+  // index
   const Array<double> get_outer_history_variables(size_t index) const;
 
 private:
   size_t m_num_history_variables;
 };
 
 } // namespace dro
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/cpp/key.cpp` & `dynareadout-23.7/lib/dynareadout/src/cpp/key.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,16 @@
     THROW_KEY_FILE_EXCEPTION("The keyword \"%s\" could not be found",
                              name.c_str());
   }
 
   return KeywordSlice(slice, slice_size);
 }
 
-KeyFile::Exception::Exception(String error_str) noexcept
+KeyFile::Exception::Exception(
+    KeyFile::Exception::ErrorString error_str) noexcept
     : m_error_str(std::move(error_str)) {}
 
 const char *KeyFile::Exception::what() const noexcept {
   return m_error_str.data();
 }
 
 Keywords KeyFile::parse(const std::filesystem::path &file_name,
@@ -178,15 +179,15 @@
   size_t num_keywords;
   char *error_string;
 
   keyword_t *keywords =
       key_file_parse(file_name.string().c_str(), &num_keywords,
                      static_cast<int>(parse_includes), &error_string);
   if (error_string) {
-    throw Exception(String(error_string));
+    throw Exception(Exception::ErrorString(error_string));
   }
 
   return Keywords(keywords, num_keywords);
 }
 
 void KeyFile::parse_with_callback(const std::filesystem::path &file_name,
                                   KeyFile::Callback callback,
@@ -206,12 +207,12 @@
                     String(const_cast<char *>(keyword_name), false),
                     std::move(card_opt), card_index);
       },
       static_cast<int>(parse_includes), &error_string, &callback, NULL, NULL,
       NULL);
 
   if (error_string) {
-    throw Exception(String(error_string));
+    throw Exception(Exception::ErrorString(error_string));
   }
 }
 
 } // namespace dro
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/cpp/key.hpp` & `dynareadout-23.7/lib/dynareadout/src/cpp/key.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -40,27 +40,28 @@
 #include <type_traits>
 #include <typeinfo>
 
 #define THROW_KEY_FILE_EXCEPTION(msg, ...)                                     \
   const int error_buffer_size = snprintf(NULL, 0, msg, __VA_ARGS__);           \
   char *error_buffer = reinterpret_cast<char *>(malloc(error_buffer_size));    \
   sprintf(error_buffer, msg, __VA_ARGS__);                                     \
-  throw dro::KeyFile::Exception(dro::String(error_buffer))
+  throw dro::KeyFile::Exception(                                               \
+      dro::KeyFile::Exception::ErrorString(error_buffer))
 
 namespace dro {
 // A Card inside of a LS Dyna key file (input deck)
 class Card {
 public:
   Card(card_t *handle) noexcept;
 
   // Initialises the parsing of the card
   void begin(uint8_t value_width = DEFAULT_VALUE_WIDTH) noexcept;
-  // Advance to the next value. Uses the value width from begin.
+  // Advance to the next value. Uses the value width from begin
   void next() noexcept;
-  // Advance to the next value. Uses the value width provided here.
+  // Advance to the next value. Uses the value width provided here
   void next(uint8_t value_width) noexcept;
   // Returns wether the card has been completely parsed. Breaks if incorrect
   // value widths have been supplied
   bool done() const noexcept;
   // Returns the type of the current value. Uses the value width from
   // begin. If CARD_PARSE_INT is returned the value can be parsed with an
   // integer type. If CARD_PARSE_FLOAT is returned the value can be parsed with
@@ -250,28 +251,43 @@
 };
 
 // This static class holds the functions for parsing LS Dyna key files
 class KeyFile {
 public:
   class Exception : public std::exception {
   public:
-    Exception(String error_str) noexcept;
+#ifdef _WIN32
+    // On windows python scripts crash when deallocated the memory of a thrown
+    // exception
+    class ErrorString : public std::string {
+    public:
+      ErrorString(char *str, bool delete_data = true) noexcept
+          : std::string(str) {
+        if (delete_data)
+          free(str);
+      }
+    };
+#else
+    using ErrorString = String;
+#endif
+
+    Exception(ErrorString error_str) noexcept;
 
     const char *what() const noexcept override;
 
   private:
-    const String m_error_str;
+    const ErrorString m_error_str;
   };
 
   using Callback = std::function<void(
       String file_name, size_t line_number, String keyword_name,
       std::optional<Card> card, size_t card_index)>;
 
-  // Parses a LS Dyna key file for keywords and their respective cards. Returns
-  // an array keywords
+  // Parses an LS Dyna key file for keywords and their respective cards. Returns
+  // an array of keywords
   // parse_includes: tells the function wether to parse include files via the
   // *INCLUDE and similar keywords or if they should be added as regular
   // keywords to the array.
   // Throws a dro::KeyFile::Exception if an error occurs.
   static Keywords parse(const std::filesystem::path &file_name,
                         bool parse_includes = true);
   // Same as parse, but instead of returning an array it calls a callback every
@@ -354,34 +370,14 @@
   }
 }
 
 template <typename T> T Card::parse_string_no_trim() const noexcept {
   return parse_string_no_trim<T>(m_handle->value_width);
 }
 
-#ifdef __GNUC__
-// clang-format off
-template <typename T>
-T Card::parse_string_no_trim(uint8_t value_width) const noexcept {
-  static_assert(is_string_v<T> && "Can parse the whole card only as string (char*, dro::String, dro::SizedString, std::string)");
-  return T{0};
-}
-
-template <typename T> T Card::parse_string_whole() const noexcept {
-  static_assert(is_string_v<T> && "Can parse the whole card only as string (char*, dro::String, dro::SizedString, std::string)");
-  return T{0};
-}
-
-template <typename T> T Card::parse_string_whole_no_trim() const noexcept {
-  static_assert(is_string_v<T> && "Can parse the whole card only as string (char*, dro::String, dro::SizedString, std::string)");
-  return T{0};
-}
-// clang-format on
-#endif
-
 template <typename... T> void Card::parse_whole(T &...rv) {
 
   int i = 0;
 
   begin();
 
   (
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/cpp/vec.hpp` & `dynareadout-23.7/lib/dynareadout/src/cpp/vec.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/d3_buffer.c` & `dynareadout-23.7/lib/dynareadout/src/d3_buffer.c`

 * *Files 1% similar despite different names*

```diff
@@ -241,31 +241,32 @@
         /* We can read all of the rest of the words from the current file*/
         if (multi_file_read(file, &ptr->multi_file_index,
                             &words_ptr[bytes_read], 1,
                             bytes_left) != bytes_left) {
           ERROR_AND_RETURN_BUFFER_PTR("Read Error");
         }
 
-        /* TODO: If bytes_left is not divisible by word size this adds an
-         * invalid value, but this doesn't really matter*/
+        /* Note: If bytes_left is not divisible by word size this adds an
+         * invalid value, but d3plot files are alway word size aligned.*/
         ptr->cur_word += bytes_left / buffer->word_size;
         bytes_read = num_bytes;
         break;
       } else {
 
         if (bytes_from_cur_file != 0) {
           /* Read the rest of the current file*/
           if (multi_file_read(file, &ptr->multi_file_index,
                               &words_ptr[bytes_read], 1,
                               bytes_from_cur_file) != bytes_from_cur_file) {
             ERROR_AND_RETURN_BUFFER_PTR("Read Error");
           }
 
-          /* TODO: If bytes_left is not divisible by word size this adds an
-           * invalid value, but this doesn't really matter*/
+          /* Note: If bytes_from_cur_file is not divisible by word size this
+           * adds an invalid value, but d3plot files are always word size
+           * aligned.*/
           ptr->cur_word += bytes_from_cur_file / buffer->word_size;
           bytes_read += bytes_from_cur_file;
         }
 
         if (!d3_buffer_next_file(buffer, ptr)) {
           if (buffer->error_string) {
             ERROR_AND_RETURN_BUFFER_F_PTR(
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/d3_buffer.h` & `dynareadout-23.7/lib/dynareadout/src/d3_buffer.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/d3_defines.h` & `dynareadout-23.7/lib/dynareadout/src/d3_defines.h`

 * *Files 6% similar despite different names*

```diff
@@ -21,52 +21,59 @@
  * misrepresented as being the original software.
  *
  * 3. This notice may not be removed or altered from any source distribution.
  ************************************************************************************/
 
 #ifndef D3_DEFINES_H
 #define D3_DEFINES_H
+#include <stddef.h>
 #include <stdint.h>
 #ifdef __cplusplus
 #include <array>
 #endif
 
 typedef uint64_t d3_word;
 
 typedef struct {
   /* Stores indices into the node_ids, node_coords, etc. arrays*/
 #ifdef __cplusplus
   std::array<d3_word, 8> node_indices;
 #else
   d3_word node_indices[8];
 #endif
+  /* Index into the parts (this those indeed refer to parts even though the
+   * documentation does not say so)*/
   d3_word material_index;
 } d3plot_solid_con;
 
 typedef d3plot_solid_con d3plot_thick_shell_con;
 
 typedef struct {
   /* Stores indices into the node_ids, node_coords, etc. arrays*/
 #ifdef __cplusplus
   std::array<d3_word, 2> node_indices;
 #else
   d3_word node_indices[2];
 #endif
   d3_word orientation_node_index;
   d3_word _null[2];
+  /* Index into the parts (this those indeed refer to parts even though the
+   * documentation does not say so)*/
   d3_word material_index;
 } d3plot_beam_con;
 
 typedef struct {
   /* Stores indices into the node_ids, node_coords, etc. arrays*/
 #ifdef __cplusplus
   std::array<d3_word, 4> node_indices;
 #else
   d3_word node_indices[4];
 #endif
+  /* Index into the parts (this those indeed refer to parts even though the
+   * documentation does not say so)*/
   d3_word material_index;
 } d3plot_shell_con;
 
 typedef struct {
   d3_word *solid_ids;
   d3_word *thick_shell_ids;
   d3_word *beam_ids;
@@ -117,16 +124,14 @@
     d3plot_tensor sigma;
     d3plot_tensor stress;
   };
   union {
     double effective_plastic_strain;
     double material_dependent_value;
   };
-  double extra1;
-  double extra2;
   union {
     d3plot_tensor epsilon;
     d3plot_tensor strain;
   };
 } d3plot_solid;
 
 /* Only used for d3plot_thick_shell and d3plot_shell*/
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/d3plot.c` & `dynareadout-23.7/lib/dynareadout/src/d3plot.c`

 * *Files 3% similar despite different names*

```diff
@@ -228,18 +228,14 @@
              values) and after the plastic
              strain tensor if output.*/
     CDA.thermal_strain_tensor_written = 1;
   } else {
     CDA.thermal_strain_tensor_written = 0;
   }
 
-  if (CDA.plastic_strain_tensor_written || CDA.thermal_strain_tensor_written) {
-    CDA.istrn = _get_nth_digit(idtdt, 4);
-  }
-
   /* Compute MDLOPT*/
   if (CDA.maxint >= 0) {
     CDA.mdlopt = 0;
   } else if (CDA.maxint < -10000) {
     CDA.mdlopt = 2;
     CDA.maxint = CDA.maxint * -1 - 10000;
   } else if (CDA.maxint < 0) {
@@ -257,35 +253,38 @@
 
       If ISTRN=1, and NEIPH>=6, last the 6 additional values are the six strain
       components.
 
       Or NELT > 0
       If NV3DT-MAXINT*(6*IOSHL(1)+IOSHL(2)+NEIPS) > 1
       Then ISTRN = 1, else ISTRN = 0*/
-    const d3_word rhs =
-        CDA.maxint * (6 * CDA.ioshl[0] + CDA.ioshl[1] + CDA.neips) +
-        8 * CDA.ioshl[2] + 4 * CDA.ioshl[3];
-    if (CDA.nv2d > rhs + 1) {
-      CDA.istrn = 1;
-    } else {
-      CDA.istrn = 0;
-    }
-
-    if (CDA.istrn == 1 && CDA.neiph >= 6) {
-      /* TODO: last the 6 additional values are the six strain*/
-    }
-
-    if (CDA.nelt > 0) {
+    if (CDA.nv2d > 0) {
+      const d3_word rhs =
+          CDA.maxint * (6 * CDA.ioshl[0] + CDA.ioshl[1] + CDA.neips) +
+          8 * CDA.ioshl[2] + 4 * CDA.ioshl[3];
+      if (CDA.nv2d > rhs + 1) {
+        CDA.istrn = 1;
+      } else {
+        CDA.istrn = 0;
+      }
+    } else if (CDA.nelt > 0) {
       if ((CDA.nv3dt -
            CDA.maxint * (6 * CDA.ioshl[0] + CDA.ioshl[1] + CDA.neips)) > 1) {
         CDA.istrn = 1;
       } else {
         CDA.istrn = 0;
       }
     }
+
+    if (CDA.istrn == 1 && CDA.neiph >= 6) {
+      /* TODO: last the 6 additional values are the six strain*/
+    }
+
+  } else {
+    CDA.istrn = _get_nth_digit(idtdt, 4);
   }
 
   if (icode != D3_CODE_OLD_DYNA3D &&
       icode != D3_CODE_NIKE3D_LS_DYNA3D_LS_NIKE3D) {
     ERROR_AND_RETURN("The given order of the elements is not supported");
   }
 
@@ -1273,52 +1272,49 @@
       return NULL;
     }
 
     size_t i = 0;
     size_t o = 0;
     while (i < *num_solids) {
       /* Docs: page 33*/
-      const size_t start = o;
+      /* 1. Sigma-x (true stress in the global system)*/
       solids[i].sigma.x = data[o++];
+      /* 2. Sigma-y*/
       solids[i].sigma.y = data[o++];
+      /* 3. Sigma-z*/
       solids[i].sigma.z = data[o++];
+      /* 4. Sigma-xy*/
       solids[i].sigma.xy = data[o++];
+      /* 5. Sigma-yz*/
       solids[i].sigma.yz = data[o++];
+      /* 6. Sigma-zx*/
       solids[i].sigma.zx = data[o++];
+      /* 7. Effective plastic strain or material dependent variable*/
       solids[i].effective_plastic_strain = data[o++];
-      if (plot_file->control_data.neiph > 0) {
-        solids[i].extra1 = data[o++];
-        if (plot_file->control_data.neiph > 1) {
-          solids[i].extra2 = data[o++];
-          if (plot_file->control_data.neiph >= 6) {
-            /* We need -1 since we start by 0 and in the docs they start with
-             * 1*/
-            solids[i].epsilon.x =
-                data[start + 7 + plot_file->control_data.neiph - 5 - 1];
-            solids[i].epsilon.y =
-                data[start + 7 + plot_file->control_data.neiph - 4 - 1];
-            solids[i].epsilon.z =
-                data[start + 7 + plot_file->control_data.neiph - 3 - 1];
-            solids[i].epsilon.xy =
-                data[start + 7 + plot_file->control_data.neiph - 2 - 1];
-            solids[i].epsilon.yz =
-                data[start + 7 + plot_file->control_data.neiph - 1 - 1];
-            solids[i].epsilon.zx =
-                data[start + 7 + plot_file->control_data.neiph - 0 - 1];
-            o = start + 7 + plot_file->control_data.neiph;
-          } else {
-            memset(&solids[i].epsilon, 0, 6 * sizeof(double));
-          }
-        } else {
-          memset(&solids[i].extra2, 0, 7 * sizeof(double));
-        }
+      if (plot_file->control_data.neiph >= 6) {
+        /* We need -1 since we start by 0 and in the docs they start with
+         * 1*/
+        /* 7+NEIPH-5. Epsilon-x*/
+        solids[i].epsilon.x = data[o + plot_file->control_data.neiph - 5 - 1];
+        /* 7+NEIPH-4. Epsilon-y*/
+        solids[i].epsilon.y = data[o + plot_file->control_data.neiph - 4 - 1];
+        /* 7+NEIPH-3. Epsilon-z*/
+        solids[i].epsilon.z = data[o + plot_file->control_data.neiph - 3 - 1];
+        /* 7+NEIPH-2. Epsilon-xy*/
+        solids[i].epsilon.xy = data[o + plot_file->control_data.neiph - 2 - 1];
+        /* 7+NEIPH-1. Epsilon-yz*/
+        solids[i].epsilon.yz = data[o + plot_file->control_data.neiph - 1 - 1];
+        /* 7+NEIPH. Epsilon-zx*/
+        solids[i].epsilon.zx = data[o + plot_file->control_data.neiph - 0 - 1];
       } else {
-        memset(&solids[i].extra1, 0, 8 * sizeof(double));
+        memset(&solids[i].epsilon, 0, 6 * sizeof(double));
       }
 
+      o += plot_file->control_data.neiph;
+
       i++;
     }
 
     free(data);
   } else {
     double *data =
         malloc((plot_file->control_data.nel8 * plot_file->control_data.nv3d) *
@@ -1341,39 +1337,29 @@
       return NULL;
     }
 
     size_t i = 0;
     size_t o = 0;
     while (i < *num_solids) {
       /* Docs: page 33*/
-      const size_t start = o;
       /* We can just copy the first 7 values*/
       memcpy(&solids[i], &data[o], 7 * sizeof(double));
       o += 7;
-      if (plot_file->control_data.neiph > 0) {
-        solids[i].extra1 = data[o++];
-        if (plot_file->control_data.neiph > 1) {
-          solids[i].extra2 = data[o++];
-          if (plot_file->control_data.neiph >= 6) {
-            /* We need -1 since we start by 0 and in the docs they start with
-             * 1*/
-            memcpy(&solids[i].epsilon,
-                   &data[start + 7 + plot_file->control_data.neiph - 5 - 1],
-                   6 * sizeof(double));
-            o = start + 7 + plot_file->control_data.neiph;
-          } else {
-            memset(&solids[i].epsilon, 0, 6 * sizeof(double));
-          }
-        } else {
-          memset(&solids[i].extra2, 0, 7 * sizeof(double));
-        }
+      if (plot_file->control_data.neiph >= 6) {
+        /* We need -1 since we start by 0 and in the docs they start with
+         * 1*/
+        memcpy(&solids[i].epsilon,
+               &data[o + plot_file->control_data.neiph - 5 - 1],
+               6 * sizeof(double));
       } else {
-        memset(&solids[i].extra1, 0, 8 * sizeof(double));
+        memset(&solids[i].epsilon, 0, 6 * sizeof(double));
       }
 
+      o += plot_file->control_data.neiph;
+
       i++;
     }
 
     free(data);
   }
 
   END_PROFILE_FUNC();
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/d3plot.h` & `dynareadout-23.7/lib/dynareadout/src/d3plot.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/d3plot_data.c` & `dynareadout-23.7/lib/dynareadout/src/d3plot_data.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/d3plot_error_macros.h` & `dynareadout-23.7/lib/dynareadout/src/d3plot_error_macros.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/d3plot_part_nodes.c` & `dynareadout-23.7/lib/dynareadout/src/d3plot_part_nodes.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/d3plot_part_nodes.h` & `dynareadout-23.7/lib/dynareadout/src/d3plot_part_nodes.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/d3plot_state.c` & `dynareadout-23.7/lib/dynareadout/src/d3plot_state.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/extra_string.c` & `dynareadout-23.7/lib/dynareadout/src/extra_string.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/extra_string.h` & `dynareadout-23.7/lib/dynareadout/src/extra_string.h`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 /* A string which allocates a part on the stack and allocates more on the heap
  * if it needs "extra" memory*/
-#define EXTRA_STRING_BUFFER_SIZE (80 + 1)
+#define EXTRA_STRING_BUFFER_SIZE                                               \
+  (80 + 2) /* LENGTH_OF_DYNA_LINE + carriage return (\r) and newline (\n)*/
 typedef struct {
   char buffer[EXTRA_STRING_BUFFER_SIZE];
   char *extra;
 } extra_string;
 
 char extra_string_get(const extra_string *str, size_t index);
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/key.c` & `dynareadout-23.7/lib/dynareadout/src/key.c`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,22 @@
  * misrepresented as being the original software.
  *
  * 3. This notice may not be removed or altered from any source distribution.
  ************************************************************************************/
 
 #include "key.h"
 #include "binary_search.h"
+#include "line.h"
 #include "profiling.h"
 #include <errno.h>
 #include <math.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 
-#define KEY_COMMENT '$'
-#define LINE_WIDTH 80
-
 #define ERROR_MSG(msg)                                                         \
   const size_t error_msg_len = strlen(msg);                                    \
   error_stack_size += error_msg_len + 1;                                       \
   error_stack = realloc(error_stack, error_stack_size);                        \
   memcpy(&error_stack[error_ptr], msg, error_msg_len);                         \
   error_ptr += error_msg_len;                                                  \
   error_stack[error_ptr] = '\n';                                               \
@@ -227,143 +225,50 @@
      * include paths*/
     (*num_include_paths_ptr)++;
     *include_paths_ptr =
         realloc(*include_paths_ptr, *num_include_paths_ptr * sizeof(char *));
     (*include_paths_ptr)[*num_include_paths_ptr - 1] = path_working_directory();
   }
 
-  extra_string line;
+  line_reader_t line_reader = new_line_reader(file);
   extra_string current_keyword_name;
   current_keyword_name.buffer[0] = '\0';
   current_keyword_name.extra = NULL;
-  line.extra = NULL;
 
   size_t current_keyword_length = 0;
   size_t current_keyword_line = (size_t)~0;
   size_t card_index = 0;
   size_t line_count = 0;
 
   char *current_multi_line_string = NULL;
   size_t current_multi_line_index = 0;
 
   /* Loop until all lines have been read or an error occurred*/
-  while (1) {
-    /* Clear extra without freeing the memory*/
-    if (line.extra) {
-      line.extra[0] = '\0';
-    }
-
-    size_t line_length = 0;
-
-    /* Find the new line*/
-    /* Read more data from the file until a new line has been found*/
-    size_t i = 0;
-    size_t comment_index = (size_t)~0;
-    /* Read the file in LINE_WIDTH sized chunks, but read LINE_WIDTH + 1
-     * characters for the first read, because a lot of lines will be exactly
-     * LINE_WIDTH characters long, therefore we read the new line directly in
-     * the first read chunk*/
-    int n = fread(line.buffer, 1, EXTRA_STRING_BUFFER_SIZE, file);
-    if ((n == 0 && feof(file)) || ferror(file)) {
-      break;
-    } else if (n < EXTRA_STRING_BUFFER_SIZE) {
-      line.buffer[n] = '\0';
-    }
-
-    /* ------------ LINE READING ------------*/
-    /* Loop until the next line has been read. After this loop the file is
-     * either at the beginning of the line after the
-     * next one, at EOF or has an error.*/
-    while (1) {
-      /* Look for the new line character and also look for the comment
-       * character*/
-      size_t j = 0;
-      while (j < (size_t)n) {
-        const char c = extra_string_get(&line, i);
-        if (c == '\n') {
-          break;
-        }
-        if (c == KEY_COMMENT && comment_index == (size_t)~0) {
-          comment_index = i;
-        }
-
-        i++;
-        j++;
-      }
-
-      line_length = i;
-
-      if (j == (size_t)n) {
-        /* New line is exactly after the line (perfect!)*/
-        if ((i < EXTRA_STRING_BUFFER_SIZE || line.extra != NULL) &&
-            extra_string_get(&line, i) == '\n') {
-          extra_string_set(&line, i, '\0');
-          break;
-        }
-
-        /* We still need to read more to find the new line*/
-      } else if (j != 0) {
-        /* New line is somewhere within LINE_WIDTH (or EXTRA_STRING_BUFFER_SIZE)
-         * characters*/
-        /* Seek back to the beginning of the line that has been "accidentally"
-         * read*/
-        fseek(file, j - n + 1, SEEK_CUR);
-        extra_string_set(&line, i, '\0');
-        break;
-      } else {
-        /* The first character that we read is a new line. Most of the time this
-         * means that
-         * 1. The line is exactly EXTRA_STRING_BUFFER_SIZE characters long or
-         * 2. The line is empty*/
-        fseek(file, 1 - n, SEEK_CUR);
-        extra_string_set(&line, i, '\0');
-        break;
-      }
-
-      /* The file ends without a new line*/
-      if (n < EXTRA_STRING_BUFFER_SIZE) {
-        break;
-      }
-
-      /* Read the next chunk of the file*/
-      line.extra = realloc(line.extra, i * sizeof(char));
-      n = fread(&line.extra[i - EXTRA_STRING_BUFFER_SIZE], 1,
-                EXTRA_STRING_BUFFER_SIZE, file);
-      if ((n == 0 && feof(file)) || ferror(file)) {
-        line.extra[i - EXTRA_STRING_BUFFER_SIZE] = '\0';
-        break;
-      }
-    }
-    /* -------------------------------------------- */
-
-    if ((line_length == 0 && n == 0 && feof(file)) || ferror(file)) {
-      break;
-    }
-
+  while (read_line(&line_reader)) {
     line_count++;
 
     /* Check if the line starts with a comment or contains a comment character*/
-    if (comment_index == 0) {
+    if (line_reader.comment_index == 0) {
       /* The entire line is a comment. Ignore it.*/
       continue;
-    } else if (comment_index != (size_t)~0) {
-      extra_string_set(&line, comment_index, '\0');
+    } else if (line_reader.comment_index != (size_t)~0) {
+      extra_string_set(&line_reader.line, line_reader.comment_index, '\0');
     }
 
     /* ------- 🐉 Here be parsings 🐉 --------- */
 
     /* Check if the line is a keyword (starts with '*')
      * Support lines being preceded by ' ' */
     int is_keyword = 0;
-    if (line_length != 0) {
-      i = 0;
-      while (extra_string_get(&line, i) == ' ') {
+    size_t i = 0;
+    if (line_reader.line_length != 0) {
+      while (extra_string_get(&line_reader.line, i) == ' ') {
         i++;
       }
-      is_keyword = extra_string_get(&line, i) == '*';
+      is_keyword = extra_string_get(&line_reader.line, i) == '*';
     }
 
     /* ------ 🔑 Keyword Parsing 🔑 --------- */
     if (is_keyword) {
       /* If we already read a keyword we need to call the callback if the
        * keyword had no cards*/
       if (current_keyword_length != 0 && card_index == 0) {
@@ -381,15 +286,16 @@
                  user_data);
 
         if (keyword_name != current_keyword_name.buffer) {
           free(keyword_name);
         }
       }
 
-      extra_string_copy(&current_keyword_name, &line, line_length, i + 1);
+      extra_string_copy(&current_keyword_name, &line_reader.line,
+                        line_reader.line_length, i + 1);
 
       /* Compute the length of the keyword*/
       current_keyword_length = 0;
       while (1) {
         const char c =
             extra_string_get(&current_keyword_name, current_keyword_length);
         if (c == ' ' || c == '\0') {
@@ -407,45 +313,46 @@
         break;
       }
 
       card_index = 0;
     } else {
       /* -------- 🃏 Card Parsing 🃏 ----------*/
       card_t card;
-      if (line_length < EXTRA_STRING_BUFFER_SIZE) {
-        card.string = line.buffer;
+      if (line_reader.line_length < EXTRA_STRING_BUFFER_SIZE) {
+        card.string = line_reader.line.buffer;
       } else {
-        card.string = malloc(line_length + 1);
-        extra_string_copy_to_string(card.string, &line, line_length);
-        card.string[line_length] = '\0';
+        card.string = malloc(line_reader.line_length + 1);
+        extra_string_copy_to_string(card.string, &line_reader.line,
+                                    line_reader.line_length);
+        card.string[line_reader.line_length] = '\0';
       }
 
       /* -------- ⛅ Include Parsing ⛅ -------*/
       if (extra_string_starts_with(&current_keyword_name, "INCLUDE")) {
         /* Also parse the INCLUDE keywords even when parse_includes is set to 0
          * to support multi line include file names*/
         if (parse_includes) {
           /* Parse all the different INCLUDE keywords*/
           if (extra_string_compare(&current_keyword_name, "INCLUDE") == 0) {
             _parse_include_file_name_card(
-                &card, &card_index, &line, line_length,
+                &card, &card_index, &line_reader.line, line_reader.line_length,
                 &current_multi_line_string, &current_multi_line_index,
                 num_include_paths_ptr, include_paths_ptr, callback, user_data,
                 &error_stack, &error_stack_size, &error_ptr, file_name,
                 line_count, root_folder_ptr);
             continue;
           } else if (extra_string_compare(&current_keyword_name,
                                           "INCLUDE_PATH") == 0) {
             /* Support multi line file names (LS Dyna Manual Volume I
              * *INCLUDE Remark 2, p. 2690)*/
             if (!_parse_multi_line_string(&current_multi_line_string,
                                           &current_multi_line_index, &card,
-                                          line_length)) {
+                                          line_reader.line_length)) {
               /* continue without calling the callback for the card*/
-              if (card.string != line.buffer) {
+              if (card.string != line_reader.line.buffer) {
                 free(card.string);
               }
               continue;
             }
 
             (*num_include_paths_ptr)++;
             *include_paths_ptr = realloc(
@@ -453,29 +360,29 @@
             (*include_paths_ptr)[*num_include_paths_ptr - 1] =
                 current_multi_line_string;
 
             current_multi_line_string = NULL;
             current_multi_line_index = 0;
 
             /* continue without calling the callback for the card*/
-            if (card.string != line.buffer) {
+            if (card.string != line_reader.line.buffer) {
               free(card.string);
             }
 
             card_index++;
             continue;
           } else if (extra_string_compare(&current_keyword_name,
                                           "INCLUDE_PATH_RELATIVE") == 0) {
             /* Support multi line file names (LS Dyna Manual Volume I
              * *INCLUDE Remark 2, p. 2690)*/
             if (!_parse_multi_line_string(&current_multi_line_string,
                                           &current_multi_line_index, &card,
-                                          line_length)) {
+                                          line_reader.line_length)) {
               /* continue without calling the callback for the card*/
-              if (card.string != line.buffer) {
+              if (card.string != line_reader.line.buffer) {
                 free(card.string);
               }
               continue;
             }
 
             char *full_include_path_name =
                 path_join(root_folder_ptr, current_multi_line_string);
@@ -486,65 +393,67 @@
             (*num_include_paths_ptr)++;
             *include_paths_ptr = realloc(
                 *include_paths_ptr, *num_include_paths_ptr * sizeof(char *));
             (*include_paths_ptr)[*num_include_paths_ptr - 1] =
                 full_include_path_name;
 
             /* continue without calling the callback for the card*/
-            if (card.string != line.buffer) {
+            if (card.string != line_reader.line.buffer) {
               free(card.string);
             }
 
             card_index++;
             continue;
           } else if (extra_string_compare(&current_keyword_name,
                                           "INCLUDE_BINARY") == 0) {
             /* Parse the first card like a normal INCLUDE*/
             if (card_index == 0) {
               _parse_include_file_name_card(
-                  &card, &card_index, &line, line_length,
-                  &current_multi_line_string, &current_multi_line_index,
-                  num_include_paths_ptr, include_paths_ptr, callback, user_data,
-                  &error_stack, &error_stack_size, &error_ptr, file_name,
-                  line_count, root_folder_ptr);
+                  &card, &card_index, &line_reader.line,
+                  line_reader.line_length, &current_multi_line_string,
+                  &current_multi_line_index, num_include_paths_ptr,
+                  include_paths_ptr, callback, user_data, &error_stack,
+                  &error_stack_size, &error_ptr, file_name, line_count,
+                  root_folder_ptr);
               continue;
             } else {
               ERROR_F(
                   "%s:%zu: Invalid number of cards for INCLUDE_BINARY keyword",
                   file_name, line_count);
             }
 
             /* continue without calling the callback for the card*/
-            if (card.string != line.buffer) {
+            if (card.string != line_reader.line.buffer) {
               free(card.string);
             }
 
             card_index++;
             continue;
           } else if (extra_string_compare(&current_keyword_name,
                                           "INCLUDE_NASTRAN") == 0) {
             /* Parse the first card like a normal INCLUDE*/
             if (card_index == 0) {
               _parse_include_file_name_card(
-                  &card, &card_index, &line, line_length,
-                  &current_multi_line_string, &current_multi_line_index,
-                  num_include_paths_ptr, include_paths_ptr, callback, user_data,
-                  &error_stack, &error_stack_size, &error_ptr, file_name,
-                  line_count, root_folder_ptr);
+                  &card, &card_index, &line_reader.line,
+                  line_reader.line_length, &current_multi_line_string,
+                  &current_multi_line_index, num_include_paths_ptr,
+                  include_paths_ptr, callback, user_data, &error_stack,
+                  &error_stack_size, &error_ptr, file_name, line_count,
+                  root_folder_ptr);
               continue;
             } else if (card_index == 1) {
               /* Ignore the card it is irrelevant for the parsing*/
             } else {
               ERROR_F(
                   "%s:%zu: Invalid number of cards for INCLUDE_NASTRAN keyword",
                   file_name, line_count);
             }
 
             /* continue without calling the callback for the card*/
-            if (card.string != line.buffer) {
+            if (card.string != line_reader.line.buffer) {
               free(card.string);
             }
 
             card_index++;
             continue;
           } else {
             char *keyword_name;
@@ -568,17 +477,17 @@
           if (extra_string_compare(&current_keyword_name, "INCLUDE") == 0 ||
               extra_string_compare(&current_keyword_name, "INCLUDE_PATH") ==
                   0 ||
               extra_string_compare(&current_keyword_name,
                                    "INCLUDE_PATH_RELATIVE") == 0) {
             if (!_parse_multi_line_string(&current_multi_line_string,
                                           &current_multi_line_index, &card,
-                                          line_length)) {
+                                          line_reader.line_length)) {
               /* continue without calling the callback for the card*/
-              if (card.string != line.buffer) {
+              if (card.string != line_reader.line.buffer) {
                 free(card.string);
               }
               continue;
             }
           } else if (extra_string_compare(&current_keyword_name,
                                           "INCLUDE_BINARY") == 0 ||
                      extra_string_compare(&current_keyword_name,
@@ -587,29 +496,29 @@
                                           "INCLUDE_TRANSFORM") == 0 ||
                      extra_string_compare(&current_keyword_name,
                                           "INCLUDE_TRANSFORM_BINARY") == 0) {
             /* Parse the first card like a normal INCLUDE*/
             if (card_index == 0) {
               if (!_parse_multi_line_string(&current_multi_line_string,
                                             &current_multi_line_index, &card,
-                                            line_length)) {
+                                            line_reader.line_length)) {
                 /* continue without calling the callback for the card*/
-                if (card.string != line.buffer) {
+                if (card.string != line_reader.line.buffer) {
                   free(card.string);
                 }
                 continue;
               }
             }
           }
         }
       }
       /* ------- ⛅ End of Include Parsing ⛅ -------*/
 
       if (current_multi_line_string) {
-        if (card.string != line.buffer) {
+        if (card.string != line_reader.line.buffer) {
           free(card.string);
         }
         card.string = current_multi_line_string;
       }
 
       char *keyword_name;
       if (current_keyword_length < EXTRA_STRING_BUFFER_SIZE) {
@@ -620,15 +529,15 @@
                                     current_keyword_length);
         keyword_name[current_keyword_length] = '\0';
       }
 
       callback(file_name, line_count, keyword_name, &card, card_index,
                user_data);
 
-      if (card.string != line.buffer) {
+      if (card.string != line_reader.line.buffer) {
         free(card.string);
         current_multi_line_string = NULL;
       }
       if (keyword_name != current_keyword_name.buffer) {
         free(keyword_name);
       }
       current_multi_line_index = 0;
@@ -690,15 +599,15 @@
   if (!num_include_paths) {
     free(num_include_paths_ptr);
   }
   if (!root_folder) {
     free(root_folder_ptr);
   }
 
-  free(line.extra);
+  free(line_reader.line.extra);
   free(current_keyword_name.extra);
 
   fclose(file);
 
   if (error_stack) {
     if (!error_string) {
       free(error_stack);
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/key.h` & `dynareadout-23.7/lib/dynareadout/src/key.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/multi_file.c` & `dynareadout-23.7/lib/dynareadout/src/multi_file.c`

 * *Files 4% similar despite different names*

```diff
@@ -138,21 +138,14 @@
   return index;
 }
 
 void multi_file_return(multi_file_t *f, multi_file_index_t *index) {
   BEGIN_PROFILE_FUNC();
   sync_lock(&f->file_handles_mutex);
 
-  /* Keep at least one file open at all times and close all other ones if
-   * returned*/
-  if (index->index != 0) {
-    fclose(index->file_handle);
-    f->file_handles[index->index].file_handle = NULL;
-  }
-
   sync_unlock(&f->file_handles[index->index].mutex);
 
   sync_unlock(&f->file_handles_mutex);
   END_PROFILE_FUNC();
 }
 
 int multi_file_seek(multi_file_t *f, multi_file_index_t *index, long offset,
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/multi_file.h` & `dynareadout-23.7/lib/dynareadout/src/multi_file.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/path.c` & `dynareadout-23.7/lib/dynareadout/src/path.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/path.h` & `dynareadout-23.7/lib/dynareadout/src/path.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/path_view.c` & `dynareadout-23.7/lib/dynareadout/src/path_view.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/path_view.h` & `dynareadout-23.7/lib/dynareadout/src/path_view.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/pgni.h` & `dynareadout-23.7/lib/dynareadout/src/pgni.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/profiling.c` & `dynareadout-23.7/lib/dynareadout/src/profiling.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/profiling.h` & `dynareadout-23.7/lib/dynareadout/src/profiling.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/python/conversions.hpp` & `dynareadout-23.7/lib/dynareadout/src/python/conversions.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/python/pybind11_d3plot.cpp` & `dynareadout-23.7/lib/dynareadout/src/python/pybind11_d3plot.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,28 @@
              try {
                return self[index];
              } catch (const std::runtime_error &) {
                throw py::index_error("Index out of range");
              }
            })
       .def("get_mid_history_variables",
-           &dro::D3plotShellsState::get_mid_history_variables)
+           &dro::D3plotShellsState::get_mid_history_variables,
+           "Returns the history variables for the mid surface of the shell "
+           "under index",
+           py::arg("index"))
       .def("get_inner_history_variables",
-           &dro::D3plotShellsState::get_inner_history_variables)
+           &dro::D3plotShellsState::get_inner_history_variables,
+           "Returns the history variables for the inner surface of the shell "
+           "under index",
+           py::arg("index"))
       .def("get_outer_history_variables",
-           &dro::D3plotShellsState::get_outer_history_variables)
+           &dro::D3plotShellsState::get_outer_history_variables,
+           "Returns the history variables for the outer surface of the shell "
+           "under index",
+           py::arg("index"))
 
       ;
 
   py::class_<dro::D3plotThickShellsState>(
       m, dro::get_array_name<d3plot_thick_shell>())
       .def("__len__", &dro::D3plotThickShellsState::size)
       .def("__getitem__",
@@ -66,45 +75,66 @@
              try {
                return self[index];
              } catch (const std::runtime_error &) {
                throw py::index_error("Index out of range");
              }
            })
       .def("get_mid_history_variables",
-           &dro::D3plotThickShellsState::get_mid_history_variables)
+           &dro::D3plotThickShellsState::get_mid_history_variables,
+           "Returns the history variables of the mid surface of the thick "
+           "shell under index",
+           py::arg("index"))
       .def("get_inner_history_variables",
-           &dro::D3plotThickShellsState::get_inner_history_variables)
+           &dro::D3plotThickShellsState::get_inner_history_variables,
+           "Returns the history variables of the inner surface of the thick "
+           "shell under index",
+           py::arg("index"))
       .def("get_outer_history_variables",
-           &dro::D3plotThickShellsState::get_outer_history_variables)
+           &dro::D3plotThickShellsState::get_outer_history_variables,
+           "Returns the history variables of the outer surface of the thick "
+           "shell under index",
+           py::arg("index"))
 
       ;
 }
 
 void add_d3plot_library_to_module(py::module_ &m) {
   add_d3plot_arrays_to_module(m);
 
   py::class_<d3plot_solid_con>(m, "d3plot_solid_con")
-      .def_readonly("node_indices", &d3plot_solid_con::node_indices)
-      .def_readonly("material_index", &d3plot_solid_con::material_index)
+      .def_readonly(
+          "node_indices", &d3plot_solid_con::node_indices,
+          "Stores indices into the node_ids, node_coords, etc. arrays")
+      .def_readonly("material_index", &d3plot_solid_con::material_index,
+                    "Index into the parts (this those indeed refer to parts "
+                    "even though the documentation does not say so)")
       .def("__str__", &dro::stream_to_string<d3plot_solid_con>)
 
       ;
 
   py::class_<d3plot_beam_con>(m, "d3plot_beam_con")
-      .def_readonly("node_indices", &d3plot_beam_con::node_indices)
+      .def_readonly(
+          "node_indices", &d3plot_beam_con::node_indices,
+          "Stores indices into the node_ids, node_coords, etc. arrays")
       .def_readonly("orientation_node_index",
                     &d3plot_beam_con::orientation_node_index)
-      .def_readonly("material_index", &d3plot_beam_con::material_index)
+      .def_readonly("material_index", &d3plot_beam_con::material_index,
+                    "Index into the parts (this those indeed refer to parts "
+                    "even though the documentation does not say so)")
       .def("__str__", &dro::stream_to_string<d3plot_beam_con>)
 
       ;
 
   py::class_<d3plot_shell_con>(m, "d3plot_shell_con")
-      .def_readonly("node_indices", &d3plot_shell_con::node_indices)
-      .def_readonly("material_index", &d3plot_shell_con::material_index)
+      .def_readonly(
+          "node_indices", &d3plot_shell_con::node_indices,
+          "Stores indices into the node_ids, node_coords, etc. arrays")
+      .def_readonly("material_index", &d3plot_shell_con::material_index,
+                    "Index into the parts (this those indeed refer to parts "
+                    "even though the documentation does not say so)")
       .def("__str__", &dro::stream_to_string<d3plot_shell_con>)
 
       ;
 
   py::class_<d3plot_tensor>(m, "d3plot_tensor")
       .def_readonly("x", &d3plot_tensor::x)
       .def_readonly("y", &d3plot_tensor::y)
@@ -148,16 +178,14 @@
   py::class_<d3plot_solid>(m, "d3plot_solid")
       .def_readonly("sigma", &d3plot_solid::sigma)
       .def_readonly("stress", &d3plot_solid::stress)
       .def_readonly("effective_plastic_strain",
                     &d3plot_solid::effective_plastic_strain)
       .def_readonly("material_dependent_value",
                     &d3plot_solid::material_dependent_value)
-      .def_readonly("extra1", &d3plot_solid::extra1)
-      .def_readonly("extra1", &d3plot_solid::extra2)
       .def_readonly("epsilon", &d3plot_solid::epsilon)
       .def_readonly("strain", &d3plot_solid::strain)
       .def("__str__", &dro::stream_to_string<d3plot_solid>)
 
       ;
 
   py::class_<d3plot_thick_shell>(m, "d3plot_thick_shell")
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/python/pybind11_module.cpp` & `dynareadout-23.7/lib/dynareadout/src/python/pybind11_module.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 namespace py = pybind11;
 
 void add_binout_library_to_module(py::module_ &m);
 void add_d3plot_library_to_module(py::module_ &m);
 void add_key_library_to_module(py::module_ &m);
 
 #ifdef NDEBUG
-PYBIND11_MODULE(dynareadout_c, m) {
+PYBIND11_MODULE(dynareadout, m) {
 #else
-PYBIND11_MODULE(dynareadout_c_d, m) {
+PYBIND11_MODULE(dynareadout_d, m) {
 #endif
   dro::add_array_to_module(m);
   add_binout_library_to_module(m);
   add_d3plot_library_to_module(m);
   add_key_library_to_module(m);
 }
```

### Comparing `dynareadout-23.6/lib/dynareadout/src/sync.c` & `dynareadout-23.7/lib/dynareadout/src/sync.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/dynareadout/src/sync.h` & `dynareadout-23.7/lib/dynareadout/src/sync.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/pybind11/LICENSE` & `dynareadout-23.7/lib/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/attr.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/attr.h`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 /// Annotation for methods
 struct is_method {
     handle class_;
     explicit is_method(const handle &c) : class_(c) {}
 };
 
+/// Annotation for setters
+struct is_setter {};
+
 /// Annotation for operators
 struct is_operator {};
 
 /// Annotation for classes that cannot be subclassed
 struct is_final {};
 
 /// Annotation for parent scope
@@ -184,16 +187,16 @@
 };
 
 /// Internal data structure which holds metadata about a bound function (signature, overloads,
 /// etc.)
 struct function_record {
     function_record()
         : is_constructor(false), is_new_style_constructor(false), is_stateless(false),
-          is_operator(false), is_method(false), has_args(false), has_kwargs(false),
-          prepend(false) {}
+          is_operator(false), is_method(false), is_setter(false), has_args(false),
+          has_kwargs(false), prepend(false) {}
 
     /// Function name
     char *name = nullptr; /* why no C++ strings? They generate heavier code.. */
 
     // User-specified documentation string
     char *doc = nullptr;
 
@@ -226,14 +229,17 @@
 
     /// True if this is an operator (__add__), etc.
     bool is_operator : 1;
 
     /// True if this is a method
     bool is_method : 1;
 
+    /// True if this is a setter
+    bool is_setter : 1;
+
     /// True if the function has a '*args' argument
     bool has_args : 1;
 
     /// True if the function has a '**kwargs' argument
     bool has_kwargs : 1;
 
     /// True if this function is to be inserted at the beginning of the overload resolution chain
@@ -395,15 +401,15 @@
     static void init(const doc &n, function_record *r) { r->doc = const_cast<char *>(n.value); }
 };
 
 /// Process an attribute specifying the function's docstring (provided as a C-style string)
 template <>
 struct process_attribute<const char *> : process_attribute_default<const char *> {
     static void init(const char *d, function_record *r) { r->doc = const_cast<char *>(d); }
-    static void init(const char *d, type_record *r) { r->doc = const_cast<char *>(d); }
+    static void init(const char *d, type_record *r) { r->doc = d; }
 };
 template <>
 struct process_attribute<char *> : process_attribute<const char *> {};
 
 /// Process an attribute indicating the function's return value policy
 template <>
 struct process_attribute<return_value_policy> : process_attribute_default<return_value_policy> {
@@ -422,14 +428,20 @@
 struct process_attribute<is_method> : process_attribute_default<is_method> {
     static void init(const is_method &s, function_record *r) {
         r->is_method = true;
         r->scope = s.class_;
     }
 };
 
+/// Process an attribute which indicates that this function is a setter
+template <>
+struct process_attribute<is_setter> : process_attribute_default<is_setter> {
+    static void init(const is_setter &, function_record *r) { r->is_setter = true; }
+};
+
 /// Process an attribute which indicates the parent scope of a method
 template <>
 struct process_attribute<scope> : process_attribute_default<scope> {
     static void init(const scope &s, function_record *r) { r->scope = s.value; }
 };
 
 /// Process an attribute which indicates that this function is an operator
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/buffer_info.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/buffer_info.h`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     std::vector<ssize_t> strides(ndim, itemsize);
     for (size_t i = 1; i < ndim; ++i) {
         strides[i] = strides[i - 1] * shape[i - 1];
     }
     return strides;
 }
 
+template <typename T, typename SFINAE = void>
+struct compare_buffer_info;
+
 PYBIND11_NAMESPACE_END(detail)
 
 /// Information record describing a Python buffer object
 struct buffer_info {
     void *ptr = nullptr;          // Pointer to the underlying storage
     ssize_t itemsize = 0;         // Size of individual items in bytes
     ssize_t size = 0;             // Total number of entries
@@ -146,14 +149,25 @@
             delete m_view;
         }
     }
 
     Py_buffer *view() const { return m_view; }
     Py_buffer *&view() { return m_view; }
 
+    /* True if the buffer item type is equivalent to `T`. */
+    // To define "equivalent" by example:
+    // `buffer_info::item_type_is_equivalent_to<int>(b)` and
+    // `buffer_info::item_type_is_equivalent_to<long>(b)` may both be true
+    // on some platforms, but `int` and `unsigned` will never be equivalent.
+    // For the ground truth, please inspect `detail::compare_buffer_info<>`.
+    template <typename T>
+    bool item_type_is_equivalent_to() const {
+        return detail::compare_buffer_info<T>::compare(*this);
+    }
+
 private:
     struct private_ctr_tag {};
 
     buffer_info(private_ctr_tag,
                 void *ptr,
                 ssize_t itemsize,
                 const std::string &format,
@@ -166,17 +180,18 @@
 
     Py_buffer *m_view = nullptr;
     bool ownview = false;
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-template <typename T, typename SFINAE = void>
+template <typename T, typename SFINAE>
 struct compare_buffer_info {
     static bool compare(const buffer_info &b) {
+        // NOLINTNEXTLINE(bugprone-sizeof-expression) Needed for `PyObject *`
         return b.format == format_descriptor<T>::format() && b.itemsize == (ssize_t) sizeof(T);
     }
 };
 
 template <typename T>
 struct compare_buffer_info<T, detail::enable_if_t<std::is_integral<T>::value>> {
     static bool compare(const buffer_info &b) {
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/cast.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/cast.h`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 #include <string>
 #include <tuple>
 #include <type_traits>
 #include <utility>
 #include <vector>
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
+
+PYBIND11_WARNING_DISABLE_MSVC(4127)
+
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <typename type, typename SFINAE = void>
 class type_caster : public type_caster_base<type> {};
 template <typename type>
 using make_caster = type_caster<intrinsic_t<type>>;
 
@@ -84,15 +87,16 @@
     type value;                                                                                   \
                                                                                                   \
 public:                                                                                           \
     static constexpr auto name = py_name;                                                         \
     template <typename T_,                                                                        \
               ::pybind11::detail::enable_if_t<                                                    \
                   std::is_same<type, ::pybind11::detail::remove_cv_t<T_>>::value,                 \
-                  int> = 0>                                                                       \
+                  int>                                                                            \
+              = 0>                                                                                \
     static ::pybind11::handle cast(                                                               \
         T_ *src, ::pybind11::return_value_policy policy, ::pybind11::handle parent) {             \
         if (!src)                                                                                 \
             return ::pybind11::none().release();                                                  \
         if (policy == ::pybind11::return_value_policy::take_ownership) {                          \
             auto h = cast(std::move(*src), policy, parent);                                       \
             delete src;                                                                           \
@@ -385,15 +389,15 @@
         }
         if (!PyUnicode_Check(load_src.ptr())) {
             return load_raw(load_src);
         }
 
         // For UTF-8 we avoid the need for a temporary `bytes` object by using
         // `PyUnicode_AsUTF8AndSize`.
-        if (PYBIND11_SILENCE_MSVC_C4127(UTF_N == 8)) {
+        if (UTF_N == 8) {
             Py_ssize_t size = -1;
             const auto *buffer
                 = reinterpret_cast<const CharT *>(PyUnicode_AsUTF8AndSize(load_src.ptr(), &size));
             if (!buffer) {
                 PyErr_Clear();
                 return false;
             }
@@ -412,15 +416,15 @@
             return false;
         }
 
         const auto *buffer
             = reinterpret_cast<const CharT *>(PYBIND11_BYTES_AS_STRING(utfNbytes.ptr()));
         size_t length = (size_t) PYBIND11_BYTES_SIZE(utfNbytes.ptr()) / sizeof(CharT);
         // Skip BOM for UTF-16/32
-        if (PYBIND11_SILENCE_MSVC_C4127(UTF_N > 8)) {
+        if (UTF_N > 8) {
             buffer++;
             length--;
         }
         value = StringType(buffer, length);
 
         // If we're loading a string_view we need to keep the encoded Python object alive:
         if (IsView) {
@@ -568,15 +572,15 @@
         }
 
         // If we're in UTF-8 mode, we have two possible failures: one for a unicode character that
         // is too high, and one for multiple unicode characters (caught later), so we need to
         // figure out how long the first encoded character is in bytes to distinguish between these
         // two errors.  We also allow want to allow unicode characters U+0080 through U+00FF, as
         // those can fit into a single char value.
-        if (PYBIND11_SILENCE_MSVC_C4127(StringCaster::UTF_N == 8) && str_len > 1 && str_len <= 4) {
+        if (StringCaster::UTF_N == 8 && str_len > 1 && str_len <= 4) {
             auto v0 = static_cast<unsigned char>(value[0]);
             // low bits only: 0-127
             // 0b110xxxxx - start of 2-byte sequence
             // 0b1110xxxx - start of 3-byte sequence
             // 0b11110xxx - start of 4-byte sequence
             size_t char0_bytes = (v0 & 0x80) == 0      ? 1
                                  : (v0 & 0xE0) == 0xC0 ? 2
@@ -594,15 +598,15 @@
                 throw value_error("Character code point not in range(0x100)");
             }
         }
 
         // UTF-16 is much easier: we can only have a surrogate pair for values above U+FFFF, thus a
         // surrogate pair with total length 2 instantly indicates a range error (but not a "your
         // string was too long" error).
-        else if (PYBIND11_SILENCE_MSVC_C4127(StringCaster::UTF_N == 16) && str_len == 2) {
+        else if (StringCaster::UTF_N == 16 && str_len == 2) {
             one_char = static_cast<CharT>(value[0]);
             if (one_char >= 0xD800 && one_char < 0xE000) {
                 throw value_error("Character code point not in range(0x10000)");
             }
         }
 
         if (str_len != 1) {
@@ -956,26 +960,26 @@
 struct move_always : std::false_type {};
 template <typename T>
 struct move_always<
     T,
     enable_if_t<
         all_of<move_is_plain_type<T>,
                negation<is_copy_constructible<T>>,
-               std::is_move_constructible<T>,
+               is_move_constructible<T>,
                std::is_same<decltype(std::declval<make_caster<T>>().operator T &()), T &>>::value>>
     : std::true_type {};
 template <typename T, typename SFINAE = void>
 struct move_if_unreferenced : std::false_type {};
 template <typename T>
 struct move_if_unreferenced<
     T,
     enable_if_t<
         all_of<move_is_plain_type<T>,
                negation<move_always<T>>,
-               std::is_move_constructible<T>,
+               is_move_constructible<T>,
                std::is_same<decltype(std::declval<make_caster<T>>().operator T &()), T &>>::value>>
     : std::true_type {};
 template <typename T>
 using move_never = none_of<move_always<T>, move_if_unreferenced<T>>;
 
 // Detect whether returning a `type` from a cast on type's type_caster is going to result in a
 // reference or pointer to a local variable of the type_caster.  Basically, only
@@ -1009,19 +1013,22 @@
 // Basic python -> C++ casting; throws if casting fails
 template <typename T, typename SFINAE>
 type_caster<T, SFINAE> &load_type(type_caster<T, SFINAE> &conv, const handle &handle) {
     static_assert(!detail::is_pyobject<T>::value,
                   "Internal error: type_caster should only be used for C++ types");
     if (!conv.load(handle, true)) {
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
-        throw cast_error("Unable to cast Python instance to C++ type (#define "
-                         "PYBIND11_DETAILED_ERROR_MESSAGES or compile in debug mode for details)");
+        throw cast_error(
+            "Unable to cast Python instance of type "
+            + str(type::handle_of(handle)).cast<std::string>()
+            + " to C++ type '?' (#define "
+              "PYBIND11_DETAILED_ERROR_MESSAGES or compile in debug mode for details)");
 #else
         throw cast_error("Unable to cast Python instance of type "
-                         + (std::string) str(type::handle_of(handle)) + " to C++ type '"
+                         + str(type::handle_of(handle)).cast<std::string>() + " to C++ type '"
                          + type_id<T>() + "'");
 #endif
     }
     return conv;
 }
 // Wrapper around the above that also constructs and returns a type_caster
 template <typename T>
@@ -1030,28 +1037,60 @@
     load_type(conv, handle);
     return conv;
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 // pytype -> C++ type
-template <typename T, detail::enable_if_t<!detail::is_pyobject<T>::value, int> = 0>
+template <typename T,
+          detail::enable_if_t<!detail::is_pyobject<T>::value
+                                  && !detail::is_same_ignoring_cvref<T, PyObject *>::value,
+                              int>
+          = 0>
 T cast(const handle &handle) {
     using namespace detail;
     static_assert(!cast_is_temporary_value_reference<T>::value,
                   "Unable to cast type to reference: value is local to type caster");
     return cast_op<T>(load_type<T>(handle));
 }
 
 // pytype -> pytype (calls converting constructor)
 template <typename T, detail::enable_if_t<detail::is_pyobject<T>::value, int> = 0>
 T cast(const handle &handle) {
     return T(reinterpret_borrow<object>(handle));
 }
 
+// Note that `cast<PyObject *>(obj)` increments the reference count of `obj`.
+// This is necessary for the case that `obj` is a temporary, and could
+// not possibly be different, given
+// 1. the established convention that the passed `handle` is borrowed, and
+// 2. we don't want to force all generic code using `cast<T>()` to special-case
+//    handling of `T` = `PyObject *` (to increment the reference count there).
+// It is the responsibility of the caller to ensure that the reference count
+// is decremented.
+template <typename T,
+          typename Handle,
+          detail::enable_if_t<detail::is_same_ignoring_cvref<T, PyObject *>::value
+                                  && detail::is_same_ignoring_cvref<Handle, handle>::value,
+                              int>
+          = 0>
+T cast(Handle &&handle) {
+    return handle.inc_ref().ptr();
+}
+// To optimize way an inc_ref/dec_ref cycle:
+template <typename T,
+          typename Object,
+          detail::enable_if_t<detail::is_same_ignoring_cvref<T, PyObject *>::value
+                                  && detail::is_same_ignoring_cvref<Object, object>::value,
+                              int>
+          = 0>
+T cast(Object &&obj) {
+    return obj.release().ptr();
+}
+
 // C++ type -> py::object
 template <typename T, detail::enable_if_t<!detail::is_pyobject<T>::value, int> = 0>
 object cast(T &&value,
             return_value_policy policy = return_value_policy::automatic_reference,
             handle parent = handle()) {
     using no_ref_T = typename std::remove_reference<T>::type;
     if (policy == return_value_policy::automatic) {
@@ -1077,20 +1116,21 @@
 }
 
 template <typename T>
 detail::enable_if_t<!detail::move_never<T>::value, T> move(object &&obj) {
     if (obj.ref_count() > 1) {
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
         throw cast_error(
-            "Unable to cast Python instance to C++ rvalue: instance has multiple references"
-            " (#define PYBIND11_DETAILED_ERROR_MESSAGES or compile in debug mode for details)");
+            "Unable to cast Python " + str(type::handle_of(obj)).cast<std::string>()
+            + " instance to C++ rvalue: instance has multiple references"
+              " (#define PYBIND11_DETAILED_ERROR_MESSAGES or compile in debug mode for details)");
 #else
-        throw cast_error("Unable to move from Python " + (std::string) str(type::handle_of(obj))
-                         + " instance to C++ " + type_id<T>()
-                         + " instance: instance has multiple references");
+        throw cast_error("Unable to move from Python "
+                         + str(type::handle_of(obj)).cast<std::string>() + " instance to C++ "
+                         + type_id<T>() + " instance: instance has multiple references");
 #endif
     }
 
     // Move into a temporary and return that, because the reference may be a local value of `conv`
     T ret = std::move(detail::load_type<T>(obj).operator T &());
     return ret;
 }
@@ -1187,17 +1227,18 @@
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 // The overloads could coexist, i.e. the #if is not strictly speaking needed,
 // but it is an easy minor optimization.
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
-inline cast_error cast_error_unable_to_convert_call_arg() {
-    return cast_error("Unable to convert call argument to Python object (#define "
-                      "PYBIND11_DETAILED_ERROR_MESSAGES or compile in debug mode for details)");
+inline cast_error cast_error_unable_to_convert_call_arg(const std::string &name) {
+    return cast_error("Unable to convert call argument '" + name
+                      + "' to Python object (#define "
+                        "PYBIND11_DETAILED_ERROR_MESSAGES or compile in debug mode for details)");
 }
 #else
 inline cast_error cast_error_unable_to_convert_call_arg(const std::string &name,
                                                         const std::string &type) {
     return cast_error("Unable to convert call argument '" + name + "' of type '" + type
                       + "' to Python object");
 }
@@ -1212,15 +1253,15 @@
 tuple make_tuple(Args &&...args_) {
     constexpr size_t size = sizeof...(Args);
     std::array<object, size> args{{reinterpret_steal<object>(
         detail::make_caster<Args>::cast(std::forward<Args>(args_), policy, nullptr))...}};
     for (size_t i = 0; i < args.size(); i++) {
         if (!args[i]) {
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
-            throw cast_error_unable_to_convert_call_arg();
+            throw cast_error_unable_to_convert_call_arg(std::to_string(i));
 #else
             std::array<std::string, size> argtypes{{type_id<Args>()...}};
             throw cast_error_unable_to_convert_call_arg(std::to_string(i), argtypes[i]);
 #endif
         }
     }
     tuple result(size);
@@ -1502,15 +1543,15 @@
 private:
     template <typename T>
     void process(list &args_list, T &&x) {
         auto o = reinterpret_steal<object>(
             detail::make_caster<T>::cast(std::forward<T>(x), policy, {}));
         if (!o) {
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
-            throw cast_error_unable_to_convert_call_arg();
+            throw cast_error_unable_to_convert_call_arg(std::to_string(args_list.size()));
 #else
             throw cast_error_unable_to_convert_call_arg(std::to_string(args_list.size()),
                                                         type_id<T>());
 #endif
         }
         args_list.append(std::move(o));
     }
@@ -1534,15 +1575,15 @@
             multiple_values_error();
 #else
             multiple_values_error(a.name);
 #endif
         }
         if (!a.value) {
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
-            throw cast_error_unable_to_convert_call_arg();
+            throw cast_error_unable_to_convert_call_arg(a.name);
 #else
             throw cast_error_unable_to_convert_call_arg(a.name, a.type);
 #endif
         }
         m_kwargs[a.name] = std::move(a.value);
     }
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/chrono.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/complex.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/detail/class.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/detail/class.h`

 * *Files 1% similar despite different names*

```diff
@@ -441,17 +441,25 @@
         clear_patients(self);
     }
 }
 
 /// Instance destructor function for all pybind11 types. It calls `type_info.dealloc`
 /// to destroy the C++ object itself, while the rest is Python bookkeeping.
 extern "C" inline void pybind11_object_dealloc(PyObject *self) {
+    auto *type = Py_TYPE(self);
+
+    // If this is a GC tracked object, untrack it first
+    // Note that the track call is implicitly done by the
+    // default tp_alloc, which we never override.
+    if (PyType_HasFeature(type, Py_TPFLAGS_HAVE_GC) != 0) {
+        PyObject_GC_UnTrack(self);
+    }
+
     clear_instance(self);
 
-    auto *type = Py_TYPE(self);
     type->tp_free(self);
 
 #if PY_VERSION_HEX < 0x03080000
     // `type->tp_dealloc != pybind11_object_dealloc` means that we're being called
     // as part of a derived type's dealloc, in which case we're not allowed to decref
     // the type here. For cross-module compatibility, we shouldn't compare directly
     // with `pybind11_object_dealloc`, but with the common one stashed in internals.
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/detail/common.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/detail/common.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,84 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #define PYBIND11_VERSION_MAJOR 2
-#define PYBIND11_VERSION_MINOR 10
+#define PYBIND11_VERSION_MINOR 11
 #define PYBIND11_VERSION_PATCH 1
 
 // Similar to Python's convention: https://docs.python.org/3/c-api/apiabiversion.html
 // Additional convention: 0xD = dev
-#define PYBIND11_VERSION_HEX 0x020A0100
+#define PYBIND11_VERSION_HEX 0x020B0100
 
-#define PYBIND11_NAMESPACE_BEGIN(name) namespace name {
-#define PYBIND11_NAMESPACE_END(name) }
+// Define some generic pybind11 helper macros for warning management.
+//
+// Note that compiler-specific push/pop pairs are baked into the
+// PYBIND11_NAMESPACE_BEGIN/PYBIND11_NAMESPACE_END pair of macros. Therefore manual
+// PYBIND11_WARNING_PUSH/PYBIND11_WARNING_POP are usually only needed in `#include` sections.
+//
+// If you find you need to suppress a warning, please try to make the suppression as local as
+// possible using these macros. Please also be sure to push/pop with the pybind11 macros. Please
+// only use compiler specifics if you need to check specific versions, e.g. Apple Clang vs. vanilla
+// Clang.
+#if defined(_MSC_VER)
+#    define PYBIND11_COMPILER_MSVC
+#    define PYBIND11_PRAGMA(...) __pragma(__VA_ARGS__)
+#    define PYBIND11_WARNING_PUSH PYBIND11_PRAGMA(warning(push))
+#    define PYBIND11_WARNING_POP PYBIND11_PRAGMA(warning(pop))
+#elif defined(__INTEL_COMPILER)
+#    define PYBIND11_COMPILER_INTEL
+#    define PYBIND11_PRAGMA(...) _Pragma(#__VA_ARGS__)
+#    define PYBIND11_WARNING_PUSH PYBIND11_PRAGMA(warning push)
+#    define PYBIND11_WARNING_POP PYBIND11_PRAGMA(warning pop)
+#elif defined(__clang__)
+#    define PYBIND11_COMPILER_CLANG
+#    define PYBIND11_PRAGMA(...) _Pragma(#__VA_ARGS__)
+#    define PYBIND11_WARNING_PUSH PYBIND11_PRAGMA(clang diagnostic push)
+#    define PYBIND11_WARNING_POP PYBIND11_PRAGMA(clang diagnostic push)
+#elif defined(__GNUC__)
+#    define PYBIND11_COMPILER_GCC
+#    define PYBIND11_PRAGMA(...) _Pragma(#__VA_ARGS__)
+#    define PYBIND11_WARNING_PUSH PYBIND11_PRAGMA(GCC diagnostic push)
+#    define PYBIND11_WARNING_POP PYBIND11_PRAGMA(GCC diagnostic pop)
+#endif
+
+#ifdef PYBIND11_COMPILER_MSVC
+#    define PYBIND11_WARNING_DISABLE_MSVC(name) PYBIND11_PRAGMA(warning(disable : name))
+#else
+#    define PYBIND11_WARNING_DISABLE_MSVC(name)
+#endif
+
+#ifdef PYBIND11_COMPILER_CLANG
+#    define PYBIND11_WARNING_DISABLE_CLANG(name) PYBIND11_PRAGMA(clang diagnostic ignored name)
+#else
+#    define PYBIND11_WARNING_DISABLE_CLANG(name)
+#endif
+
+#ifdef PYBIND11_COMPILER_GCC
+#    define PYBIND11_WARNING_DISABLE_GCC(name) PYBIND11_PRAGMA(GCC diagnostic ignored name)
+#else
+#    define PYBIND11_WARNING_DISABLE_GCC(name)
+#endif
+
+#ifdef PYBIND11_COMPILER_INTEL
+#    define PYBIND11_WARNING_DISABLE_INTEL(name) PYBIND11_PRAGMA(warning disable name)
+#else
+#    define PYBIND11_WARNING_DISABLE_INTEL(name)
+#endif
+
+#define PYBIND11_NAMESPACE_BEGIN(name)                                                            \
+    namespace name {                                                                              \
+    PYBIND11_WARNING_PUSH
+
+#define PYBIND11_NAMESPACE_END(name)                                                              \
+    PYBIND11_WARNING_POP                                                                          \
+    }
 
 // Robust support for some features and loading modules compiled against different pybind versions
 // requires forcing hidden visibility on pybind code, so we enforce this by setting the attribute
 // on the main `pybind11` namespace.
 #if !defined(PYBIND11_NAMESPACE)
 #    ifdef __GNUG__
 #        define PYBIND11_NAMESPACE pybind11 __attribute__((visibility("hidden")))
@@ -92,21 +153,18 @@
 #        define PYBIND11_EXPORT __declspec(dllexport)
 #    else
 #        define PYBIND11_EXPORT __attribute__((visibility("default")))
 #    endif
 #endif
 
 #if !defined(PYBIND11_EXPORT_EXCEPTION)
-#    ifdef __MINGW32__
-// workaround for:
-// error: 'dllexport' implies default visibility, but xxx has already been declared with a
-// different visibility
-#        define PYBIND11_EXPORT_EXCEPTION
-#    else
+#    if defined(__apple_build_version__)
 #        define PYBIND11_EXPORT_EXCEPTION PYBIND11_EXPORT
+#    else
+#        define PYBIND11_EXPORT_EXCEPTION
 #    endif
 #endif
 
 // For CUDA, GCC7, GCC8:
 // PYBIND11_NOINLINE_FORCED is incompatible with `-Wattributes -Werror`.
 // When defining PYBIND11_NOINLINE_FORCED, it is best to also use `-Wno-attributes`.
 // However, the measured shared-library size saving when using noinline are only
@@ -150,17 +208,17 @@
    properly in Visual Studio since 2015. */
 #if defined(_MSC_VER)
 #    define HAVE_SNPRINTF 1
 #endif
 
 /// Include Python header, disable linking to pythonX_d.lib on Windows in debug mode
 #if defined(_MSC_VER)
-#    pragma warning(push)
+PYBIND11_WARNING_PUSH
+PYBIND11_WARNING_DISABLE_MSVC(4505)
 // C4505: 'PySlice_GetIndicesEx': unreferenced local function has been removed (PyPy only)
-#    pragma warning(disable : 4505)
 #    if defined(_DEBUG) && !defined(Py_DEBUG)
 // Workaround for a VS 2022 issue.
 // NOTE: This workaround knowingly violates the Python.h include order requirement:
 // https://docs.python.org/3/c-api/intro.html#include-files
 // See https://github.com/pybind/pybind11/pull/3497 for full context.
 #        include <yvals.h>
 #        if _MSVC_STL_VERSION >= 143
@@ -235,15 +293,15 @@
 #endif
 
 #if defined(_MSC_VER)
 #    if defined(PYBIND11_DEBUG_MARKER)
 #        define _DEBUG
 #        undef PYBIND11_DEBUG_MARKER
 #    endif
-#    pragma warning(pop)
+PYBIND11_WARNING_POP
 #endif
 
 #include <cstddef>
 #include <cstring>
 #include <exception>
 #include <forward_list>
 #include <memory>
@@ -261,14 +319,20 @@
 #endif
 
 // Must be after including <version> or one of the other headers specified by the standard
 #if defined(__cpp_lib_char8_t) && __cpp_lib_char8_t >= 201811L
 #    define PYBIND11_HAS_U8STRING
 #endif
 
+// See description of PR #4246:
+#if !defined(PYBIND11_NO_ASSERT_GIL_HELD_INCREF_DECREF) && !defined(NDEBUG)                       \
+    && !defined(PYPY_VERSION) && !defined(PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF)
+#    define PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
+#endif
+
 // #define PYBIND11_STR_LEGACY_PERMISSIVE
 // If DEFINED, pybind11::str can hold PyUnicodeObject or PyBytesObject
 //             (probably surprising and never documented, but this was the
 //             legacy behavior until and including v2.6.x). As a side-effect,
 //             pybind11::isinstance<str>() is true for both pybind11::str and
 //             pybind11::bytes.
 // If UNDEFINED, pybind11::str can only hold PyUnicodeObject, and
@@ -365,15 +429,15 @@
         }                                                                                         \
         PYBIND11_CATCH_INIT_EXCEPTIONS                                                            \
     }                                                                                             \
     PyObject *pybind11_init()
 
 /** \rst
     This macro creates the entry point that will be invoked when the Python interpreter
-    imports an extension module. The module name is given as the fist argument and it
+    imports an extension module. The module name is given as the first argument and it
     should not be in quotes. The second macro argument defines a variable of type
     `py::module_` which can be used to initialize the module.
 
     The entry point is marked as "maybe unused" to aid dead-code detection analysis:
     since the entry point is typically only looked up at runtime and not referenced
     during translation, it would otherwise appear as unused ("dead") code.
 
@@ -590,14 +654,18 @@
 struct remove_cvref {
     using type = remove_cv_t<remove_reference_t<T>>;
 };
 template <class T>
 using remove_cvref_t = typename remove_cvref<T>::type;
 #endif
 
+/// Example usage: is_same_ignoring_cvref<T, PyObject *>::value
+template <typename T, typename U>
+using is_same_ignoring_cvref = std::is_same<detail::remove_cvref_t<T>, U>;
+
 /// Index sequences
 #if defined(PYBIND11_CPP14)
 using std::index_sequence;
 using std::make_index_sequence;
 #else
 template <size_t...>
 struct index_sequence {};
@@ -683,15 +751,24 @@
 struct remove_class<R (C::*)(A...)> {
     using type = R(A...);
 };
 template <typename C, typename R, typename... A>
 struct remove_class<R (C::*)(A...) const> {
     using type = R(A...);
 };
-
+#ifdef __cpp_noexcept_function_type
+template <typename C, typename R, typename... A>
+struct remove_class<R (C::*)(A...) noexcept> {
+    using type = R(A...);
+};
+template <typename C, typename R, typename... A>
+struct remove_class<R (C::*)(A...) const noexcept> {
+    using type = R(A...);
+};
+#endif
 /// Helper template to strip away type modifiers
 template <typename T>
 struct intrinsic_type {
     using type = T;
 };
 template <typename T>
 struct intrinsic_type<const T> {
@@ -900,30 +977,21 @@
 using expand_side_effects = bool[];
 #    define PYBIND11_EXPAND_SIDE_EFFECTS(PATTERN)                                                 \
         (void) pybind11::detail::expand_side_effects { ((PATTERN), void(), false)..., false }
 #endif
 
 PYBIND11_NAMESPACE_END(detail)
 
-#if defined(_MSC_VER)
-#    pragma warning(push)
-#    pragma warning(disable : 4275)
-//     warning C4275: An exported class was derived from a class that wasn't exported.
-//     Can be ignored when derived from a STL class.
-#endif
 /// C++ bindings of builtin Python exceptions
 class PYBIND11_EXPORT_EXCEPTION builtin_exception : public std::runtime_error {
 public:
     using std::runtime_error::runtime_error;
     /// Set the error using the Python C API
     virtual void set_error() const = 0;
 };
-#if defined(_MSC_VER)
-#    pragma warning(pop)
-#endif
 
 #define PYBIND11_RUNTIME_EXCEPTION(name, type)                                                    \
     class PYBIND11_EXPORT_EXCEPTION name : public builtin_exception {                             \
     public:                                                                                       \
         using builtin_exception::builtin_exception;                                               \
         name() : name("") {}                                                                      \
         void set_error() const override { PyErr_SetString(type, what()); }                        \
@@ -950,14 +1018,23 @@
     assert(!PyErr_Occurred());
     throw std::runtime_error(reason);
 }
 
 template <typename T, typename SFINAE = void>
 struct format_descriptor {};
 
+template <typename T>
+struct format_descriptor<
+    T,
+    detail::enable_if_t<detail::is_same_ignoring_cvref<T, PyObject *>::value>> {
+    static constexpr const char c = 'O';
+    static constexpr const char value[2] = {c, '\0'};
+    static std::string format() { return std::string(1, c); }
+};
+
 PYBIND11_NAMESPACE_BEGIN(detail)
 // Returns the index of the given type in the type char array below, and in the list in numpy.h
 // The order here is: bool; 8 ints ((signed,unsigned)x(8,16,32,64)bits); float,double,long double;
 // complex float,double,long double.  Note that the long double types only participate when long
 // double is actually longer than double (it isn't under MSVC).
 // NB: not only the string below but also complex.h and numpy.h rely on this order.
 template <typename T, typename SFINAE = void>
@@ -1144,25 +1221,14 @@
 #if defined(__GNUG__) && !defined(__clang__) && !defined(__INTEL_COMPILER)
 #    define PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(...)                       \
         detail::silence_unused_warnings(__VA_ARGS__)
 #else
 #    define PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(...)
 #endif
 
-#if defined(_MSC_VER) // All versions (as of July 2021).
-
-// warning C4127: Conditional expression is constant
-constexpr inline bool silence_msvc_c4127(bool cond) { return cond; }
-
-#    define PYBIND11_SILENCE_MSVC_C4127(...) ::pybind11::detail::silence_msvc_c4127(__VA_ARGS__)
-
-#else
-#    define PYBIND11_SILENCE_MSVC_C4127(...) __VA_ARGS__
-#endif
-
 #if defined(__clang__)                                                                            \
     && (defined(__apple_build_version__) /* AppleClang 13.0.0.13000029 was the only data point    \
                                             available. */                                         \
         || (__clang_major__ >= 7                                                                  \
             && __clang_major__ <= 12) /* Clang 3, 5, 13, 14, 15 do not generate the warning. */   \
     )
 #    define PYBIND11_DETECTED_CLANG_WITH_MISLEADING_CALL_STD_MOVE_EXPLICITLY_WARNING
@@ -1174,15 +1240,16 @@
 // test_kwargs_and_defaults.cpp:46:68: note: call 'std::move' explicitly to avoid copying
 //     m.def("args_function", [](py::args args) -> py::tuple { return args; });
 //                                                                    ^~~~
 //                                                                    std::move(args)
 #endif
 
 // Pybind offers detailed error messages by default for all builts that are debug (through the
-// negation of ndebug). This can also be manually enabled by users, for any builds, through
-// defining PYBIND11_DETAILED_ERROR_MESSAGES.
+// negation of NDEBUG). This can also be manually enabled by users, for any builds, through
+// defining PYBIND11_DETAILED_ERROR_MESSAGES. This information is primarily useful for those
+// who are writing (as opposed to merely using) libraries that use pybind11.
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES) && !defined(NDEBUG)
 #    define PYBIND11_DETAILED_ERROR_MESSAGES
 #endif
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/detail/descr.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/detail/descr.h`

 * *Files 5% similar despite different names*

```diff
@@ -139,19 +139,32 @@
 constexpr descr<0> concat() { return {}; }
 
 template <size_t N, typename... Ts>
 constexpr descr<N, Ts...> concat(const descr<N, Ts...> &descr) {
     return descr;
 }
 
+#ifdef __cpp_fold_expressions
+template <size_t N1, size_t N2, typename... Ts1, typename... Ts2>
+constexpr descr<N1 + N2 + 2, Ts1..., Ts2...> operator,(const descr<N1, Ts1...> &a,
+                                                       const descr<N2, Ts2...> &b) {
+    return a + const_name(", ") + b;
+}
+
+template <size_t N, typename... Ts, typename... Args>
+constexpr auto concat(const descr<N, Ts...> &d, const Args &...args) {
+    return (d, ..., args);
+}
+#else
 template <size_t N, typename... Ts, typename... Args>
 constexpr auto concat(const descr<N, Ts...> &d, const Args &...args)
     -> decltype(std::declval<descr<N + 2, Ts...>>() + concat(args...)) {
     return d + const_name(", ") + concat(args...);
 }
+#endif
 
 template <size_t N, typename... Ts>
 constexpr descr<N + 2, Ts...> type_descr(const descr<N, Ts...> &descr) {
     return const_name("{") + descr + const_name("}");
 }
 
 PYBIND11_NAMESPACE_END(detail)
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/detail/init.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/detail/init.h`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 */
 
 #pragma once
 
 #include "class.h"
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
+
+PYBIND11_WARNING_DISABLE_MSVC(4127)
+
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <>
 class type_caster<value_and_holder> {
 public:
     bool load(handle h, bool) {
         value = reinterpret_cast<value_and_holder *>(h.ptr());
@@ -111,15 +114,15 @@
 // If we don't need an alias (because this class doesn't have one, or because the final type is
 // inherited on the Python side) we can simply take over ownership.  Otherwise we need to try to
 // construct an Alias from the returned base instance.
 template <typename Class>
 void construct(value_and_holder &v_h, Cpp<Class> *ptr, bool need_alias) {
     PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
     no_nullptr(ptr);
-    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias && !is_alias<Class>(ptr)) {
+    if (Class::has_alias && need_alias && !is_alias<Class>(ptr)) {
         // We're going to try to construct an alias by moving the cpp type.  Whether or not
         // that succeeds, we still need to destroy the original cpp pointer (either the
         // moved away leftover, if the alias construction works, or the value itself if we
         // throw an error), but we can't just call `delete ptr`: it might have a special
         // deleter, or might be shared_from_this.  So we construct a holder around it as if
         // it was a normal instance, then steal the holder away into a local variable; thus
         // the holder and destruction happens when we leave the C++ scope, and the holder
@@ -152,15 +155,15 @@
 // constructors).
 template <typename Class>
 void construct(value_and_holder &v_h, Holder<Class> holder, bool need_alias) {
     PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
     auto *ptr = holder_helper<Holder<Class>>::get(holder);
     no_nullptr(ptr);
     // If we need an alias, check that the held pointer is actually an alias instance
-    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias && !is_alias<Class>(ptr)) {
+    if (Class::has_alias && need_alias && !is_alias<Class>(ptr)) {
         throw type_error("pybind11::init(): construction failed: returned holder-wrapped instance "
                          "is not an alias instance");
     }
 
     v_h.value_ptr() = ptr;
     v_h.type->init_instance(v_h.inst, &holder);
 }
@@ -168,30 +171,30 @@
 // return-by-value version 1: returning a cpp class by value.  If the class has an alias and an
 // alias is required the alias must have an `Alias(Cpp &&)` constructor so that we can construct
 // the alias from the base when needed (i.e. because of Python-side inheritance).  When we don't
 // need it, we simply move-construct the cpp value into a new instance.
 template <typename Class>
 void construct(value_and_holder &v_h, Cpp<Class> &&result, bool need_alias) {
     PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
-    static_assert(std::is_move_constructible<Cpp<Class>>::value,
+    static_assert(is_move_constructible<Cpp<Class>>::value,
                   "pybind11::init() return-by-value factory function requires a movable class");
-    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias) {
+    if (Class::has_alias && need_alias) {
         construct_alias_from_cpp<Class>(is_alias_constructible<Class>{}, v_h, std::move(result));
     } else {
         v_h.value_ptr() = new Cpp<Class>(std::move(result));
     }
 }
 
 // return-by-value version 2: returning a value of the alias type itself.  We move-construct an
 // Alias instance (even if no the python-side inheritance is involved).  The is intended for
 // cases where Alias initialization is always desired.
 template <typename Class>
 void construct(value_and_holder &v_h, Alias<Class> &&result, bool) {
     static_assert(
-        std::is_move_constructible<Alias<Class>>::value,
+        is_move_constructible<Alias<Class>>::value,
         "pybind11::init() return-by-alias-value factory function requires a movable alias class");
     v_h.value_ptr() = new Alias<Class>(std::move(result));
 }
 
 // Implementing class for py::init<...>()
 template <typename... Args>
 struct constructor {
@@ -202,18 +205,19 @@
             [](value_and_holder &v_h, Args... args) {
                 v_h.value_ptr() = construct_or_initialize<Cpp<Class>>(std::forward<Args>(args)...);
             },
             is_new_style_constructor(),
             extra...);
     }
 
-    template <typename Class,
-              typename... Extra,
-              enable_if_t<Class::has_alias && std::is_constructible<Cpp<Class>, Args...>::value,
-                          int> = 0>
+    template <
+        typename Class,
+        typename... Extra,
+        enable_if_t<Class::has_alias && std::is_constructible<Cpp<Class>, Args...>::value, int>
+        = 0>
     static void execute(Class &cl, const Extra &...extra) {
         cl.def(
             "__init__",
             [](value_and_holder &v_h, Args... args) {
                 if (Py_TYPE(v_h.inst) == v_h.type->type) {
                     v_h.value_ptr()
                         = construct_or_initialize<Cpp<Class>>(std::forward<Args>(args)...);
@@ -222,18 +226,19 @@
                         = construct_or_initialize<Alias<Class>>(std::forward<Args>(args)...);
                 }
             },
             is_new_style_constructor(),
             extra...);
     }
 
-    template <typename Class,
-              typename... Extra,
-              enable_if_t<Class::has_alias && !std::is_constructible<Cpp<Class>, Args...>::value,
-                          int> = 0>
+    template <
+        typename Class,
+        typename... Extra,
+        enable_if_t<Class::has_alias && !std::is_constructible<Cpp<Class>, Args...>::value, int>
+        = 0>
     static void execute(Class &cl, const Extra &...extra) {
         cl.def(
             "__init__",
             [](value_and_holder &v_h, Args... args) {
                 v_h.value_ptr()
                     = construct_or_initialize<Alias<Class>>(std::forward<Args>(args)...);
             },
@@ -241,18 +246,19 @@
             extra...);
     }
 };
 
 // Implementing class for py::init_alias<...>()
 template <typename... Args>
 struct alias_constructor {
-    template <typename Class,
-              typename... Extra,
-              enable_if_t<Class::has_alias && std::is_constructible<Alias<Class>, Args...>::value,
-                          int> = 0>
+    template <
+        typename Class,
+        typename... Extra,
+        enable_if_t<Class::has_alias && std::is_constructible<Alias<Class>, Args...>::value, int>
+        = 0>
     static void execute(Class &cl, const Extra &...extra) {
         cl.def(
             "__init__",
             [](value_and_holder &v_h, Args... args) {
                 v_h.value_ptr()
                     = construct_or_initialize<Alias<Class>>(std::forward<Args>(args)...);
             },
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/detail/internals.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/detail/internals.h`

 * *Files 12% similar despite different names*

```diff
@@ -30,23 +30,34 @@
 /// newer ABI.
 ///
 /// WARNING: If you choose to manually increase the ABI version, note that
 /// pybind11 may not be tested as thoroughly with a non-default ABI version, and
 /// further ABI-incompatible changes may be made before the ABI is officially
 /// changed to the new version.
 #ifndef PYBIND11_INTERNALS_VERSION
-#    define PYBIND11_INTERNALS_VERSION 4
+#    if PY_VERSION_HEX >= 0x030C0000
+// Version bump for Python 3.12+, before first 3.12 beta release.
+#        define PYBIND11_INTERNALS_VERSION 5
+#    else
+#        define PYBIND11_INTERNALS_VERSION 4
+#    endif
 #endif
 
+// This requirement is mainly to reduce the support burden (see PR #4570).
+static_assert(PY_VERSION_HEX < 0x030C0000 || PYBIND11_INTERNALS_VERSION >= 5,
+              "pybind11 ABI version 5 is the minimum for Python 3.12+");
+
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 using ExceptionTranslator = void (*)(std::exception_ptr);
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
+constexpr const char *internals_function_record_capsule_name = "pybind11_function_record_capsule";
+
 // Forward declarations
 inline PyTypeObject *make_static_property_type();
 inline PyTypeObject *make_default_metaclass();
 inline PyObject *make_object_base_type(PyTypeObject *metaclass);
 
 // The old Python Thread Local Storage (TLS) API is deprecated in Python 3.7 in favor of the new
 // Thread Specific Storage (TSS) API.
@@ -108,15 +119,16 @@
 
 // Python loads modules by default with dlopen with the RTLD_LOCAL flag; under libc++ and possibly
 // other STLs, this means `typeid(A)` from one module won't equal `typeid(A)` from another module
 // even when `A` is the same, non-hidden-visibility type (e.g. from a common include).  Under
 // libstdc++, this doesn't happen: equality and the type_index hash are based on the type name,
 // which works.  If not under a known-good stl, provide our own name-based hash and equality
 // functions that use the type name.
-#if defined(__GLIBCXX__)
+#if (PYBIND11_INTERNALS_VERSION <= 4 && defined(__GLIBCXX__))                                     \
+    || (PYBIND11_INTERNALS_VERSION >= 5 && !defined(_LIBCPP_VERSION))
 inline bool same_type(const std::type_info &lhs, const std::type_info &rhs) { return lhs == rhs; }
 using type_hash = std::hash<std::type_index>;
 using type_equal_to = std::equal_to<std::type_index>;
 #else
 inline bool same_type(const std::type_info &lhs, const std::type_info &rhs) {
     return lhs.name() == rhs.name() || std::strcmp(lhs.name(), rhs.name()) == 0;
 }
@@ -178,14 +190,24 @@
     // Unused if PYBIND11_SIMPLE_GIL_MANAGEMENT is defined:
     PYBIND11_TLS_KEY_INIT(tstate)
 #    if PYBIND11_INTERNALS_VERSION > 4
     PYBIND11_TLS_KEY_INIT(loader_life_support_tls_key)
 #    endif // PYBIND11_INTERNALS_VERSION > 4
     // Unused if PYBIND11_SIMPLE_GIL_MANAGEMENT is defined:
     PyInterpreterState *istate = nullptr;
+
+#    if PYBIND11_INTERNALS_VERSION > 4
+    // Note that we have to use a std::string to allocate memory to ensure a unique address
+    // We want unique addresses since we use pointer equality to compare function records
+    std::string function_record_capsule_name = internals_function_record_capsule_name;
+#    endif
+
+    internals() = default;
+    internals(const internals &other) = delete;
+    internals &operator=(const internals &other) = delete;
     ~internals() {
 #    if PYBIND11_INTERNALS_VERSION > 4
         PYBIND11_TLS_FREE(loader_life_support_tls_key);
 #    endif // PYBIND11_INTERNALS_VERSION > 4
 
         // This destructor is called *after* Py_Finalize() in finalize_interpreter().
         // That *SHOULD BE* fine. The following details what happens when PyThread_tss_free is
@@ -405,14 +427,46 @@
     } catch (const builtin_exception &e) {
         e.set_error();
         return;
     }
 }
 #endif
 
+inline object get_python_state_dict() {
+    object state_dict;
+#if PYBIND11_INTERNALS_VERSION <= 4 || PY_VERSION_HEX < 0x03080000 || defined(PYPY_VERSION)
+    state_dict = reinterpret_borrow<object>(PyEval_GetBuiltins());
+#else
+#    if PY_VERSION_HEX < 0x03090000
+    PyInterpreterState *istate = _PyInterpreterState_Get();
+#    else
+    PyInterpreterState *istate = PyInterpreterState_Get();
+#    endif
+    if (istate) {
+        state_dict = reinterpret_borrow<object>(PyInterpreterState_GetDict(istate));
+    }
+#endif
+    if (!state_dict) {
+        raise_from(PyExc_SystemError, "pybind11::detail::get_python_state_dict() FAILED");
+    }
+    return state_dict;
+}
+
+inline object get_internals_obj_from_state_dict(handle state_dict) {
+    return reinterpret_borrow<object>(dict_getitemstring(state_dict.ptr(), PYBIND11_INTERNALS_ID));
+}
+
+inline internals **get_internals_pp_from_capsule(handle obj) {
+    void *raw_ptr = PyCapsule_GetPointer(obj.ptr(), /*name=*/nullptr);
+    if (raw_ptr == nullptr) {
+        raise_from(PyExc_SystemError, "pybind11::detail::get_internals_pp_from_capsule() FAILED");
+    }
+    return static_cast<internals **>(raw_ptr);
+}
+
 /// Return a reference to the current `internals` data
 PYBIND11_NOINLINE internals &get_internals() {
     auto **&internals_pp = get_internals_pp();
     if (internals_pp && *internals_pp) {
         return **internals_pp;
     }
 
@@ -429,20 +483,20 @@
         ~gil_scoped_acquire_local() { PyGILState_Release(state); }
         const PyGILState_STATE state;
     } gil;
 #    endif
 #endif
     error_scope err_scope;
 
-    PYBIND11_STR_TYPE id(PYBIND11_INTERNALS_ID);
-    auto builtins = handle(PyEval_GetBuiltins());
-    if (builtins.contains(id) && isinstance<capsule>(builtins[id])) {
-        internals_pp = static_cast<internals **>(capsule(builtins[id]));
-
-        // We loaded builtins through python's builtins, which means that our `error_already_set`
+    dict state_dict = get_python_state_dict();
+    if (object internals_obj = get_internals_obj_from_state_dict(state_dict)) {
+        internals_pp = get_internals_pp_from_capsule(internals_obj);
+    }
+    if (internals_pp && *internals_pp) {
+        // We loaded the internals through `state_dict`, which means that our `error_already_set`
         // and `builtin_exception` may be different local classes than the ones set up in the
         // initial exception translator, below, so add another for our local exception classes.
         //
         // libstdc++ doesn't require this (types there are identified only by name)
         // libc++ with CPython doesn't require this (types are explicitly exported)
         // libc++ with PyPy still need it, awaiting further investigation
 #if !defined(__GLIBCXX__)
@@ -452,32 +506,31 @@
         if (!internals_pp) {
             internals_pp = new internals *();
         }
         auto *&internals_ptr = *internals_pp;
         internals_ptr = new internals();
 #if defined(WITH_THREAD)
 
-#    if PY_VERSION_HEX < 0x03090000
-        PyEval_InitThreads();
-#    endif
         PyThreadState *tstate = PyThreadState_Get();
+        // NOLINTNEXTLINE(bugprone-assignment-in-if-condition)
         if (!PYBIND11_TLS_KEY_CREATE(internals_ptr->tstate)) {
             pybind11_fail("get_internals: could not successfully initialize the tstate TSS key!");
         }
         PYBIND11_TLS_REPLACE_VALUE(internals_ptr->tstate, tstate);
 
 #    if PYBIND11_INTERNALS_VERSION > 4
+        // NOLINTNEXTLINE(bugprone-assignment-in-if-condition)
         if (!PYBIND11_TLS_KEY_CREATE(internals_ptr->loader_life_support_tls_key)) {
             pybind11_fail("get_internals: could not successfully initialize the "
                           "loader_life_support TSS key!");
         }
 #    endif
         internals_ptr->istate = tstate->interp;
 #endif
-        builtins[id] = capsule(internals_pp);
+        state_dict[PYBIND11_INTERNALS_ID] = capsule(internals_pp);
         internals_ptr->registered_exception_translators.push_front(&translate_exception);
         internals_ptr->static_property_type = make_static_property_type();
         internals_ptr->default_metaclass = make_default_metaclass();
         internals_ptr->instance_base = make_object_base_type(internals_ptr->default_metaclass);
     }
     return **internals_pp;
 }
@@ -501,14 +554,15 @@
     // plausible number).
     PYBIND11_TLS_KEY_INIT(loader_life_support_tls_key)
 
     // Holds the shared TLS key for the loader_life_support stack.
     struct shared_loader_life_support_data {
         PYBIND11_TLS_KEY_INIT(loader_life_support_tls_key)
         shared_loader_life_support_data() {
+            // NOLINTNEXTLINE(bugprone-assignment-in-if-condition)
             if (!PYBIND11_TLS_KEY_CREATE(loader_life_support_tls_key)) {
                 pybind11_fail("local_internals: could not successfully initialize the "
                               "loader_life_support TLS key!");
             }
         }
         // We can't help but leak the TLS key, because Python never unloads extension modules.
     };
@@ -544,14 +598,33 @@
 template <typename... Args>
 const char *c_str(Args &&...args) {
     auto &strings = get_internals().static_strings;
     strings.emplace_front(std::forward<Args>(args)...);
     return strings.front().c_str();
 }
 
+inline const char *get_function_record_capsule_name() {
+#if PYBIND11_INTERNALS_VERSION > 4
+    return get_internals().function_record_capsule_name.c_str();
+#else
+    return nullptr;
+#endif
+}
+
+// Determine whether or not the following capsule contains a pybind11 function record.
+// Note that we use `internals` to make sure that only ABI compatible records are touched.
+//
+// This check is currently used in two places:
+// - An important optimization in functional.h to avoid overhead in C++ -> Python -> C++
+// - The sibling feature of cpp_function to allow overloads
+inline bool is_function_record_capsule(const capsule &cap) {
+    // Pointer equality as we rely on internals() to ensure unique pointers
+    return cap.name() == get_function_record_capsule_name();
+}
+
 PYBIND11_NAMESPACE_END(detail)
 
 /// Returns a named pointer that is shared among all extension modules (using the same
 /// pybind11 version) running in the current interpreter. Names starting with underscores
 /// are reserved for internal usage. Returns `nullptr` if no matching entry was found.
 PYBIND11_NOINLINE void *get_shared_data(const std::string &name) {
     auto &internals = detail::get_internals();
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/detail/type_caster_base.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files 8% similar despite different names*

```diff
@@ -254,17 +254,17 @@
     instance *inst = nullptr;
     size_t index = 0u;
     const detail::type_info *type = nullptr;
     void **vh = nullptr;
 
     // Main constructor for a found value/holder:
     value_and_holder(instance *i, const detail::type_info *type, size_t vpos, size_t index)
-        : inst{i}, index{index}, type{type}, vh{inst->simple_layout
-                                                    ? inst->simple_value_holder
-                                                    : &inst->nonsimple.values_and_holders[vpos]} {}
+        : inst{i}, index{index}, type{type},
+          vh{inst->simple_layout ? inst->simple_value_holder
+                                 : &inst->nonsimple.values_and_holders[vpos]} {}
 
     // Default constructor (used to signal a value-and-holder not found by get_value_and_holder())
     value_and_holder() = default;
 
     // Used for past-the-end iterator
     explicit value_and_holder(size_t index) : index{index} {}
 
@@ -818,49 +818,207 @@
 using movable_cast_op_type
     = conditional_t<std::is_pointer<typename std::remove_reference<T>::type>::value,
                     typename std::add_pointer<intrinsic_t<T>>::type,
                     conditional_t<std::is_rvalue_reference<T>::value,
                                   typename std::add_rvalue_reference<intrinsic_t<T>>::type,
                                   typename std::add_lvalue_reference<intrinsic_t<T>>::type>>;
 
-// std::is_copy_constructible isn't quite enough: it lets std::vector<T> (and similar) through when
-// T is non-copyable, but code containing such a copy constructor fails to actually compile.
-template <typename T, typename SFINAE = void>
-struct is_copy_constructible : std::is_copy_constructible<T> {};
+// Does the container have a mapped type and is it recursive?
+// Implemented by specializations below.
+template <typename Container, typename SFINAE = void>
+struct container_mapped_type_traits {
+    static constexpr bool has_mapped_type = false;
+    static constexpr bool has_recursive_mapped_type = false;
+};
+
+template <typename Container>
+struct container_mapped_type_traits<
+    Container,
+    typename std::enable_if<
+        std::is_same<typename Container::mapped_type, Container>::value>::type> {
+    static constexpr bool has_mapped_type = true;
+    static constexpr bool has_recursive_mapped_type = true;
+};
+
+template <typename Container>
+struct container_mapped_type_traits<
+    Container,
+    typename std::enable_if<
+        negation<std::is_same<typename Container::mapped_type, Container>>::value>::type> {
+    static constexpr bool has_mapped_type = true;
+    static constexpr bool has_recursive_mapped_type = false;
+};
+
+// Does the container have a value type and is it recursive?
+// Implemented by specializations below.
+template <typename Container, typename SFINAE = void>
+struct container_value_type_traits : std::false_type {
+    static constexpr bool has_value_type = false;
+    static constexpr bool has_recursive_value_type = false;
+};
+
+template <typename Container>
+struct container_value_type_traits<
+    Container,
+    typename std::enable_if<
+        std::is_same<typename Container::value_type, Container>::value>::type> {
+    static constexpr bool has_value_type = true;
+    static constexpr bool has_recursive_value_type = true;
+};
 
-// Specialization for types that appear to be copy constructible but also look like stl containers
-// (we specifically check for: has `value_type` and `reference` with `reference = value_type&`): if
-// so, copy constructability depends on whether the value_type is copy constructible.
 template <typename Container>
-struct is_copy_constructible<
+struct container_value_type_traits<
     Container,
-    enable_if_t<
-        all_of<std::is_copy_constructible<Container>,
-               std::is_same<typename Container::value_type &, typename Container::reference>,
-               // Avoid infinite recursion
-               negation<std::is_same<Container, typename Container::value_type>>>::value>>
-    : is_copy_constructible<typename Container::value_type> {};
+    typename std::enable_if<
+        negation<std::is_same<typename Container::value_type, Container>>::value>::type> {
+    static constexpr bool has_value_type = true;
+    static constexpr bool has_recursive_value_type = false;
+};
+
+/*
+ * Tag to be used for representing the bottom of recursively defined types.
+ * Define this tag so we don't have to use void.
+ */
+struct recursive_bottom {};
+
+/*
+ * Implementation detail of `recursive_container_traits` below.
+ * `T` is the `value_type` of the container, which might need to be modified to
+ * avoid recursive types and const types.
+ */
+template <typename T, bool is_this_a_map>
+struct impl_type_to_check_recursively {
+    /*
+     * If the container is recursive, then no further recursion should be done.
+     */
+    using if_recursive = recursive_bottom;
+    /*
+     * Otherwise yield `T` unchanged.
+     */
+    using if_not_recursive = T;
+};
+
+/*
+ * For pairs - only as value type of a map -, the first type should remove the `const`.
+ * Also, if the map is recursive, then the recursive checking should consider
+ * the first type only.
+ */
+template <typename A, typename B>
+struct impl_type_to_check_recursively<std::pair<A, B>, /* is_this_a_map = */ true> {
+    using if_recursive = typename std::remove_const<A>::type;
+    using if_not_recursive = std::pair<typename std::remove_const<A>::type, B>;
+};
+
+/*
+ * Implementation of `recursive_container_traits` below.
+ */
+template <typename Container, typename SFINAE = void>
+struct impl_recursive_container_traits {
+    using type_to_check_recursively = recursive_bottom;
+};
+
+template <typename Container>
+struct impl_recursive_container_traits<
+    Container,
+    typename std::enable_if<container_value_type_traits<Container>::has_value_type>::type> {
+    static constexpr bool is_recursive
+        = container_mapped_type_traits<Container>::has_recursive_mapped_type
+          || container_value_type_traits<Container>::has_recursive_value_type;
+    /*
+     * This member dictates which type Pybind11 should check recursively in traits
+     * such as `is_move_constructible`, `is_copy_constructible`, `is_move_assignable`, ...
+     * Direct access to `value_type` should be avoided:
+     * 1. `value_type` might recursively contain the type again
+     * 2. `value_type` of STL map types is `std::pair<A const, B>`, the `const`
+     *    should be removed.
+     *
+     */
+    using type_to_check_recursively = typename std::conditional<
+        is_recursive,
+        typename impl_type_to_check_recursively<
+            typename Container::value_type,
+            container_mapped_type_traits<Container>::has_mapped_type>::if_recursive,
+        typename impl_type_to_check_recursively<
+            typename Container::value_type,
+            container_mapped_type_traits<Container>::has_mapped_type>::if_not_recursive>::type;
+};
+
+/*
+ * This trait defines the `type_to_check_recursively` which is needed to properly
+ * handle recursively defined traits such as `is_move_constructible` without going
+ * into an infinite recursion.
+ * Should be used instead of directly accessing the `value_type`.
+ * It cancels the recursion by returning the `recursive_bottom` tag.
+ *
+ * The default definition of `type_to_check_recursively` is as follows:
+ *
+ * 1. By default, it is `recursive_bottom`, so that the recursion is canceled.
+ * 2. If the type is non-recursive and defines a `value_type`, then the `value_type` is used.
+ *    If the `value_type` is a pair and a `mapped_type` is defined,
+ *    then the `const` is removed from the first type.
+ * 3. If the type is recursive and `value_type` is not a pair, then `recursive_bottom` is returned.
+ * 4. If the type is recursive and `value_type` is a pair and a `mapped_type` is defined,
+ *    then `const` is removed from the first type and the first type is returned.
+ *
+ * This behavior can be extended by the user as seen in test_stl_binders.cpp.
+ *
+ * This struct is exactly the same as impl_recursive_container_traits.
+ * The duplication achieves that user-defined specializations don't compete
+ * with internal specializations, but take precedence.
+ */
+template <typename Container, typename SFINAE = void>
+struct recursive_container_traits : impl_recursive_container_traits<Container> {};
+
+template <typename T>
+struct is_move_constructible
+    : all_of<std::is_move_constructible<T>,
+             is_move_constructible<
+                 typename recursive_container_traits<T>::type_to_check_recursively>> {};
+
+template <>
+struct is_move_constructible<recursive_bottom> : std::true_type {};
+
+// Likewise for std::pair
+// (after C++17 it is mandatory that the move constructor not exist when the two types aren't
+// themselves move constructible, but this can not be relied upon when T1 or T2 are themselves
+// containers).
+template <typename T1, typename T2>
+struct is_move_constructible<std::pair<T1, T2>>
+    : all_of<is_move_constructible<T1>, is_move_constructible<T2>> {};
+
+// std::is_copy_constructible isn't quite enough: it lets std::vector<T> (and similar) through when
+// T is non-copyable, but code containing such a copy constructor fails to actually compile.
+template <typename T>
+struct is_copy_constructible
+    : all_of<std::is_copy_constructible<T>,
+             is_copy_constructible<
+                 typename recursive_container_traits<T>::type_to_check_recursively>> {};
+
+template <>
+struct is_copy_constructible<recursive_bottom> : std::true_type {};
 
 // Likewise for std::pair
 // (after C++17 it is mandatory that the copy constructor not exist when the two types aren't
 // themselves copy constructible, but this can not be relied upon when T1 or T2 are themselves
 // containers).
 template <typename T1, typename T2>
 struct is_copy_constructible<std::pair<T1, T2>>
     : all_of<is_copy_constructible<T1>, is_copy_constructible<T2>> {};
 
 // The same problems arise with std::is_copy_assignable, so we use the same workaround.
-template <typename T, typename SFINAE = void>
-struct is_copy_assignable : std::is_copy_assignable<T> {};
-template <typename Container>
-struct is_copy_assignable<Container,
-                          enable_if_t<all_of<std::is_copy_assignable<Container>,
-                                             std::is_same<typename Container::value_type &,
-                                                          typename Container::reference>>::value>>
-    : is_copy_assignable<typename Container::value_type> {};
+template <typename T>
+struct is_copy_assignable
+    : all_of<
+          std::is_copy_assignable<T>,
+          is_copy_assignable<typename recursive_container_traits<T>::type_to_check_recursively>> {
+};
+
+template <>
+struct is_copy_assignable<recursive_bottom> : std::true_type {};
+
 template <typename T1, typename T2>
 struct is_copy_assignable<std::pair<T1, T2>>
     : all_of<is_copy_assignable<T1>, is_copy_assignable<T2>> {};
 
 PYBIND11_NAMESPACE_END(detail)
 
 // polymorphic_type_hook<itype>::get(src, tinfo) determines whether the object pointed
@@ -990,21 +1148,30 @@
        decltype argument to apply SFINAE to the public copy/move constructors.*/
     template <typename T, typename = enable_if_t<is_copy_constructible<T>::value>>
     static auto make_copy_constructor(const T *)
         -> decltype(new T(std::declval<const T>()), Constructor{}) {
         return [](const void *arg) -> void * { return new T(*reinterpret_cast<const T *>(arg)); };
     }
 
-    template <typename T, typename = enable_if_t<std::is_move_constructible<T>::value>>
+    template <typename T, typename = enable_if_t<is_move_constructible<T>::value>>
     static auto make_move_constructor(const T *)
         -> decltype(new T(std::declval<T &&>()), Constructor{}) {
         return [](const void *arg) -> void * {
             return new T(std::move(*const_cast<T *>(reinterpret_cast<const T *>(arg))));
         };
     }
 
     static Constructor make_copy_constructor(...) { return nullptr; }
     static Constructor make_move_constructor(...) { return nullptr; }
 };
 
+PYBIND11_NOINLINE std::string type_info_description(const std::type_info &ti) {
+    if (auto *type_data = get_type_info(ti)) {
+        handle th((PyObject *) type_data->type);
+        return th.attr("__module__").cast<std::string>() + '.'
+               + th.attr("__qualname__").cast<std::string>();
+    }
+    return clean_type_id(ti.name());
+}
+
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/detail/typeid.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/eigen.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/eigen/matrix.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,48 @@
 /*
-    pybind11/eigen.h: Transparent conversion for dense and sparse Eigen matrices
+    pybind11/eigen/matrix.h: Transparent conversion for dense and sparse Eigen matrices
 
     Copyright (c) 2016 Wenzel Jakob <wenzel.jakob@epfl.ch>
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
+#include "../numpy.h"
+#include "common.h"
+
 /* HINT: To suppress warnings originating from the Eigen headers, use -isystem.
    See also:
        https://stackoverflow.com/questions/2579576/i-dir-vs-isystem-dir
        https://stackoverflow.com/questions/1741816/isystem-for-ms-visual-studio-c-compiler
 */
-
-#include "numpy.h"
-
-// The C4127 suppression was introduced for Eigen 3.4.0. In theory we could
-// make it version specific, or even remove it later, but considering that
-// 1. C4127 is generally far more distracting than useful for modern template code, and
-// 2. we definitely want to ignore any MSVC warnings originating from Eigen code,
-//    it is probably best to keep this around indefinitely.
-#if defined(_MSC_VER)
-#    pragma warning(push)
-#    pragma warning(disable : 4127) // C4127: conditional expression is constant
-#    pragma warning(disable : 5054) // https://github.com/pybind/pybind11/pull/3741
+PYBIND11_WARNING_PUSH
+PYBIND11_WARNING_DISABLE_MSVC(5054) // https://github.com/pybind/pybind11/pull/3741
 //       C5054: operator '&': deprecated between enumerations of different types
-#elif defined(__MINGW32__)
-#    pragma GCC diagnostic push
-#    pragma GCC diagnostic ignored "-Wmaybe-uninitialized"
+#if defined(__MINGW32__)
+PYBIND11_WARNING_DISABLE_GCC("-Wmaybe-uninitialized")
 #endif
 
 #include <Eigen/Core>
 #include <Eigen/SparseCore>
 
-#if defined(_MSC_VER)
-#    pragma warning(pop)
-#elif defined(__MINGW32__)
-#    pragma GCC diagnostic pop
-#endif
+PYBIND11_WARNING_POP
 
 // Eigen prior to 3.2.7 doesn't have proper move constructors--but worse, some classes get implicit
 // move constructors that break things.  We could detect this an explicitly copy, but an extra copy
 // of matrices seems highly undesirable.
 static_assert(EIGEN_VERSION_AT_LEAST(3, 2, 7),
-              "Eigen support in pybind11 requires Eigen >= 3.2.7");
+              "Eigen matrix support in pybind11 requires Eigen >= 3.2.7");
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
+PYBIND11_WARNING_DISABLE_MSVC(4127)
+
 // Provide a convenience alias for easier pass-by-ref usage with fully dynamic strides:
 using EigenDStride = Eigen::Stride<Eigen::Dynamic, Eigen::Dynamic>;
 template <typename MatrixType>
 using EigenDRef = Eigen::Ref<MatrixType, 0, EigenDStride>;
 template <typename MatrixType>
 using EigenDMap = Eigen::Map<MatrixType, 0, EigenDStride>;
 
@@ -186,29 +176,28 @@
         }
 
         if (dims == 2) { // Matrix type: require exact match (or dynamic)
 
             EigenIndex np_rows = a.shape(0), np_cols = a.shape(1),
                        np_rstride = a.strides(0) / static_cast<ssize_t>(sizeof(Scalar)),
                        np_cstride = a.strides(1) / static_cast<ssize_t>(sizeof(Scalar));
-            if ((PYBIND11_SILENCE_MSVC_C4127(fixed_rows) && np_rows != rows)
-                || (PYBIND11_SILENCE_MSVC_C4127(fixed_cols) && np_cols != cols)) {
+            if ((fixed_rows && np_rows != rows) || (fixed_cols && np_cols != cols)) {
                 return false;
             }
 
             return {np_rows, np_cols, np_rstride, np_cstride};
         }
 
         // Otherwise we're storing an n-vector.  Only one of the strides will be used, but
         // whichever is used, we want the (single) numpy stride value.
         const EigenIndex n = a.shape(0),
                          stride = a.strides(0) / static_cast<ssize_t>(sizeof(Scalar));
 
         if (vector) { // Eigen type is a compile-time vector
-            if (PYBIND11_SILENCE_MSVC_C4127(fixed) && size != n) {
+            if (fixed && size != n) {
                 return false; // Vector size mismatch
             }
             return {rows == 1 ? 1 : n, cols == 1 ? 1 : n, stride};
         }
         if (fixed) {
             // The type has a fixed size, but is not a vector: abort
             return false;
@@ -217,15 +206,15 @@
             // Since this isn't a vector, cols must be != 1.  We allow this only if it exactly
             // equals the number of elements (rows is Dynamic, and so 1 row is allowed).
             if (cols != n) {
                 return false;
             }
             return {1, n, stride};
         } // Otherwise it's either fully dynamic, or column dynamic; both become a column vector
-        if (PYBIND11_SILENCE_MSVC_C4127(fixed_rows) && rows != n) {
+        if (fixed_rows && rows != n) {
             return false;
         }
         return {n, 1, stride};
     }
 
     static constexpr bool show_writeable
         = is_eigen_dense_map<Type>::value && is_eigen_mutable_map<Type>::value;
@@ -295,14 +284,16 @@
 }
 
 // Type caster for regular, dense matrix types (e.g. MatrixXd), but not maps/refs/etc. of dense
 // types.
 template <typename Type>
 struct type_caster<Type, enable_if_t<is_eigen_dense_plain<Type>::value>> {
     using Scalar = typename Type::Scalar;
+    static_assert(!std::is_pointer<Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using props = EigenProps<Type>;
 
     bool load(handle src, bool convert) {
         // If we're in no-convert mode, only load if given an array of the correct type
         if (!convert && !isinstance<array_t<Scalar>>(src)) {
             return false;
         }
@@ -413,14 +404,17 @@
 private:
     Type value;
 };
 
 // Base class for casting reference/map/block/etc. objects back to python.
 template <typename MapType>
 struct eigen_map_caster {
+    static_assert(!std::is_pointer<typename MapType::Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
+
 private:
     using props = EigenProps<MapType>;
 
 public:
     // Directly referencing a ref/map's data is a bit dangerous (whatever the map/ref points to has
     // to stay around), but we'll allow it under the assumption that you know what you're doing
     // (and have an appropriate keep_alive in place).  We return a numpy array pointing directly at
@@ -465,14 +459,16 @@
     Eigen::Ref<PlainObjectType, 0, StrideType>,
     enable_if_t<is_eigen_dense_map<Eigen::Ref<PlainObjectType, 0, StrideType>>::value>>
     : public eigen_map_caster<Eigen::Ref<PlainObjectType, 0, StrideType>> {
 private:
     using Type = Eigen::Ref<PlainObjectType, 0, StrideType>;
     using props = EigenProps<Type>;
     using Scalar = typename props::Scalar;
+    static_assert(!std::is_pointer<Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using MapType = Eigen::Map<PlainObjectType, 0, StrideType>;
     using Array
         = array_t<Scalar,
                   array::forcecast
                       | ((props::row_major ? props::inner_stride : props::outer_stride) == 1
                              ? array::c_style
                          : (props::row_major ? props::outer_stride : props::inner_stride) == 1
@@ -612,14 +608,17 @@
 
 // type_caster for special matrix types (e.g. DiagonalMatrix), which are EigenBase, but not
 // EigenDense (i.e. they don't have a data(), at least not with the usual matrix layout).
 // load() is not supported, but we can cast them into the python domain by first copying to a
 // regular Eigen::Matrix, then casting that.
 template <typename Type>
 struct type_caster<Type, enable_if_t<is_eigen_other<Type>::value>> {
+    static_assert(!std::is_pointer<typename Type::Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
+
 protected:
     using Matrix
         = Eigen::Matrix<typename Type::Scalar, Type::RowsAtCompileTime, Type::ColsAtCompileTime>;
     using props = EigenProps<Matrix>;
 
 public:
     static handle cast(const Type &src, return_value_policy /* policy */, handle /* parent */) {
@@ -640,14 +639,16 @@
     template <typename>
     using cast_op_type = Type;
 };
 
 template <typename Type>
 struct type_caster<Type, enable_if_t<is_eigen_sparse<Type>::value>> {
     using Scalar = typename Type::Scalar;
+    static_assert(!std::is_pointer<Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using StorageIndex = remove_reference_t<decltype(*std::declval<Type>().outerIndexPtr())>;
     using Index = typename Type::Index;
     static constexpr bool rowMajor = Type::IsRowMajor;
 
     bool load(handle src, bool) {
         if (!src) {
             return false;
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/embed.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/embed.h`

 * *Files 9% similar despite different names*

```diff
@@ -82,46 +82,34 @@
 };
 
 inline wchar_t *widen_chars(const char *safe_arg) {
     wchar_t *widened_arg = Py_DecodeLocale(safe_arg, nullptr);
     return widened_arg;
 }
 
-PYBIND11_NAMESPACE_END(detail)
-
-/** \rst
-    Initialize the Python interpreter. No other pybind11 or CPython API functions can be
-    called before this is done; with the exception of `PYBIND11_EMBEDDED_MODULE`. The
-    optional `init_signal_handlers` parameter can be used to skip the registration of
-    signal handlers (see the `Python documentation`_ for details). Calling this function
-    again after the interpreter has already been initialized is a fatal error.
-
-    If initializing the Python interpreter fails, then the program is terminated.  (This
-    is controlled by the CPython runtime and is an exception to pybind11's normal behavior
-    of throwing exceptions on errors.)
-
-    The remaining optional parameters, `argc`, `argv`, and `add_program_dir_to_path` are
-    used to populate ``sys.argv`` and ``sys.path``.
-    See the |PySys_SetArgvEx documentation|_ for details.
-
-    .. _Python documentation: https://docs.python.org/3/c-api/init.html#c.Py_InitializeEx
-    .. |PySys_SetArgvEx documentation| replace:: ``PySys_SetArgvEx`` documentation
-    .. _PySys_SetArgvEx documentation: https://docs.python.org/3/c-api/init.html#c.PySys_SetArgvEx
- \endrst */
-inline void initialize_interpreter(bool init_signal_handlers = true,
-                                   int argc = 0,
-                                   const char *const *argv = nullptr,
-                                   bool add_program_dir_to_path = true) {
+inline void precheck_interpreter() {
     if (Py_IsInitialized() != 0) {
         pybind11_fail("The interpreter is already running");
     }
+}
 
-#if PY_VERSION_HEX < 0x030B0000
+#if !defined(PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX)
+#    define PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX (0x03080000)
+#endif
 
+#if PY_VERSION_HEX < PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX
+inline void initialize_interpreter_pre_pyconfig(bool init_signal_handlers,
+                                                int argc,
+                                                const char *const *argv,
+                                                bool add_program_dir_to_path) {
+    detail::precheck_interpreter();
     Py_InitializeEx(init_signal_handlers ? 1 : 0);
+#    if defined(WITH_THREAD) && PY_VERSION_HEX < 0x03070000
+    PyEval_InitThreads();
+#    endif
 
     // Before it was special-cased in python 3.8, passing an empty or null argv
     // caused a segfault, so we have to reimplement the special case ourselves.
     bool special_case = (argv == nullptr || argc <= 0);
 
     const char *const empty_argv[]{"\0"};
     const char *const *safe_argv = special_case ? empty_argv : argv;
@@ -143,41 +131,83 @@
         }
         widened_argv[ii] = widened_argv_entries.back().get();
     }
 
     auto *pysys_argv = widened_argv.get();
 
     PySys_SetArgvEx(argc, pysys_argv, static_cast<int>(add_program_dir_to_path));
-#else
-    PyConfig config;
-    PyConfig_InitIsolatedConfig(&config);
-    config.isolated = 0;
-    config.use_environment = 1;
-    config.install_signal_handlers = init_signal_handlers ? 1 : 0;
+}
+#endif
 
-    PyStatus status = PyConfig_SetBytesArgv(&config, argc, const_cast<char *const *>(argv));
-    if (PyStatus_Exception(status)) {
+PYBIND11_NAMESPACE_END(detail)
+
+#if PY_VERSION_HEX >= PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX
+inline void initialize_interpreter(PyConfig *config,
+                                   int argc = 0,
+                                   const char *const *argv = nullptr,
+                                   bool add_program_dir_to_path = true) {
+    detail::precheck_interpreter();
+    PyStatus status = PyConfig_SetBytesArgv(config, argc, const_cast<char *const *>(argv));
+    if (PyStatus_Exception(status) != 0) {
         // A failure here indicates a character-encoding failure or the python
         // interpreter out of memory. Give up.
-        PyConfig_Clear(&config);
-        throw std::runtime_error(PyStatus_IsError(status) ? status.err_msg
-                                                          : "Failed to prepare CPython");
-    }
-    status = Py_InitializeFromConfig(&config);
-    PyConfig_Clear(&config);
-    if (PyStatus_Exception(status)) {
-        throw std::runtime_error(PyStatus_IsError(status) ? status.err_msg
-                                                          : "Failed to init CPython");
+        PyConfig_Clear(config);
+        throw std::runtime_error(PyStatus_IsError(status) != 0 ? status.err_msg
+                                                               : "Failed to prepare CPython");
+    }
+    status = Py_InitializeFromConfig(config);
+    if (PyStatus_Exception(status) != 0) {
+        PyConfig_Clear(config);
+        throw std::runtime_error(PyStatus_IsError(status) != 0 ? status.err_msg
+                                                               : "Failed to init CPython");
     }
     if (add_program_dir_to_path) {
         PyRun_SimpleString("import sys, os.path; "
                            "sys.path.insert(0, "
                            "os.path.abspath(os.path.dirname(sys.argv[0])) "
                            "if sys.argv and os.path.exists(sys.argv[0]) else '')");
     }
+    PyConfig_Clear(config);
+}
+#endif
+
+/** \rst
+    Initialize the Python interpreter. No other pybind11 or CPython API functions can be
+    called before this is done; with the exception of `PYBIND11_EMBEDDED_MODULE`. The
+    optional `init_signal_handlers` parameter can be used to skip the registration of
+    signal handlers (see the `Python documentation`_ for details). Calling this function
+    again after the interpreter has already been initialized is a fatal error.
+
+    If initializing the Python interpreter fails, then the program is terminated.  (This
+    is controlled by the CPython runtime and is an exception to pybind11's normal behavior
+    of throwing exceptions on errors.)
+
+    The remaining optional parameters, `argc`, `argv`, and `add_program_dir_to_path` are
+    used to populate ``sys.argv`` and ``sys.path``.
+    See the |PySys_SetArgvEx documentation|_ for details.
+
+    .. _Python documentation: https://docs.python.org/3/c-api/init.html#c.Py_InitializeEx
+    .. |PySys_SetArgvEx documentation| replace:: ``PySys_SetArgvEx`` documentation
+    .. _PySys_SetArgvEx documentation: https://docs.python.org/3/c-api/init.html#c.PySys_SetArgvEx
+ \endrst */
+inline void initialize_interpreter(bool init_signal_handlers = true,
+                                   int argc = 0,
+                                   const char *const *argv = nullptr,
+                                   bool add_program_dir_to_path = true) {
+#if PY_VERSION_HEX < PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX
+    detail::initialize_interpreter_pre_pyconfig(
+        init_signal_handlers, argc, argv, add_program_dir_to_path);
+#else
+    PyConfig config;
+    PyConfig_InitPythonConfig(&config);
+    // See PR #4473 for background
+    config.parse_argv = 0;
+
+    config.install_signal_handlers = init_signal_handlers ? 1 : 0;
+    initialize_interpreter(&config, argc, argv, add_program_dir_to_path);
 #endif
 }
 
 /** \rst
     Shut down the Python interpreter. No pybind11 or CPython API functions can be called
     after this. In addition, pybind11 objects must not outlive the interpreter:
 
@@ -209,24 +239,22 @@
         itself cannot completely unload binary extension modules and there are several
         caveats with regard to interpreter restarting. All the details can be found
         in the CPython documentation. In short, not all interpreter memory may be
         freed, either due to reference cycles or user-created global data.
 
  \endrst */
 inline void finalize_interpreter() {
-    handle builtins(PyEval_GetBuiltins());
-    const char *id = PYBIND11_INTERNALS_ID;
-
     // Get the internals pointer (without creating it if it doesn't exist).  It's possible for the
     // internals to be created during Py_Finalize() (e.g. if a py::capsule calls `get_internals()`
     // during destruction), so we get the pointer-pointer here and check it after Py_Finalize().
     detail::internals **internals_ptr_ptr = detail::get_internals_pp();
-    // It could also be stashed in builtins, so look there too:
-    if (builtins.contains(id) && isinstance<capsule>(builtins[id])) {
-        internals_ptr_ptr = capsule(builtins[id]);
+    // It could also be stashed in state_dict, so look there too:
+    if (object internals_obj
+        = get_internals_obj_from_state_dict(detail::get_python_state_dict())) {
+        internals_ptr_ptr = detail::get_internals_pp_from_capsule(internals_obj);
     }
     // Local internals contains data managed by the current interpreter, so we must clear them to
     // avoid undefined behaviors when initializing another interpreter
     detail::get_local_internals().registered_types_cpp.clear();
     detail::get_local_internals().registered_exception_translators.clear();
 
     Py_Finalize();
@@ -257,14 +285,23 @@
     explicit scoped_interpreter(bool init_signal_handlers = true,
                                 int argc = 0,
                                 const char *const *argv = nullptr,
                                 bool add_program_dir_to_path = true) {
         initialize_interpreter(init_signal_handlers, argc, argv, add_program_dir_to_path);
     }
 
+#if PY_VERSION_HEX >= PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX
+    explicit scoped_interpreter(PyConfig *config,
+                                int argc = 0,
+                                const char *const *argv = nullptr,
+                                bool add_program_dir_to_path = true) {
+        initialize_interpreter(config, argc, argv, add_program_dir_to_path);
+    }
+#endif
+
     scoped_interpreter(const scoped_interpreter &) = delete;
     scoped_interpreter(scoped_interpreter &&other) noexcept { other.is_valid = false; }
     scoped_interpreter &operator=(const scoped_interpreter &) = delete;
     scoped_interpreter &operator=(scoped_interpreter &&) = delete;
 
     ~scoped_interpreter() {
         if (is_valid) {
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/eval.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/functional.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/functional.h`

 * *Files 3% similar despite different names*

```diff
@@ -44,17 +44,24 @@
            a full C++ -> Python -> C++ roundtrip, which can be prohibitive.
            Here, we try to at least detect the case where the function is
            stateless (i.e. function pointer or lambda function without
            captured variables), in which case the roundtrip can be avoided.
          */
         if (auto cfunc = func.cpp_function()) {
             auto *cfunc_self = PyCFunction_GET_SELF(cfunc.ptr());
-            if (isinstance<capsule>(cfunc_self)) {
+            if (cfunc_self == nullptr) {
+                PyErr_Clear();
+            } else if (isinstance<capsule>(cfunc_self)) {
                 auto c = reinterpret_borrow<capsule>(cfunc_self);
-                auto *rec = (function_record *) c;
+
+                function_record *rec = nullptr;
+                // Check that we can safely reinterpret the capsule into a function_record
+                if (detail::is_function_record_capsule(c)) {
+                    rec = c.get_pointer<function_record>();
+                }
 
                 while (rec != nullptr) {
                     if (rec->is_stateless
                         && same_type(typeid(function_type),
                                      *reinterpret_cast<const std::type_info *>(rec->data[1]))) {
                         struct capture {
                             function_type f;
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/gil.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/gil.h`

 * *Files 4% similar despite different names*

```diff
@@ -148,16 +148,16 @@
             // Python >= 3.7 can remove this, it's an int before 3.7
             // NOLINTNEXTLINE(readability-qualified-auto)
             auto key = internals.tstate;
             PYBIND11_TLS_DELETE_VALUE(key);
         }
     }
 
-    gil_scoped_release(const gil_scoped_acquire &) = delete;
-    gil_scoped_release &operator=(const gil_scoped_acquire &) = delete;
+    gil_scoped_release(const gil_scoped_release &) = delete;
+    gil_scoped_release &operator=(const gil_scoped_release &) = delete;
 
     /// This method will disable the PyThreadState_DeleteCurrent call and the
     /// GIL won't be acquired. This method should be used if the interpreter
     /// could be shutting down when this is called, as thread deletion is not
     /// allowed during shutdown. Check _Py_IsFinalizing() on Python 3.7+, and
     /// protect subsequent code.
     PYBIND11_NOINLINE void disarm() { active = false; }
@@ -199,15 +199,15 @@
 
 class gil_scoped_release {
     PyThreadState *state;
 
 public:
     gil_scoped_release() : state{PyEval_SaveThread()} {}
     gil_scoped_release(const gil_scoped_release &) = delete;
-    gil_scoped_release &operator=(const gil_scoped_acquire &) = delete;
+    gil_scoped_release &operator=(const gil_scoped_release &) = delete;
     ~gil_scoped_release() { PyEval_RestoreThread(state); }
     void disarm() {}
 };
 
 #    endif // PYBIND11_SIMPLE_GIL_MANAGEMENT
 
 #else // WITH_THREAD
@@ -226,14 +226,14 @@
 class gil_scoped_release {
 public:
     gil_scoped_release() {
         // Trick to suppress `unused variable` error messages (at call sites).
         (void) (this != (this + 1));
     }
     gil_scoped_release(const gil_scoped_release &) = delete;
-    gil_scoped_release &operator=(const gil_scoped_acquire &) = delete;
+    gil_scoped_release &operator=(const gil_scoped_release &) = delete;
     void disarm() {}
 };
 
 #endif // WITH_THREAD
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/iostream.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/numpy.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/numpy.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
    upon the library user. */
 static_assert(sizeof(::pybind11::ssize_t) == sizeof(Py_intptr_t), "ssize_t != Py_intptr_t");
 static_assert(std::is_signed<Py_intptr_t>::value, "Py_intptr_t must be signed");
 // We now can reinterpret_cast between py::ssize_t and Py_intptr_t (MSVC + PyPy cares)
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
+PYBIND11_WARNING_DISABLE_MSVC(4127)
+
 class array; // Forward declaration
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <>
 struct handle_type_name<array> {
     static constexpr auto name = const_name("numpy.ndarray");
@@ -558,14 +560,16 @@
         args["names"] = std::move(names);
         args["formats"] = std::move(formats);
         args["offsets"] = std::move(offsets);
         args["itemsize"] = pybind11::int_(itemsize);
         m_ptr = from_args(args).release().ptr();
     }
 
+    /// Return dtype for the given typenum (one of the NPY_TYPES).
+    /// https://numpy.org/devdocs/reference/c-api/array.html#c.PyArray_DescrFromType
     explicit dtype(int typenum)
         : object(detail::npy_api::get().PyArray_DescrFromType_(typenum), stolen_t{}) {
         if (m_ptr == nullptr) {
             throw error_already_set();
         }
     }
 
@@ -871,15 +875,15 @@
      * Returns a proxy object that provides access to the array's data without bounds or
      * dimensionality checking.  Will throw if the array is missing the `writeable` flag.  Use with
      * care: the array must not be destroyed or reshaped for the duration of the returned object,
      * and the caller must take care not to access invalid dimensions or dimension indices.
      */
     template <typename T, ssize_t Dims = -1>
     detail::unchecked_mutable_reference<T, Dims> mutable_unchecked() & {
-        if (PYBIND11_SILENCE_MSVC_C4127(Dims >= 0) && ndim() != Dims) {
+        if (Dims >= 0 && ndim() != Dims) {
             throw std::domain_error("array has incorrect number of dimensions: "
                                     + std::to_string(ndim()) + "; expected "
                                     + std::to_string(Dims));
         }
         return detail::unchecked_mutable_reference<T, Dims>(
             mutable_data(), shape(), strides(), ndim());
     }
@@ -889,15 +893,15 @@
      * dimensionality checking.  Unlike `mutable_unchecked()`, this does not require that the
      * underlying array have the `writable` flag.  Use with care: the array must not be destroyed
      * or reshaped for the duration of the returned object, and the caller must take care not to
      * access invalid dimensions or dimension indices.
      */
     template <typename T, ssize_t Dims = -1>
     detail::unchecked_reference<T, Dims> unchecked() const & {
-        if (PYBIND11_SILENCE_MSVC_C4127(Dims >= 0) && ndim() != Dims) {
+        if (Dims >= 0 && ndim() != Dims) {
             throw std::domain_error("array has incorrect number of dimensions: "
                                     + std::to_string(ndim()) + "; expected "
                                     + std::to_string(Dims));
         }
         return detail::unchecked_reference<T, Dims>(data(), shape(), strides(), ndim());
     }
 
@@ -1115,18 +1119,18 @@
     template <ssize_t Dims = -1>
     detail::unchecked_mutable_reference<T, Dims> mutable_unchecked() & {
         return array::mutable_unchecked<T, Dims>();
     }
 
     /**
      * Returns a proxy object that provides const access to the array's data without bounds or
-     * dimensionality checking.  Unlike `unchecked()`, this does not require that the underlying
-     * array have the `writable` flag.  Use with care: the array must not be destroyed or reshaped
-     * for the duration of the returned object, and the caller must take care not to access invalid
-     * dimensions or dimension indices.
+     * dimensionality checking.  Unlike `mutable_unchecked()`, this does not require that the
+     * underlying array have the `writable` flag.  Use with care: the array must not be destroyed
+     * or reshaped for the duration of the returned object, and the caller must take care not to
+     * access invalid dimensions or dimension indices.
      */
     template <ssize_t Dims = -1>
     detail::unchecked_reference<T, Dims> unchecked() const & {
         return array::unchecked<T, Dims>();
     }
 
     /// Ensure that the argument is a NumPy array of the correct dtype (and if not, try to convert
@@ -1277,20 +1281,24 @@
                                              npy_api::NPY_CFLOAT_,
                                              npy_api::NPY_CDOUBLE_,
                                              npy_api::NPY_CLONGDOUBLE_};
 
 public:
     static constexpr int value = values[detail::is_fmt_numeric<T>::index];
 
-    static pybind11::dtype dtype() {
-        if (auto *ptr = npy_api::get().PyArray_DescrFromType_(value)) {
-            return reinterpret_steal<pybind11::dtype>(ptr);
-        }
-        pybind11_fail("Unsupported buffer format!");
-    }
+    static pybind11::dtype dtype() { return pybind11::dtype(/*typenum*/ value); }
+};
+
+template <typename T>
+struct npy_format_descriptor<T, enable_if_t<is_same_ignoring_cvref<T, PyObject *>::value>> {
+    static constexpr auto name = const_name("object");
+
+    static constexpr int value = npy_api::NPY_OBJECT_;
+
+    static pybind11::dtype dtype() { return pybind11::dtype(/*typenum*/ value); }
 };
 
 #define PYBIND11_DECL_CHAR_FMT                                                                    \
     static constexpr auto name = const_name("S") + const_name<N>();                               \
     static pybind11::dtype dtype() {                                                              \
         return pybind11::dtype(std::string("S") + std::to_string(N));                             \
     }
@@ -1465,15 +1473,15 @@
             Name, offsetof(T, Field), sizeof(decltype(std::declval<T>().Field)),                  \
                 ::pybind11::format_descriptor<decltype(std::declval<T>().Field)>::format(),       \
                 ::pybind11::detail::npy_format_descriptor<                                        \
                     decltype(std::declval<T>().Field)>::dtype()                                   \
         }
 
 // Extract name, offset and format descriptor for a struct field
-#    define PYBIND11_FIELD_DESCRIPTOR(T, Field) PYBIND11_FIELD_DESCRIPTOR_EX(T, Field, #    Field)
+#    define PYBIND11_FIELD_DESCRIPTOR(T, Field) PYBIND11_FIELD_DESCRIPTOR_EX(T, Field, #Field)
 
 // The main idea of this macro is borrowed from https://github.com/swansontec/map-macro
 // (C) William Swanson, Paul Fultz
 #    define PYBIND11_EVAL0(...) __VA_ARGS__
 #    define PYBIND11_EVAL1(...) PYBIND11_EVAL0(PYBIND11_EVAL0(PYBIND11_EVAL0(__VA_ARGS__)))
 #    define PYBIND11_EVAL2(...) PYBIND11_EVAL1(PYBIND11_EVAL1(PYBIND11_EVAL1(__VA_ARGS__)))
 #    define PYBIND11_EVAL3(...) PYBIND11_EVAL2(PYBIND11_EVAL2(PYBIND11_EVAL2(__VA_ARGS__)))
@@ -1861,17 +1869,18 @@
         if (size == 1 && ndim == 0) {
             PYBIND11_EXPAND_SIDE_EFFECTS(params[VIndex] = buffers[BIndex].ptr);
             return cast(
                 returned_array::call(f, *reinterpret_cast<param_n_t<Index> *>(params[Index])...));
         }
 
         auto result = returned_array::create(trivial, shape);
+
+        PYBIND11_WARNING_PUSH
 #ifdef PYBIND11_DETECTED_CLANG_WITH_MISLEADING_CALL_STD_MOVE_EXPLICITLY_WARNING
-#    pragma clang diagnostic push
-#    pragma clang diagnostic ignored "-Wreturn-std-move"
+        PYBIND11_WARNING_DISABLE_CLANG("-Wreturn-std-move")
 #endif
 
         if (size == 0) {
             return result;
         }
 
         /* Call the function */
@@ -1879,17 +1888,15 @@
         if (trivial == broadcast_trivial::non_trivial) {
             apply_broadcast(buffers, params, mutable_data, size, shape, i_seq, vi_seq, bi_seq);
         } else {
             apply_trivial(buffers, params, mutable_data, size, i_seq, vi_seq, bi_seq);
         }
 
         return result;
-#ifdef PYBIND11_DETECTED_CLANG_WITH_MISLEADING_CALL_STD_MOVE_EXPLICITLY_WARNING
-#    pragma clang diagnostic pop
-#endif
+        PYBIND11_WARNING_POP
     }
 
     template <size_t... Index, size_t... VIndex, size_t... BIndex>
     void apply_trivial(std::array<buffer_info, NVectorized> &buffers,
                        std::array<void *, N> &params,
                        Return *out,
                        size_t size,
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/operators.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/pybind11.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/pybind11.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,27 +31,28 @@
 #    define PYBIND11_STD_LAUNDER
 #    define PYBIND11_HAS_STD_LAUNDER 0
 #endif
 #if defined(__GNUG__) && !defined(__clang__)
 #    include <cxxabi.h>
 #endif
 
+PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
+
 /* https://stackoverflow.com/questions/46798456/handling-gccs-noexcept-type-warning
    This warning is about ABI compatibility, not code health.
    It is only actually needed in a couple places, but apparently GCC 7 "generates this warning if
    and only if the first template instantiation ... involves noexcept" [stackoverflow], therefore
    it could get triggered from seemingly random places, depending on user code.
    No other GCC version generates this warning.
  */
 #if defined(__GNUC__) && __GNUC__ == 7
-#    pragma GCC diagnostic push
-#    pragma GCC diagnostic ignored "-Wnoexcept-type"
+PYBIND11_WARNING_DISABLE_GCC("-Wnoexcept-type")
 #endif
 
-PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
+PYBIND11_WARNING_DISABLE_MSVC(4127)
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 // Apply all the extensions translators from a list
 // Return true if one of the translators completed without raising an exception
 // itself. Return of false indicates that if there are other translators
 // available, they should be tried.
@@ -79,14 +80,15 @@
 
 /// Wraps an arbitrary C++ function/method/lambda function/.. into a callable Python object
 class cpp_function : public function {
 public:
     cpp_function() = default;
     // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(std::nullptr_t) {}
+    cpp_function(std::nullptr_t, const is_setter &) {}
 
     /// Construct a cpp_function from a vanilla function pointer
     template <typename Return, typename... Args, typename... Extra>
     // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(Return (*f)(Args...), const Extra &...extra) {
         initialize(f, f, extra...);
     }
@@ -173,42 +175,40 @@
         /* Store the function including any extra state it might have (e.g. a lambda capture
          * object) */
         // The unique_ptr makes sure nothing is leaked in case of an exception.
         auto unique_rec = make_function_record();
         auto *rec = unique_rec.get();
 
         /* Store the capture object directly in the function record if there is enough space */
-        if (PYBIND11_SILENCE_MSVC_C4127(sizeof(capture) <= sizeof(rec->data))) {
+        if (sizeof(capture) <= sizeof(rec->data)) {
             /* Without these pragmas, GCC warns that there might not be
                enough space to use the placement new operator. However, the
                'if' statement above ensures that this is the case. */
-#if defined(__GNUG__) && __GNUC__ >= 6 && !defined(__clang__) && !defined(__INTEL_COMPILER)
-#    pragma GCC diagnostic push
-#    pragma GCC diagnostic ignored "-Wplacement-new"
+            PYBIND11_WARNING_PUSH
+
+#if defined(__GNUG__) && __GNUC__ >= 6
+            PYBIND11_WARNING_DISABLE_GCC("-Wplacement-new")
 #endif
+
             new ((capture *) &rec->data) capture{std::forward<Func>(f)};
-#if defined(__GNUG__) && __GNUC__ >= 6 && !defined(__clang__) && !defined(__INTEL_COMPILER)
-#    pragma GCC diagnostic pop
-#endif
-#if defined(__GNUG__) && !PYBIND11_HAS_STD_LAUNDER && !defined(__INTEL_COMPILER)
-#    pragma GCC diagnostic push
-#    pragma GCC diagnostic ignored "-Wstrict-aliasing"
+
+#if !PYBIND11_HAS_STD_LAUNDER
+            PYBIND11_WARNING_DISABLE_GCC("-Wstrict-aliasing")
 #endif
+
             // UB without std::launder, but without breaking ABI and/or
             // a significant refactoring it's "impossible" to solve.
             if (!std::is_trivially_destructible<capture>::value) {
                 rec->free_data = [](function_record *r) {
                     auto data = PYBIND11_STD_LAUNDER((capture *) &r->data);
                     (void) data;
                     data->~capture();
                 };
             }
-#if defined(__GNUG__) && !PYBIND11_HAS_STD_LAUNDER && !defined(__INTEL_COMPILER)
-#    pragma GCC diagnostic pop
-#endif
+            PYBIND11_WARNING_POP
         } else {
             rec->data[0] = new capture{std::forward<Func>(f)};
             rec->free_data = [](function_record *r) { delete ((capture *) r->data[0]); };
         }
 
         /* Type casters for the function arguments and return value */
         using cast_in = argument_loader<Args...>;
@@ -241,18 +241,24 @@
             return_value_policy policy
                 = return_value_policy_override<Return>::policy(call.func.policy);
 
             /* Function scope guard -- defaults to the compile-to-nothing `void_type` */
             using Guard = extract_guard_t<Extra...>;
 
             /* Perform the function call */
-            handle result
-                = cast_out::cast(std::move(args_converter).template call<Return, Guard>(cap->f),
-                                 policy,
-                                 call.parent);
+            handle result;
+            if (call.func.is_setter) {
+                (void) std::move(args_converter).template call<Return, Guard>(cap->f);
+                result = none().release();
+            } else {
+                result = cast_out::cast(
+                    std::move(args_converter).template call<Return, Guard>(cap->f),
+                    policy,
+                    call.parent);
+            }
 
             /* Invoke call policy post-call hook */
             process_attributes<Extra...>::postcall(call, result);
 
             return result;
         };
 
@@ -464,21 +470,28 @@
             rec->sibling = PYBIND11_INSTANCE_METHOD_GET_FUNCTION(rec->sibling.ptr());
         }
 
         detail::function_record *chain = nullptr, *chain_start = rec;
         if (rec->sibling) {
             if (PyCFunction_Check(rec->sibling.ptr())) {
                 auto *self = PyCFunction_GET_SELF(rec->sibling.ptr());
-                capsule rec_capsule = isinstance<capsule>(self) ? reinterpret_borrow<capsule>(self)
-                                                                : capsule(self);
-                chain = (detail::function_record *) rec_capsule;
-                /* Never append a method to an overload chain of a parent class;
-                   instead, hide the parent's overloads in this case */
-                if (!chain->scope.is(rec->scope)) {
+                if (!isinstance<capsule>(self)) {
                     chain = nullptr;
+                } else {
+                    auto rec_capsule = reinterpret_borrow<capsule>(self);
+                    if (detail::is_function_record_capsule(rec_capsule)) {
+                        chain = rec_capsule.get_pointer<detail::function_record>();
+                        /* Never append a method to an overload chain of a parent class;
+                           instead, hide the parent's overloads in this case */
+                        if (!chain->scope.is(rec->scope)) {
+                            chain = nullptr;
+                        }
+                    } else {
+                        chain = nullptr;
+                    }
                 }
             }
             // Don't trigger for things like the default __init__, which are wrapper_descriptors
             // that we are intentionally replacing
             else if (!rec->sibling.is_none() && rec->name[0] != '_') {
                 pybind11_fail("Cannot overload existing non-function object \""
                               + std::string(rec->name) + "\" with a function of the same name");
@@ -491,14 +504,15 @@
             std::memset(rec->def, 0, sizeof(PyMethodDef));
             rec->def->ml_name = rec->name;
             rec->def->ml_meth
                 = reinterpret_cast<PyCFunction>(reinterpret_cast<void (*)()>(dispatcher));
             rec->def->ml_flags = METH_VARARGS | METH_KEYWORDS;
 
             capsule rec_capsule(unique_rec.release(),
+                                detail::get_function_record_capsule_name(),
                                 [](void *ptr) { destruct((detail::function_record *) ptr); });
             guarded_strdup.release();
 
             object scope_module;
             if (rec->scope) {
                 if (hasattr(rec->scope, "__module__")) {
                     scope_module = rec->scope.attr("__module__");
@@ -657,18 +671,21 @@
             rec = next;
         }
     }
 
     /// Main dispatch logic for calls to functions bound using pybind11
     static PyObject *dispatcher(PyObject *self, PyObject *args_in, PyObject *kwargs_in) {
         using namespace detail;
+        assert(isinstance<capsule>(self));
 
         /* Iterator over the list of potentially admissible overloads */
-        const function_record *overloads = (function_record *) PyCapsule_GetPointer(self, nullptr),
+        const function_record *overloads = reinterpret_cast<function_record *>(
+                                  PyCapsule_GetPointer(self, get_function_record_capsule_name())),
                               *it = overloads;
+        assert(overloads != nullptr);
 
         /* Need to know how many arguments + keyword arguments there are to pick the right
            overload */
         const auto n_args_in = (size_t) PyTuple_GET_SIZE(args_in);
 
         handle parent = n_args_in > 0 ? PyTuple_GET_ITEM(args_in, 0) : nullptr,
                result = PYBIND11_TRY_NEXT_OVERLOAD;
@@ -1412,17 +1429,17 @@
     void_t<decltype(static_cast<void (*)(void *, size_t)>(T::operator delete))>> : std::true_type {
 };
 /// Call class-specific delete if it exists or global otherwise. Can also be an overload set.
 template <typename T, enable_if_t<has_operator_delete<T>::value, int> = 0>
 void call_operator_delete(T *p, size_t, size_t) {
     T::operator delete(p);
 }
-template <
-    typename T,
-    enable_if_t<!has_operator_delete<T>::value && has_operator_delete_size<T>::value, int> = 0>
+template <typename T,
+          enable_if_t<!has_operator_delete<T>::value && has_operator_delete_size<T>::value, int>
+          = 0>
 void call_operator_delete(T *p, size_t s, size_t) {
     T::operator delete(p, s);
 }
 
 inline void call_operator_delete(void *p, size_t s, size_t a) {
     (void) s;
     (void) a;
@@ -1715,15 +1732,16 @@
         return def_property_static(name, fget, nullptr, extra...);
     }
 
     /// Uses return_value_policy::reference_internal by default
     template <typename Getter, typename Setter, typename... Extra>
     class_ &
     def_property(const char *name, const Getter &fget, const Setter &fset, const Extra &...extra) {
-        return def_property(name, fget, cpp_function(method_adaptor<type>(fset)), extra...);
+        return def_property(
+            name, fget, cpp_function(method_adaptor<type>(fset), is_setter()), extra...);
     }
     template <typename Getter, typename... Extra>
     class_ &def_property(const char *name,
                          const Getter &fget,
                          const cpp_function &fset,
                          const Extra &...extra) {
         return def_property(name,
@@ -1826,16 +1844,15 @@
     static void init_holder(detail::instance *inst,
                             detail::value_and_holder &v_h,
                             const holder_type *holder_ptr,
                             const void * /* dummy -- not enable_shared_from_this<T>) */) {
         if (holder_ptr) {
             init_holder_from_existing(v_h, holder_ptr, std::is_copy_constructible<holder_type>());
             v_h.set_holder_constructed();
-        } else if (PYBIND11_SILENCE_MSVC_C4127(detail::always_construct_holder<holder_type>::value)
-                   || inst->owned) {
+        } else if (detail::always_construct_holder<holder_type>::value || inst->owned) {
             new (std::addressof(v_h.holder<holder_type>())) holder_type(v_h.value_ptr<type>());
             v_h.set_holder_constructed();
         }
     }
 
     /// Performs instance initialization including constructing a holder and registering the known
     /// instance.  Should be called as soon as the `type` value_ptr is set for an instance.  Takes
@@ -1867,17 +1884,30 @@
                 v_h.value_ptr<type>(), v_h.type->type_size, v_h.type->type_align);
         }
         v_h.value_ptr() = nullptr;
     }
 
     static detail::function_record *get_function_record(handle h) {
         h = detail::get_function(h);
-        return h ? (detail::function_record *) reinterpret_borrow<capsule>(
-                   PyCFunction_GET_SELF(h.ptr()))
-                 : nullptr;
+        if (!h) {
+            return nullptr;
+        }
+
+        handle func_self = PyCFunction_GET_SELF(h.ptr());
+        if (!func_self) {
+            throw error_already_set();
+        }
+        if (!isinstance<capsule>(func_self)) {
+            return nullptr;
+        }
+        auto cap = reinterpret_borrow<capsule>(func_self);
+        if (!detail::is_function_record_capsule(cap)) {
+            return nullptr;
+        }
+        return cap.get_pointer<detail::function_record>();
     }
 };
 
 /// Binds an existing constructor taking arguments Args...
 template <typename... Args>
 detail::initimpl::constructor<Args...> init() {
     return {};
@@ -1946,37 +1976,43 @@
             [](handle arg) -> str {
                 object type_name = type::handle_of(arg).attr("__name__");
                 return pybind11::str("{}.{}").format(std::move(type_name), enum_name(arg));
             },
             name("name"),
             is_method(m_base));
 
-        m_base.attr("__doc__") = static_property(
-            cpp_function(
-                [](handle arg) -> std::string {
-                    std::string docstring;
-                    dict entries = arg.attr("__entries");
-                    if (((PyTypeObject *) arg.ptr())->tp_doc) {
-                        docstring += std::string(((PyTypeObject *) arg.ptr())->tp_doc) + "\n\n";
-                    }
-                    docstring += "Members:";
-                    for (auto kv : entries) {
-                        auto key = std::string(pybind11::str(kv.first));
-                        auto comment = kv.second[int_(1)];
-                        docstring += "\n\n  " + key;
-                        if (!comment.is_none()) {
-                            docstring += " : " + (std::string) pybind11::str(comment);
+        if (options::show_enum_members_docstring()) {
+            m_base.attr("__doc__") = static_property(
+                cpp_function(
+                    [](handle arg) -> std::string {
+                        std::string docstring;
+                        dict entries = arg.attr("__entries");
+                        if (((PyTypeObject *) arg.ptr())->tp_doc) {
+                            docstring += std::string(
+                                reinterpret_cast<PyTypeObject *>(arg.ptr())->tp_doc);
+                            docstring += "\n\n";
                         }
-                    }
-                    return docstring;
-                },
-                name("__doc__")),
-            none(),
-            none(),
-            "");
+                        docstring += "Members:";
+                        for (auto kv : entries) {
+                            auto key = std::string(pybind11::str(kv.first));
+                            auto comment = kv.second[int_(1)];
+                            docstring += "\n\n  ";
+                            docstring += key;
+                            if (!comment.is_none()) {
+                                docstring += " : ";
+                                docstring += pybind11::str(comment).cast<std::string>();
+                            }
+                        }
+                        return docstring;
+                    },
+                    name("__doc__")),
+                none(),
+                none(),
+                "");
+        }
 
         m_base.attr("__members__") = static_property(cpp_function(
                                                          [](handle arg) -> dict {
                                                              dict entries = arg.attr("__entries"),
                                                                   m;
                                                              for (auto kv : entries) {
                                                                  m[kv.first] = kv.second[int_(0)];
@@ -2848,11 +2884,7 @@
         PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), name, fn, __VA_ARGS__);
 #define PYBIND11_OVERLOAD(ret_type, cname, fn, ...)                                               \
     PYBIND11_OVERRIDE(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), fn, __VA_ARGS__)
 #define PYBIND11_OVERLOAD_PURE(ret_type, cname, fn, ...)                                          \
     PYBIND11_OVERRIDE_PURE(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), fn, __VA_ARGS__);
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
-
-#if defined(__GNUC__) && __GNUC__ == 7
-#    pragma GCC diagnostic pop // -Wnoexcept-type
-#endif
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/pytypes.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/pytypes.h`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 #ifdef PYBIND11_HAS_STRING_VIEW
 #    include <string_view>
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
+PYBIND11_WARNING_DISABLE_MSVC(4127)
+
 /* A few forward declarations */
 class handle;
 class object;
 class str;
 class iterator;
 class type;
 struct arg;
@@ -226,15 +228,16 @@
 
     /// Enable implicit conversion through ``T::operator PyObject *()``.
     template <
         typename T,
         detail::enable_if_t<detail::all_of<detail::none_of<std::is_base_of<handle, T>,
                                                            detail::is_pyobj_ptr_or_nullptr_t<T>>,
                                            std::is_convertible<T, PyObject *>>::value,
-                            int> = 0>
+                            int>
+        = 0>
     // NOLINTNEXTLINE(google-explicit-constructor)
     handle(T &obj) : m_ptr(obj) {}
 
     /// Return the underlying ``PyObject *`` pointer
     PyObject *ptr() const { return m_ptr; }
     PyObject *&ptr() { return m_ptr; }
 
@@ -243,24 +246,34 @@
         preferable to use the `object` class which derives from `handle` and calls
         this function automatically. Returns a reference to itself.
     \endrst */
     const handle &inc_ref() const & {
 #ifdef PYBIND11_HANDLE_REF_DEBUG
         inc_ref_counter(1);
 #endif
+#ifdef PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
+        if (m_ptr != nullptr && !PyGILState_Check()) {
+            throw_gilstate_error("pybind11::handle::inc_ref()");
+        }
+#endif
         Py_XINCREF(m_ptr);
         return *this;
     }
 
     /** \rst
         Manually decrease the reference count of the Python object. Usually, it is
         preferable to use the `object` class which derives from `handle` and calls
         this function automatically. Returns a reference to itself.
     \endrst */
     const handle &dec_ref() const & {
+#ifdef PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
+        if (m_ptr != nullptr && !PyGILState_Check()) {
+            throw_gilstate_error("pybind11::handle::dec_ref()");
+        }
+#endif
         Py_XDECREF(m_ptr);
         return *this;
     }
 
     /** \rst
         Attempt to cast the Python object into the given C++ type. A `cast_error`
         will be throw upon failure.
@@ -279,16 +292,41 @@
     bool operator!=(const handle &h) const { return m_ptr != h.m_ptr; }
     PYBIND11_DEPRECATED("Use handle::operator bool() instead")
     bool check() const { return m_ptr != nullptr; }
 
 protected:
     PyObject *m_ptr = nullptr;
 
-#ifdef PYBIND11_HANDLE_REF_DEBUG
 private:
+#ifdef PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
+    void throw_gilstate_error(const std::string &function_name) const {
+        fprintf(
+            stderr,
+            "%s is being called while the GIL is either not held or invalid. Please see "
+            "https://pybind11.readthedocs.io/en/stable/advanced/"
+            "misc.html#common-sources-of-global-interpreter-lock-errors for debugging advice.\n"
+            "If you are convinced there is no bug in your code, you can #define "
+            "PYBIND11_NO_ASSERT_GIL_HELD_INCREF_DECREF"
+            "to disable this check. In that case you have to ensure this #define is consistently "
+            "used for all translation units linked into a given pybind11 extension, otherwise "
+            "there will be ODR violations.",
+            function_name.c_str());
+        fflush(stderr);
+        if (Py_TYPE(m_ptr)->tp_name != nullptr) {
+            fprintf(stderr,
+                    "The failing %s call was triggered on a %s object.\n",
+                    function_name.c_str(),
+                    Py_TYPE(m_ptr)->tp_name);
+            fflush(stderr);
+        }
+        throw std::runtime_error(function_name + " PyGILState_Check() failure.");
+    }
+#endif
+
+#ifdef PYBIND11_HANDLE_REF_DEBUG
     static std::size_t inc_ref_counter(std::size_t add) {
         thread_local std::size_t counter = 0;
         counter += add;
         return counter;
     }
 
 public:
@@ -426,74 +464,94 @@
     return {h, object::stolen_t{}};
 }
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 // Equivalent to obj.__class__.__name__ (or obj.__name__ if obj is a class).
 inline const char *obj_class_name(PyObject *obj) {
-    if (Py_TYPE(obj) == &PyType_Type) {
+    if (PyType_Check(obj)) {
         return reinterpret_cast<PyTypeObject *>(obj)->tp_name;
     }
     return Py_TYPE(obj)->tp_name;
 }
 
 std::string error_string();
 
+// The code in this struct is very unusual, to minimize the chances of
+// masking bugs (elsewhere) by errors during the error handling (here).
+// This is meant to be a lifeline for troubleshooting long-running processes
+// that crash under conditions that are virtually impossible to reproduce.
+// Low-level implementation alternatives are preferred to higher-level ones
+// that might raise cascading exceptions. Last-ditch-kind-of attempts are made
+// to report as much of the original error as possible, even if there are
+// secondary issues obtaining some of the details.
 struct error_fetch_and_normalize {
-    // Immediate normalization is long-established behavior (starting with
-    // https://github.com/pybind/pybind11/commit/135ba8deafb8bf64a15b24d1513899eb600e2011
-    // from Sep 2016) and safest. Normalization could be deferred, but this could mask
-    // errors elsewhere, the performance gain is very minor in typical situations
-    // (usually the dominant bottleneck is EH unwinding), and the implementation here
-    // would be more complex.
+    // This comment only applies to Python <= 3.11:
+    //     Immediate normalization is long-established behavior (starting with
+    //     https://github.com/pybind/pybind11/commit/135ba8deafb8bf64a15b24d1513899eb600e2011
+    //     from Sep 2016) and safest. Normalization could be deferred, but this could mask
+    //     errors elsewhere, the performance gain is very minor in typical situations
+    //     (usually the dominant bottleneck is EH unwinding), and the implementation here
+    //     would be more complex.
+    // Starting with Python 3.12, PyErr_Fetch() normalizes exceptions immediately.
+    // Any errors during normalization are tracked under __notes__.
     explicit error_fetch_and_normalize(const char *called) {
         PyErr_Fetch(&m_type.ptr(), &m_value.ptr(), &m_trace.ptr());
         if (!m_type) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " called while "
                             "Python error indicator not set.");
         }
         const char *exc_type_name_orig = detail::obj_class_name(m_type.ptr());
         if (exc_type_name_orig == nullptr) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " failed to obtain the name "
                             "of the original active exception type.");
         }
         m_lazy_error_string = exc_type_name_orig;
+#if PY_VERSION_HEX >= 0x030C0000
+        // The presence of __notes__ is likely due to exception normalization
+        // errors, although that is not necessarily true, therefore insert a
+        // hint only:
+        if (PyObject_HasAttrString(m_value.ptr(), "__notes__")) {
+            m_lazy_error_string += "[WITH __notes__]";
+        }
+#else
         // PyErr_NormalizeException() may change the exception type if there are cascading
         // failures. This can potentially be extremely confusing.
         PyErr_NormalizeException(&m_type.ptr(), &m_value.ptr(), &m_trace.ptr());
         if (m_type.ptr() == nullptr) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " failed to normalize the "
                             "active exception.");
         }
         const char *exc_type_name_norm = detail::obj_class_name(m_type.ptr());
-        if (exc_type_name_orig == nullptr) {
+        if (exc_type_name_norm == nullptr) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " failed to obtain the name "
                             "of the normalized active exception type.");
         }
-#if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x07030a00
+#    if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x07030a00
         // This behavior runs the risk of masking errors in the error handling, but avoids a
         // conflict with PyPy, which relies on the normalization here to change OSError to
         // FileNotFoundError (https://github.com/pybind/pybind11/issues/4075).
         m_lazy_error_string = exc_type_name_norm;
-#else
+#    else
         if (exc_type_name_norm != m_lazy_error_string) {
             std::string msg = std::string(called)
                               + ": MISMATCH of original and normalized "
                                 "active exception types: ";
             msg += "ORIGINAL ";
             msg += m_lazy_error_string;
             msg += " REPLACED BY ";
             msg += exc_type_name_norm;
             msg += ": " + format_value_and_trace();
             pybind11_fail(msg);
         }
+#    endif
 #endif
     }
 
     error_fetch_and_normalize(const error_fetch_and_normalize &) = delete;
     error_fetch_and_normalize(error_fetch_and_normalize &&) = delete;
 
     std::string format_value_and_trace() const {
@@ -521,14 +579,48 @@
                         message_error_string = detail::error_string();
                         result = message_unavailable_exc;
                     } else {
                         result = std::string(buffer, static_cast<std::size_t>(length));
                     }
                 }
             }
+#if PY_VERSION_HEX >= 0x030B0000
+            auto notes
+                = reinterpret_steal<object>(PyObject_GetAttrString(m_value.ptr(), "__notes__"));
+            if (!notes) {
+                PyErr_Clear(); // No notes is good news.
+            } else {
+                auto len_notes = PyList_Size(notes.ptr());
+                if (len_notes < 0) {
+                    result += "\nFAILURE obtaining len(__notes__): " + detail::error_string();
+                } else {
+                    result += "\n__notes__ (len=" + std::to_string(len_notes) + "):";
+                    for (ssize_t i = 0; i < len_notes; i++) {
+                        PyObject *note = PyList_GET_ITEM(notes.ptr(), i);
+                        auto note_bytes = reinterpret_steal<object>(
+                            PyUnicode_AsEncodedString(note, "utf-8", "backslashreplace"));
+                        if (!note_bytes) {
+                            result += "\nFAILURE obtaining __notes__[" + std::to_string(i)
+                                      + "]: " + detail::error_string();
+                        } else {
+                            char *buffer = nullptr;
+                            Py_ssize_t length = 0;
+                            if (PyBytes_AsStringAndSize(note_bytes.ptr(), &buffer, &length)
+                                == -1) {
+                                result += "\nFAILURE formatting __notes__[" + std::to_string(i)
+                                          + "]: " + detail::error_string();
+                            } else {
+                                result += '\n';
+                                result += std::string(buffer, static_cast<std::size_t>(length));
+                            }
+                        }
+                    }
+                }
+            }
+#endif
         } else {
             result = "<MESSAGE UNAVAILABLE>";
         }
         if (result.empty()) {
             result = "<EMPTY MESSAGE>";
         }
 
@@ -619,20 +711,14 @@
 
 inline std::string error_string() {
     return error_fetch_and_normalize("pybind11::detail::error_string").error_string();
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
-#if defined(_MSC_VER)
-#    pragma warning(push)
-#    pragma warning(disable : 4275 4251)
-//     warning C4275: An exported class was derived from a class that wasn't exported.
-//     Can be ignored when derived from a STL class.
-#endif
 /// Fetch and hold an error which was already set in Python.  An instance of this is typically
 /// thrown to propagate python-side errors back through C++ which can either be caught manually or
 /// else falls back to the function dispatcher (which then raises the captured error back to
 /// python).
 class PYBIND11_EXPORT_EXCEPTION error_already_set : public std::exception {
 public:
     /// Fetches the current Python exception (using PyErr_Fetch()), which will clear the
@@ -684,17 +770,14 @@
 private:
     std::shared_ptr<detail::error_fetch_and_normalize> m_fetched_error;
 
     /// WARNING: This custom deleter needs to acquire the Python GIL. This can lead to
     ///          crashes (undefined behavior) if the Python interpreter is finalizing.
     static void m_fetched_error_deleter(detail::error_fetch_and_normalize *raw_ptr);
 };
-#if defined(_MSC_VER)
-#    pragma warning(pop)
-#endif
 
 /// Replaces the current Python error indicator with the chosen error, performing a
 /// 'raise from' to indicate that the chosen error was caused by the original error.
 inline void raise_from(PyObject *type, const char *message) {
     // Based on _PyErr_FormatVFromCause:
     // https://github.com/python/cpython/blob/467ab194fc6189d9f7310c89937c51abeac56839/Python/errors.c#L405
     // See https://github.com/pybind/pybind11/pull/2112 for details.
@@ -889,18 +972,16 @@
 }
 // The following casting version is implemented in cast.h:
 template <typename T, enable_if_t<!is_pyobject<T>::value, int> = 0>
 object object_or_cast(T &&o);
 // Match a PyObject*, which we want to convert directly to handle via its converting constructor
 inline handle object_or_cast(PyObject *ptr) { return ptr; }
 
-#if defined(_MSC_VER) && _MSC_VER < 1920
-#    pragma warning(push)
-#    pragma warning(disable : 4522) // warning C4522: multiple assignment operators specified
-#endif
+PYBIND11_WARNING_PUSH
+PYBIND11_WARNING_DISABLE_MSVC(4522) // warning C4522: multiple assignment operators specified
 template <typename Policy>
 class accessor : public object_api<accessor<Policy>> {
     using key_type = typename Policy::key_type;
 
 public:
     accessor(handle obj, key_type key) : obj(obj), key(std::move(key)) {}
     accessor(const accessor &) = default;
@@ -956,17 +1037,15 @@
     }
 
 private:
     handle obj;
     key_type key;
     mutable object cache;
 };
-#if defined(_MSC_VER) && _MSC_VER < 1920
-#    pragma warning(pop)
-#endif
+PYBIND11_WARNING_POP
 
 PYBIND11_NAMESPACE_BEGIN(accessor_policies)
 struct obj_attr {
     using key_type = object;
     static object get(handle obj, handle key) { return getattr(obj, key); }
     static void set(handle obj, handle key, handle val) { setattr(obj, key, val); }
 };
@@ -1698,15 +1777,15 @@
 PYBIND11_NAMESPACE_BEGIN(detail)
 // Converts a value to the given unsigned type.  If an error occurs, you get back (Unsigned) -1;
 // otherwise you get back the unsigned long or unsigned long long value cast to (Unsigned).
 // (The distinction is critically important when casting a returned -1 error value to some other
 // unsigned type: (A)-1 != (B)-1 when A and B are unsigned types of different sizes).
 template <typename Unsigned>
 Unsigned as_unsigned(PyObject *o) {
-    if (PYBIND11_SILENCE_MSVC_C4127(sizeof(Unsigned) <= sizeof(unsigned long))) {
+    if (sizeof(Unsigned) <= sizeof(unsigned long)) {
         unsigned long v = PyLong_AsUnsignedLong(o);
         return v == (unsigned long) -1 && PyErr_Occurred() ? (Unsigned) -1 : (Unsigned) v;
     }
     unsigned long long v = PyLong_AsUnsignedLongLong(o);
     return v == (unsigned long long) -1 && PyErr_Occurred() ? (Unsigned) -1 : (Unsigned) v;
 }
 PYBIND11_NAMESPACE_END(detail)
@@ -1715,15 +1794,15 @@
 public:
     PYBIND11_OBJECT_CVT(int_, object, PYBIND11_LONG_CHECK, PyNumber_Long)
     int_() : object(PyLong_FromLong(0), stolen_t{}) {}
     // Allow implicit conversion from C++ integral types:
     template <typename T, detail::enable_if_t<std::is_integral<T>::value, int> = 0>
     // NOLINTNEXTLINE(google-explicit-constructor)
     int_(T value) {
-        if (PYBIND11_SILENCE_MSVC_C4127(sizeof(T) <= sizeof(long))) {
+        if (sizeof(T) <= sizeof(long)) {
             if (std::is_signed<T>::value) {
                 m_ptr = PyLong_FromLong((long) value);
             } else {
                 m_ptr = PyLong_FromUnsignedLong((unsigned long) value);
             }
         } else {
             if (std::is_signed<T>::value) {
@@ -1847,36 +1926,21 @@
     capsule(const void *value, PyCapsule_Destructor destructor)
         : object(PyCapsule_New(const_cast<void *>(value), nullptr, destructor), stolen_t{}) {
         if (!m_ptr) {
             throw error_already_set();
         }
     }
 
+    /// Capsule name is nullptr.
     capsule(const void *value, void (*destructor)(void *)) {
-        m_ptr = PyCapsule_New(const_cast<void *>(value), nullptr, [](PyObject *o) {
-            // guard if destructor called while err indicator is set
-            error_scope error_guard;
-            auto destructor = reinterpret_cast<void (*)(void *)>(PyCapsule_GetContext(o));
-            if (destructor == nullptr && PyErr_Occurred()) {
-                throw error_already_set();
-            }
-            const char *name = get_name_in_error_scope(o);
-            void *ptr = PyCapsule_GetPointer(o, name);
-            if (ptr == nullptr) {
-                throw error_already_set();
-            }
-
-            if (destructor != nullptr) {
-                destructor(ptr);
-            }
-        });
+        initialize_with_void_ptr_destructor(value, nullptr, destructor);
+    }
 
-        if (!m_ptr || PyCapsule_SetContext(m_ptr, reinterpret_cast<void *>(destructor)) != 0) {
-            throw error_already_set();
-        }
+    capsule(const void *value, const char *name, void (*destructor)(void *)) {
+        initialize_with_void_ptr_destructor(value, name, destructor);
     }
 
     explicit capsule(void (*destructor)()) {
         m_ptr = PyCapsule_New(reinterpret_cast<void *>(destructor), nullptr, [](PyObject *o) {
             const char *name = get_name_in_error_scope(o);
             auto destructor = reinterpret_cast<void (*)()>(PyCapsule_GetPointer(o, name));
             if (destructor == nullptr) {
@@ -1936,14 +2000,40 @@
         if ((name == nullptr) && PyErr_Occurred()) {
             // write out and consume error raised by call to PyCapsule_GetName
             PyErr_WriteUnraisable(o);
         }
 
         return name;
     }
+
+    void initialize_with_void_ptr_destructor(const void *value,
+                                             const char *name,
+                                             void (*destructor)(void *)) {
+        m_ptr = PyCapsule_New(const_cast<void *>(value), name, [](PyObject *o) {
+            // guard if destructor called while err indicator is set
+            error_scope error_guard;
+            auto destructor = reinterpret_cast<void (*)(void *)>(PyCapsule_GetContext(o));
+            if (destructor == nullptr && PyErr_Occurred()) {
+                throw error_already_set();
+            }
+            const char *name = get_name_in_error_scope(o);
+            void *ptr = PyCapsule_GetPointer(o, name);
+            if (ptr == nullptr) {
+                throw error_already_set();
+            }
+
+            if (destructor != nullptr) {
+                destructor(ptr);
+            }
+        });
+
+        if (!m_ptr || PyCapsule_SetContext(m_ptr, reinterpret_cast<void *>(destructor)) != 0) {
+            throw error_already_set();
+        }
+    }
 };
 
 class tuple : public object {
 public:
     PYBIND11_OBJECT_CVT(tuple, object, PyTuple_Check, PySequence_Tuple)
     template <typename SzType = ssize_t,
               detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/stl/filesystem.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/stl.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/stl.h`

 * *Files 2% similar despite different names*

```diff
@@ -269,19 +269,19 @@
             }
             PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
 
     PYBIND11_TYPE_CASTER(ArrayType,
-                         const_name("List[") + value_conv::name
+                         const_name<Resizable>(const_name(""), const_name("Annotated["))
+                             + const_name("List[") + value_conv::name + const_name("]")
                              + const_name<Resizable>(const_name(""),
-                                                     const_name("[") + const_name<Size>()
-                                                         + const_name("]"))
-                             + const_name("]"));
+                                                     const_name(", FixedSize(")
+                                                         + const_name<Size>() + const_name(")]")));
 };
 
 template <typename Type, size_t Size>
 struct type_caster<std::array<Type, Size>>
     : array_caster<std::array<Type, Size>, Type, false, Size> {};
 
 template <typename Type>
@@ -312,14 +312,15 @@
     static handle cast(T &&src, return_value_policy policy, handle parent) {
         if (!src) {
             return none().release();
         }
         if (!std::is_lvalue_reference<T>::value) {
             policy = return_value_policy_override<Value>::policy(policy);
         }
+        // NOLINTNEXTLINE(bugprone-unchecked-optional-access)
         return value_conv::cast(*std::forward<T>(src), policy, parent);
     }
 
     bool load(handle src, bool convert) {
         if (!src) {
             return false;
         }
```

### Comparing `dynareadout-23.6/lib/pybind11/include/pybind11/stl_bind.h` & `dynareadout-23.7/lib/pybind11/include/pybind11/stl_bind.h`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,21 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "detail/common.h"
+#include "detail/type_caster_base.h"
+#include "cast.h"
 #include "operators.h"
 
 #include <algorithm>
 #include <sstream>
+#include <type_traits>
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 /* SFINAE helper class used by 'is_comparable */
 template <typename T>
 struct container_traits {
@@ -54,17 +57,19 @@
     T,
     enable_if_t<container_traits<T>::is_element && container_traits<T>::is_comparable>>
     : std::true_type {};
 
 /* For a vector/map data structure, recursively check the value type
    (which is std::pair for maps) */
 template <typename T>
-struct is_comparable<T, enable_if_t<container_traits<T>::is_vector>> {
-    static constexpr const bool value = is_comparable<typename T::value_type>::value;
-};
+struct is_comparable<T, enable_if_t<container_traits<T>::is_vector>>
+    : is_comparable<typename recursive_container_traits<T>::type_to_check_recursively> {};
+
+template <>
+struct is_comparable<recursive_bottom> : std::true_type {};
 
 /* For pairs, recursively check the two data types */
 template <typename T>
 struct is_comparable<T, enable_if_t<container_traits<T>::is_pair>> {
     static constexpr const bool value = is_comparable<typename T::first_type>::value
                                         && is_comparable<typename T::second_type>::value;
 };
@@ -348,21 +353,25 @@
 template <typename Vector, typename Class_>
 void vector_accessor(enable_if_t<vector_needs_copy<Vector>::value, Class_> &cl) {
     using T = typename Vector::value_type;
     using SizeType = typename Vector::size_type;
     using DiffType = typename Vector::difference_type;
     using ItType = typename Vector::iterator;
     cl.def("__getitem__", [](const Vector &v, DiffType i) -> T {
-        if (i < 0 && (i += v.size()) < 0) {
-            throw index_error();
+        if (i < 0) {
+            i += v.size();
+            if (i < 0) {
+                throw index_error();
+            }
         }
-        if ((SizeType) i >= v.size()) {
+        auto i_st = static_cast<SizeType>(i);
+        if (i_st >= v.size()) {
             throw index_error();
         }
-        return v[(SizeType) i];
+        return v[i_st];
     });
 
     cl.def(
         "__iter__",
         [](Vector &v) {
             return make_iterator<return_value_policy::copy, ItType, ItType, T>(v.begin(), v.end());
         },
@@ -632,57 +641,138 @@
             }
             s << '}';
             return s.str();
         },
         "Return the canonical string representation of this map.");
 }
 
-template <typename Map>
+template <typename KeyType>
 struct keys_view {
-    Map &map;
+    virtual size_t len() = 0;
+    virtual iterator iter() = 0;
+    virtual bool contains(const KeyType &k) = 0;
+    virtual bool contains(const object &k) = 0;
+    virtual ~keys_view() = default;
 };
 
-template <typename Map>
+template <typename MappedType>
 struct values_view {
-    Map &map;
+    virtual size_t len() = 0;
+    virtual iterator iter() = 0;
+    virtual ~values_view() = default;
 };
 
-template <typename Map>
+template <typename KeyType, typename MappedType>
 struct items_view {
+    virtual size_t len() = 0;
+    virtual iterator iter() = 0;
+    virtual ~items_view() = default;
+};
+
+template <typename Map, typename KeysView>
+struct KeysViewImpl : public KeysView {
+    explicit KeysViewImpl(Map &map) : map(map) {}
+    size_t len() override { return map.size(); }
+    iterator iter() override { return make_key_iterator(map.begin(), map.end()); }
+    bool contains(const typename Map::key_type &k) override { return map.find(k) != map.end(); }
+    bool contains(const object &) override { return false; }
+    Map &map;
+};
+
+template <typename Map, typename ValuesView>
+struct ValuesViewImpl : public ValuesView {
+    explicit ValuesViewImpl(Map &map) : map(map) {}
+    size_t len() override { return map.size(); }
+    iterator iter() override { return make_value_iterator(map.begin(), map.end()); }
+    Map &map;
+};
+
+template <typename Map, typename ItemsView>
+struct ItemsViewImpl : public ItemsView {
+    explicit ItemsViewImpl(Map &map) : map(map) {}
+    size_t len() override { return map.size(); }
+    iterator iter() override { return make_iterator(map.begin(), map.end()); }
     Map &map;
 };
 
 PYBIND11_NAMESPACE_END(detail)
 
 template <typename Map, typename holder_type = std::unique_ptr<Map>, typename... Args>
 class_<Map, holder_type> bind_map(handle scope, const std::string &name, Args &&...args) {
     using KeyType = typename Map::key_type;
     using MappedType = typename Map::mapped_type;
-    using KeysView = detail::keys_view<Map>;
-    using ValuesView = detail::values_view<Map>;
-    using ItemsView = detail::items_view<Map>;
+    using StrippedKeyType = detail::remove_cvref_t<KeyType>;
+    using StrippedMappedType = detail::remove_cvref_t<MappedType>;
+    using KeysView = detail::keys_view<StrippedKeyType>;
+    using ValuesView = detail::values_view<StrippedMappedType>;
+    using ItemsView = detail::items_view<StrippedKeyType, StrippedMappedType>;
     using Class_ = class_<Map, holder_type>;
 
     // If either type is a non-module-local bound type then make the map binding non-local as well;
     // otherwise (e.g. both types are either module-local or converting) the map will be
     // module-local.
     auto *tinfo = detail::get_type_info(typeid(MappedType));
     bool local = !tinfo || tinfo->module_local;
     if (local) {
         tinfo = detail::get_type_info(typeid(KeyType));
         local = !tinfo || tinfo->module_local;
     }
 
     Class_ cl(scope, name.c_str(), pybind11::module_local(local), std::forward<Args>(args)...);
-    class_<KeysView> keys_view(
-        scope, ("KeysView[" + name + "]").c_str(), pybind11::module_local(local));
-    class_<ValuesView> values_view(
-        scope, ("ValuesView[" + name + "]").c_str(), pybind11::module_local(local));
-    class_<ItemsView> items_view(
-        scope, ("ItemsView[" + name + "]").c_str(), pybind11::module_local(local));
+    static constexpr auto key_type_descr = detail::make_caster<KeyType>::name;
+    static constexpr auto mapped_type_descr = detail::make_caster<MappedType>::name;
+    std::string key_type_name(key_type_descr.text), mapped_type_name(mapped_type_descr.text);
+
+    // If key type isn't properly wrapped, fall back to C++ names
+    if (key_type_name == "%") {
+        key_type_name = detail::type_info_description(typeid(KeyType));
+    }
+    // Similarly for value type:
+    if (mapped_type_name == "%") {
+        mapped_type_name = detail::type_info_description(typeid(MappedType));
+    }
+
+    // Wrap KeysView[KeyType] if it wasn't already wrapped
+    if (!detail::get_type_info(typeid(KeysView))) {
+        class_<KeysView> keys_view(
+            scope, ("KeysView[" + key_type_name + "]").c_str(), pybind11::module_local(local));
+        keys_view.def("__len__", &KeysView::len);
+        keys_view.def("__iter__",
+                      &KeysView::iter,
+                      keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
+        );
+        keys_view.def("__contains__",
+                      static_cast<bool (KeysView::*)(const KeyType &)>(&KeysView::contains));
+        // Fallback for when the object is not of the key type
+        keys_view.def("__contains__",
+                      static_cast<bool (KeysView::*)(const object &)>(&KeysView::contains));
+    }
+    // Similarly for ValuesView:
+    if (!detail::get_type_info(typeid(ValuesView))) {
+        class_<ValuesView> values_view(scope,
+                                       ("ValuesView[" + mapped_type_name + "]").c_str(),
+                                       pybind11::module_local(local));
+        values_view.def("__len__", &ValuesView::len);
+        values_view.def("__iter__",
+                        &ValuesView::iter,
+                        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
+        );
+    }
+    // Similarly for ItemsView:
+    if (!detail::get_type_info(typeid(ItemsView))) {
+        class_<ItemsView> items_view(
+            scope,
+            ("ItemsView[" + key_type_name + ", ").append(mapped_type_name + "]").c_str(),
+            pybind11::module_local(local));
+        items_view.def("__len__", &ItemsView::len);
+        items_view.def("__iter__",
+                       &ItemsView::iter,
+                       keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
+        );
+    }
 
     cl.def(init<>());
 
     // Register stream insertion operator (if possible)
     detail::map_if_insertion_operator<Map, Class_>(cl, name);
 
     cl.def(
@@ -694,27 +784,33 @@
         "__iter__",
         [](Map &m) { return make_key_iterator(m.begin(), m.end()); },
         keep_alive<0, 1>() /* Essential: keep map alive while iterator exists */
     );
 
     cl.def(
         "keys",
-        [](Map &m) { return KeysView{m}; },
+        [](Map &m) {
+            return std::unique_ptr<KeysView>(new detail::KeysViewImpl<Map, KeysView>(m));
+        },
         keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def(
         "values",
-        [](Map &m) { return ValuesView{m}; },
+        [](Map &m) {
+            return std::unique_ptr<ValuesView>(new detail::ValuesViewImpl<Map, ValuesView>(m));
+        },
         keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def(
         "items",
-        [](Map &m) { return ItemsView{m}; },
+        [](Map &m) {
+            return std::unique_ptr<ItemsView>(new detail::ItemsViewImpl<Map, ItemsView>(m));
+        },
         keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def(
         "__getitem__",
         [](Map &m, const KeyType &k) -> MappedType & {
             auto it = m.find(k);
@@ -745,41 +841,11 @@
             throw key_error();
         }
         m.erase(it);
     });
 
     cl.def("__len__", &Map::size);
 
-    keys_view.def("__len__", [](KeysView &view) { return view.map.size(); });
-    keys_view.def(
-        "__iter__",
-        [](KeysView &view) { return make_key_iterator(view.map.begin(), view.map.end()); },
-        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
-    );
-    keys_view.def("__contains__", [](KeysView &view, const KeyType &k) -> bool {
-        auto it = view.map.find(k);
-        if (it == view.map.end()) {
-            return false;
-        }
-        return true;
-    });
-    // Fallback for when the object is not of the key type
-    keys_view.def("__contains__", [](KeysView &, const object &) -> bool { return false; });
-
-    values_view.def("__len__", [](ValuesView &view) { return view.map.size(); });
-    values_view.def(
-        "__iter__",
-        [](ValuesView &view) { return make_value_iterator(view.map.begin(), view.map.end()); },
-        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
-    );
-
-    items_view.def("__len__", [](ItemsView &view) { return view.map.size(); });
-    items_view.def(
-        "__iter__",
-        [](ItemsView &view) { return make_iterator(view.map.begin(), view.map.end()); },
-        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
-    );
-
     return cl;
 }
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `dynareadout-23.6/pyproject.toml` & `dynareadout-23.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynareadout"
-version = "23.06"
+version = "23.07"
 authors = [
   { name = "PucklaJ", email = "jonaas.pucher000000@gmail.com"},
 ]
-description = "Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python"
+description = "High-Performance and Thread-Safe library for parsing binary output files and key files of LS Dyna (d3plot, binout, input deck)"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
   "Programming Language :: C",
   "Programming Language :: C++",
   "License :: OSI Approved :: zlib/libpng License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
   "Topic :: Scientific/Engineering",
 ]
-dependencies = [
-  "lsst-utils"
-]
 
 [project.urls]
 "Homepage" = "https://github.com/PucklaJ/dynareadout"
 "Bug Trackers" = "https://github.com/PucklaJ/dynareadout/issues"
```

### Comparing `dynareadout-23.6/setup.py` & `dynareadout-23.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,52 +13,53 @@
     compile_args.append("/DTHREAD_SAFE")
 else:
     compile_args.append("-std=c++17")
     compile_args.append("-w")
     compile_args.append("-DTHREAD_SAFE")
     link_args.append("-lpthread")
 
-dynareadout_c = Extension(
-    name='dynareadout_c',
+dynareadout = Extension(
+    name='dynareadout',
     extra_compile_args=compile_args,
     extra_link_args=link_args,
     include_dirs=[
         os.path.join(this_dir, 'lib', 'pybind11', 'include'),
         os.path.join(dynareadout_dir, 'src'),
         os.path.join(dynareadout_dir, 'src', 'cpp')
     ],
     sources=[
         # C Source Files
         os.path.join(dynareadout_dir, 'src', 'binary_search.c'),
-        os.path.join(dynareadout_dir, 'src', 'binout.c'),
         os.path.join(dynareadout_dir, 'src', 'binout_directory.c'),
         os.path.join(dynareadout_dir, 'src', 'binout_glob.c'),
         os.path.join(dynareadout_dir, 'src', 'binout_read.c'),
+        os.path.join(dynareadout_dir, 'src', 'binout.c'),
         os.path.join(dynareadout_dir, 'src', 'd3_buffer.c'),
-        os.path.join(dynareadout_dir, 'src', 'd3plot.c'),
         os.path.join(dynareadout_dir, 'src', 'd3plot_data.c'),
         os.path.join(dynareadout_dir, 'src', 'd3plot_part_nodes.c'),
         os.path.join(dynareadout_dir, 'src', 'd3plot_state.c'),
+        os.path.join(dynareadout_dir, 'src', 'd3plot.c'),
         os.path.join(dynareadout_dir, 'src', 'extra_string.c'),
         os.path.join(dynareadout_dir, 'src', 'key.c'),
+        os.path.join(dynareadout_dir, 'src', 'line.c'),
         os.path.join(dynareadout_dir, 'src', 'multi_file.c'),
-        os.path.join(dynareadout_dir, 'src', 'path.c'),
         os.path.join(dynareadout_dir, 'src', 'path_view.c'),
+        os.path.join(dynareadout_dir, 'src', 'path.c'),
         os.path.join(dynareadout_dir, 'src', 'sync.c'),
         # C++ Source Files
         os.path.join(dynareadout_dir, 'src', 'cpp', 'binout.cpp'),
-        os.path.join(dynareadout_dir, 'src', 'cpp', 'd3plot.cpp'),
         os.path.join(dynareadout_dir, 'src', 'cpp', 'd3plot_part.cpp'),
         os.path.join(dynareadout_dir, 'src', 'cpp', 'd3plot_state.cpp'),
+        os.path.join(dynareadout_dir, 'src', 'cpp', 'd3plot.cpp'),
         os.path.join(dynareadout_dir, 'src', 'cpp', 'key.cpp'),
         # C++ Source Files for pybind11 module
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_binout.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_d3plot.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_key.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_module.cpp'),
     ])
 
 setup(name='dynareadout',
-      version='23.06',
-      ext_modules=[dynareadout_c],
+      version='23.07',
+      ext_modules=[dynareadout],
       zip_safe=False,
       include_package_data=True)
```

### Comparing `dynareadout-23.6/src/dynareadout.egg-info/PKG-INFO` & `dynareadout-23.7/src/dynareadout.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dynareadout
-Version: 23.6
-Summary: Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
+Version: 23.7
+Summary: High-Performance and Thread-Safe library for parsing binary output files and key files of LS Dyna (d3plot, binout, input deck)
 Author-email: PucklaJ <jonaas.pucher000000@gmail.com>
 Project-URL: Homepage, https://github.com/PucklaJ/dynareadout
 Project-URL: Bug Trackers, https://github.com/PucklaJ/dynareadout/issues
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: zlib/libpng License
 Classifier: Operating System :: Microsoft :: Windows
@@ -14,64 +14,53 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dynareadout
 
-An Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
+High-Performance and Thread-Safe C/C++ library for parsing binary output files and key files of LS Dyna (d3plot, binout, input deck) with bindings for python.
 
 ## Documentation
 
 You can find a [Wiki](https://github.com/PucklaJ/dynareadout/wiki) with API Documentation for python.
 
 ## Examples
 
 ### Binout
 
 ```python
-from dynareadout import Binout, BinoutType
+from dynareadout import Binout
 
 bin_file = None
 try:
   # This library also supports opening multiple binout files at once by globing them
-  bin_file = Binout("simulation/binout*")
+  bin_file = Binout("path/to/your/binout*")
 except RuntimeError as e:
   print("Failed to open binout: {}".format(e))
   exit(1)
 
 # Print the children of the binout
 children = bin_file.read("/")
 for (i, child) in enumerate(children):
   print("Child {}: {}".format(i, child))
 
 # Read some data. This read method can read variables with different types, but
 # there are also read methods for particular types
 node_ids = bin_file.read("nodout/ids")
-for (i, nid) in enumerate(node_ids):
-  print("Node ID {}: {}".format(i, nid))
+for i in range(len(node_ids)):
+  print("Node ID {}: {}".format(i, node_ids[i]))
 
-# You can also read this variable with the read method of the particular type
-# First find out what the type is
-node_ids_type = bin_file.get_type_id("/nodout/metadata/ids")
-
-# Then read the data using the special read method.
-# If you already know the exact type and path of a variable
-# these methods can be a bit more performant,
-# since the library does not need the get the type and path first.
-if node_ids_type == BinoutType.Int32:
-  node_ids = bin_file.read_int32("/nodout/metadata/ids")
-elif node_ids_type == BinoutType.Int64:
-  node_ids = bin_file.read_int64("/nodout/metadata/ids")
-else:
-  print("The node ids are not 32-Bit or 64-Bit integers")
-  exit(1)
+# You can also find out if a variable exists
+node_ids_exist = bin_file.variable_exists("/nodout/metadata/ids")
 
-for (i, nid) in enumerate(node_ids):
-  print("Node ID {}: {}".format(i, nid))
+# Get the number of time steps in the binout
+nodout_timesteps = bin_file.get_num_timesteps("/nodout")
+# The time steps can vary inside the binout
+rcforc_timesteps = bin_file.get_num_timesteps("/rcforc")
 
 # If you want to read "timed" data (x_displacement, x_force, etc.) you can do so also with the read method
 x_displacement = bin_file.read("nodout/x_displacement")
 for (t, time_step) in enumerate(x_displacement):
   for (n, x_disp) in enumerate(time_step):
     print("X Displacement time_step={}, node_id={}: {}".format(t, node_ids[n], x_displacement[t][n]))
 ```
@@ -80,16 +69,16 @@
 
 ```python
 from dynareadout import D3plot
 
 plot_file = None
 try:
   # Just give it the first d3plot file and it opens all of them
-  plot_file = D3plot("simulation/d3plot")
-except e as RuntimeError:
+  plot_file = D3plot("path/to/your/d3plot")
+except RuntimeError as e:
   print("Failed to open: {}".format(e))
   exit(1)
 
 # Read the title
 title = plot_file.read_title()
 print("Title: {}".format(title))
 
@@ -106,27 +95,27 @@
 ```
 
 ### KeyFile
 
 ```python
 from dynareadout import key_file_parse
 
-keywords = key_file_parse("simulation/input.k")
+keywords = key_file_parse("path/to/your/input.k")
 
 # Parse all nodes
 node_keywords = keywords["NODE"]
 
+# Loop over all *NODE keywords
 for i in range(len(node_keywords)):
+  # Loop over all cards of each *NODE keyword
   for j in range(len(node_keywords[i])):
     node = node_keywords[i][j]
-    node_data = node.parse_whole([8, 16, 16, 16])
-    nid = node_data[0]
-    x = node_data[1]
-    y = node_data[2]
-    z = node_data[3]
+    # Then you can parse the variables of each card as integers and floats
+    # The list of integers holds all the widths of each variable in the card in characters
+    nid, x, y, z = node.parse_whole([8, 16, 16, 16])
 
     print(f"NODE {nid:d}: ({x:.3f}; {y:.3f}; {z:.3f})")
 ```
 
 ## Other languages
 
 This library is also available for C and C++ this version can be found [here](https://github.com/PucklaJ/dynareadout).
```

### Comparing `dynareadout-23.6/src/dynareadout.egg-info/SOURCES.txt` & `dynareadout-23.7/src/dynareadout.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 lib/dynareadout/src/d3plot_part_nodes.c
 lib/dynareadout/src/d3plot_part_nodes.h
 lib/dynareadout/src/d3plot_state.c
 lib/dynareadout/src/extra_string.c
 lib/dynareadout/src/extra_string.h
 lib/dynareadout/src/key.c
 lib/dynareadout/src/key.h
+lib/dynareadout/src/line.c
+lib/dynareadout/src/line.h
 lib/dynareadout/src/multi_file.c
 lib/dynareadout/src/multi_file.h
 lib/dynareadout/src/path.c
 lib/dynareadout/src/path.h
 lib/dynareadout/src/path_view.c
 lib/dynareadout/src/path_view.h
 lib/dynareadout/src/pgni.h
@@ -72,22 +74,24 @@
 lib/pybind11/include/pybind11/numpy.h
 lib/pybind11/include/pybind11/operators.h
 lib/pybind11/include/pybind11/options.h
 lib/pybind11/include/pybind11/pybind11.h
 lib/pybind11/include/pybind11/pytypes.h
 lib/pybind11/include/pybind11/stl.h
 lib/pybind11/include/pybind11/stl_bind.h
+lib/pybind11/include/pybind11/type_caster_pyobject_ptr.h
 lib/pybind11/include/pybind11/detail/class.h
 lib/pybind11/include/pybind11/detail/common.h
 lib/pybind11/include/pybind11/detail/descr.h
 lib/pybind11/include/pybind11/detail/init.h
 lib/pybind11/include/pybind11/detail/internals.h
 lib/pybind11/include/pybind11/detail/type_caster_base.h
 lib/pybind11/include/pybind11/detail/typeid.h
+lib/pybind11/include/pybind11/eigen/common.h
+lib/pybind11/include/pybind11/eigen/matrix.h
+lib/pybind11/include/pybind11/eigen/tensor.h
 lib/pybind11/include/pybind11/stl/filesystem.h
-src/dynareadout/__init__.py
 src/dynareadout.egg-info/PKG-INFO
 src/dynareadout.egg-info/SOURCES.txt
 src/dynareadout.egg-info/dependency_links.txt
 src/dynareadout.egg-info/not-zip-safe
-src/dynareadout.egg-info/requires.txt
 src/dynareadout.egg-info/top_level.txt
```

