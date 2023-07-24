# Comparing `tmp/fastlane_bot-0.88.1.tar.gz` & `tmp/fastlane_bot-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlane_bot-0.88.1.tar", last modified: Mon Jul 24 11:48:22 2023, max compression
+gzip compressed data, was "fastlane_bot-0.9.1.tar", last modified: Fri Jul 21 19:12:21 2023, max compression
```

## Comparing `fastlane_bot-0.88.1.tar` & `fastlane_bot-0.9.1.tar`

### file list

```diff
@@ -1,102 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.158315 fastlane_bot-0.88.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-24 11:48:22.158315 fastlane_bot-0.88.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.142315 fastlane_bot-0.88.1/fastlane_bot/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44456 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.146315 fastlane_bot-0.88.1/fastlane_bot/config/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/config/cloaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/config/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/config/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/config/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/config/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/config/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/config/selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.146315 fastlane_bot-0.88.1/fastlane_bot/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   192059 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/data/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/data/pools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.146315 fastlane_bot-0.88.1/fastlane_bot/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.150315 fastlane_bot-0.88.1/fastlane_bot/events/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/exchanges/bancor_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/exchanges/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/exchanges/carbon_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/exchanges/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/exchanges/sushiswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/exchanges/uniswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/exchanges/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.150315 fastlane_bot-0.88.1/fastlane_bot/events/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/managers/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/managers/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/managers/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/managers/pools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.150315 fastlane_bot-0.88.1/fastlane_bot/events/pools/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/pools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/pools/bancor_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/pools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/pools/carbon_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/pools/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/pools/sushiswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/pools/uniswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/pools/uniswap_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.154315 fastlane_bot-0.88.1/fastlane_bot/events/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/tests/convert_py_test_to_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/tests/test_exchanges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/tests/test_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.154315 fastlane_bot-0.88.1/fastlane_bot/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/helpers/poolandtokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/helpers/receipthandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/helpers/routehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/helpers/submithandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/helpers/tradeinstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/helpers/txhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/helpers/univ3calc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.154315 fastlane_bot-0.88.1/fastlane_bot/modes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/modes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/modes/base_pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/modes/base_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/modes/pairwise_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/modes/pairwise_single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.158315 fastlane_bot-0.88.1/fastlane_bot/modes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/modes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/modes/tests/test_pairwise_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/modes/triangle_bancor_v3_two_hop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/modes/triangle_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/modes/triangle_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/modes/triangle_single_bancor3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.158315 fastlane_bot-0.88.1/fastlane_bot/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/tools/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    75829 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/tools/arbgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85741 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/tools/cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/tools/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/tools/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/tools/simplepair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/tools/tokenscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/tools/univ3calc_DELETE.py
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/fastlane_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:48:22.142315 fastlane_bot-0.88.1/fastlane_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-24 11:48:22.000000 fastlane_bot-0.88.1/fastlane_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-24 11:48:22.000000 fastlane_bot-0.88.1/fastlane_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:48:22.000000 fastlane_bot-0.88.1/fastlane_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 11:48:22.000000 fastlane_bot-0.88.1/fastlane_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 11:48:22.000000 fastlane_bot-0.88.1/fastlane_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 11:48:22.158315 fastlane_bot-0.88.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-24 11:46:41.000000 fastlane_bot-0.88.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:21.002983 fastlane_bot-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-21 19:12:21.002983 fastlane_bot-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.990982 fastlane_bot-0.9.1/fastlane_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43066 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.994982 fastlane_bot-0.9.1/fastlane_bot/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/cloaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.994982 fastlane_bot-0.9.1/fastlane_bot/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192059 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/data/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/data/pools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.994982 fastlane_bot-0.9.1/fastlane_bot/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.994982 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/bancor_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/carbon_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/sushiswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/uniswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.994982 fastlane_bot-0.9.1/fastlane_bot/events/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/managers/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/managers/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/managers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/managers/pools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.998983 fastlane_bot-0.9.1/fastlane_bot/events/pools/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/bancor_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/carbon_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/sushiswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/uniswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/uniswap_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.998983 fastlane_bot-0.9.1/fastlane_bot/events/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/convert_py_test_to_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/test_exchanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/test_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.998983 fastlane_bot-0.9.1/fastlane_bot/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/poolandtokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/receipthandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/routehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/submithandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/tradeinstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/txhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/univ3calc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:21.002983 fastlane_bot-0.9.1/fastlane_bot/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/base_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/base_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/pairwise_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/pairwise_single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:21.002983 fastlane_bot-0.9.1/fastlane_bot/modes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/tests/test_pairwise_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/triangle_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/triangle_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/triangle_single_bancor3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:21.002983 fastlane_bot-0.9.1/fastlane_bot/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75829 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/arbgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85741 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/simplepair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/tokenscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/univ3calc_DELETE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.990982 fastlane_bot-0.9.1/fastlane_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-21 19:12:20.000000 fastlane_bot-0.9.1/fastlane_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-21 19:12:20.000000 fastlane_bot-0.9.1/fastlane_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:12:20.000000 fastlane_bot-0.9.1/fastlane_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-21 19:12:20.000000 fastlane_bot-0.9.1/fastlane_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 19:12:20.000000 fastlane_bot-0.9.1/fastlane_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:12:21.002983 fastlane_bot-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/setup.py
```

### Comparing `fastlane_bot-0.88.1/LICENSE` & `fastlane_bot-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/PKG-INFO` & `fastlane_bot-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlane_bot
-Version: 0.88.1
+Version: 0.9.1
 Summary: Carbon Arbitrage Bot, an open-source arbitrage protocol, allows any user to perform arbitrage between Bancor ecosystem protocols and external exchanges and redirect arbitrage profits back to the protocol.
 Home-page: https://github.com/bancorprotocol/carbon-bot
 Author: Bancor Network
 Author-email: mike@bancor.network
 Requires-Python: >= 3.8, != 3.11.*
 Description-Content-Type: text/markdown
 Provides-Extra: complete
```

### Comparing `fastlane_bot-0.88.1/README.md` & `fastlane_bot-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/bot.py` & `fastlane_bot-0.9.1/fastlane_bot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 from fastlane_bot.tools.optimizer import CPCArbOptimizer
 from .events.interface import QueryInterface
 from .modes.pairwise_multi import FindArbitrageMultiPairwise
 from .modes.pairwise_single import FindArbitrageSinglePairwise
 from .modes.triangle_multi import ArbitrageFinderTriangleMulti
 from .modes.triangle_single import ArbitrageFinderTriangleSingle
 from .modes.triangle_single_bancor3 import ArbitrageFinderTriangleSingleBancor3
-from .modes.triangle_bancor_v3_two_hop import ArbitrageFinderTriangleBancor3TwoHop
 from .utils import num_format, log_format, num_format_float
 
 
 @dataclass
 class CarbonBotBase:
     """
     Base class for the business logic of the bot.
@@ -415,25 +414,23 @@
             return FindArbitrageMultiPairwise
         elif arb_mode in {"triangle", "triangle_single"}:
             return ArbitrageFinderTriangleSingle
         elif arb_mode in {"multi_triangle", "triangle_multi"}:
             return ArbitrageFinderTriangleMulti
         elif arb_mode in {"bancor_v3", "single_triangle_bancor3"}:
             return ArbitrageFinderTriangleSingleBancor3
-        elif arb_mode in {"b3_two_hop"}:
-            return ArbitrageFinderTriangleBancor3TwoHop
 
     def _run(
         self,
         flashloan_tokens: List[str],
         CCm: CPCContainer,
         *,
         result=None,
         arb_mode: str = None,
-        randomizer=int,
+        randomizer=True,
         data_validator=True,
     ) -> Optional[Tuple[str, List[Any]]]:
         """
         Runs the bot.
 
         Parameters
         ----------
@@ -441,16 +438,16 @@
             The tokens to flashloan.
         CCm: CPCContainer
             The container.
         result: str
             The result type.
         arb_mode: str
             The arbitrage mode.
-        randomizer: int
-            randomizer (int): The number of arb opportunities to randomly pick from, sorted by expected profit.
+        randomizer: bool
+            Whether to randomize the arbitrage opportunities.
         data_validator: bool
             If extra data validation should be performed
 
         Returns
         -------
         Optional[Tuple[str, List[Any]]]
             The result.
@@ -472,15 +469,15 @@
             return r
 
         if r is None or len(r) == 0:
             self.ConfigObj.logger.info("No eligible arb opportunities.")
             return None
 
         self.ConfigObj.logger.info(f"Found {len(r)} eligible arb opportunities.")
-        r = self.randomize(arb_opps=r, randomizer=randomizer)
+        r = random.choice(r) if randomizer else r
         if data_validator or arb_mode == "bancor_v3":
             # Add random chance if we should check or not
             r = self.validate_optimizer_trades(arb_opp=r, arb_mode=arb_mode, arb_finder=finder)
             if r is None:
                 self.ConfigObj.logger.info("Math validation eliminated arb opportunity, restarting.")
                 return None
             if self.validate_pool_data(arb_opp=r):
@@ -520,15 +517,15 @@
 
         (
             ordered_trade_instructions_dct,
             tx_in_count,
         ) = self._simple_ordering_by_src_token(
             best_trade_instructions_dic, best_src_token
         )
-        if arb_mode == "bancor_v3" or arb_mode == "b3_two_hop":
+        if arb_mode == "bancor_v3":
 
             cids = []
             for pool in ordered_trade_instructions_dct:
                 pool_cid = pool["cid"]
                 if "-0" in pool_cid or "-1" in pool_cid:
                     self.ConfigObj.logger.debug(f"Math arb validation not currently supported for arbs with Carbon, returning to main flow.")
                     return arb_opp
@@ -614,36 +611,14 @@
 
             elif current_pool.tkn0_balance != fetched_pool["tkn0_balance"] or current_pool.tkn1_balance != fetched_pool["tkn1_balance"]:
                 self.ConfigObj.logger.debug(f"{ex_name} pool not up to date, updating and restarting.")
                 return False
             
         return True
 
-    @staticmethod
-    def randomize(arb_opps, randomizer: int = 1):
-        """
-        Sorts arb opportunities by profit, then returns a random element from the top N arbs, with N being the value input in randomizer.
-        :param arb_opps: Arb opportunities
-        :param randomizer: the number of arb ops to choose from after sorting by profit. For example, a value of 3 would be the top 3 arbs by profitability.
-        returns:
-            A randomly selected arb opportunity.
-
-        """
-        if arb_opps is None:
-            return None
-        if len(arb_opps) > 0:
-            arb_opps.sort(key=lambda x: x[0], reverse=True)
-            if randomizer < 1:
-                randomizer = 1
-            if len(arb_opps) < randomizer:
-                randomizer = len(arb_opps)
-            top_n_arbs = arb_opps[:randomizer]
-            return random.choice(top_n_arbs)
-        else:
-            return None
     def _validate_pool_data_logging(self, pool_cid: str, fetched_pool: Dict[str, Any]) -> None:
         """
         Logs the pool data validation.
 
         Parameters
         ----------
         pool_cid: str
@@ -827,19 +802,14 @@
         )
 
         # Calculate the trade instructions
         calculated_trade_instructions = tx_route_handler.calculate_trade_outputs(
             agg_trade_instructions
         )
 
-        # Aggregate multiple Bancor V3 trades into a single trade
-        calculated_trade_instructions = tx_route_handler.aggregate_bancor_v3_trades(
-            calculated_trade_instructions
-        )
-
         # Get the flashloan token
         fl_token = fl_token_with_weth = calculated_trade_instructions[0].tknin_key
 
         # If the flashloan token is WETH, then use ETH
         if fl_token == T.WETH:
             fl_token = T.NATIVE_ETH
 
@@ -898,15 +868,15 @@
         self.handle_logging_for_trade_instructions(
             3, # The log id
             flashloan_amount=flashloan_amount,
         )
 
         # Encode the trade instructions
         encoded_trade_instructions = tx_route_handler.custom_data_encoder(
-            calculated_trade_instructions
+            agg_trade_instructions
         )
 
         # Get the deadline
         deadline = self._get_deadline()
 
         # Get the route struct
         route_struct = [
@@ -1159,15 +1129,15 @@
                     (x.params.tkny_addr == self.ConfigObj.WETH_ADDRESS)
                     or (x.params.tknx_addr == self.ConfigObj.WETH_ADDRESS)
                 )
             ]
             CCm = CPCContainer([x for x in CCm if x not in filter_out_weth])
         return CCm
 
-    def run_continuous_mode(self, flashloan_tokens: List[str], arb_mode: str, run_data_validator: bool, randomizer: int):
+    def run_continuous_mode(self, flashloan_tokens: List[str], arb_mode: str, run_data_validator: bool, randomizer: bool):
         """
         Run the bot in continuous mode.
 
         Parameters
         ----------
         flashloan_tokens: List[str]
             The flashloan tokens
@@ -1196,15 +1166,15 @@
             except self.NoArbAvailable as e:
                 self.ConfigObj.logger.debug(f"[bot:run:single] {e}")
             except Exception as e:
                 self.ConfigObj.logger.error(f"[bot:run:continuous] {e}")
                 time.sleep(self.polling_interval)
 
     def run_single_mode(
-        self, flashloan_tokens: List[str], CCm: CPCContainer, arb_mode: str, run_data_validator: bool, randomizer: int
+        self, flashloan_tokens: List[str], CCm: CPCContainer, arb_mode: str, run_data_validator: bool, randomizer: bool
     ):
         """
         Run the bot in single mode.
 
         Parameters
         ----------
         flashloan_tokens: List[str]
@@ -1231,15 +1201,15 @@
         *,
         flashloan_tokens: List[str] = None,
         CCm: CPCContainer = None,
         polling_interval: int = None,
         mode: str = None,
         arb_mode: str = None,
         run_data_validator: bool = False,
-        randomizer: int = 0
+        randomizer: bool = False
     ):
         """
         Runs the bot.
 
         Parameters
         ----------
         flashloan_tokens: List[str]
```

### Comparing `fastlane_bot-0.88.1/fastlane_bot/config/base.py` & `fastlane_bot-0.9.1/fastlane_bot/config/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/config/cloaker.py` & `fastlane_bot-0.9.1/fastlane_bot/config/cloaker.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/config/config.py` & `fastlane_bot-0.9.1/fastlane_bot/config/config.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/config/connect.py` & `fastlane_bot-0.9.1/fastlane_bot/config/connect.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/config/db.py` & `fastlane_bot-0.9.1/fastlane_bot/config/db.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/config/logger.py` & `fastlane_bot-0.9.1/fastlane_bot/config/logger.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/config/network.py` & `fastlane_bot-0.9.1/fastlane_bot/config/network.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/config/provider.py` & `fastlane_bot-0.9.1/fastlane_bot/config/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             address=self.w3.toChecksumAddress(N.FASTLANE_CONTRACT_ADDRESS),
             abi=FAST_LANE_CONTRACT_ABI,
         )
         reward_percent, max_profit = self.BANCOR_ARBITRAGE_CONTRACT.caller.rewards()
 
         self.ARB_REWARD_PERCENTAGE = str(int(reward_percent) / 1000000)
         self.ARB_MAX_PROFIT = str(int(max_profit) / (10 ** 18))
-        self.EXPECTED_GAS_MODIFIER = "0.85"
+        self.EXPECTED_GAS_MODIFIER = "0.8"
 
 
 class _ConfigProviderTenderly(ConfigProvider):
     """
     Fastlane bot config -- provider [Tenderly]
     """
     PROVIDER = S.PROVIDER_TENDERLY
```

### Comparing `fastlane_bot-0.88.1/fastlane_bot/config/selectors.py` & `fastlane_bot-0.9.1/fastlane_bot/config/selectors.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/data/abi.py` & `fastlane_bot-0.9.1/fastlane_bot/data/abi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/data/pools.py` & `fastlane_bot-0.9.1/fastlane_bot/data/pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/exchanges/__init__.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/exchanges/bancor_v3.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/bancor_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/exchanges/base.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/exchanges/carbon_v1.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/carbon_v1.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/exchanges/factory.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/factory.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/exchanges/sushiswap_v2.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/sushiswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/exchanges/uniswap_v2.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/uniswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/exchanges/uniswap_v3.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/interface.py` & `fastlane_bot-0.9.1/fastlane_bot/events/interface.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/managers/base.py` & `fastlane_bot-0.9.1/fastlane_bot/events/managers/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/managers/contracts.py` & `fastlane_bot-0.9.1/fastlane_bot/events/managers/contracts.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/managers/events.py` & `fastlane_bot-0.9.1/fastlane_bot/events/managers/events.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/managers/manager.py` & `fastlane_bot-0.9.1/fastlane_bot/events/managers/manager.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/managers/pools.py` & `fastlane_bot-0.9.1/fastlane_bot/events/managers/pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/pools/__init__.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/pools/bancor_v3.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/bancor_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/pools/base.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/pools/carbon_v1.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/carbon_v1.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/pools/factory.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/factory.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/pools/sushiswap_v2.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/sushiswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/pools/uniswap_v2.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/uniswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/pools/uniswap_v3.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/tests/convert_py_test_to_jupyter.py` & `fastlane_bot-0.9.1/fastlane_bot/events/tests/convert_py_test_to_jupyter.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/tests/test_exchanges.py` & `fastlane_bot-0.9.1/fastlane_bot/events/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/tests/test_interface.py` & `fastlane_bot-0.9.1/fastlane_bot/events/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/tests/test_manager.py` & `fastlane_bot-0.9.1/fastlane_bot/events/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/tests/test_pools.py` & `fastlane_bot-0.9.1/fastlane_bot/events/tests/test_pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/tests/test_utils.py` & `fastlane_bot-0.9.1/fastlane_bot/events/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/events/utils.py` & `fastlane_bot-0.9.1/fastlane_bot/events/utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/helpers/poolandtokens.py` & `fastlane_bot-0.9.1/fastlane_bot/helpers/poolandtokens.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/helpers/routehandler.py` & `fastlane_bot-0.9.1/fastlane_bot/helpers/routehandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,52 +363,15 @@
         slices.append(df.loc[current_slice])
 
         min_index = []
         for df in slices:
             min_index += [min(df.index.values)]
 
         return list(zip(min_index, slices))
-
-    @staticmethod
-    def aggregate_bancor_v3_trades(calculated_trade_instructions: List[TradeInstruction]):
-        """
-        This function aggregates Bancor V3 trades into a single multi-hop when possible
-
-        Parameters
-        ----------
-        calculated_trade_instructions: List[TradeInstruction]
-            Trade instructions that have already had trades calculated
-
-
-        Returns
-        -------
-        calculated_trade_instructions
-            The trade instructions now with Bancor V3 trades combined into single trades when possible.
-        """
-
-        for idx, trade in enumerate(calculated_trade_instructions):
-            if idx > 0:
-                if trade.exchange_name == "bancor_v3" and calculated_trade_instructions[idx - 1].exchange_name == "bancor_v3":
-                    trade_before = calculated_trade_instructions[idx - 1]
-                    # This checks for a two-hop trade through BNT and combines them
-                    if trade_before.tknout_key == "BNT-FF1C" and trade.tknin_key == "BNT-FF1C":
-                        new_trade_instruction = TradeInstruction(ConfigObj=trade.ConfigObj, cid=trade_before.cid,
-                                                                 amtin=trade_before.amtin, amtout=trade.amtout,
-                                                                 tknin=trade_before.tknin_key, tknout=trade.tknout_key,
-                                                                 pair_sorting="", raw_txs="[]", db=trade.db)
-                        calculated_trade_instructions[idx - 1] = new_trade_instruction
-                        calculated_trade_instructions.pop(idx)
-
-        return calculated_trade_instructions
-
-
-
-
-
-
+ 
     def aggregate_carbon_trades(self, trade_instructions_objects: List[TradeInstruction]) -> List[TradeInstruction]:
         """
         Aggregate carbon independent IDs and create trade instructions.
 
         This function takes a list of dictionaries containing trade instructions,
         aggregates the instructions with carbon independent IDs, and creates
         a list of TradeInstruction objects.
```

### Comparing `fastlane_bot-0.88.1/fastlane_bot/helpers/submithandler.py` & `fastlane_bot-0.9.1/fastlane_bot/helpers/submithandler.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/helpers/tradeinstruction.py` & `fastlane_bot-0.9.1/fastlane_bot/helpers/tradeinstruction.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/helpers/txhelpers.py` & `fastlane_bot-0.9.1/fastlane_bot/helpers/txhelpers.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/helpers/univ3calc.py` & `fastlane_bot-0.9.1/fastlane_bot/helpers/univ3calc.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/modes/base.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/modes/base_pairwise.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/base_pairwise.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/modes/base_triangle.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/base_triangle.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         Returns
         -------
         combos : list
             List of combos
 
         """
         combos = []
-        if arb_mode in ["single_triangle_bancor3", "bancor_v3", "b3_two_hop"]:
+        if arb_mode in ["single_triangle_bancor3", "bancor_v3"]:
             combos = [
                 (tkn0, tkn1)
                 for tkn0, tkn1 in itertools.product(flashloan_tokens, flashloan_tokens)
                 # note that the pair is tkn0/tkn1, ie tkn1 is the quote token
                 if tkn0 != tkn1
             ]
         else:
@@ -148,15 +148,15 @@
                         arb_mode,
                         combos,
                     )
         return combos
 
     @staticmethod
     def get_mono_direction_carbon_curves(
-        miniverse: List[Any], trade_instructions_df: pd.DataFrame, token_in: str=None
+        miniverse: List[Any], token_in: str, trade_instructions_df: pd.DataFrame
     ) -> List[Any]:
         """
         Get mono direction carbon curves for triangular arbitrage
 
         Parameters
         ----------
         miniverse : list
```

### Comparing `fastlane_bot-0.88.1/fastlane_bot/modes/pairwise_multi.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/pairwise_multi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/modes/pairwise_single.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/pairwise_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/modes/tests/test_pairwise_single.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/tests/test_pairwise_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/modes/triangle_bancor_v3_two_hop.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/triangle_single_bancor3.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 from typing import Union, List, Tuple, Any, Iterable
 
 from fastlane_bot.modes.base_triangle import ArbitrageFinderTriangleBase
 from fastlane_bot.tools.cpc import CPCContainer, T, ConstantProductCurve
 from fastlane_bot.tools.optimizer import CPCArbOptimizer
 
 
-class ArbitrageFinderTriangleBancor3TwoHop(ArbitrageFinderTriangleBase):
+class ArbitrageFinderTriangleSingleBancor3(ArbitrageFinderTriangleBase):
     """
     Bancor V3 triangular arbitrage finder mode
     """
 
-    arb_mode = "b3_two_hop"
+    arb_mode = "single_triangle_bancor3"
 
     def find_arbitrage(self, candidates: List[Any] = None, ops: Tuple = None, best_profit: float = 0, profit_src: float = 0) -> Union[List, Tuple]:
         """
         see base.py
         """
         if self.base_exchange != "bancor_v3":
             self.ConfigObj.logger.warning(
@@ -115,15 +115,15 @@
                 trade_instructions_dic,
                 src_token,
                 trade_instructions,
             )
 
         return candidates if self.result == self.AO_CANDIDATES else ops
 
-    def get_tkn(self, pool: Any, tkn_num: int) -> str:
+    def get_tkn(self, pool: ConstantProductCurve, tkn_num: int) -> str:
         """
         Gets the token ID from a pool object
 
         Parameters
         ----------
         pool: ConstantProductCurve
             The ConstantProductCurve object
@@ -181,28 +181,31 @@
         flt: str
 
         Returns
         -------
         float
         """
         pools = self.get_exact_pools(cids=cids)
-        tkn1 = self.get_tkn(pool=pools[0], tkn_num=1) if self.get_tkn(pool=pools[0], tkn_num=1) != flt else self.get_tkn(pool=pools[0], tkn_num=0)
-        p0t0 = pools[0].x if self.get_tkn(pool=pools[0], tkn_num=0) == flt else pools[0].y
-        p0t1 = pools[0].y if self.get_tkn(pool=pools[0], tkn_num=0) == flt else pools[0].x
-        p1t0 = pools[1].x if tkn1 == self.get_tkn(pool=pools[1], tkn_num=0) else pools[1].y
-        p1t1 = pools[1].y if tkn1 == self.get_tkn(pool=pools[1], tkn_num=0) else pools[1].x
-        p2t0 = pools[2].x if self.get_tkn(pool=pools[2], tkn_num=0) != flt else pools[2].y
-        p2t1 = pools[2].y if self.get_tkn(pool=pools[2], tkn_num=0) != flt else pools[2].x
-        fee0 = self.get_fee_safe(pools[0].fee)
+        tkn0 = self.get_tkn(pool=pools[0], tkn_num=0)
+        tkn1 = self.get_tkn(pool=pools[0], tkn_num=1)
+        tkn2 = self.get_tkn(pool=pools[1], tkn_num=0)
+        tkn5 = self.get_tkn(pool=pools[2], tkn_num=0)
+        p0t0 = pools[0].x_act if tkn0 == flt else pools[0].y_act
+        p0t1 = pools[0].y_act if tkn0 == flt else pools[0].x_act
+        p2t1 = pools[2].x_act if tkn5 == flt else pools[2].y_act
+        p2t0 = pools[2].y_act if tkn5 == flt else pools[2].x_act
         fee1 = self.get_fee_safe(pools[1].fee)
-        fee2 = self.get_fee_safe(pools[2].fee)
 
         if pools[1].params.exchange == "carbon_v1":
             return self.get_exact_input_with_carbon(p0t0, p0t1, p2t0, p2t1, pools[1])
 
+        p1t0 = pools[1].x if tkn1 == tkn2 else pools[1].y
+        p1t1 = pools[1].y if tkn1 == tkn2 else pools[1].x
+        fee0 = 0
+        fee2 = 0
         return self.max_arb_trade_in_constant_product(p0t0, p0t1, p1t0, p1t1, p2t0, p2t1, fee0=fee0, fee1=fee1, fee2=fee2)
 
     def get_exact_input_with_carbon(self, p0t0: float, p0t1: float, p2t0: float, p2t1: float, carbon_pool: ConstantProductCurve) -> float:
         """
         Gets the optimal trade 0 amount for a triangular arb cycle with a single Carbon order in the middle
 
         Parameters
@@ -213,18 +216,18 @@
         p2t1: float
         carbon_pool: ConstantProductCurve
 
         Returns
         -------
         float
         """
-        y = carbon_pool.y
-        z = carbon_pool.z
-        A = carbon_pool.A
-        B = carbon_pool.B
+        y = carbon_pool.params['y']
+        z = carbon_pool.params['yint']
+        A = carbon_pool.params['A']
+        B = carbon_pool.params['B']
         C = (B * z + A * y) ** 2
         D = B * A * z + A ** 2 * y
         return self.max_arb_trade_in_cp_carbon_cp(p0t0, p0t1, p2t0, p2t1, C, D, z)
 
     @staticmethod
     def max_arb_trade_in_cp_carbon_cp(p0t0: float, p0t1: float, p2t0: float, p2t1: float, C: float, D: float, z: float) -> float:
         """
@@ -347,15 +350,15 @@
 
             bancor_v3_curve_0 = (
                 self.CCm.bypairs(f"{T.BNT}/{tkn0}")
                 .byparams(exchange="bancor_v3")
                 .curves
             )
             bancor_v3_curve_1 = (
-                self.CCm.bypairs(f"{T.BNT}/{tkn1}")
+                self.CCm.bypairs(f"BNT-FF1C/{tkn1}")
                 .byparams(exchange="bancor_v3")
                 .curves
             )
             if bancor_v3_curve_0 is None or bancor_v3_curve_1 is None:
                 continue
             if len(bancor_v3_curve_0) == 0 or len(bancor_v3_curve_1) == 0:
                 continue
@@ -364,9 +367,9 @@
             if external_curves:
                 for curve in external_curves:
                     miniverses += [bancor_v3_curve_0 + bancor_v3_curve_1 + [curve]]
             if carbon_curves:
                 miniverses += [bancor_v3_curve_0 + bancor_v3_curve_1 + carbon_curves]
 
             if len(miniverses) > 0:
-                all_miniverses += list(zip([tkn1] * len(miniverses), miniverses))
+                all_miniverses += list(zip([T.BNT] * len(miniverses), miniverses))
         return all_miniverses
```

### Comparing `fastlane_bot-0.88.1/fastlane_bot/modes/triangle_multi.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/triangle_multi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/modes/triangle_single.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/triangle_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/testing.py` & `fastlane_bot-0.9.1/fastlane_bot/testing.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/tools/analyzer.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/analyzer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/tools/arbgraphs.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/arbgraphs.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/tools/cpc.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/cpc.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/tools/optimizer.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/optimizer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/tools/params.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/params.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/tools/simplepair.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/simplepair.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/tools/tokenscale.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/tokenscale.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/tools/univ3calc_DELETE.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/univ3calc_DELETE.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot/utils.py` & `fastlane_bot-0.9.1/fastlane_bot/utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.88.1/fastlane_bot.egg-info/PKG-INFO` & `fastlane_bot-0.9.1/fastlane_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlane-bot
-Version: 0.88.1
+Version: 0.9.1
 Summary: Carbon Arbitrage Bot, an open-source arbitrage protocol, allows any user to perform arbitrage between Bancor ecosystem protocols and external exchanges and redirect arbitrage profits back to the protocol.
 Home-page: https://github.com/bancorprotocol/carbon-bot
 Author: Bancor Network
 Author-email: mike@bancor.network
 Requires-Python: >= 3.8, != 3.11.*
 Description-Content-Type: text/markdown
 Provides-Extra: complete
```

### Comparing `fastlane_bot-0.88.1/fastlane_bot.egg-info/SOURCES.txt` & `fastlane_bot-0.9.1/fastlane_bot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 fastlane_bot/helpers/univ3calc.py
 fastlane_bot/modes/__init__.py
 fastlane_bot/modes/base.py
 fastlane_bot/modes/base_pairwise.py
 fastlane_bot/modes/base_triangle.py
 fastlane_bot/modes/pairwise_multi.py
 fastlane_bot/modes/pairwise_single.py
-fastlane_bot/modes/triangle_bancor_v3_two_hop.py
 fastlane_bot/modes/triangle_multi.py
 fastlane_bot/modes/triangle_single.py
 fastlane_bot/modes/triangle_single_bancor3.py
 fastlane_bot/modes/tests/__init__.py
 fastlane_bot/modes/tests/test_pairwise_single.py
 fastlane_bot/tools/__init__.py
 fastlane_bot/tools/analyzer.py
```

### Comparing `fastlane_bot-0.88.1/setup.py` & `fastlane_bot-0.9.1/setup.py`

 * *Files identical despite different names*

