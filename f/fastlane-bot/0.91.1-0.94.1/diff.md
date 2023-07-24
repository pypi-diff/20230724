# Comparing `tmp/fastlane_bot-0.91.1.tar.gz` & `tmp/fastlane_bot-0.94.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlane_bot-0.91.1.tar", last modified: Mon Jul 24 11:55:43 2023, max compression
+gzip compressed data, was "fastlane_bot-0.94.1.tar", last modified: Mon Jul 24 17:59:12 2023, max compression
```

## Comparing `fastlane_bot-0.91.1.tar` & `fastlane_bot-0.94.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.885092 fastlane_bot-0.91.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-24 11:55:43.885092 fastlane_bot-0.91.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.873092 fastlane_bot-0.91.1/fastlane_bot/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44456 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.877092 fastlane_bot-0.91.1/fastlane_bot/config/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/config/cloaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/config/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/config/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/config/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/config/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/config/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/config/selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.877092 fastlane_bot-0.91.1/fastlane_bot/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   192059 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/data/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/data/pools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.877092 fastlane_bot-0.91.1/fastlane_bot/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.877092 fastlane_bot-0.91.1/fastlane_bot/events/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/exchanges/bancor_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/exchanges/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/exchanges/carbon_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/exchanges/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/exchanges/sushiswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/exchanges/uniswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/exchanges/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.877092 fastlane_bot-0.91.1/fastlane_bot/events/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/managers/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/managers/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/managers/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/managers/pools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.877092 fastlane_bot-0.91.1/fastlane_bot/events/pools/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/pools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/pools/bancor_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/pools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/pools/carbon_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/pools/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/pools/sushiswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/pools/uniswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/pools/uniswap_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.881092 fastlane_bot-0.91.1/fastlane_bot/events/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/tests/convert_py_test_to_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/tests/test_exchanges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/tests/test_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.881092 fastlane_bot-0.91.1/fastlane_bot/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/helpers/poolandtokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/helpers/receipthandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/helpers/routehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/helpers/submithandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/helpers/tradeinstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/helpers/txhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/helpers/univ3calc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.881092 fastlane_bot-0.91.1/fastlane_bot/modes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/modes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/modes/base_pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/modes/base_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/modes/pairwise_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/modes/pairwise_single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.881092 fastlane_bot-0.91.1/fastlane_bot/modes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/modes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/modes/tests/test_pairwise_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/modes/triangle_bancor_v3_two_hop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/modes/triangle_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/modes/triangle_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/modes/triangle_single_bancor3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.885092 fastlane_bot-0.91.1/fastlane_bot/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/tools/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    75829 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/tools/arbgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85741 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/tools/cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/tools/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/tools/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/tools/simplepair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/tools/tokenscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/tools/univ3calc_DELETE.py
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/fastlane_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:55:43.873092 fastlane_bot-0.91.1/fastlane_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-24 11:55:43.000000 fastlane_bot-0.91.1/fastlane_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-24 11:55:43.000000 fastlane_bot-0.91.1/fastlane_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:55:43.000000 fastlane_bot-0.91.1/fastlane_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 11:55:43.000000 fastlane_bot-0.91.1/fastlane_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 11:55:43.000000 fastlane_bot-0.91.1/fastlane_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 11:55:43.885092 fastlane_bot-0.91.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-24 11:54:28.000000 fastlane_bot-0.91.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.731870 fastlane_bot-0.94.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-24 17:59:12.731870 fastlane_bot-0.94.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.719871 fastlane_bot-0.94.1/fastlane_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44456 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.723871 fastlane_bot-0.94.1/fastlane_bot/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/config/cloaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/config/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/config/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/config/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/config/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/config/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.723871 fastlane_bot-0.94.1/fastlane_bot/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192059 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/data/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/data/pools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.723871 fastlane_bot-0.94.1/fastlane_bot/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.723871 fastlane_bot-0.94.1/fastlane_bot/events/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/exchanges/bancor_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/exchanges/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/exchanges/carbon_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/exchanges/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/exchanges/sushiswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/exchanges/uniswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/exchanges/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.723871 fastlane_bot-0.94.1/fastlane_bot/events/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/managers/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/managers/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/managers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/managers/pools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.723871 fastlane_bot-0.94.1/fastlane_bot/events/pools/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/pools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/pools/bancor_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/pools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/pools/carbon_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/pools/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/pools/sushiswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/pools/uniswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/pools/uniswap_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.727870 fastlane_bot-0.94.1/fastlane_bot/events/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/tests/convert_py_test_to_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/tests/test_exchanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/tests/test_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.727870 fastlane_bot-0.94.1/fastlane_bot/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/helpers/poolandtokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/helpers/receipthandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/helpers/routehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/helpers/submithandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/helpers/tradeinstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/helpers/txhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/helpers/univ3calc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.727870 fastlane_bot-0.94.1/fastlane_bot/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/modes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/modes/base_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/modes/base_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/modes/pairwise_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/modes/pairwise_single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.727870 fastlane_bot-0.94.1/fastlane_bot/modes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/modes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/modes/tests/test_pairwise_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/modes/triangle_bancor_v3_two_hop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/modes/triangle_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/modes/triangle_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/modes/triangle_single_bancor3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.731870 fastlane_bot-0.94.1/fastlane_bot/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/tools/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75829 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/tools/arbgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85741 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/tools/cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/tools/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/tools/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/tools/simplepair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/tools/tokenscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/tools/univ3calc_DELETE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/fastlane_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:59:12.719871 fastlane_bot-0.94.1/fastlane_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-24 17:59:12.000000 fastlane_bot-0.94.1/fastlane_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-24 17:59:12.000000 fastlane_bot-0.94.1/fastlane_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:59:12.000000 fastlane_bot-0.94.1/fastlane_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 17:59:12.000000 fastlane_bot-0.94.1/fastlane_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 17:59:12.000000 fastlane_bot-0.94.1/fastlane_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 17:59:12.731870 fastlane_bot-0.94.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-24 17:58:01.000000 fastlane_bot-0.94.1/setup.py
```

### Comparing `fastlane_bot-0.91.1/LICENSE` & `fastlane_bot-0.94.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/PKG-INFO` & `fastlane_bot-0.94.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: fastlane_bot
-Version: 0.91.1
-Summary: Carbon Arbitrage Bot, an open-source arbitrage protocol, allows any user to perform arbitrage between Bancor ecosystem protocols and external exchanges and redirect arbitrage profits back to the protocol.
-Home-page: https://github.com/bancorprotocol/carbon-bot
-Author: Bancor Network
-Author-email: mike@bancor.network
-Requires-Python: >= 3.8, != 3.11.*
-Description-Content-Type: text/markdown
-Provides-Extra: complete
-License-File: LICENSE
-
 # Fastlane Arbitrage Bot
 
 ## ⚠️ WARNING: Use at Your Own Risk
 
 The Fastlane Bot requires an Ethereum private key. **Your funds are AT RISK when you run the Fastlane Arbitrage Bot**. Read the _Preparation_ section below. The bot is provided as-is, with the authors and the Bprotocol Foundation not liable for any losses.
 
 ## Overview
@@ -41,14 +29,19 @@
 cd fastlane-bot
 pip install -r requirements.txt
 python setup.py install
 ```
 
 [sim]:https://github.com/bancorprotocol/carbon-simulator
 
+### Legacy Installation (v1.0)
+You can access the legacy version of the Fastlane Arbitrage Bot, which was solely designed to facilitate single triangle arbitrage transactions which both initiate and conclude with BNT on the Bancor V3 exchange, by referring to the following link:
+
+[github.com/bancorprotocol/fastlane-bot/releases/tag/v1.0](https://github.com/bancorprotocol/fastlane-bot/releases/tag/v1.0)
+
 ### Preparation
 
 The Fastlane Arbitrage Bot needs access to an Ethereum wallet's private key. **THIS KEY IS AT RISK AND SHOULD NOT BE USED ELSEWHERE**. Maintain some ETH in the wallet for gas fees and regularly sweep profits. Supply the private key to the bot using an environment variable, as shown:
 
 ```bash
 set ETH_PRIVATE_KEY_BE_CAREFUL="0x9c..."
 ```
@@ -125,8 +118,8 @@
 ## Change Log
 
 We follow [semantic versioning][semver] (`major.minor.patch`), updating the major number for backward incompatible API changes, minor for compatible changes, and patch for minor patches.
 
 [semver]:https://semver.org/
 
 - **v2.0** - Complete rewrite to include Carbon along with Bancor.
-- **v1.0** - Initial bot version for Bancor protocol pools only.
+- **v1.0** - Initial bot version for Bancor protocol pools only.
```

### Comparing `fastlane_bot-0.91.1/README.md` & `fastlane_bot-0.94.1/fastlane_bot.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: fastlane-bot
+Version: 0.94.1
+Summary: Carbon Arbitrage Bot, an open-source arbitrage protocol, allows any user to perform arbitrage between Bancor ecosystem protocols and external exchanges and redirect arbitrage profits back to the protocol.
+Home-page: https://github.com/bancorprotocol/carbon-bot
+Author: Bancor Network
+Author-email: mike@bancor.network
+Requires-Python: >= 3.8, != 3.11.*
+Description-Content-Type: text/markdown
+Provides-Extra: complete
+License-File: LICENSE
+
 # Fastlane Arbitrage Bot
 
 ## ⚠️ WARNING: Use at Your Own Risk
 
 The Fastlane Bot requires an Ethereum private key. **Your funds are AT RISK when you run the Fastlane Arbitrage Bot**. Read the _Preparation_ section below. The bot is provided as-is, with the authors and the Bprotocol Foundation not liable for any losses.
 
 ## Overview
@@ -29,14 +41,19 @@
 cd fastlane-bot
 pip install -r requirements.txt
 python setup.py install
 ```
 
 [sim]:https://github.com/bancorprotocol/carbon-simulator
 
+### Legacy Installation (v1.0)
+You can access the legacy version of the Fastlane Arbitrage Bot, which was solely designed to facilitate single triangle arbitrage transactions which both initiate and conclude with BNT on the Bancor V3 exchange, by referring to the following link:
+
+[github.com/bancorprotocol/fastlane-bot/releases/tag/v1.0](https://github.com/bancorprotocol/fastlane-bot/releases/tag/v1.0)
+
 ### Preparation
 
 The Fastlane Arbitrage Bot needs access to an Ethereum wallet's private key. **THIS KEY IS AT RISK AND SHOULD NOT BE USED ELSEWHERE**. Maintain some ETH in the wallet for gas fees and regularly sweep profits. Supply the private key to the bot using an environment variable, as shown:
 
 ```bash
 set ETH_PRIVATE_KEY_BE_CAREFUL="0x9c..."
 ```
@@ -113,8 +130,8 @@
 ## Change Log
 
 We follow [semantic versioning][semver] (`major.minor.patch`), updating the major number for backward incompatible API changes, minor for compatible changes, and patch for minor patches.
 
 [semver]:https://semver.org/
 
 - **v2.0** - Complete rewrite to include Carbon along with Bancor.
-- **v1.0** - Initial bot version for Bancor protocol pools only.
+- **v1.0** - Initial bot version for Bancor protocol pools only.
```

### Comparing `fastlane_bot-0.91.1/fastlane_bot/bot.py` & `fastlane_bot-0.94.1/fastlane_bot/bot.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/config/base.py` & `fastlane_bot-0.94.1/fastlane_bot/config/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/config/cloaker.py` & `fastlane_bot-0.94.1/fastlane_bot/config/cloaker.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/config/config.py` & `fastlane_bot-0.94.1/fastlane_bot/config/config.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/config/connect.py` & `fastlane_bot-0.94.1/fastlane_bot/config/connect.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/config/db.py` & `fastlane_bot-0.94.1/fastlane_bot/config/db.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/config/logger.py` & `fastlane_bot-0.94.1/fastlane_bot/config/logger.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/config/network.py` & `fastlane_bot-0.94.1/fastlane_bot/config/network.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/config/provider.py` & `fastlane_bot-0.94.1/fastlane_bot/config/provider.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/config/selectors.py` & `fastlane_bot-0.94.1/fastlane_bot/config/selectors.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/data/abi.py` & `fastlane_bot-0.94.1/fastlane_bot/data/abi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/data/pools.py` & `fastlane_bot-0.94.1/fastlane_bot/data/pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/exchanges/__init__.py` & `fastlane_bot-0.94.1/fastlane_bot/events/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/exchanges/bancor_v3.py` & `fastlane_bot-0.94.1/fastlane_bot/events/exchanges/bancor_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/exchanges/base.py` & `fastlane_bot-0.94.1/fastlane_bot/events/exchanges/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/exchanges/carbon_v1.py` & `fastlane_bot-0.94.1/fastlane_bot/events/exchanges/carbon_v1.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/exchanges/factory.py` & `fastlane_bot-0.94.1/fastlane_bot/events/exchanges/factory.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/exchanges/sushiswap_v2.py` & `fastlane_bot-0.94.1/fastlane_bot/events/exchanges/sushiswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/exchanges/uniswap_v2.py` & `fastlane_bot-0.94.1/fastlane_bot/events/exchanges/uniswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/exchanges/uniswap_v3.py` & `fastlane_bot-0.94.1/fastlane_bot/events/exchanges/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/interface.py` & `fastlane_bot-0.94.1/fastlane_bot/events/interface.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/managers/base.py` & `fastlane_bot-0.94.1/fastlane_bot/events/managers/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/managers/contracts.py` & `fastlane_bot-0.94.1/fastlane_bot/events/managers/contracts.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/managers/events.py` & `fastlane_bot-0.94.1/fastlane_bot/events/managers/events.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/managers/manager.py` & `fastlane_bot-0.94.1/fastlane_bot/events/managers/manager.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/managers/pools.py` & `fastlane_bot-0.94.1/fastlane_bot/events/managers/pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/pools/__init__.py` & `fastlane_bot-0.94.1/fastlane_bot/events/pools/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/pools/bancor_v3.py` & `fastlane_bot-0.94.1/fastlane_bot/events/pools/bancor_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/pools/base.py` & `fastlane_bot-0.94.1/fastlane_bot/events/pools/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/pools/carbon_v1.py` & `fastlane_bot-0.94.1/fastlane_bot/events/pools/carbon_v1.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/pools/factory.py` & `fastlane_bot-0.94.1/fastlane_bot/events/pools/factory.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/pools/sushiswap_v2.py` & `fastlane_bot-0.94.1/fastlane_bot/events/pools/sushiswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/pools/uniswap_v2.py` & `fastlane_bot-0.94.1/fastlane_bot/events/pools/uniswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/pools/uniswap_v3.py` & `fastlane_bot-0.94.1/fastlane_bot/events/pools/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/tests/convert_py_test_to_jupyter.py` & `fastlane_bot-0.94.1/fastlane_bot/events/tests/convert_py_test_to_jupyter.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/tests/test_exchanges.py` & `fastlane_bot-0.94.1/fastlane_bot/events/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/tests/test_interface.py` & `fastlane_bot-0.94.1/fastlane_bot/events/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/tests/test_manager.py` & `fastlane_bot-0.94.1/fastlane_bot/events/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/tests/test_pools.py` & `fastlane_bot-0.94.1/fastlane_bot/events/tests/test_pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/tests/test_utils.py` & `fastlane_bot-0.94.1/fastlane_bot/events/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/events/utils.py` & `fastlane_bot-0.94.1/fastlane_bot/events/utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/helpers/poolandtokens.py` & `fastlane_bot-0.94.1/fastlane_bot/helpers/poolandtokens.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/helpers/routehandler.py` & `fastlane_bot-0.94.1/fastlane_bot/helpers/routehandler.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/helpers/submithandler.py` & `fastlane_bot-0.94.1/fastlane_bot/helpers/submithandler.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/helpers/tradeinstruction.py` & `fastlane_bot-0.94.1/fastlane_bot/helpers/tradeinstruction.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/helpers/txhelpers.py` & `fastlane_bot-0.94.1/fastlane_bot/helpers/txhelpers.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/helpers/univ3calc.py` & `fastlane_bot-0.94.1/fastlane_bot/helpers/univ3calc.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/modes/base.py` & `fastlane_bot-0.94.1/fastlane_bot/modes/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/modes/base_pairwise.py` & `fastlane_bot-0.94.1/fastlane_bot/modes/base_pairwise.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/modes/base_triangle.py` & `fastlane_bot-0.94.1/fastlane_bot/modes/base_triangle.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/modes/pairwise_multi.py` & `fastlane_bot-0.94.1/fastlane_bot/modes/pairwise_multi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/modes/pairwise_single.py` & `fastlane_bot-0.94.1/fastlane_bot/modes/pairwise_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/modes/tests/test_pairwise_single.py` & `fastlane_bot-0.94.1/fastlane_bot/modes/tests/test_pairwise_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/modes/triangle_bancor_v3_two_hop.py` & `fastlane_bot-0.94.1/fastlane_bot/modes/triangle_bancor_v3_two_hop.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/modes/triangle_multi.py` & `fastlane_bot-0.94.1/fastlane_bot/modes/triangle_multi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/modes/triangle_single.py` & `fastlane_bot-0.94.1/fastlane_bot/modes/triangle_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/modes/triangle_single_bancor3.py` & `fastlane_bot-0.94.1/fastlane_bot/modes/triangle_single_bancor3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/testing.py` & `fastlane_bot-0.94.1/fastlane_bot/testing.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/tools/analyzer.py` & `fastlane_bot-0.94.1/fastlane_bot/tools/analyzer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/tools/arbgraphs.py` & `fastlane_bot-0.94.1/fastlane_bot/tools/arbgraphs.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/tools/cpc.py` & `fastlane_bot-0.94.1/fastlane_bot/tools/cpc.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/tools/optimizer.py` & `fastlane_bot-0.94.1/fastlane_bot/tools/optimizer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/tools/params.py` & `fastlane_bot-0.94.1/fastlane_bot/tools/params.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/tools/simplepair.py` & `fastlane_bot-0.94.1/fastlane_bot/tools/simplepair.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/tools/tokenscale.py` & `fastlane_bot-0.94.1/fastlane_bot/tools/tokenscale.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/tools/univ3calc_DELETE.py` & `fastlane_bot-0.94.1/fastlane_bot/tools/univ3calc_DELETE.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot/utils.py` & `fastlane_bot-0.94.1/fastlane_bot/utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/fastlane_bot.egg-info/PKG-INFO` & `fastlane_bot-0.94.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fastlane-bot
-Version: 0.91.1
+Name: fastlane_bot
+Version: 0.94.1
 Summary: Carbon Arbitrage Bot, an open-source arbitrage protocol, allows any user to perform arbitrage between Bancor ecosystem protocols and external exchanges and redirect arbitrage profits back to the protocol.
 Home-page: https://github.com/bancorprotocol/carbon-bot
 Author: Bancor Network
 Author-email: mike@bancor.network
 Requires-Python: >= 3.8, != 3.11.*
 Description-Content-Type: text/markdown
 Provides-Extra: complete
@@ -41,14 +41,19 @@
 cd fastlane-bot
 pip install -r requirements.txt
 python setup.py install
 ```
 
 [sim]:https://github.com/bancorprotocol/carbon-simulator
 
+### Legacy Installation (v1.0)
+You can access the legacy version of the Fastlane Arbitrage Bot, which was solely designed to facilitate single triangle arbitrage transactions which both initiate and conclude with BNT on the Bancor V3 exchange, by referring to the following link:
+
+[github.com/bancorprotocol/fastlane-bot/releases/tag/v1.0](https://github.com/bancorprotocol/fastlane-bot/releases/tag/v1.0)
+
 ### Preparation
 
 The Fastlane Arbitrage Bot needs access to an Ethereum wallet's private key. **THIS KEY IS AT RISK AND SHOULD NOT BE USED ELSEWHERE**. Maintain some ETH in the wallet for gas fees and regularly sweep profits. Supply the private key to the bot using an environment variable, as shown:
 
 ```bash
 set ETH_PRIVATE_KEY_BE_CAREFUL="0x9c..."
 ```
```

### Comparing `fastlane_bot-0.91.1/fastlane_bot.egg-info/SOURCES.txt` & `fastlane_bot-0.94.1/fastlane_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.91.1/setup.py` & `fastlane_bot-0.94.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,27 +11,53 @@
 from setuptools import find_packages, setup
 
 import os
 from dotenv import load_dotenv
 
 # Load .env file
 env_file = '.env'
-assert os.path.exists(env_file), "The .env file is missing. See README.md for instructions"
+try:
+    assert os.path.exists(env_file), "The .env file is missing. See README.md for instructions"
+except AssertionError as e:
+    # Create .env file
+    print("Creating .env file. Please update it with your environment variables. See README.md for instructions")
+    with open(env_file, 'w') as f:
+        f.write(f"export WEB3_ALCHEMY_PROJECT_ID=\n")
+        f.write(f"export ETH_PRIVATE_KEY_BE_CAREFUL=\n")
+        f.write(f"export DEFAULT_MIN_PROFIT_BNT=200\n")
+        f.write(f"export ETHERSCAN_TOKEN=\n")
+        f.write(f"export TENDERLY_FORK_ID=\n")
+        f.write(f"export TENDERLY_ACCESS_KEY=\n")
+        f.write(f"export TENDERLY_PROJECT=\n")
+        f.write(f"export TENDERLY_USER=\n")
+
 load_dotenv(env_file)
 
 # Check for required variables
 required_vars = ['WEB3_ALCHEMY_PROJECT_ID',
                  'ETH_PRIVATE_KEY_BE_CAREFUL',
+                 'DEFAULT_MIN_PROFIT_BNT',
                  'ETHERSCAN_TOKEN',
-                 'TENDERLY_FORK_ID']
-
-for var in required_vars:
-    assert var in os.environ, f"The {var} environment variable is missing in .env file. See README.md for instructions"
-    if var != 'TENDERLY_FORK_ID':
-        assert os.environ[var], f"The {var} environment variable cannot be blank or None"
+                 'TENDERLY_FORK_ID',
+                 'TENDERLY_ACCESS_KEY',
+                 'TENDERLY_PROJECT',
+                 'TENDERLY_USER']
+
+with open(env_file, 'a') as f:
+    for var in required_vars:
+        if var not in os.environ:
+            print(f"The {var} environment variable is missing in .env file. Adding it with a default empty value. See README.md for instructions")
+            if var == 'DEFAULT_MIN_PROFIT_BNT':
+                f.write(f"export {var}=1\n")
+                os.environ[var] = '1'
+            else:
+                f.write(f"export {var}=\n")
+                os.environ[var] = ''  # Optionally update the current environment as well
+        if os.environ[var] == '' and 'TENDERLY' not in var and 'ETHERSCAN_TOKEN' not in var:
+            raise Exception(f"The {var} environment variable cannot be None. Please update the .env file. See README.md for instructions")
 
 import brownie_setup
 
 with open("fastlane_bot/__init__.py") as fd:
     version = re.search(
         r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE
     )[1]
```
