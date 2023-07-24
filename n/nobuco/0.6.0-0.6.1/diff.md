# Comparing `tmp/nobuco-0.6.0.tar.gz` & `tmp/nobuco-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.6.0.tar", last modified: Thu Jul 20 18:31:09 2023, max compression
+gzip compressed data, was "nobuco-0.6.1.tar", last modified: Mon Jul 24 13:34:25 2023, max compression
```

## Comparing `nobuco-0.6.0.tar` & `nobuco-0.6.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.457288 nobuco-0.6.0/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.6.0/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-20 18:31:09.457288 nobuco-0.6.0/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    24311 2023-07-01 11:16:21.000000 nobuco-0.6.0/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.449288 nobuco-0.6.0/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-06-23 09:29:01.000000 nobuco-0.6.0/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13988 2023-07-20 10:12:52.000000 nobuco-0.6.0/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.449288 nobuco-0.6.0/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.6.0/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1360 2023-07-20 18:20:30.000000 nobuco-0.6.0/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4095 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.449288 nobuco-0.6.0/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.449288 nobuco-0.6.0/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.6.0/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1113 2023-07-20 18:19:12.000000 nobuco-0.6.0/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.449288 nobuco-0.6.0/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.453288 nobuco-0.6.0/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/attention.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14555 2023-07-11 12:33:40.000000 nobuco-0.6.0/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-07-11 12:35:48.000000 nobuco-0.6.0/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6449 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11315 2023-07-11 12:35:48.000000 nobuco-0.6.0/nobuco/node_converters/tensor_manipulation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/tensor_shape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/torchvision.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.453288 nobuco-0.6.0/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10069 2023-07-20 10:14:17.000000 nobuco-0.6.0/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.457288 nobuco-0.6.0/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.449288 nobuco-0.6.0/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-20 18:31:09.000000 nobuco-0.6.0/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-07-20 18:31:09.000000 nobuco-0.6.0/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-20 18:31:09.000000 nobuco-0.6.0/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-07-20 18:31:09.000000 nobuco-0.6.0/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-07-20 18:31:09.000000 nobuco-0.6.0/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      735 2023-07-20 18:26:47.000000 nobuco-0.6.0/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-20 18:31:09.457288 nobuco-0.6.0/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.301624 nobuco-0.6.1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.6.1/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-24 13:34:25.301624 nobuco-0.6.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24311 2023-07-01 11:16:21.000000 nobuco-0.6.1/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.297624 nobuco-0.6.1/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-06-23 09:29:01.000000 nobuco-0.6.1/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13988 2023-07-20 10:12:52.000000 nobuco-0.6.1/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.297624 nobuco-0.6.1/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.6.1/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1358 2023-07-24 13:27:30.000000 nobuco-0.6.1/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4274 2023-07-24 13:14:20.000000 nobuco-0.6.1/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.297624 nobuco-0.6.1/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.301624 nobuco-0.6.1/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-07-24 13:29:19.000000 nobuco-0.6.1/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1113 2023-07-20 18:19:12.000000 nobuco-0.6.1/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.301624 nobuco-0.6.1/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.301624 nobuco-0.6.1/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/attention.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16532 2023-07-24 13:27:30.000000 nobuco-0.6.1/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-07-11 12:35:48.000000 nobuco-0.6.1/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4029 2023-07-23 08:12:26.000000 nobuco-0.6.1/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6726 2023-07-23 08:18:17.000000 nobuco-0.6.1/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11559 2023-07-23 08:26:17.000000 nobuco-0.6.1/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/tensor_shape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/torchvision.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.301624 nobuco-0.6.1/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10069 2023-07-23 20:33:27.000000 nobuco-0.6.1/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.301624 nobuco-0.6.1/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.297624 nobuco-0.6.1/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-24 13:34:25.000000 nobuco-0.6.1/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-07-24 13:34:25.000000 nobuco-0.6.1/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-24 13:34:25.000000 nobuco-0.6.1/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-07-24 13:34:25.000000 nobuco-0.6.1/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-07-24 13:34:25.000000 nobuco-0.6.1/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      735 2023-07-24 13:33:26.000000 nobuco-0.6.1/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-24 13:34:25.301624 nobuco-0.6.1/setup.cfg
```

### Comparing `nobuco-0.6.0/LICENSE` & `nobuco-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/PKG-INFO` & `nobuco-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.6.0
+Version: 0.6.1
 Summary: Pytorch to Tensorflow conversion made intuitive
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
 Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
 Keywords: pytorch,tensorflow,keras,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nobuco-0.6.0/README.md` & `nobuco-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/__init__.py` & `nobuco-0.6.1/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/commons.py` & `nobuco-0.6.1/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/convert.py` & `nobuco-0.6.1/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/converters/channel_ordering.py` & `nobuco-0.6.1/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/converters/node_converter.py` & `nobuco-0.6.1/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/converters/tensor.py` & `nobuco-0.6.1/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/converters/type_cast.py` & `nobuco-0.6.1/nobuco/converters/type_cast.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 TF_TYPE_PRIORITY_LIST = [
     tf.complex128,
     tf.complex64,
 
     tf.float64,
     tf.float32,
     # tf.float16,
-    tf.int32,
+
     tf.int64,
-    # tf.int16,
-    # tf.int8,
+    tf.int32,
+    tf.int16,
+    tf.int8,
 ]
 
 
 def tf_cast_recursively(inputs, type_priority_list=None):
     if type_priority_list is None:
         type_priority_list = TF_TYPE_PRIORITY_LIST
 
@@ -28,15 +29,15 @@
     for t in tensors:
         if t.dtype in type_priority_list:
             p = type_priority_list.index(t.dtype)
         else:
             raise Exception(f'Unsupported dtype: {t.dtype}')
         min_priority = min(min_priority, p)
 
-    if min_priority not in type_priority_list:
+    if min_priority >= len(type_priority_list):
         return inputs
 
     target_dtype = type_priority_list[min_priority]
 
     def collect_func(obj):
         return isinstance(obj, TF_TENSOR_CLASSES)
```

### Comparing `nobuco-0.6.0/nobuco/converters/validation.py` & `nobuco-0.6.1/nobuco/converters/validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import traceback
 import warnings
 from enum import Enum
 import math
 
+import numpy as np
 import torch
 
 from nobuco.commons import ChannelOrder, TF_TENSOR_CLASSES
 from nobuco.converters.channel_ordering import t_keras2pytorch, pytorch2keras_recursively
 from nobuco.locate.link import get_link_to_obj
 from nobuco.util import str_parents, collect_recursively
 
@@ -88,16 +89,20 @@
             raise Exception(f"Tensor shapes don't match: (Pytorch) {list(t_pt.shape)} vs {list(t_tf.shape)} (Tensorflow)")
 
         # if t_tf.dtype != t_pt.dtype:
         #     raise Exception(f"Tensor dtypes don't match: (Pytorch) {t_pt.dtype} vs {t_tf.dtype} (Tensorflow)")
 
     def calc_diff(t1, t2):
         def calc_diff_numerical(t1, t2):
-            diff = t1 - t2
-            return diff.abs().max().detach().cpu().numpy()
+            nan_mask = torch.isnan(t1) & torch.isnan(t2)
+            diff = t1[~nan_mask] - t2[~nan_mask]
+            if diff.numel() == 0:
+                return 0
+            else:
+                return diff.abs().max().detach().cpu().numpy()
 
         def calc_diff_boolean(t1, t2):
             diff = t1 ^ t2
             return diff.to(torch.float32).max()
 
         if t1.numel() == t2.numel() == 0:
             return 0
```

### Comparing `nobuco-0.6.0/nobuco/entity/keras.py` & `nobuco-0.6.1/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/entity/pytorch.py` & `nobuco-0.6.1/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/funcs.py` & `nobuco-0.6.1/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/layers/channel_order.py` & `nobuco-0.6.1/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/layers/container.py` & `nobuco-0.6.1/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/layers/weight.py` & `nobuco-0.6.1/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/locate/link.py` & `nobuco-0.6.1/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/locate/locate.py` & `nobuco-0.6.1/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/activation.py` & `nobuco-0.6.1/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/attention.py` & `nobuco-0.6.1/nobuco/node_converters/attention.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/boolean.py` & `nobuco-0.6.1/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/boolean_mask.py` & `nobuco-0.6.1/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/comparison.py` & `nobuco-0.6.1/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/convolution.py` & `nobuco-0.6.1/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/dropout.py` & `nobuco-0.6.1/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/interpolation.py` & `nobuco-0.6.1/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/linear.py` & `nobuco-0.6.1/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/math.py` & `nobuco-0.6.1/nobuco/node_converters/math.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import math
 from typing import Optional, Union, List, Tuple, Sequence, Any
 
+import keras.layers
 from torch import Tensor
 from torch.types import _int, _bool, Number, _dtype, _size, _layout, _device
 
 import tensorflow as tf
 import torch
 
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
@@ -64,14 +66,61 @@
                 input = _permute(perm)(input)
             out = tf.reduce_mean(input, axis=dim, keepdims=keepdim)
             out = set_channel_order(out, ChannelOrder.PYTORCH)
             return out
     return func
 
 
+@converter(torch.std, torch.Tensor.std, channel_ordering_strategy=ChannelOrderingStrategy.MANUAL)
+def converter_std(input: Tensor, dim, unbiased: _bool=True, keepdim: _bool=False, *, out: Optional[Tensor]=None):
+    n_dims = input.dim()
+
+    def var_unbiased(input, axis, keepdims=False):
+        input_means = tf.reduce_mean(input, axis=axis, keepdims=True)
+        squared_deviations = tf.square(input - input_means)
+
+        if input.dtype in (tf.complex64, tf.complex128):
+            squared_deviations = tf.abs(squared_deviations)
+
+        sum = tf.reduce_sum(squared_deviations, axis=axis, keepdims=keepdims)
+        shape = tf.shape(input)
+        n = math.prod(shape[i] for i in axis)
+        # [sic] This implementation follows Pytorch behaviour, i.e. makes NaNs when n==1
+        return sum / tf.cast(n - 1, dtype=sum.dtype)
+
+    def std(input, axis, unbiased=True, keepdims=False):
+        if unbiased:
+            var = var_unbiased(input, axis=axis, keepdims=keepdims)
+            return tf.sqrt(var)
+        else:
+            return tf.math.reduce_std(input, axis=axis, keepdims=keepdims)
+
+    def func(input, dim, unbiased=True, keepdim=False, *, out=None):
+        if dim is not None:
+            dim = _ensure_iterable(dim)
+
+        order = get_channel_order(input)
+
+        if keepdim:
+            dim = _dims_make_positive(dim, n_dims)
+            if order == ChannelOrder.TENSORFLOW:
+                dim = dims_pytorch2keras(dim, n_dims)
+            out = std(input, axis=dim, unbiased=unbiased, keepdims=keepdim)
+            out = set_channel_order(out, order)
+            return out
+        else:
+            if order == ChannelOrder.TENSORFLOW:
+                perm = perm_keras2pytorch(n_dims)
+                input = _permute(perm)(input)
+            out = std(input, axis=dim, unbiased=unbiased, keepdims=keepdim)
+            out = set_channel_order(out, ChannelOrder.PYTORCH)
+            return out
+    return func
+
+
 @converter(torch.sin, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_sin(input, *args, **kwargs):
     def func(input, *args, **kwargs):
         return tf.math.sin(input)
     return func
```

### Comparing `nobuco-0.6.0/nobuco/node_converters/misc.py` & `nobuco-0.6.1/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/normalization.py` & `nobuco-0.6.1/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/padding.py` & `nobuco-0.6.1/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/pooling.py` & `nobuco-0.6.1/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/recurrent.py` & `nobuco-0.6.1/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/slice.py` & `nobuco-0.6.1/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/node_converters/tensor_cast.py` & `nobuco-0.6.1/nobuco/node_converters/tensor_cast.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,18 @@
         tf_type = tf.float64
     elif dtype == torch.int32:
         tf_type = tf.int32
     elif dtype == torch.int64:
         tf_type = tf.int64
     elif dtype == torch.bool:
         tf_type = tf.bool
+    elif dtype == torch.complex64:
+        tf_type = tf.complex64
+    elif dtype == torch.complex128:
+        tf_type = tf.complex128
     elif dtype is None:
         tf_type = None
     else:
         raise Exception('Unsupported dtype: ', dtype)
     return tf_type
```

### Comparing `nobuco-0.6.0/nobuco/node_converters/tensor_creation.py` & `nobuco-0.6.1/nobuco/node_converters/tensor_creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,7 +130,14 @@
         _mask_is_float = torch.is_floating_point(mask)
         if not _mask_is_float:
             raise Exception('Not supported yet')
 
     def func(mask, mask_name, other_type, other_name, target_type, check_other=True):
         return mask
     return func
+
+
+@converter(torch.complex, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_complex(real: Tensor, imag: Tensor, *, out: Optional[Tensor]=None):
+    def func(real, imag, *, out=None):
+        return tf.complex(real, imag)
+    return func
```

### Comparing `nobuco-0.6.0/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.6.1/nobuco/node_converters/tensor_manipulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,22 @@
     perm = np.swapaxes(a, dim0, dim1).shape
 
     def func(input, dim0, dim1):
         return _permute_inner(perm)(input)
     return func
 
 
+@converter(torch.Tensor.t, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_t(self: Tensor):
+    assert self.dim() == 2
+    def func(self):
+        return tf.transpose(self, perm=(1, 0))
+    return func
+
+
 # tensor.T
 @converter(torch.Tensor.__getattribute__, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_getattribute(self, attribute):
     if attribute == 'T':
         def func(self, attribute):
             return _permute_inner([1, 0])(self)
     else:
```

### Comparing `nobuco-0.6.0/nobuco/trace/tensor_storage.py` & `nobuco-0.6.1/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/trace/trace.py` & `nobuco-0.6.1/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/util.py` & `nobuco-0.6.1/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/vis/console_stylizer.py` & `nobuco-0.6.1/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco/vis/html_stylizer.py` & `nobuco-0.6.1/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/nobuco.egg-info/PKG-INFO` & `nobuco-0.6.1/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.6.0
+Version: 0.6.1
 Summary: Pytorch to Tensorflow conversion made intuitive
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
 Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
 Keywords: pytorch,tensorflow,keras,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nobuco-0.6.0/nobuco.egg-info/SOURCES.txt` & `nobuco-0.6.1/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.0/pyproject.toml` & `nobuco-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.6.0"
+version = "0.6.1"
 description = "Pytorch to Tensorflow conversion made intuitive"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

