# Comparing `tmp/flumine-2.3.6.tar.gz` & `tmp/flumine-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flumine-2.3.6.tar", last modified: Thu Apr 27 08:39:23 2023, max compression
+gzip compressed data, was "dist/flumine-2.3.7.tar", last modified: Mon Jul 24 08:08:05 2023, max compression
```

## Comparing `flumine-2.3.6.tar` & `flumine-2.3.7.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-27 08:39:23.000000 flumine-2.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-27 08:39:01.000000 flumine-2.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/baseflumine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/clients/baseclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/clients/betconnectclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/clients/betfairclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/clients/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/clients/simulatedclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/controls/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/controls/clientcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/controls/loggingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/controls/tradingcontrols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/execution/baseexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/execution/betfairexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/execution/simulatedexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/execution/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/flumine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/markets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/markets/blotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/markets/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/markets/markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/markets/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/order/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/orderpackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/ordertype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/order/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/patching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23526 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/simulation/simulatedorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/simulation/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/strategy/runnercontext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/strategy/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/basestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/datastream.py
--rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/historicalstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/marketstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/orderstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/simulatedorderstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/sportsdatastream.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/streams/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-04-27 08:39:01.000000 flumine-2.3.6/flumine/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 08:39:23.000000 flumine-2.3.6/flumine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:39:23.000000 flumine-2.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-27 08:39:01.000000 flumine-2.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:23.000000 flumine-2.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_baseflumine.py
--rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_blotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_clientcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    19619 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    63899 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_flumine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_fluminesimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_loggingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    21094 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_orderpackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_ordertype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_runnercontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_simulated_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    60568 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_simulatedorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    40617 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_tradingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-04-27 08:39:01.000000 flumine-2.3.6/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-24 08:08:05.000000 flumine-2.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-24 08:07:43.000000 flumine-2.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/baseflumine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/clients/baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/clients/betconnectclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/clients/betfairclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/clients/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/clients/simulatedclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/controls/clientcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/controls/loggingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/controls/tradingcontrols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/execution/baseexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/execution/betfairexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/execution/simulatedexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/execution/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/flumine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/markets/blotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/markets/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/markets/markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/markets/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/order/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/orderpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/ordertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/patching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23526 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/simulation/simulatedorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/simulation/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/strategy/runnercontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/strategy/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/basestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/historicalstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/marketstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/orderstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/simulatedorderstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/sportsdatastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 08:08:05.000000 flumine-2.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-24 08:07:43.000000 flumine-2.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24925 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_baseflumine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_blotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_clientcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19619 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63899 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_flumine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_fluminesimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_loggingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21094 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_orderpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_ordertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_runnercontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_simulated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60568 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_simulatedorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40617 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_tradingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_worker.py
```

### Comparing `flumine-2.3.6/PKG-INFO` & `flumine-2.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flumine
-Version: 2.3.6
+Version: 2.3.7
 Summary: Betting trading framework
 Home-page: https://github.com/betcode-org/flumine
 Author: Liam Pauling
 Author-email: a@unknown.com
 License: MIT
 Description: <p align="center">
           <a href="https://github.com/betcode-org">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flumine Version: 2.3.6 Summary: Betting trading
+Metadata-Version: 2.1 Name: flumine Version: 2.3.7 Summary: Betting trading
 framework Home-page: https://github.com/betcode-org/flumine Author: Liam
 Pauling Author-email: a@unknown.com License: MIT Description:
                           [docs/images/logo-full.png]
 # flÅ«mine ![Build Status](https://github.com/betcode-org/flumine/actions/
 workflows/test.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/
 github/liampauling/flumine/badge.svg?branch=master)](https://coveralls.io/
 github/liampauling/flumine?branch=master) [![PyPI version](https://
```

### Comparing `flumine-2.3.6/README.md` & `flumine-2.3.7/README.md`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/__init__.py` & `flumine-2.3.7/flumine/__init__.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/baseflumine.py` & `flumine-2.3.7/flumine/baseflumine.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,16 @@
                             "market_id": market_id,
                             "latency": latency,
                             "pt": market_book.publish_time,
                         },
                     )
 
             market = self.markets.markets.get(market_id)
-            if market is None:
+            market_is_new = market is None
+            if market_is_new:
                 market = self._add_market(market_id, market_book)
             elif market.closed:
                 self.markets.add_market(market_id, market)
 
             if market_book.status == "CLOSED":
                 self.handler_queue.put(events.CloseMarketEvent(market_book))
                 continue
@@ -159,14 +160,18 @@
             market(market_book)
 
             # process middleware
             for middleware in self._market_middleware:
                 utils.call_middleware_error_handling(middleware, market)
 
             for strategy in self.strategies:
+                if market_is_new:
+                    utils.call_strategy_error_handling(
+                        strategy.process_new_market, market, market_book
+                    )
                 if utils.call_strategy_error_handling(
                     strategy.check_market, market, market_book
                 ):
                     utils.call_strategy_error_handling(
                         strategy.process_market_book, market, market_book
                     )
```

### Comparing `flumine-2.3.6/flumine/clients/baseclient.py` & `flumine-2.3.7/flumine/clients/baseclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/clients/betconnectclient.py` & `flumine-2.3.7/flumine/clients/betconnectclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/clients/betfairclient.py` & `flumine-2.3.7/flumine/clients/betfairclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Optional
+from typing import Optional, Union
 from betfairlightweight import BetfairError, resources
 from betfairlightweight.metadata import currency_parameters
 
 from .baseclient import BaseClient
 from .clients import ExchangeType
 
 logger = logging.getLogger(__name__)
@@ -34,28 +34,30 @@
                 extra={
                     "client": self.betting_client,
                     "trading_function": "login",
                     "response": e,
                 },
             )
 
-    def keep_alive(self) -> Optional[resources.KeepAliveResource]:
+    def keep_alive(self) -> Optional[Union[resources.KeepAliveResource, bool]]:
         if self.betting_client.session_expired:
             try:
                 return self.betting_client.keep_alive()
             except BetfairError as e:
                 logger.error(
                     "BetfairClient `keep_alive` error",
                     exc_info=True,
                     extra={
                         "client": self.betting_client,
                         "trading_function": "keep_alive",
                         "response": e,
                     },
                 )
+        else:
+            return True
 
     def logout(self) -> Optional[resources.LogoutResource]:
         try:
             return self.betting_client.logout()
         except BetfairError as e:
             logger.error(
                 "BetfairClient `logout` error",
```

### Comparing `flumine-2.3.6/flumine/clients/clients.py` & `flumine-2.3.7/flumine/clients/clients.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/clients/simulatedclient.py` & `flumine-2.3.7/flumine/clients/simulatedclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/config.py` & `flumine-2.3.7/flumine/config.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/controls/__init__.py` & `flumine-2.3.7/flumine/controls/__init__.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/controls/clientcontrols.py` & `flumine-2.3.7/flumine/controls/clientcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/controls/loggingcontrols.py` & `flumine-2.3.7/flumine/controls/loggingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/controls/tradingcontrols.py` & `flumine-2.3.7/flumine/controls/tradingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/events/events.py` & `flumine-2.3.7/flumine/events/events.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/exceptions.py` & `flumine-2.3.7/flumine/exceptions.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/execution/baseexecution.py` & `flumine-2.3.7/flumine/execution/baseexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/execution/betfairexecution.py` & `flumine-2.3.7/flumine/execution/betfairexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/execution/simulatedexecution.py` & `flumine-2.3.7/flumine/execution/simulatedexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/execution/transaction.py` & `flumine-2.3.7/flumine/execution/transaction.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/flumine.py` & `flumine-2.3.7/flumine/flumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/markets/blotter.py` & `flumine-2.3.7/flumine/markets/blotter.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/markets/market.py` & `flumine-2.3.7/flumine/markets/market.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/markets/markets.py` & `flumine-2.3.7/flumine/markets/markets.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/markets/middleware.py` & `flumine-2.3.7/flumine/markets/middleware.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/order/order.py` & `flumine-2.3.7/flumine/order/order.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/order/orderpackage.py` & `flumine-2.3.7/flumine/order/orderpackage.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/order/ordertype.py` & `flumine-2.3.7/flumine/order/ordertype.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/order/process.py` & `flumine-2.3.7/flumine/order/process.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/order/responses.py` & `flumine-2.3.7/flumine/order/responses.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/order/trade.py` & `flumine-2.3.7/flumine/order/trade.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/patching.py` & `flumine-2.3.7/flumine/patching.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/simulation/simulatedorder.py` & `flumine-2.3.7/flumine/simulation/simulatedorder.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/simulation/simulation.py` & `flumine-2.3.7/flumine/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/simulation/utils.py` & `flumine-2.3.7/flumine/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/strategy/runnercontext.py` & `flumine-2.3.7/flumine/strategy/runnercontext.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/strategy/strategy.py` & `flumine-2.3.7/flumine/strategy/strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,18 @@
         if market_book.streaming_unique_id not in self.stream_ids:
             return False  # strategy not subscribed to market stream
         elif self.check_market_book(market, market_book):
             return True
         else:
             return False
 
+    def process_new_market(self, market: Market, market_book: MarketBook) -> None:
+        # called when a market is newly added to the framework
+        return
+
     def check_market_book(self, market: Market, market_book: MarketBook) -> bool:
         # process_market_book only executed if this returns True
         return False
 
     def process_market_book(self, market: Market, market_book: MarketBook) -> None:
         # process marketBook; place/cancel/replace orders
         return
@@ -228,15 +232,15 @@
             return self.historic_stream_ids
         else:
             return [stream.stream_id for stream in self.streams]
 
     @property
     def info(self) -> dict:
         return {
-            "name": self.name,
+            "strategy_name": self.name,
             "market_filter": self.market_filter,
             "market_data_filter": self.market_data_filter,
             "streaming_timeout": self.streaming_timeout,
             "conflate_ms": self.conflate_ms,
             "stream_ids": self.stream_ids,
             "max_selection_exposure": self.max_selection_exposure,
             "max_order_exposure": self.max_order_exposure,
```

### Comparing `flumine-2.3.6/flumine/streams/basestream.py` & `flumine-2.3.7/flumine/streams/basestream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/streams/datastream.py` & `flumine-2.3.7/flumine/streams/datastream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/streams/historicalstream.py` & `flumine-2.3.7/flumine/streams/historicalstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/streams/marketstream.py` & `flumine-2.3.7/flumine/streams/marketstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/streams/orderstream.py` & `flumine-2.3.7/flumine/streams/orderstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/streams/simulatedorderstream.py` & `flumine-2.3.7/flumine/streams/simulatedorderstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/streams/sportsdatastream.py` & `flumine-2.3.7/flumine/streams/sportsdatastream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/streams/streams.py` & `flumine-2.3.7/flumine/streams/streams.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/flumine/utils.py` & `flumine-2.3.7/flumine/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,23 +103,21 @@
         prices.extend(arange(as_dec(cursor), as_dec(cutoff), as_dec(1 / step)))
         cursor = cutoff
     prices.append(as_dec(MAX_PRICE))
     return prices
 
 
 def make_line_prices(min_unit: float, max_unit: float, interval: float) -> list:
-    prices = []
+    prices = [min_unit]
     price = min_unit
     while True:
         price += interval
         if price > max_unit:
-            break
-        else:
-            prices.append(price)
-    return prices
+            return prices
+        prices.append(price)
 
 
 PRICES = make_prices(MIN_PRICE, CUTOFFS)
 PRICES_FLOAT = [float(price) for price in PRICES]
 FINEST_PRICES = make_prices(MIN_PRICE, ((1000, 100),))
```

### Comparing `flumine-2.3.6/flumine/worker.py` & `flumine-2.3.7/flumine/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     """Attempt keep alive if required or
     login if keep alive failed
     """
     for client in flumine.clients:
         if client.EXCHANGE == ExchangeType.BETFAIR:
             if client.betting_client.session_token:
                 resp = client.keep_alive()
-                if resp is None or resp.status == "SUCCESS":
+                if resp is True or resp.status == "SUCCESS":
                     continue
         elif client.EXCHANGE == ExchangeType.BETCONNECT:
             resp = client.keep_alive()
             if resp:
                 continue
         # keep-alive failed lets try a login
         client.login()
```

### Comparing `flumine-2.3.6/flumine.egg-info/PKG-INFO` & `flumine-2.3.7/flumine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flumine
-Version: 2.3.6
+Version: 2.3.7
 Summary: Betting trading framework
 Home-page: https://github.com/betcode-org/flumine
 Author: Liam Pauling
 Author-email: a@unknown.com
 License: MIT
 Description: <p align="center">
           <a href="https://github.com/betcode-org">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flumine Version: 2.3.6 Summary: Betting trading
+Metadata-Version: 2.1 Name: flumine Version: 2.3.7 Summary: Betting trading
 framework Home-page: https://github.com/betcode-org/flumine Author: Liam
 Pauling Author-email: a@unknown.com License: MIT Description:
                           [docs/images/logo-full.png]
 # flÅ«mine ![Build Status](https://github.com/betcode-org/flumine/actions/
 workflows/test.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/
 github/liampauling/flumine/badge.svg?branch=master)](https://coveralls.io/
 github/liampauling/flumine?branch=master) [![PyPI version](https://
```

### Comparing `flumine-2.3.6/flumine.egg-info/SOURCES.txt` & `flumine-2.3.7/flumine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/setup.py` & `flumine-2.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_baseflumine.py` & `flumine-2.3.7/tests/test_baseflumine.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from unittest import mock
 
 from flumine.baseflumine import (
     BaseFlumine,
     FlumineException,
     MaxTransactionCount,
     SimulatedMiddleware,
+    Market,
 )
 from flumine.clients import ExchangeType
 from flumine.exceptions import ClientError
 
 
 class BaseFlumineTest(unittest.TestCase):
     def setUp(self):
@@ -130,18 +131,32 @@
 
     def test__add_default_workers(self):
         self.base_flumine._add_default_workers()
         self.assertEqual(len(self.base_flumine._workers), 0)
 
     def test__process_market_books(self):
         mock_event = mock.Mock()
-        mock_market_book = mock.Mock(publish_time_epoch=123)
+        self.base_flumine.streams = mock.Mock()
+        mock_strategy = mock.Mock()
+        self.base_flumine.add_strategy(mock_strategy)
+        mock_market_book = mock.Mock(publish_time_epoch=123, market_id="1.123")
         mock_market_book.runners = []
         mock_event.event = [mock_market_book]
-        self.base_flumine._process_market_books(mock_event)
+        for call_count in range(1, 5):
+            # process_new_market must be called only once, the first time
+            with self.subTest(call_count=call_count):
+                self.base_flumine._process_market_books(mock_event)
+                mock_strategy.process_new_market.assert_called_once()
+                self.assertEqual(
+                    mock_strategy.process_market_book.call_count, call_count
+                )
+        market, market_book = mock_strategy.process_new_market.call_args[0]
+        self.assertIs(market_book, mock_market_book)
+        self.assertIsInstance(market, Market)
+        self.assertIs(market.market_book, mock_market_book)
 
     @mock.patch("flumine.baseflumine.utils.call_strategy_error_handling")
     def test__process_sports_data(self, mock_call_strategy_error_handling):
         mock_market = mock.Mock()
         self.base_flumine.markets._markets = {"1.1": mock_market}
         mock_strategy_one = mock.Mock(stream_ids=[123])
         mock_strategy_two = mock.Mock(stream_ids=[])
```

### Comparing `flumine-2.3.6/tests/test_blotter.py` & `flumine-2.3.7/tests/test_blotter.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_clientcontrols.py` & `flumine-2.3.7/tests/test_clientcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_clients.py` & `flumine-2.3.7/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_config.py` & `flumine-2.3.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_events.py` & `flumine-2.3.7/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_execution.py` & `flumine-2.3.7/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_flumine.py` & `flumine-2.3.7/tests/test_flumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_fluminesimulation.py` & `flumine-2.3.7/tests/test_fluminesimulation.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_integration.py` & `flumine-2.3.7/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_loggingcontrols.py` & `flumine-2.3.7/tests/test_loggingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_markets.py` & `flumine-2.3.7/tests/test_markets.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_middleware.py` & `flumine-2.3.7/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_order.py` & `flumine-2.3.7/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_orderpackage.py` & `flumine-2.3.7/tests/test_orderpackage.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_ordertype.py` & `flumine-2.3.7/tests/test_ordertype.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_process.py` & `flumine-2.3.7/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_responses.py` & `flumine-2.3.7/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_runnercontext.py` & `flumine-2.3.7/tests/test_runnercontext.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_simulated_utils.py` & `flumine-2.3.7/tests/test_simulated_utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_simulatedorder.py` & `flumine-2.3.7/tests/test_simulatedorder.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_strategy.py` & `flumine-2.3.7/tests/test_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,17 @@
     )
     def test_check_market_pass(self, mock_check_market_book, mock_market_stream_ids):
         mock_market = mock.Mock()
         mock_market_book = mock.Mock(streaming_unique_id=12)
         self.assertTrue(self.strategy.check_market(mock_market, mock_market_book))
         mock_check_market_book.assert_called_with(mock_market, mock_market_book)
 
+    def test_process_new_market(self):
+        self.strategy.process_new_market(None, None)
+
     def test_check_market_book(self):
         self.assertFalse(self.strategy.check_market_book(None, None))
 
     def test_process_market_book(self):
         self.strategy.process_market_book(None, None)
 
     def test_check_sports_no_subscribed(self):
@@ -272,15 +275,15 @@
     def test_info(self):
         self.assertEqual(
             self.strategy.info,
             {
                 "conflate_ms": self.conflate_ms,
                 "market_data_filter": self.mock_market_data_filter,
                 "market_filter": self.mock_market_filter,
-                "name": "test",
+                "strategy_name": "test",
                 "name_hash": "a94a8fe5ccb19",
                 "stream_ids": [],
                 "streaming_timeout": self.streaming_timeout,
                 "context": {"trigger": 0.123},
                 "max_live_trade_count": 4,
                 "max_order_exposure": 2,
                 "max_selection_exposure": 1,
```

### Comparing `flumine-2.3.6/tests/test_streams.py` & `flumine-2.3.7/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_trade.py` & `flumine-2.3.7/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_tradingcontrols.py` & `flumine-2.3.7/tests/test_tradingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_transaction.py` & `flumine-2.3.7/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.6/tests/test_utils.py` & `flumine-2.3.7/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     #     utils.arange()
 
     def test_make_prices(self):
         prices = utils.make_prices(utils.MIN_PRICE, utils.CUTOFFS)
         self.assertEqual(len(prices), 350)
 
     def test_make_line_prices(self):
-        prices = utils.make_line_prices(-0.5, 9.5, 1.0)
+        prices = utils.make_line_prices(0.5, 9.5, 1.0)
         self.assertEqual(prices, [0.5, 1.5, 2.5, 3.5, 4.5, 5.5, 6.5, 7.5, 8.5, 9.5])
 
     def test_get_nearest_price(self):
         self.assertEqual(utils.get_nearest_price(1.011), 1.01)
         self.assertEqual(utils.get_nearest_price(0), 1.01)
         self.assertEqual(utils.get_nearest_price(1001), 1000)
         self.assertEqual(utils.get_nearest_price(2.01), 2.02)
```

### Comparing `flumine-2.3.6/tests/test_worker.py` & `flumine-2.3.7/tests/test_worker.py`

 * *Files identical despite different names*

