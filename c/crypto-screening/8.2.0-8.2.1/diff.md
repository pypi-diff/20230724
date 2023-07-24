# Comparing `tmp/crypto-screening-8.2.0.tar.gz` & `tmp/crypto-screening-8.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.2.0.tar", last modified: Mon Jul 24 09:53:55 2023, max compression
+gzip compressed data, was "crypto-screening-8.2.1.tar", last modified: Mon Jul 24 11:56:38 2023, max compression
```

## Comparing `crypto-screening-8.2.0.tar` & `crypto-screening-8.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.916527 crypto-screening-8.2.0/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:53:55.000000 crypto-screening-8.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-24 09:53:55.916527 crypto-screening-8.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.2.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.2.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.883527 crypto-screening-8.2.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.891527 crypto-screening-8.2.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17733 2023-07-22 15:48:11.000000 crypto-screening-8.2.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4773 2023-07-22 15:47:32.000000 crypto-screening-8.2.0/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.894527 crypto-screening-8.2.0/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.2.0/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.2.0/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.897527 crypto-screening-8.2.0/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.2.0/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24665 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16516 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21653 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    17728 2023-07-24 09:40:24.000000 crypto-screening-8.2.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19520 2023-07-22 15:47:21.000000 crypto-screening-8.2.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.2.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.2.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.2.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.905527 crypto-screening-8.2.0/crypto_screening/screeners/
--rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.2.0/crypto_screening/screeners/__init__.py
--rw-rw-rw-   0        0        0    23312 2023-07-24 09:37:18.000000 crypto-screening-8.2.0/crypto_screening/screeners/base.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.908527 crypto-screening-8.2.0/crypto_screening/screeners/callbacks/
--rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.2.0/crypto_screening/screeners/callbacks/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.2.0/crypto_screening/screeners/callbacks/base.py
--rw-rw-rw-   0        0        0     4400 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/screeners/callbacks/database.py
--rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/screeners/callbacks/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.910527 crypto-screening-8.2.0/crypto_screening/screeners/collectors/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.2.0/crypto_screening/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6271 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.2.0/crypto_screening/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.2.0/crypto_screening/screeners/combined.py
--rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.2.0/crypto_screening/screeners/container.py
--rw-rw-rw-   0        0        0    10976 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/screeners/database.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.913525 crypto-screening-8.2.0/crypto_screening/screeners/foundation/
--rw-rw-rw-   0        0        0    10462 2023-07-24 09:37:33.000000 crypto-screening-8.2.0/crypto_screening/screeners/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.2.0/crypto_screening/screeners/foundation/protocols.py
--rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.2.0/crypto_screening/screeners/foundation/state.py
--rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.2.0/crypto_screening/screeners/foundation/waiting.py
--rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/screeners/market.py
--rw-rw-rw-   0        0        0    22099 2023-07-24 09:38:59.000000 crypto-screening-8.2.0/crypto_screening/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11814 2023-07-24 09:39:14.000000 crypto-screening-8.2.0/crypto_screening/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11410 2023-07-24 09:39:34.000000 crypto-screening-8.2.0/crypto_screening/screeners/orders.py
--rw-rw-rw-   0        0        0    16921 2023-07-24 09:39:41.000000 crypto-screening-8.2.0/crypto_screening/screeners/recorder.py
--rw-rw-rw-   0        0        0    11479 2023-07-24 09:39:59.000000 crypto-screening-8.2.0/crypto_screening/screeners/trades.py
--rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.2.0/crypto_screening/screeners/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.875518 crypto-screening-8.2.0/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.913525 crypto-screening-8.2.0/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.2.0/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-8.2.0/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.915526 crypto-screening-8.2.0/crypto_screening/utils/
--rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.2.0/crypto_screening/utils/base.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-8.2.0/crypto_screening/utils/process.py
--rw-rw-rw-   0        0        0     3605 2023-07-22 15:45:17.000000 crypto-screening-8.2.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.888527 crypto-screening-8.2.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-24 09:53:55.000000 crypto-screening-8.2.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2023-07-24 09:53:55.000000 crypto-screening-8.2.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:53:55.000000 crypto-screening-8.2.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-24 09:53:55.000000 crypto-screening-8.2.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-24 09:53:55.000000 crypto-screening-8.2.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-24 09:49:05.000000 crypto-screening-8.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.2.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 09:53:55.916527 crypto-screening-8.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-24 09:48:54.000000 crypto-screening-8.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.706159 crypto-screening-8.2.1/
+-rw-rw-rw-   0        0        0      196 2023-07-24 11:56:36.000000 crypto-screening-8.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-24 11:56:38.706159 crypto-screening-8.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.2.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.2.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.533609 crypto-screening-8.2.1/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.556159 crypto-screening-8.2.1/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17733 2023-07-22 15:48:11.000000 crypto-screening-8.2.1/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4773 2023-07-22 15:47:32.000000 crypto-screening-8.2.1/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.585159 crypto-screening-8.2.1/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.2.1/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.2.1/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.608190 crypto-screening-8.2.1/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.2.1/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24665 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16516 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21653 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    17772 2023-07-24 11:55:18.000000 crypto-screening-8.2.1/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19550 2023-07-24 11:56:16.000000 crypto-screening-8.2.1/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.2.1/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.2.1/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.2.1/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.640189 crypto-screening-8.2.1/crypto_screening/screeners/
+-rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.2.1/crypto_screening/screeners/__init__.py
+-rw-rw-rw-   0        0        0    23312 2023-07-24 09:37:18.000000 crypto-screening-8.2.1/crypto_screening/screeners/base.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.658190 crypto-screening-8.2.1/crypto_screening/screeners/callbacks/
+-rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.2.1/crypto_screening/screeners/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.2.1/crypto_screening/screeners/callbacks/base.py
+-rw-rw-rw-   0        0        0     4400 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/screeners/callbacks/database.py
+-rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/screeners/callbacks/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.677159 crypto-screening-8.2.1/crypto_screening/screeners/collectors/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.2.1/crypto_screening/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6271 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.2.1/crypto_screening/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.2.1/crypto_screening/screeners/combined.py
+-rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.2.1/crypto_screening/screeners/container.py
+-rw-rw-rw-   0        0        0    10976 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/screeners/database.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.694160 crypto-screening-8.2.1/crypto_screening/screeners/foundation/
+-rw-rw-rw-   0        0        0    10462 2023-07-24 09:37:33.000000 crypto-screening-8.2.1/crypto_screening/screeners/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.2.1/crypto_screening/screeners/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.2.1/crypto_screening/screeners/foundation/state.py
+-rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.2.1/crypto_screening/screeners/foundation/waiting.py
+-rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/screeners/market.py
+-rw-rw-rw-   0        0        0    22099 2023-07-24 09:38:59.000000 crypto-screening-8.2.1/crypto_screening/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11814 2023-07-24 09:39:14.000000 crypto-screening-8.2.1/crypto_screening/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11410 2023-07-24 09:39:34.000000 crypto-screening-8.2.1/crypto_screening/screeners/orders.py
+-rw-rw-rw-   0        0        0    16921 2023-07-24 09:39:41.000000 crypto-screening-8.2.1/crypto_screening/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11479 2023-07-24 09:39:59.000000 crypto-screening-8.2.1/crypto_screening/screeners/trades.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.2.1/crypto_screening/screeners/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.520609 crypto-screening-8.2.1/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.699190 crypto-screening-8.2.1/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.2.1/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10471 2023-07-24 11:53:22.000000 crypto-screening-8.2.1/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.705159 crypto-screening-8.2.1/crypto_screening/utils/
+-rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.2.1/crypto_screening/utils/base.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-8.2.1/crypto_screening/utils/process.py
+-rw-rw-rw-   0        0        0     3527 2023-07-24 11:53:22.000000 crypto-screening-8.2.1/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.548160 crypto-screening-8.2.1/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-24 11:56:38.000000 crypto-screening-8.2.1/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-07-24 11:56:38.000000 crypto-screening-8.2.1/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 11:56:38.000000 crypto-screening-8.2.1/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-24 11:56:38.000000 crypto-screening-8.2.1/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-24 11:56:38.000000 crypto-screening-8.2.1/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-24 11:56:36.000000 crypto-screening-8.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.2.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 11:56:38.706159 crypto-screening-8.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-24 11:56:25.000000 crypto-screening-8.2.1/setup.py
```

### Comparing `crypto-screening-8.2.0/PKG-INFO` & `crypto-screening-8.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.2.0
+Version: 8.2.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.2.0/README.md` & `crypto-screening-8.2.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/build.py` & `crypto-screening-8.2.1/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/collect/assets.py` & `crypto-screening-8.2.1/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/collect/exchanges.py` & `crypto-screening-8.2.1/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.2.1/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.2.1/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/collect/market/orders.py` & `crypto-screening-8.2.1/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.2.1/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.2.1/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.2.1/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/collect/market/trades.py` & `crypto-screening-8.2.1/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/collect/screeners.py` & `crypto-screening-8.2.1/crypto_screening/collect/screeners.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Optional, Dict, Iterable,
     Set, Union, Tuple, List
 )
 
 import pandas as pd
 from attrs import define
 
-from crypto_screening.symbols import symbol_to_pair, symbol_to_parts
+from crypto_screening.symbols import symbol_to_pair, symbol_to_parts, adjust_symbol
 from crypto_screening.collect.symbols import (
     matching_symbol_pair, MarketSymbolSignature, exchanges_symbols
 )
 from crypto_screening.screeners import BaseScreener, BaseMarketScreener
 
 __all__ = [
     "matching_screener_signatures",
@@ -154,26 +154,26 @@
 
     data = data or matching_screener_pairs(
         screeners=screeners, matches=matches,
         separator=separator, empty=empty
     )
 
     for screener1, screener2 in data:
-        currency1 = symbol_to_pair(screener1.symbol).quote
-        currency2 = symbol_to_pair(screener2.symbol).quote
+        asset1, currency1 = symbol_to_parts(adjust_symbol(screener1.symbol))
+        asset2, currency2 = symbol_to_pair(adjust_symbol(screener2.symbol))
 
         pairs.append(
             (
                 MarketScreenerSignature(
-                    asset=currency1, currency=currency1,
+                    asset=asset1, currency=currency1,
                     exchange=screener1.exchange,
                     screener=screener1
                 ),
                 MarketScreenerSignature(
-                    asset=currency2, currency=currency2,
+                    asset=asset2, currency=currency2,
                     exchange=screener2.exchange,
                     screener=screener2
                 )
             )
         )
     # end for
```

### Comparing `crypto-screening-8.2.0/crypto_screening/collect/symbols.py` & `crypto-screening-8.2.1/crypto_screening/collect/symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,16 +620,16 @@
     new_pairs = []
 
     pairs = pairs or matching_symbol_pairs(
         data=data, matches=matches, separator=separator
     )
 
     for (exchange1, symbol1), (exchange2, symbol2) in pairs:
-        asset1, currency1 = symbol_to_parts(symbol1)
-        asset2, currency2 = symbol_to_parts(symbol2)
+        asset1, currency1 = symbol_to_parts(adjust_symbol(symbol1))
+        asset2, currency2 = symbol_to_parts(adjust_symbol(symbol2))
 
         new_pairs.append(
             (
                 MarketSymbolSignature(
                     asset=asset1, currency=currency1,
                     exchange=exchange1
                 ),
```

### Comparing `crypto-screening-8.2.0/crypto_screening/dataset.py` & `crypto-screening-8.2.1/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/exchanges.py` & `crypto-screening-8.2.1/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/interval.py` & `crypto-screening-8.2.1/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/base.py` & `crypto-screening-8.2.1/crypto_screening/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/callbacks/base.py` & `crypto-screening-8.2.1/crypto_screening/screeners/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/callbacks/database.py` & `crypto-screening-8.2.1/crypto_screening/screeners/callbacks/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/callbacks/sockets.py` & `crypto-screening-8.2.1/crypto_screening/screeners/callbacks/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/collectors/base.py` & `crypto-screening-8.2.1/crypto_screening/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/collectors/database.py` & `crypto-screening-8.2.1/crypto_screening/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/collectors/sockets.py` & `crypto-screening-8.2.1/crypto_screening/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/combined.py` & `crypto-screening-8.2.1/crypto_screening/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/container.py` & `crypto-screening-8.2.1/crypto_screening/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/database.py` & `crypto-screening-8.2.1/crypto_screening/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/foundation/data.py` & `crypto-screening-8.2.1/crypto_screening/screeners/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/foundation/protocols.py` & `crypto-screening-8.2.1/crypto_screening/screeners/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/foundation/state.py` & `crypto-screening-8.2.1/crypto_screening/screeners/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/foundation/waiting.py` & `crypto-screening-8.2.1/crypto_screening/screeners/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/market.py` & `crypto-screening-8.2.1/crypto_screening/screeners/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/ohlcv.py` & `crypto-screening-8.2.1/crypto_screening/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/orderbook.py` & `crypto-screening-8.2.1/crypto_screening/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/orders.py` & `crypto-screening-8.2.1/crypto_screening/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/recorder.py` & `crypto-screening-8.2.1/crypto_screening/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/trades.py` & `crypto-screening-8.2.1/crypto_screening/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/screeners/waiting.py` & `crypto-screening-8.2.1/crypto_screening/screeners/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.2.1/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/symbols.py` & `crypto-screening-8.2.1/crypto_screening/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,18 @@
     :return: The symbol.
     """
 
     if separator is None:
         separator = Separator.value
     # end if
 
+    if separator not in symbol:
+        symbol = adjust_symbol(symbol, separator=separator)
+    # end if
+
     if separator in symbol:
         base = symbol[:symbol.find(separator)]
         quote = symbol[symbol.find(separator) + len(separator):]
 
     else:
         raise ValueError(
             f"Cannot separate symbol '{symbol}' because "
```

### Comparing `crypto-screening-8.2.0/crypto_screening/utils/base.py` & `crypto-screening-8.2.1/crypto_screening/utils/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/utils/process.py` & `crypto-screening-8.2.1/crypto_screening/utils/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/crypto_screening/validate.py` & `crypto-screening-8.2.1/crypto_screening/validate.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,21 +21,18 @@
 
     :param symbol: The symbol of the assets.
     :param symbols: The valid symbols.
 
     :return: The validation-value.
     """
 
-    symbols = [adjust_symbol(symbol=s) for s in symbols]
-
-    symbol = find_string_value(
-        value=adjust_symbol(symbol=symbol), values=symbols
+    return (
+        adjust_symbol(symbol=symbol) in
+        [adjust_symbol(symbol=s) for s in symbols]
     )
-
-    return symbol in symbols
 # end is_valid_symbol
 
 def validate_symbol(
         exchange: str,
         symbol: str,
         symbols: Iterable[str],
         exchanges: Optional[Iterable[str]] = None,
```

### Comparing `crypto-screening-8.2.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.2.1/crypto_screening.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.2.0
+Version: 8.2.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.2.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.2.1/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.0/pyproject.toml` & `crypto-screening-8.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.2.0'
+version = '8.2.1'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.2.0/setup.py` & `crypto-screening-8.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='8.2.0',
+        version='8.2.1',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

