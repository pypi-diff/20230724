# Comparing `tmp/flumine-2.3.7.tar.gz` & `tmp/flumine-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flumine-2.3.7.tar", last modified: Mon Jul 24 08:08:05 2023, max compression
+gzip compressed data, was "dist/flumine-2.4.0.tar", last modified: Mon Jul 24 10:17:30 2023, max compression
```

## Comparing `flumine-2.3.7.tar` & `flumine-2.4.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-24 08:08:05.000000 flumine-2.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-24 08:07:43.000000 flumine-2.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/baseflumine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/clients/baseclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/clients/betconnectclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/clients/betfairclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/clients/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/clients/simulatedclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/controls/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/controls/clientcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/controls/loggingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/controls/tradingcontrols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/execution/baseexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/execution/betfairexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/execution/simulatedexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/execution/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/flumine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/markets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/markets/blotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/markets/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/markets/markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/markets/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/order/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/orderpackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/ordertype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/order/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/patching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23526 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/simulation/simulatedorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/simulation/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/strategy/runnercontext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/strategy/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/basestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/datastream.py
--rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/historicalstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/marketstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/orderstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/simulatedorderstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/sportsdatastream.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/streams/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-24 08:07:43.000000 flumine-2.3.7/flumine/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 08:08:05.000000 flumine-2.3.7/flumine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 08:08:05.000000 flumine-2.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-24 08:07:43.000000 flumine-2.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:08:05.000000 flumine-2.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24925 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_baseflumine.py
--rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_blotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_clientcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    19619 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    63899 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_flumine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_fluminesimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_loggingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    21094 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_orderpackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_ordertype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_runnercontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_simulated_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    60568 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_simulatedorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    40617 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_tradingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-07-24 08:07:43.000000 flumine-2.3.7/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-24 10:17:30.000000 flumine-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-24 10:17:12.000000 flumine-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/baseflumine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/clients/baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/clients/betconnectclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/clients/betfairclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/clients/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/clients/simulatedclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/controls/clientcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/controls/loggingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/controls/tradingcontrols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/execution/baseexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/execution/betfairexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/execution/simulatedexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/execution/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/flumine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/markets/blotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/markets/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/markets/markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14302 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/markets/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/order/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/orderpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/ordertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/patching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/simulation/simulatedorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/simulation/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/strategy/runnercontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/strategy/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/basestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/historicalstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/marketstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/orderstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/simulatedorderstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/sportsdatastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:17:30.000000 flumine-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-24 10:17:12.000000 flumine-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24925 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_baseflumine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_blotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_clientcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19619 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63899 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_flumine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_fluminesimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_loggingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21248 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_orderpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_ordertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_runnercontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_simulated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61695 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_simulatedorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40617 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_tradingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_worker.py
```

### Comparing `flumine-2.3.7/PKG-INFO` & `flumine-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flumine
-Version: 2.3.7
+Version: 2.4.0
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
-Metadata-Version: 2.1 Name: flumine Version: 2.3.7 Summary: Betting trading
+Metadata-Version: 2.1 Name: flumine Version: 2.4.0 Summary: Betting trading
 framework Home-page: https://github.com/betcode-org/flumine Author: Liam
 Pauling Author-email: a@unknown.com License: MIT Description:
                           [docs/images/logo-full.png]
 # flÅ«mine ![Build Status](https://github.com/betcode-org/flumine/actions/
 workflows/test.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/
 github/liampauling/flumine/badge.svg?branch=master)](https://coveralls.io/
 github/liampauling/flumine?branch=master) [![PyPI version](https://
```

### Comparing `flumine-2.3.7/README.md` & `flumine-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/__init__.py` & `flumine-2.4.0/flumine/__init__.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/baseflumine.py` & `flumine-2.4.0/flumine/baseflumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/clients/baseclient.py` & `flumine-2.4.0/flumine/clients/baseclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/clients/betconnectclient.py` & `flumine-2.4.0/flumine/clients/betconnectclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/clients/betfairclient.py` & `flumine-2.4.0/flumine/clients/betfairclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/clients/clients.py` & `flumine-2.4.0/flumine/clients/clients.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/clients/simulatedclient.py` & `flumine-2.4.0/flumine/clients/simulatedclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/config.py` & `flumine-2.4.0/flumine/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import socket
 
 simulated = False
 simulated_strategy_isolation = True
+simulation_available_prices = False
 
 instance_id = None  # instance id (e.g. AWS ec2 instanceId)
 
 customer_strategy_ref = socket.gethostname()[
     :15
 ]  # ie. docker container id (used as order customerStrategyRefs)
```

### Comparing `flumine-2.3.7/flumine/controls/__init__.py` & `flumine-2.4.0/flumine/controls/__init__.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/controls/clientcontrols.py` & `flumine-2.4.0/flumine/controls/clientcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/controls/loggingcontrols.py` & `flumine-2.4.0/flumine/controls/loggingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/controls/tradingcontrols.py` & `flumine-2.4.0/flumine/controls/tradingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/events/events.py` & `flumine-2.4.0/flumine/events/events.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/exceptions.py` & `flumine-2.4.0/flumine/exceptions.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/execution/baseexecution.py` & `flumine-2.4.0/flumine/execution/baseexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/execution/betfairexecution.py` & `flumine-2.4.0/flumine/execution/betfairexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/execution/simulatedexecution.py` & `flumine-2.4.0/flumine/execution/simulatedexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/execution/transaction.py` & `flumine-2.4.0/flumine/execution/transaction.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/flumine.py` & `flumine-2.4.0/flumine/flumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/markets/blotter.py` & `flumine-2.4.0/flumine/markets/blotter.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/markets/market.py` & `flumine-2.4.0/flumine/markets/market.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/markets/markets.py` & `flumine-2.4.0/flumine/markets/markets.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/markets/middleware.py` & `flumine-2.4.0/flumine/markets/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,23 +193,28 @@
         # isolation per strategy (default)
         if config.simulated_strategy_isolation:
             for strategy, orders in market.blotter._strategy_orders.items():
                 live_orders = [
                     o for o in orders if o.status in LIVE_STATUS and o.simulated
                 ]
                 if live_orders:
-                    _lookup = {k: v.traded.copy() for k, v in market_analytics.items()}
+                    _lookup = {
+                        k: (v.runner, v.traded.copy())
+                        for k, v in market_analytics.items()
+                    }
                     live_orders_sorted = self._sort_orders(live_orders)
                     for order in live_orders_sorted:
                         runner_traded = _lookup[(order.selection_id, order.handicap)]
                         order.simulated(market.market_book, runner_traded)
         else:  # isolation per instance
             live_orders = list(market.blotter.live_orders)
             if live_orders:
-                _lookup = {k: v.traded.copy() for k, v in market_analytics.items()}
+                _lookup = {
+                    k: (v.runner, v.traded.copy()) for k, v in market_analytics.items()
+                }
                 live_orders_sorted = self._sort_orders(live_orders)
                 for order in live_orders_sorted:
                     if order.status in LIVE_STATUS and order.simulated:
                         runner_traded = _lookup[(order.selection_id, order.handicap)]
                         order.simulated(market.market_book, runner_traded)
 
     @staticmethod
@@ -247,29 +252,29 @@
                 (runner.selection_id, runner.handicap)
             ] = RunnerAnalytics(runner)
         runner_analytics(runner)
 
 
 class RunnerAnalytics:
     def __init__(self, runner: RunnerBook):
-        self._runner = runner
+        self.runner = runner
         self.traded = {}  # price: size traded since last update
         self._traded_volume = runner.ex.traded_volume
         self._p_v = {
             i["price"]: i["size"] for i in runner.ex.traded_volume
         }  # cached current volume
 
     def __call__(self, runner: RunnerBook):
         _tv = runner.ex.traded_volume
         if self._traded_volume == _tv:
             self.traded = {}
         else:
             self.traded = self._calculate_traded(_tv)
             self._traded_volume = _tv
-        self._runner = runner
+        self.runner = runner
 
     def _calculate_traded(self, traded_volume: list) -> dict:
         p_v, traded = self._p_v, {}
         # create dictionary
         c_v = {i["price"]: i["size"] for i in traded_volume}
         # calculate difference
         for key, value in c_v.items():
```

### Comparing `flumine-2.3.7/flumine/order/order.py` & `flumine-2.4.0/flumine/order/order.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/order/orderpackage.py` & `flumine-2.4.0/flumine/order/orderpackage.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/order/ordertype.py` & `flumine-2.4.0/flumine/order/ordertype.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/order/process.py` & `flumine-2.4.0/flumine/order/process.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/order/responses.py` & `flumine-2.4.0/flumine/order/responses.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/order/trade.py` & `flumine-2.4.0/flumine/order/trade.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/patching.py` & `flumine-2.4.0/flumine/patching.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/simulation/simulatedorder.py` & `flumine-2.4.0/flumine/simulation/simulatedorder.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.size_cancelled = 0.0
         self.size_lapsed = 0.0
         self.size_voided = 0.0
         self.market_version = None  # version at place so we can lapse if needed
         self._piq = 0.0
         self._bsp_reconciled = False
 
-    def __call__(self, market_book: MarketBook, traded: dict) -> None:
+    def __call__(self, market_book: MarketBook, runner_traded: tuple) -> None:
         # simulates order matching
         if self._bsp_reconciled is False and market_book.bsp_reconciled:
             if self.take_sp:
                 runner = self._get_runner(market_book)
                 self._process_sp(market_book.publish_time_epoch, runner)
                 return
             else:
@@ -48,17 +48,23 @@
                 self.market_version = market_book.version  # update for next time
                 if market_book.status == "SUSPENDED":  # Material change
                     if self.order.order_type.persistence_type == "LAPSE":
                         self.size_lapsed += self.size_remaining
                         return
 
             # todo estimated piq cancellations
+            traded = runner_traded[1]
             if traded:
                 self._process_traded(market_book.publish_time_epoch, traded)
 
+            if config.simulation_available_prices:
+                self._process_available(
+                    market_book.publish_time_epoch, runner_traded[0]
+                )
+
     def place(
         self, order_package, market_book: MarketBook, instruction: dict, bet_id: int
     ) -> SimulatedPlaceResponse:
         # simulates placeOrder request->matching->response
         # validate market status
         if market_book.status != "OPEN":
             self.size_voided += self.size_remaining
@@ -460,14 +466,45 @@
             self._piq -= _traded_size
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(
                     "Simulated order {0} PIQ: {1}".format(self.order.id, self._piq)
                 )
             return traded_size
 
+    def _process_available(self, publish_time: int, runner: RunnerBook) -> None:
+        # todo prevent double counting
+        price = self.order.order_type.price
+        side = self.side
+        if side == "BACK":
+            for update in runner.ex.available_to_back:
+                if update["price"] >= price:
+                    self._calculate_process_available(
+                        publish_time, update["price"], update["size"]
+                    )
+        elif side == "LAY":
+            for update in runner.ex.available_to_lay:
+                if update["price"] <= price:
+                    self._calculate_process_available(
+                        publish_time, update["price"], update["size"]
+                    )
+
+    def _calculate_process_available(
+        self, publish_time: int, price: float, size: float
+    ) -> None:
+        size = round(min(self.size_remaining, size), 2)
+        if size:
+            self._update_matched(
+                [
+                    publish_time,
+                    price,
+                    size,
+                ]
+            )
+        self._piq = 0
+
     @property
     def take_sp(self) -> bool:
         if self.order.order_type.ORDER_TYPE == OrderTypes.LIMIT:
             if self.order.order_type.persistence_type == "MARKET_ON_CLOSE":
                 return True
             return False
         else:
```

### Comparing `flumine-2.3.7/flumine/simulation/simulation.py` & `flumine-2.4.0/flumine/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/simulation/utils.py` & `flumine-2.4.0/flumine/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/strategy/runnercontext.py` & `flumine-2.4.0/flumine/strategy/runnercontext.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/strategy/strategy.py` & `flumine-2.4.0/flumine/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/streams/basestream.py` & `flumine-2.4.0/flumine/streams/basestream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/streams/datastream.py` & `flumine-2.4.0/flumine/streams/datastream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/streams/historicalstream.py` & `flumine-2.4.0/flumine/streams/historicalstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/streams/marketstream.py` & `flumine-2.4.0/flumine/streams/marketstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/streams/orderstream.py` & `flumine-2.4.0/flumine/streams/orderstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/streams/simulatedorderstream.py` & `flumine-2.4.0/flumine/streams/simulatedorderstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/streams/sportsdatastream.py` & `flumine-2.4.0/flumine/streams/sportsdatastream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/streams/streams.py` & `flumine-2.4.0/flumine/streams/streams.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/utils.py` & `flumine-2.4.0/flumine/utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine/worker.py` & `flumine-2.4.0/flumine/worker.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/flumine.egg-info/PKG-INFO` & `flumine-2.4.0/flumine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flumine
-Version: 2.3.7
+Version: 2.4.0
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
-Metadata-Version: 2.1 Name: flumine Version: 2.3.7 Summary: Betting trading
+Metadata-Version: 2.1 Name: flumine Version: 2.4.0 Summary: Betting trading
 framework Home-page: https://github.com/betcode-org/flumine Author: Liam
 Pauling Author-email: a@unknown.com License: MIT Description:
                           [docs/images/logo-full.png]
 # flÅ«mine ![Build Status](https://github.com/betcode-org/flumine/actions/
 workflows/test.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/
 github/liampauling/flumine/badge.svg?branch=master)](https://coveralls.io/
 github/liampauling/flumine?branch=master) [![PyPI version](https://
```

### Comparing `flumine-2.3.7/flumine.egg-info/SOURCES.txt` & `flumine-2.4.0/flumine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/setup.py` & `flumine-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_baseflumine.py` & `flumine-2.4.0/tests/test_baseflumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_blotter.py` & `flumine-2.4.0/tests/test_blotter.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_clientcontrols.py` & `flumine-2.4.0/tests/test_clientcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_clients.py` & `flumine-2.4.0/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_config.py` & `flumine-2.4.0/tests/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from flumine import config
 
 
 class ConfigTest(unittest.TestCase):
     def test_init(self):
         self.assertFalse(config.simulated)
         self.assertTrue(config.simulated_strategy_isolation)
+        self.assertFalse(config.simulation_available_prices)
         self.assertIsInstance(config.customer_strategy_ref, str)
         self.assertIsInstance(config.process_id, int)
         self.assertIsNone(config.current_time)
         self.assertFalse(config.raise_errors)
         self.assertEqual(config.max_execution_workers, 32)
         self.assertFalse(config.async_place_orders)
         self.assertEqual(config.place_latency, 0.120)
```

### Comparing `flumine-2.3.7/tests/test_events.py` & `flumine-2.4.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_execution.py` & `flumine-2.4.0/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_flumine.py` & `flumine-2.4.0/tests/test_flumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_fluminesimulation.py` & `flumine-2.4.0/tests/test_fluminesimulation.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_integration.py` & `flumine-2.4.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_loggingcontrols.py` & `flumine-2.4.0/tests/test_loggingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_markets.py` & `flumine-2.4.0/tests/test_markets.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_middleware.py` & `flumine-2.4.0/tests/test_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,20 +274,23 @@
         )
         mock_order_three = mock.Mock(
             selection_id=123, handicap=1, status=OrderStatus.EXECUTABLE, simulated=False
         )
         mock_market.blotter._strategy_orders = {
             "test": [mock_order, mock_order_two, mock_order_three]
         }
+        mock_runner = mock.Mock(traded={1: 2})
         mock_market_analytics = {
-            (mock_order.selection_id, mock_order.handicap): mock.Mock(traded={1: 2})
+            (mock_order.selection_id, mock_order.handicap): mock_runner
         }
         mock_market.market_book = mock_market_book
         self.middleware._process_simulated_orders(mock_market, mock_market_analytics)
-        mock_order.simulated.assert_called_with(mock_market_book, {1: 2})
+        mock_order.simulated.assert_called_with(
+            mock_market_book, (mock_runner.runner, {1: 2})
+        )
         mock_order_two.simulated.assert_not_called()
 
     @mock.patch("flumine.markets.middleware.config")
     def test__process_simulated_orders(self, mock_config):
         mock_config.simulated_strategy_isolation = False
         mock_market_book = mock.Mock()
         mock_market = mock.Mock()
@@ -303,20 +306,23 @@
             selection_id=123, handicap=1, status=OrderStatus.EXECUTABLE, simulated=False
         )
         mock_market.blotter.live_orders = [
             mock_order,
             mock_order_two,
             mock_order_three,
         ]
+        mock_runner = mock.Mock(traded={1: 2})
         mock_market_analytics = {
-            (mock_order.selection_id, mock_order.handicap): mock.Mock(traded={1: 2})
+            (mock_order.selection_id, mock_order.handicap): mock_runner
         }
         mock_market.market_book = mock_market_book
         self.middleware._process_simulated_orders(mock_market, mock_market_analytics)
-        mock_order.simulated.assert_called_with(mock_market_book, {1: 2})
+        mock_order.simulated.assert_called_with(
+            mock_market_book, (mock_runner.runner, {1: 2})
+        )
         mock_order_two.simulated.assert_not_called()
 
     def test__sort_orders(self):
         order_one = mock.Mock(side="LAY", bet_id=1)
         order_one.order_type.price = 1.01
         order_two = mock.Mock(side="LAY", bet_id=2)
         order_two.order_type.price = 1.02
@@ -368,15 +374,15 @@
 class RunnerAnalyticsTest(unittest.TestCase):
     def setUp(self) -> None:
         self.mock_runner = mock.Mock()
         self.mock_runner.ex.traded_volume = [{"price": 1.01, "size": 2}]
         self.runner_analytics = RunnerAnalytics(self.mock_runner)
 
     def test_init(self):
-        self.assertEqual(self.runner_analytics._runner, self.mock_runner)
+        self.assertEqual(self.runner_analytics.runner, self.mock_runner)
         self.assertEqual(
             self.runner_analytics._traded_volume, self.mock_runner.ex.traded_volume
         )
         self.assertEqual(self.runner_analytics.traded, {})
         self.assertEqual(self.runner_analytics._p_v, {1.01: 2})
 
     @mock.patch("flumine.markets.middleware.RunnerAnalytics._calculate_traded")
@@ -384,15 +390,15 @@
         mock_runner = mock.Mock()
         self.runner_analytics(mock_runner)
         mock__calculate_traded.assert_called_with(mock_runner.ex.traded_volume)
         self.assertEqual(
             self.runner_analytics._traded_volume, mock_runner.ex.traded_volume
         )
         self.assertEqual(self.runner_analytics.traded, mock__calculate_traded())
-        self.assertEqual(self.runner_analytics._runner, mock_runner)
+        self.assertEqual(self.runner_analytics.runner, mock_runner)
 
     def test__calculate_traded_dict_empty(self):
         self.runner_analytics._traded_volume = []
         self.assertEqual(self.runner_analytics._calculate_traded([]), {})
 
     def test__calculate_traded_dict_same(self):
         traded_volume = [{"price": 1.01, "size": 69}]
```

### Comparing `flumine-2.3.7/tests/test_order.py` & `flumine-2.4.0/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_orderpackage.py` & `flumine-2.4.0/tests/test_orderpackage.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_ordertype.py` & `flumine-2.4.0/tests/test_ordertype.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_process.py` & `flumine-2.4.0/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_responses.py` & `flumine-2.4.0/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_runnercontext.py` & `flumine-2.4.0/tests/test_runnercontext.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_simulated_utils.py` & `flumine-2.4.0/tests/test_simulated_utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_simulatedorder.py` & `flumine-2.4.0/tests/test_simulatedorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._process_traded")
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._process_sp")
     def test_call_process_traded(
         self, mock__process_sp, mock__process_traded, _, mock__get_runner
     ):
         mock_market_book = mock.Mock(bsp_reconciled=False)
         traded = {1: 2}
-        self.simulated(mock_market_book, traded)
+        mock_runner_book = mock.Mock()
+        self.simulated(mock_market_book, (mock_runner_book, traded))
         mock__process_sp.assert_not_called()
         mock__process_traded.assert_called_with(
             mock_market_book.publish_time_epoch, traded
         )
 
     @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._get_runner")
     @mock.patch(
@@ -1111,14 +1112,39 @@
 
     def test__calculate_process_traded_piq_match(self):
         self.simulated._piq = 4.00
         self.assertEqual(self.simulated._calculate_process_traded(1234585, 20.00), 12)
         self.assertEqual(self.simulated.matched, [[1234585, 12, 2.0]])
         self.assertEqual(self.simulated._piq, 0)
 
+    def test__process_available_back(self):
+        mock_runner = mock.Mock()
+        mock_runner.ex.available_to_back = [
+            {"price": 13, "size": 1},
+            {"price": 12, "size": 1},
+        ]
+        self.simulated._process_available(123, mock_runner)
+        self.assertEqual(self.simulated.matched, [[123, 13, 1], [123, 12, 1]])
+
+    def test_process_available_lay(self):
+        self.simulated.order.side = "LAY"
+        mock_runner = mock.Mock()
+        mock_runner.ex.available_to_lay = [
+            {"price": 10, "size": 1},
+            {"price": 11, "size": 1},
+        ]
+        self.simulated._process_available(123, mock_runner)
+        self.assertEqual(self.simulated.matched, [[123, 10, 1], [123, 11, 1]])
+
+    @mock.patch("flumine.simulation.simulatedorder.SimulatedOrder._update_matched")
+    def test__calculate_process_available(self, mock__update_matched):
+        self.simulated._calculate_process_available(123, 12, 2)
+        mock__update_matched.assert_called_with([123, 12, 2])
+        self.assertEqual(self.simulated._piq, 0)
+
     def test_take_sp(self):
         self.assertFalse(self.simulated.take_sp)
         self.simulated.order.order_type.ORDER_TYPE = OrderTypes.LIMIT_ON_CLOSE
         self.assertTrue(self.simulated.take_sp)
         self.simulated.order.order_type.ORDER_TYPE = OrderTypes.MARKET_ON_CLOSE
         self.assertTrue(self.simulated.take_sp)
         self.simulated.order.order_type.ORDER_TYPE = OrderTypes.LIMIT
```

### Comparing `flumine-2.3.7/tests/test_strategy.py` & `flumine-2.4.0/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_streams.py` & `flumine-2.4.0/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_trade.py` & `flumine-2.4.0/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_tradingcontrols.py` & `flumine-2.4.0/tests/test_tradingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_transaction.py` & `flumine-2.4.0/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_utils.py` & `flumine-2.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.3.7/tests/test_worker.py` & `flumine-2.4.0/tests/test_worker.py`

 * *Files identical despite different names*

