# Comparing `tmp/torch_migraphx-0.0.tar.gz` & `tmp/torch_migraphx-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/shiv/torch_migraphx/dist/.tmp-_adbmlof/torch_migraphx-0.0.tar", last modified: Mon May  8 23:30:45 2023, max compression
+gzip compressed data, was "dist/torch_migraphx-0.0.1.tar", last modified: Mon Jul 24 18:37:29 2023, max compression
```

## Comparing `torch_migraphx-0.0.tar` & `torch_migraphx-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,80 @@
-drwxrwxr-x   0 shiv      (1000) shiv      (1000)        0 2023-05-08 23:30:45.000000 torch_migraphx-0.0/
--rw-rw-r--   0 shiv      (1000) shiv      (1000)     1522 2023-05-08 23:21:52.000000 torch_migraphx-0.0/LICENSE
--rw-rw-r--   0 shiv      (1000) shiv      (1000)      571 2023-05-08 23:30:45.000000 torch_migraphx-0.0/PKG-INFO
--rw-rw-r--   0 shiv      (1000) shiv      (1000)        0 2023-05-08 23:09:43.000000 torch_migraphx-0.0/README.md
--rw-rw-r--   0 shiv      (1000) shiv      (1000)      545 2023-05-08 23:30:30.000000 torch_migraphx-0.0/pyproject.toml
--rw-rw-r--   0 shiv      (1000) shiv      (1000)       38 2023-05-08 23:30:45.000000 torch_migraphx-0.0/setup.cfg
-drwxrwxr-x   0 shiv      (1000) shiv      (1000)        0 2023-05-08 23:30:45.000000 torch_migraphx-0.0/src/
-drwxrwxr-x   0 shiv      (1000) shiv      (1000)        0 2023-05-08 23:30:45.000000 torch_migraphx-0.0/src/torch_migraphx/
--rw-rw-r--   0 shiv      (1000) shiv      (1000)        0 2023-05-08 23:04:15.000000 torch_migraphx-0.0/src/torch_migraphx/__init__.py
-drwxrwxr-x   0 shiv      (1000) shiv      (1000)        0 2023-05-08 23:30:45.000000 torch_migraphx-0.0/src/torch_migraphx.egg-info/
--rw-rw-r--   0 shiv      (1000) shiv      (1000)      571 2023-05-08 23:30:45.000000 torch_migraphx-0.0/src/torch_migraphx.egg-info/PKG-INFO
--rw-rw-r--   0 shiv      (1000) shiv      (1000)      231 2023-05-08 23:30:45.000000 torch_migraphx-0.0/src/torch_migraphx.egg-info/SOURCES.txt
--rw-rw-r--   0 shiv      (1000) shiv      (1000)        1 2023-05-08 23:30:45.000000 torch_migraphx-0.0/src/torch_migraphx.egg-info/dependency_links.txt
--rw-rw-r--   0 shiv      (1000) shiv      (1000)       15 2023-05-08 23:30:45.000000 torch_migraphx-0.0/src/torch_migraphx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.081145 torch_migraphx-0.0.1/
+-rw-rw-r--   0 root         (0) root         (0)      870 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     1522 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      125 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      607 2023-07-24 18:37:29.081145 torch_migraphx-0.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/README.md
+-rw-rw-r--   0 root         (0) root         (0)      102 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)       79 2023-07-24 18:37:29.081145 torch_migraphx-0.0.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     5485 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.077145 torch_migraphx-0.0.1/torch_migraphx/
+-rw-rw-r--   0 root         (0) root         (0)       42 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/_C.py
+-rw-rw-r--   0 root         (0) root         (0)      210 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.077145 torch_migraphx-0.0.1/torch_migraphx/csrc/
+-rw-rw-r--   0 root         (0) root         (0)     3356 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/csrc/mgx_util.cpp
+-rw-rw-r--   0 root         (0) root         (0)     1970 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/csrc/mgx_util.h
+-rw-rw-r--   0 root         (0) root         (0)     3616 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/csrc/par_for.h
+-rw-rw-r--   0 root         (0) root         (0)     5271 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/csrc/torch_migraphx_py.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.077145 torch_migraphx-0.0.1/torch_migraphx/dynamo/
+-rw-rw-r--   0 root         (0) root         (0)       30 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/dynamo/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2991 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/dynamo/backends.py
+-rw-rw-r--   0 root         (0) root         (0)     4689 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/dynamo/lower_dynamo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.077145 torch_migraphx-0.0.1/torch_migraphx/dynamo/passes/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/dynamo/passes/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2164 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/dynamo/passes/const_fold.py
+-rw-rw-r--   0 root         (0) root         (0)     2505 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/dynamo/passes/contiguous_outputs.py
+-rw-rw-r--   0 root         (0) root         (0)     5090 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/dynamo/passes/partition.py
+-rw-rw-r--   0 root         (0) root         (0)     2486 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/dynamo/passes/pass_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     5080 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/dynamo/passes/remove_ops.py
+-rw-rw-r--   0 root         (0) root         (0)     2070 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/dynamo/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.081145 torch_migraphx-0.0.1/torch_migraphx/fx/
+-rw-rw-r--   0 root         (0) root         (0)      249 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2085 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/converter_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.081145 torch_migraphx-0.0.1/torch_migraphx/fx/converters/
+-rw-rw-r--   0 root         (0) root         (0)      249 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/converters/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    51223 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/converters/acc_ops_converters.py
+-rw-rw-r--   0 root         (0) root         (0)    25931 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/converters/aten_ops_converters.py
+-rw-rw-r--   0 root         (0) root         (0)     2151 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/converters/builtin_converters.py
+-rw-rw-r--   0 root         (0) root         (0)     7876 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/converters/module_converters.py
+-rw-rw-r--   0 root         (0) root         (0)     3133 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/converters/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5912 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/fx2mgx.py
+-rw-rw-r--   0 root         (0) root         (0)     9724 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/lower.py
+-rw-rw-r--   0 root         (0) root         (0)     3881 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/lower_setting.py
+-rw-rw-r--   0 root         (0) root         (0)     9725 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/mgx_module.py
+-rw-rw-r--   0 root         (0) root         (0)     7717 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/observer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.081145 torch_migraphx-0.0.1/torch_migraphx/fx/passes/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/passes/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3874 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/passes/graph_opts.py
+-rw-rw-r--   0 root         (0) root         (0)     2801 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/passes/lower_basic_pass.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/passes/lower_basic_pass_aten.py
+-rw-rw-r--   0 root         (0) root         (0)     9788 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/passes/lower_pass_manager_builder.py
+-rw-rw-r--   0 root         (0) root         (0)     6763 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/passes/pass_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     6691 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/passes/remove_duplicate_output_args.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.081145 torch_migraphx-0.0.1/torch_migraphx/fx/tools/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5138 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tools/mgx_benchmark.py
+-rw-rw-r--   0 root         (0) root         (0)     3521 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tools/mgx_minimizer.py
+-rw-rw-r--   0 root         (0) root         (0)     1983 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tools/mgx_onnx.py
+-rw-rw-r--   0 root         (0) root         (0)     4517 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tools/mgx_splitter.py
+-rw-rw-r--   0 root         (0) root         (0)     3295 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tools/timing_cache_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.081145 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.081145 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/acc_tracer/
+-rw-rw-r--   0 root         (0) root         (0)       29 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/acc_tracer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    21920 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/acc_tracer/acc_normalizer.py
+-rw-rw-r--   0 root         (0) root         (0)     3395 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/acc_tracer/acc_op_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    56255 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/acc_tracer/acc_ops.py
+-rw-rw-r--   0 root         (0) root         (0)     4282 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/acc_tracer/acc_shape_prop.py
+-rw-rw-r--   0 root         (0) root         (0)    27124 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/acc_tracer/acc_tracer.py
+-rw-rw-r--   0 root         (0) root         (0)     4682 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/acc_tracer/acc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.081145 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/aten_tracer/
+-rw-rw-r--   0 root         (0) root         (0)       30 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/aten_tracer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2989 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/tracer/aten_tracer/aten_tracer.py
+-rw-rw-r--   0 root         (0) root         (0)     6853 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/torch_migraphx/fx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:37:29.077145 torch_migraphx-0.0.1/torch_migraphx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      607 2023-07-24 18:37:29.000000 torch_migraphx-0.0.1/torch_migraphx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-07-24 18:37:29.000000 torch_migraphx-0.0.1/torch_migraphx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 18:37:29.000000 torch_migraphx-0.0.1/torch_migraphx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-24 18:37:29.000000 torch_migraphx-0.0.1/torch_migraphx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-24 18:37:29.000000 torch_migraphx-0.0.1/torch_migraphx.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        5 2023-07-24 18:21:14.000000 torch_migraphx-0.0.1/version.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `torch_migraphx-0.0/LICENSE` & `torch_migraphx-0.0.1/LICENSE`

 * *Files identical despite different names*

