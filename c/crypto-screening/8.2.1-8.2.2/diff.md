# Comparing `tmp/crypto-screening-8.2.1.tar.gz` & `tmp/crypto-screening-8.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.2.1.tar", last modified: Mon Jul 24 11:56:38 2023, max compression
+gzip compressed data, was "crypto-screening-8.2.2.tar", last modified: Mon Jul 24 18:34:38 2023, max compression
```

## Comparing `crypto-screening-8.2.1.tar` & `crypto-screening-8.2.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.706159 crypto-screening-8.2.1/
--rw-rw-rw-   0        0        0      196 2023-07-24 11:56:36.000000 crypto-screening-8.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-24 11:56:38.706159 crypto-screening-8.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.2.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.2.1/build.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.533609 crypto-screening-8.2.1/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.556159 crypto-screening-8.2.1/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17733 2023-07-22 15:48:11.000000 crypto-screening-8.2.1/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4773 2023-07-22 15:47:32.000000 crypto-screening-8.2.1/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.585159 crypto-screening-8.2.1/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.2.1/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.2.1/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.608190 crypto-screening-8.2.1/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.2.1/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24665 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16516 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21653 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    17772 2023-07-24 11:55:18.000000 crypto-screening-8.2.1/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19550 2023-07-24 11:56:16.000000 crypto-screening-8.2.1/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.2.1/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.2.1/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.2.1/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.640189 crypto-screening-8.2.1/crypto_screening/screeners/
--rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.2.1/crypto_screening/screeners/__init__.py
--rw-rw-rw-   0        0        0    23312 2023-07-24 09:37:18.000000 crypto-screening-8.2.1/crypto_screening/screeners/base.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.658190 crypto-screening-8.2.1/crypto_screening/screeners/callbacks/
--rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.2.1/crypto_screening/screeners/callbacks/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.2.1/crypto_screening/screeners/callbacks/base.py
--rw-rw-rw-   0        0        0     4400 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/screeners/callbacks/database.py
--rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/screeners/callbacks/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.677159 crypto-screening-8.2.1/crypto_screening/screeners/collectors/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.2.1/crypto_screening/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6271 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.2.1/crypto_screening/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.2.1/crypto_screening/screeners/combined.py
--rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.2.1/crypto_screening/screeners/container.py
--rw-rw-rw-   0        0        0    10976 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/screeners/database.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.694160 crypto-screening-8.2.1/crypto_screening/screeners/foundation/
--rw-rw-rw-   0        0        0    10462 2023-07-24 09:37:33.000000 crypto-screening-8.2.1/crypto_screening/screeners/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.2.1/crypto_screening/screeners/foundation/protocols.py
--rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.2.1/crypto_screening/screeners/foundation/state.py
--rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.2.1/crypto_screening/screeners/foundation/waiting.py
--rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.2.1/crypto_screening/screeners/market.py
--rw-rw-rw-   0        0        0    22099 2023-07-24 09:38:59.000000 crypto-screening-8.2.1/crypto_screening/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11814 2023-07-24 09:39:14.000000 crypto-screening-8.2.1/crypto_screening/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11410 2023-07-24 09:39:34.000000 crypto-screening-8.2.1/crypto_screening/screeners/orders.py
--rw-rw-rw-   0        0        0    16921 2023-07-24 09:39:41.000000 crypto-screening-8.2.1/crypto_screening/screeners/recorder.py
--rw-rw-rw-   0        0        0    11479 2023-07-24 09:39:59.000000 crypto-screening-8.2.1/crypto_screening/screeners/trades.py
--rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.2.1/crypto_screening/screeners/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.520609 crypto-screening-8.2.1/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.699190 crypto-screening-8.2.1/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.2.1/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10471 2023-07-24 11:53:22.000000 crypto-screening-8.2.1/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.705159 crypto-screening-8.2.1/crypto_screening/utils/
--rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.2.1/crypto_screening/utils/base.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-8.2.1/crypto_screening/utils/process.py
--rw-rw-rw-   0        0        0     3527 2023-07-24 11:53:22.000000 crypto-screening-8.2.1/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:56:38.548160 crypto-screening-8.2.1/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-24 11:56:38.000000 crypto-screening-8.2.1/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2023-07-24 11:56:38.000000 crypto-screening-8.2.1/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 11:56:38.000000 crypto-screening-8.2.1/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-24 11:56:38.000000 crypto-screening-8.2.1/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-24 11:56:38.000000 crypto-screening-8.2.1/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-24 11:56:36.000000 crypto-screening-8.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.2.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 11:56:38.706159 crypto-screening-8.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-24 11:56:25.000000 crypto-screening-8.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.510038 crypto-screening-8.2.2/
+-rw-rw-rw-   0        0        0      196 2023-07-24 18:34:36.000000 crypto-screening-8.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-24 18:34:38.510038 crypto-screening-8.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.2.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.2.2/build.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.348652 crypto-screening-8.2.2/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.366227 crypto-screening-8.2.2/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.2.2/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     5005 2023-07-24 18:29:23.000000 crypto-screening-8.2.2/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.386309 crypto-screening-8.2.2/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.2.2/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.2.2/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.2.2/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.2.2/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.388818 crypto-screening-8.2.2/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.2.2/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24665 2023-07-24 09:29:05.000000 crypto-screening-8.2.2/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16516 2023-07-24 09:29:05.000000 crypto-screening-8.2.2/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21653 2023-07-24 09:29:05.000000 crypto-screening-8.2.2/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.2.2/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    17976 2023-07-24 18:15:45.000000 crypto-screening-8.2.2/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19569 2023-07-24 18:21:12.000000 crypto-screening-8.2.2/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.2.2/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.2.2/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.2.2/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.446350 crypto-screening-8.2.2/crypto_screening/screeners/
+-rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.2.2/crypto_screening/screeners/__init__.py
+-rw-rw-rw-   0        0        0    23312 2023-07-24 09:37:18.000000 crypto-screening-8.2.2/crypto_screening/screeners/base.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.467943 crypto-screening-8.2.2/crypto_screening/screeners/callbacks/
+-rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.2.2/crypto_screening/screeners/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.2.2/crypto_screening/screeners/callbacks/base.py
+-rw-rw-rw-   0        0        0     4400 2023-07-24 09:29:05.000000 crypto-screening-8.2.2/crypto_screening/screeners/callbacks/database.py
+-rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.2.2/crypto_screening/screeners/callbacks/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.486794 crypto-screening-8.2.2/crypto_screening/screeners/collectors/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.2.2/crypto_screening/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6271 2023-07-24 09:29:05.000000 crypto-screening-8.2.2/crypto_screening/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.2.2/crypto_screening/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.2.2/crypto_screening/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.2.2/crypto_screening/screeners/combined.py
+-rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.2.2/crypto_screening/screeners/container.py
+-rw-rw-rw-   0        0        0    10976 2023-07-24 09:29:05.000000 crypto-screening-8.2.2/crypto_screening/screeners/database.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.501459 crypto-screening-8.2.2/crypto_screening/screeners/foundation/
+-rw-rw-rw-   0        0        0    10462 2023-07-24 09:37:33.000000 crypto-screening-8.2.2/crypto_screening/screeners/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.2.2/crypto_screening/screeners/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.2.2/crypto_screening/screeners/foundation/state.py
+-rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.2.2/crypto_screening/screeners/foundation/waiting.py
+-rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.2.2/crypto_screening/screeners/market.py
+-rw-rw-rw-   0        0        0    22099 2023-07-24 09:38:59.000000 crypto-screening-8.2.2/crypto_screening/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11814 2023-07-24 09:39:14.000000 crypto-screening-8.2.2/crypto_screening/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11410 2023-07-24 09:39:34.000000 crypto-screening-8.2.2/crypto_screening/screeners/orders.py
+-rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.2.2/crypto_screening/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11479 2023-07-24 09:39:59.000000 crypto-screening-8.2.2/crypto_screening/screeners/trades.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.2.2/crypto_screening/screeners/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.341053 crypto-screening-8.2.2/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.502459 crypto-screening-8.2.2/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.2.2/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10471 2023-07-24 11:53:22.000000 crypto-screening-8.2.2/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.509037 crypto-screening-8.2.2/crypto_screening/utils/
+-rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.2.2/crypto_screening/utils/base.py
+-rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.2.2/crypto_screening/utils/process.py
+-rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.2.2/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:34:38.364257 crypto-screening-8.2.2/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-24 18:34:38.000000 crypto-screening-8.2.2/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-07-24 18:34:38.000000 crypto-screening-8.2.2/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 18:34:38.000000 crypto-screening-8.2.2/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-24 18:34:38.000000 crypto-screening-8.2.2/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-24 18:34:38.000000 crypto-screening-8.2.2/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-24 18:34:36.000000 crypto-screening-8.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.2.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.2.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 18:34:38.510038 crypto-screening-8.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-24 18:34:27.000000 crypto-screening-8.2.2/setup.py
```

### Comparing `crypto-screening-8.2.1/PKG-INFO` & `crypto-screening-8.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.2.1
+Version: 8.2.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.2.1/README.md` & `crypto-screening-8.2.2/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/build.py` & `crypto-screening-8.2.2/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/collect/assets.py` & `crypto-screening-8.2.2/crypto_screening/collect/symbols.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,550 +1,647 @@
-# assets.py
+# symbols.py
 
-from typing import Optional, Dict, Iterable, Set, Union
+import warnings
+from typing import (
+    Optional, Dict, Iterable,
+    Set, Union, Tuple
+)
 
-from crypto_screening.utils.process import mutual_string_values
-from crypto_screening.symbols import symbol_to_parts, symbol_to_pair
-from crypto_screening.collect.exchanges import exchanges_data
-from crypto_screening.collect.symbols import (
-    all_exchange_symbols, exchange_symbols
+from attrs import define
+
+from represent import represent
+
+from multithreading import Caller, multi_threaded_call
+
+from crypto_screening.utils.process import (
+    find_string_value, upper_string_values,
+    mutual_string_values, string_in_values
 )
+from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
+from crypto_screening.symbols import (
+    symbol_to_parts, adjust_symbol, Separator
+)
+from crypto_screening.validate import validate_exchange
+from crypto_screening.collect.exchanges import exchanges_data
 
 __all__ = [
-    "exchanges_assets",
-    "mutual_exchanges_assets",
-    "exchange_assets",
-    "exchange_quote_assets",
-    "exchange_base_assets",
-    "all_exchange_assets",
-    "all_exchange_base_assets",
-    "all_exchange_quote_assets",
-    "exchanges_base_assets",
-    "exchanges_quote_assets",
-    "mutual_exchanges_base_assets",
-    "mutual_exchanges_quote_assets",
-    "exchanges_symbols_assets",
-    "exchanges_symbols_quote_assets",
-    "exchanges_symbols_base_assets"
+    "exchanges_symbols",
+    "mutual_exchanges_symbols",
+    "include_symbols",
+    "exclude_symbols",
+    "exchange_symbols",
+    "all_exchange_symbols",
+    "matching_symbol_pair",
+    "matching_symbol_pairs",
+    "MarketSymbolSignature",
+    "matching_symbol_signatures",
+    "include_exchanges_symbols",
+    "exclude_exchanges_symbols",
+    "all_exchanges_symbols"
 ]
 
-def all_exchange_assets(
-        exchange: str,
+def include_symbols(
+        symbols: Iterable[str],
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
+        bases: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None,
+        included: Optional[Iterable[str]] = None
 ) -> Set[str]:
     """
-    Collects the symbols from the exchanges.
+    Removes all symbols with not matching base or quote.
 
-    :param exchange: The name of the exchange.
+    :param symbols: The symbols to filter.
+    :param separator: The separator for the symbols.
+    :param bases: The bases to include.
     :param adjust: The value to adjust the invalid exchanges.
-    :param separator: The separator of the assets.
+    :param quotes: The quotes to include.
+    :param included: The symbols to include.
 
-    :return: The data of the exchanges.
+    :return: The filtered symbols.
     """
 
-    symbols = all_exchange_symbols(
-        exchange=exchange, adjust=adjust, separator=separator
-    )
+    saved = set()
 
-    assets = []
+    quotes = upper_string_values(quotes or [])
+    bases = upper_string_values(bases or [])
+    included = upper_string_values(included or [])
 
     for symbol in symbols:
-        base, quote = symbol_to_parts(symbol=symbol, separator=separator)
+        if symbol in included:
+            saved.add(symbol)
+
+            continue
+        # end if
+
+        try:
+            symbol = adjust_symbol(symbol=symbol, separator=separator)
+
+        except ValueError as e:
+            if adjust:
+                continue
 
-        if base not in assets:
-            assets.append(base)
+            else:
+                raise e
+            # end if
+        # end try
+
+        if symbol in included:
+            saved.add(symbol)
+
+            continue
         # end if
 
-        if quote not in assets:
-            assets.append(quote)
+        base, quote = symbol_to_parts(
+            symbol=symbol, separator=separator
+        )
+
+        if (
+            string_in_values(value=base, values=bases) or
+            string_in_values(value=quote, values=quotes)
+        ):
+            saved.add(symbol)
         # end if
     # end for
 
-    return set(assets)
-# end all_exchange_assets
+    return saved
+# end include_symbols
 
-def all_exchange_base_assets(
-        exchange: str,
+def exclude_symbols(
+        symbols: Iterable[str],
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
+        bases: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None,
+        excluded: Optional[Iterable[str]] = None
 ) -> Set[str]:
     """
-    Collects the symbols from the exchanges.
+    Removes all symbols with the matching base or quote.
 
-    :param exchange: The name of the exchange.
+    :param symbols: The symbols to filter.
+    :param separator: The separator for the symbols.
+    :param bases: The bases to exclude.
+    :param quotes: The quotes to exclude.
     :param adjust: The value to adjust the invalid exchanges.
-    :param separator: The separator of the assets.
+    :param excluded: The symbols to exclude.
 
-    :return: The data of the exchanges.
+    :return: The filtered symbols.
     """
 
-    symbols = all_exchange_symbols(
-        exchange=exchange, adjust=adjust, separator=separator
-    )
+    saved = set()
 
-    assets = []
+    quotes = upper_string_values(quotes or [])
+    bases = upper_string_values(bases or [])
+    excluded = upper_string_values(excluded or [])
 
     for symbol in symbols:
-        base, _ = symbol_to_parts(symbol=symbol, separator=separator)
+        if symbol in excluded:
+            continue
+        # end if
+
+        try:
+            symbol = adjust_symbol(symbol=symbol, separator=separator)
 
-        if base not in assets:
-            assets.append(base)
+        except ValueError as e:
+            if adjust:
+                continue
+
+            else:
+                raise e
+            # end if
+        # end try
+
+        if symbol in excluded:
+            continue
         # end if
+
+        base, quote = symbol_to_parts(symbol=symbol, separator=separator)
+
+        if (
+            string_in_values(value=base, values=bases) or
+            string_in_values(value=quote, values=quotes)
+        ):
+            continue
+        # end if
+
+        saved.add(symbol)
     # end for
 
-    return set(assets)
-# end all_exchange_base_assets
+    return set(saved)
+# end exclude_symbols
 
-def all_exchange_quote_assets(
-        exchange: str,
-        separator: Optional[str] = None,
-        adjust: Optional[bool] = True,
-) -> Set[str]:
+def include_exchanges_symbols(
+        data: Dict[str, Iterable[str]],
+        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+) -> Dict[str, Set[str]]:
     """
-    Collects the symbols from the exchanges.
+    Removes all symbols with not matching base or quote.
 
-    :param exchange: The name of the exchange.
-    :param adjust: The value to adjust the invalid exchanges.
-    :param separator: The separator of the assets.
+    :param data: The data to filter.
+    :param bases: The bases to include.
+    :param quotes: The quotes to include.
+    :param included: The symbols to include.
 
-    :return: The data of the exchanges.
+    :return: The filtered symbols.
     """
 
-    symbols = all_exchange_symbols(
-        exchange=exchange, adjust=adjust, separator=separator
-    )
+    if all(value is None for value in (bases, quotes, included)):
+        return {exchange: set(symbols) for exchange, symbols in data.items()}
+    # end if
+
+    if not isinstance(quotes, dict):
+        saved_quotes = quotes
+        quotes = {exchange: saved_quotes for exchange in data}
+    # end if
+
+    if not isinstance(bases, dict):
+        saved_bases = bases
+        bases = {exchange: saved_bases for exchange in data}
+    # end if
+
+    if not isinstance(included, dict):
+        saved_included = included
+        included = {exchange: saved_included for exchange in data}
+    # end if
 
-    assets = []
+    return {
+        exchange: saved for exchange, symbols in data.items()
+        if (
+            saved := include_symbols(
+                symbols=symbols,
+                bases=bases.get(exchange, None),
+                quotes=quotes.get(exchange, None),
+                included=included.get(exchange, None)
+            )
+        )
+    }
+# end include_exchanges_symbols
 
-    for symbol in symbols:
-        _, quote = symbol_to_parts(symbol=symbol, separator=separator)
+def exclude_exchanges_symbols(
+        data: Dict[str, Iterable[str]],
+        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+) -> Dict[str, Set[str]]:
+    """
+    Removes all symbols with the matching base or quote.
 
-        if quote not in assets:
-            assets.append(quote)
-        # end if
-    # end for
+    :param data: The data to filter.
+    :param bases: The bases to exclude.
+    :param quotes: The quotes to exclude.
+    :param excluded: The symbols to exclude.
+
+    :return: The filtered symbols.
+    """
+
+    if all(value is None for value in (bases, quotes, excluded)):
+        return {exchange: set(symbols) for exchange, symbols in data.items()}
+    # end if
+
+    if not isinstance(quotes, dict):
+        saved_quotes = quotes
+        quotes = {exchange: saved_quotes for exchange in data}
+    # end if
+
+    if not isinstance(bases, dict):
+        saved_bases = bases
+        bases = {exchange: saved_bases for exchange in data}
+    # end if
+
+    if not isinstance(excluded, dict):
+        saved_excluded = excluded
+        excluded = {exchange: saved_excluded for exchange in data}
+    # end if
 
-    return set(assets)
-# end all_exchange_quote_assets
+    return {
+        exchange: saved for exchange, symbols in data.items()
+        if (
+            saved := exclude_symbols(
+                symbols=symbols,
+                bases=bases.get(exchange, None),
+                quotes=quotes.get(exchange, None),
+                excluded=excluded.get(exchange, None)
+            )
+        )
+    }
+# end exclude_exchanges_symbols
 
-def exchange_assets(
+def all_exchange_symbols(
         exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
-        bases: Optional[Iterable[str]] = None,
-        quotes: Optional[Iterable[str]] = None,
-        included: Optional[Iterable[str]] = None,
-        excluded: Optional[Iterable[str]] = None
+        test: Optional[bool] = False
 ) -> Set[str]:
     """
-    Collects the assets from the exchanges.
+    Collects the symbols from the exchanges.
 
     :param exchange: The name of the exchange.
-    :param bases: The bases of the asset pairs.
-    :param quotes: The quotes of the asset pairs.
     :param adjust: The value to adjust the invalid exchanges.
-    :param separator: The separator for the symbols.
-    :param included: The symbols to include.
-    :param excluded: The excluded symbols.
+    :param separator: The separator of the assets.
+    :param test: Include test assets.
 
     :return: The data of the exchanges.
     """
 
-    symbols = exchange_symbols(
-        exchange=exchange, separator=separator, bases=bases,
-        quotes=quotes, excluded=excluded, adjust=adjust, included=included
-    )
+    validate_exchange(exchange=exchange, exchanges=EXCHANGE_NAMES)
 
-    assets = []
+    try:
+        found_symbols: Iterable[str] = EXCHANGES[
+            find_string_value(value=exchange, values=EXCHANGES)
+        ].symbols()
 
-    for symbol in symbols:
-        base, quote = symbol_to_parts(symbol=symbol, separator=separator)
+    except Exception as e:
+        error_message = (
+            f"Cannot fetch symbols of '{exchange}' exchange: {str(e)}."
+        )
+
+        if not adjust:
+            raise RuntimeError(error_message)
 
-        if base not in assets:
-            assets.append(base)
+        else:
+            warnings.warn(error_message)
+
+            return set()
         # end if
+    # end try
+
+    symbols = set()
 
-        if quote not in assets:
-            assets.append(quote)
+    if separator is None:
+        separator = Separator.value
+    # end if
+
+    for symbol in found_symbols:
+        try:
+            symbol = adjust_symbol(symbol=symbol, separator=separator)
+
+            if symbol.count(separator) != 1:
+                raise ValueError(
+                    f"Invalid symbol structure: {symbol}. "
+                    f"Symbol must contain only one separator."
+                )
+            # end if
+
+        except ValueError as e:
+            if adjust:
+                continue
+
+            else:
+                raise e
+            # end if
+        # end try
+
+        base, quote = symbol_to_parts(symbol=symbol, separator=separator)
+
+        if (not test) and base.startswith("TEST") and quote.startswith("TEST"):
+            continue
         # end if
+
+        symbols.add(symbol)
     # end for
 
-    return set(assets)
-# end exchange_assets
+    return symbols
+# end all_exchange_symbols
 
-def exchange_base_assets(
-        exchange: str,
+def all_exchanges_symbols(
+        exchanges: Iterable[str],
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
-        bases: Optional[Iterable[str]] = None,
-        quotes: Optional[Iterable[str]] = None,
-        included: Optional[Iterable[str]] = None,
-        excluded: Optional[Iterable[str]] = None
-) -> Set[str]:
+        test: Optional[bool] = False
+) -> Dict[str, Set[str]]:
     """
-    Collects the assets from the exchanges.
+    Collects the symbols from the exchanges.
 
-    :param exchange: The name of the exchange.
-    :param bases: The bases of the asset pairs.
+    :param exchanges: The name of the exchange.
     :param adjust: The value to adjust the invalid exchanges.
-    :param quotes: The quotes of the asset pairs.
-    :param separator: The separator for the symbols.
-    :param included: The symbols to include.
-    :param excluded: The excluded symbols.
+    :param separator: The separator of the assets.
+    :param test: Include test assets.
 
     :return: The data of the exchanges.
     """
 
-    symbols = exchange_symbols(
-        exchange=exchange, separator=separator, bases=bases,
-        quotes=quotes, excluded=excluded, adjust=adjust, included=included
+    results = multi_threaded_call(
+        [
+            Caller(
+                target=all_exchange_symbols, kwargs=dict(
+                    exchange=exchange, separator=separator,
+                    adjust=adjust, test=test
+                ), identifier=exchange
+            ) for exchange in exchanges
+        ]
     )
 
-    assets = []
-
-    for symbol in symbols:
-        base, _ = symbol_to_parts(symbol=symbol, separator=separator)
-
-        if base not in assets:
-            assets.append(base)
-        # end if
-    # end for
-
-    return set(assets)
-# end exchange_assets
+    return {
+        exchange: results.results(exchange).returns
+        for exchange in exchanges
+    }
+# end all_exchanges_symbols
 
-def exchange_quote_assets(
-        exchange: str,
+def exchange_symbols(
+        exchange: Optional[str] = None,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         bases: Optional[Iterable[str]] = None,
         quotes: Optional[Iterable[str]] = None,
         included: Optional[Iterable[str]] = None,
         excluded: Optional[Iterable[str]] = None
 ) -> Set[str]:
     """
-    Collects the assets from the exchanges.
+    Collects the symbols from the exchanges.
 
     :param exchange: The name of the exchange.
-    :param bases: The bases of the asset pairs.
-    :param adjust: The value to adjust the invalid exchanges.
     :param quotes: The quotes of the asset pairs.
-    :param separator: The separator for the symbols.
+    :param adjust: The value to adjust the invalid exchanges.
+    :param bases: The bases of the asset pairs.
+    :param separator: The separator of the assets.
     :param included: The symbols to include.
     :param excluded: The excluded symbols.
 
     :return: The data of the exchanges.
     """
 
-    symbols = exchange_symbols(
-        exchange=exchange, separator=separator, bases=bases,
-        quotes=quotes, excluded=excluded, adjust=adjust, included=included
+    symbols = all_exchange_symbols(
+        exchange=exchange, adjust=adjust, separator=separator
     )
 
-    assets = []
-
-    for symbol in symbols:
-        _, quote = symbol_to_parts(symbol=symbol, separator=separator)
-
-        if quote not in assets:
-            assets.append(quote)
-        # end if
-    # end for
-
-    return set(assets)
-# end exchange_assets
-
-def exchanges_assets(
-        exchanges: Optional[Iterable[str]] = None,
-        adjust: Optional[bool] = True,
-        separator: Optional[str] = None,
-        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
-) -> Dict[str, Set[str]]:
-    """
-    Collects the symbols from the exchanges.
-
-    :param exchanges: The exchanges.
-    :param quotes: The quotes of the asset pairs.
-    :param bases: The bases of the asset pairs.
-    :param excluded: The excluded symbols.
-    :param adjust: The value to adjust the invalid exchanges.
-    :param separator: The separator of the assets.
-    :param included: The symbols to include.
-    :param bases: The bases of the asset pairs.
-
-    :return: The data of the exchanges.
-    """
+    symbols = (
+        symbols if all(value is None for value in (included, bases, quotes)) else
+        include_symbols(
+            symbols=symbols, included=included,
+            bases=bases, quotes=quotes, separator=separator
+        )
+    )
 
-    return exchanges_data(
-        collector=exchange_assets,
-        exchanges=exchanges, quotes=quotes, excluded=excluded,
-        adjust=adjust, separator=separator, bases=bases, included=included
+    return symbols if excluded is None else exclude_symbols(
+        symbols=symbols, excluded=excluded, separator=separator, adjust=adjust
     )
-# end exchanges_assets
+# end exchange_symbols
 
-def exchanges_base_assets(
+def exchanges_symbols(
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
 ) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
-    :param bases: The bases of the asset pairs.
     :param excluded: The excluded symbols.
     :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
     :param included: The symbols to include.
     :param bases: The bases of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
     return exchanges_data(
-        collector=exchange_base_assets,
+        collector=exchange_symbols,
         exchanges=exchanges, quotes=quotes, excluded=excluded,
-        adjust=adjust, separator=separator, bases=bases, included=included
+        adjust=adjust, separator=separator, included=included, bases=bases
     )
-# end exchanges_assets
+# end exchanges_symbols
 
-def exchanges_quote_assets(
+def mutual_exchanges_symbols(
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        data: Optional[Dict[str, Iterable[str]]] = None
 ) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
-    :param bases: The bases of the asset pairs.
     :param excluded: The excluded symbols.
     :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
+    :param data: The data to search in.
     :param included: The symbols to include.
     :param bases: The bases of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
-    return exchanges_data(
-        collector=exchange_quote_assets,
-        exchanges=exchanges, quotes=quotes, excluded=excluded,
-        adjust=adjust, separator=separator, bases=bases, included=included
+    return mutual_string_values(
+        data=data or exchanges_symbols(
+            exchanges=exchanges, quotes=quotes, excluded=excluded,
+            adjust=adjust, separator=separator, included=included, bases=bases
+        )
     )
-# end exchanges_quote_assets
+# end mutual_exchanges_symbols
 
-def exchanges_symbols_assets(
-        data: Dict[str, Iterable[str]],
+AssetMatches = Iterable[Iterable[str]]
+
+def matching_symbol_pair(
+        symbol1: str,
+        symbol2: str, /, *,
+        matches: Optional[AssetMatches] = None,
         separator: Optional[str] = None
-) -> Dict[str, Set[str]]:
+) -> bool:
     """
-    Finds the currencies from the screeners.
+    Checks if the symbols are valid with the matching currencies.
 
-    :param data: The data to process.
+    :param symbol1: The first ticker.
+    :param symbol2: The second ticker.
+    :param matches: The currencies.
     :param separator: The separator of the assets.
 
-    :return: The currencies from the screeners.
+    :return: The validation value for the symbols.
     """
 
-    result = {}
-
-    for exchange, symbols in data.items():
-        result.setdefault(exchange, []).extend(symbols)
-    # end for
+    symbol1 = adjust_symbol(symbol=symbol1, separator=separator)
+    symbol2 = adjust_symbol(symbol=symbol2, separator=separator)
 
-    results = {}
+    if symbol1 == symbol2:
+        return True
+    # end if
 
-    for exchange, symbols in result.items():
-        assets = []
+    asset1, currency1 = symbol_to_parts(symbol=symbol1, separator=separator)
+    asset2, currency2 = symbol_to_parts(symbol=symbol2, separator=separator)
 
-        for symbol in set(symbols):
-            base, quote = symbol_to_parts(symbol=symbol, separator=separator)
+    if asset1 != asset2:
+        return False
+    # end if
 
-            if base not in assets:
-                assets.append(base)
-            # end if
+    matches = matches or []
 
-            if quote not in assets:
-                assets.append(quote)
-            # end if
-        # end for
+    for matches in matches:
+        if (currency1 in matches) and (currency2 in matches):
+            return True
+        # end if
 
-        results.setdefault(exchange, assets)
+        if (
+            ((currency1 in matches) and (currency2 not in matches)) or
+            ((currency1 not in matches) and (currency2 in matches))
+        ):
+            return False
+        # end if
     # end for
 
-    return results
-# end exchanges_symbols_assets
+    return False
+# end matching_symbol_pair
+
+ExchangeSymbolPairs = Set[Tuple[Tuple[str, str], Tuple[str, str]]]
+ExchangesAssetMatches = Union[Dict[Iterable[str], AssetMatches], AssetMatches]
 
-def exchanges_symbols_base_assets(
+def matching_symbol_pairs(
         data: Dict[str, Iterable[str]],
+        matches: Optional[ExchangesAssetMatches] = None,
         separator: Optional[str] = None
-) -> Dict[str, Set[str]]:
+) -> ExchangeSymbolPairs:
     """
-    Finds the currencies from the screeners.
+    Checks if the symbols are valid with the matching currencies.
 
-    :param data: The data to process.
+    :param data: The symbols.
+    :param matches: The currencies.
     :param separator: The separator of the assets.
 
-    :return: The currencies from the screeners.
+    :return: The validation value for the symbols.
     """
 
-    result = {}
+    pairs = []
+    exchange_symbol_pairs = []
 
     for exchange, symbols in data.items():
-        result.setdefault(exchange, []).extend(symbols)
+        exchange_symbol_pairs.extend([(exchange, symbol) for symbol in symbols])
     # end for
 
-    return {
-        exchange: list(
-            set(
-                symbol_to_pair(symbol=symbol, separator=separator).base
-                for symbol in set(symbols)
+    for exchange1, symbol1 in exchange_symbol_pairs:
+        for exchange2, symbol2 in exchange_symbol_pairs:
+            exchanges_matches = (
+                matches if not isinstance(matches, dict) else
+                [*matches.get(exchange1, []), *matches.get(exchange2, [])]
             )
-        )
-
-        for exchange, symbols in result.items()
-    }
-# end exchanges_symbols_base_assets
 
-def exchanges_symbols_quote_assets(
-        data: Dict[str, Iterable[str]],
-        separator: Optional[str] = None
-) -> Dict[str, Set[str]]:
-    """
-    Finds the currencies from the screeners.
-
-    :param data: The data to process.
-    :param separator: The separator of the assets.
-
-    :return: The currencies from the screeners.
-    """
-
-    result = {}
-
-    for exchange, symbols in data.items():
-        result.setdefault(exchange, []).extend(symbols)
+            if (
+                (exchange1 != exchange2) and
+                matching_symbol_pair(
+                    symbol1, symbol2,
+                    matches=exchanges_matches or None,
+                    separator=separator
+                )
+            ):
+                pairs.append(
+                    ((exchange1, symbol1), (exchange2, symbol2))
+                )
+            # end if
+        # end for
     # end for
 
-    return {
-        exchange: list(
-            set(
-                symbol_to_pair(symbol=symbol, separator=separator).quote
-                for symbol in set(symbols)
-            )
-        )
-        for exchange, symbols in result.items()
-    }
-# end exchanges_symbols_quote_assets
+    return set(pairs)
+# end matching_symbol_pairs
 
-def mutual_exchanges_assets(
-        exchanges: Optional[Iterable[str]] = None,
-        adjust: Optional[bool] = True,
-        separator: Optional[str] = None,
-        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        data: Optional[Dict[str, Iterable[str]]] = None
-) -> Dict[str, Set[str]]:
+@define(repr=False, unsafe_hash=True)
+@represent
+class MarketSymbolSignature:
+    """A class to represent the data for the execution of a trade."""
+
+    asset: str
+    currency: str
+    exchange: str
+# end MarketPairSignature
+
+def matching_symbol_signatures(
+        pairs: Optional[ExchangeSymbolPairs] = None,
+        data: Optional[Dict[str, Iterable[str]]] = None,
+        matches: Optional[ExchangesAssetMatches] = None,
+        separator: Optional[str] = None
+) -> Set[Tuple[MarketSymbolSignature, MarketSymbolSignature]]:
     """
-    Collects the symbols from the exchanges.
+    Checks if the screeners are valid with the matching currencies.
 
-    :param exchanges: The exchanges.
-    :param quotes: The quotes of the asset pairs.
-    :param bases: The bases of the asset pairs.
-    :param excluded: The excluded symbols.
-    :param adjust: The value to adjust the invalid exchanges.
+    :param data: The data for the pairs.
+    :param pairs: The pairs' data.
+    :param matches: The currencies.
     :param separator: The separator of the assets.
-    :param data: The data to search in.
-    :param included: The symbols to include.
 
-    :return: The data of the exchanges.
+    :return: The validation value for the symbols.
     """
 
-    return mutual_string_values(
-        data=data or exchanges_assets(
-            exchanges=exchanges, quotes=quotes, bases=bases, included=included,
-            excluded=excluded, adjust=adjust, separator=separator
+    if (data is None) and (pairs is None):
+        raise ValueError(
+            f"One of 'pairs' and 'data' parameters must be given, "
+            f"when 'pairs' is superior to 'data'."
         )
-    )
-# end mutual_exchanges_assets
-
-def mutual_exchanges_base_assets(
-        exchanges: Optional[Iterable[str]] = None,
-        adjust: Optional[bool] = True,
-        separator: Optional[str] = None,
-        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        data: Optional[Dict[str, Iterable[str]]] = None
-) -> Dict[str, Set[str]]:
-    """
-    Collects the symbols from the exchanges.
-
-    :param exchanges: The exchanges.
-    :param quotes: The quotes of the asset pairs.
-    :param bases: The bases of the asset pairs.
-    :param excluded: The excluded symbols.
-    :param adjust: The value to adjust the invalid exchanges.
-    :param separator: The separator of the assets.
-    :param data: The data to search in.
-    :param included: The symbols to include.
-
-    :return: The data of the exchanges.
-    """
 
-    return mutual_string_values(
-        data=data or exchanges_base_assets(
-            exchanges=exchanges, quotes=quotes, bases=bases, included=included,
-            excluded=excluded, adjust=adjust, separator=separator
+    elif (not pairs) and (not data):
+        return set()
+    # end if
+
+    new_pairs = []
+
+    pairs = pairs or matching_symbol_pairs(
+        data=data, matches=matches, separator=separator
+    )
+
+    for (exchange1, symbol1), (exchange2, symbol2) in pairs:
+        asset1, currency1 = symbol_to_parts(adjust_symbol(symbol1))
+        asset2, currency2 = symbol_to_parts(adjust_symbol(symbol2))
+
+        new_pairs.append(
+            (
+                MarketSymbolSignature(
+                    asset=asset1, currency=currency1,
+                    exchange=exchange1
+                ),
+                MarketSymbolSignature(
+                    asset=asset2, currency=currency2,
+                    exchange=exchange2
+                )
+            )
         )
-    )
-# end mutual_exchanges_base_assets
-
-def mutual_exchanges_quote_assets(
-        exchanges: Optional[Iterable[str]] = None,
-        adjust: Optional[bool] = True,
-        separator: Optional[str] = None,
-        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        data: Optional[Dict[str, Iterable[str]]] = None
-) -> Dict[str, Set[str]]:
-    """
-    Collects the symbols from the exchanges.
-
-    :param exchanges: The exchanges.
-    :param quotes: The quotes of the asset pairs.
-    :param bases: The bases of the asset pairs.
-    :param excluded: The excluded symbols.
-    :param adjust: The value to adjust the invalid exchanges.
-    :param separator: The separator of the assets.
-    :param data: The data to search in.
-    :param included: The symbols to include.
-
-    :return: The data of the exchanges.
-    """
+    # end for
 
-    return mutual_string_values(
-        data=data or exchanges_quote_assets(
-            exchanges=exchanges, quotes=quotes, bases=bases, included=included,
-            excluded=excluded, adjust=adjust, separator=separator
-        )
-    )
-# end mutual_exchanges_quote_assets
+    return set(new_pairs)
+# end matching_symbol_signatures
```

### Comparing `crypto-screening-8.2.1/crypto_screening/collect/exchanges.py` & `crypto-screening-8.2.2/crypto_screening/collect/exchanges.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # exchanges.py
 
 from typing import (
     Optional, Dict, Iterable,
-    Callable, Union, TypeVar
+    Callable, Union, TypeVar, Any
 )
 
 from multithreading import Caller, multi_threaded_call
 
 from crypto_screening.exchanges import EXCHANGE_NAMES
 from crypto_screening.validate import validate_exchange
 from crypto_screening.utils.process import (
-    find_string_value, lower_string_values
+    find_string_value, lower_string_values, string_in_values
 )
 
 __all__ = [
     "exchanges_data",
     "exchanges_values"
 ]
 
@@ -59,14 +59,35 @@
     ):
         values = {exchange: values_data for exchange in exchanges}
     # end if
 
     return values
 # end exchanges_values
 
+def exchange_value(
+        exchange: str,
+        values: Union[Any, Dict[str, Any]],
+        default: Optional[Any] = None
+) -> Any:
+    """
+    Finds the value of the exchange or returns the default.
+
+    :param exchange: The exchange name.
+    :param values: The values of the exchanges.
+    :param default: The default value.
+
+    :return: The value of the exchange.
+    """
+
+    return (
+        (values[exchange] if exchange in values else default)
+        if isinstance(values, dict) else values
+    )
+# end exchange_value
+
 def exchanges_data(
         collector: Collector,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         exchanges: Optional[Iterable[str]] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
@@ -95,17 +116,15 @@
     quotes = exchanges_values(exchanges=exchanges, values=quotes)
     included = exchanges_values(exchanges=exchanges, values=included)
     excluded = exchanges_values(exchanges=exchanges, values=excluded)
 
     markets = []
 
     for exchange in exchanges:
-        exchange = find_string_value(value=exchange, values=EXCHANGE_NAMES)
-
-        if exchange not in EXCHANGE_NAMES:
+        if string_in_values(value=exchange, values=EXCHANGE_NAMES):
             if adjust:
                 continue
 
             else:
                 validate_exchange(exchange=exchange, exchanges=EXCHANGE_NAMES)
             # end if
         # end if
@@ -113,37 +132,27 @@
         markets.append(exchange)
     # end for
 
     callers = []
     data: Dict[str, Caller] = {}
 
     for exchange in markets:
+        saved_exchange = exchange
+
         exchange = find_string_value(value=exchange, values=exchanges)
 
-        exchange_bases = (
-            (bases[exchange] if exchange in bases else None)
-            if isinstance(bases, dict) else bases
-        )
-        exchange_quotes = (
-            (quotes[exchange] if exchange in quotes else None)
-            if isinstance(quotes, dict) else quotes
-        )
-        exchange_included = (
-            (included[exchange] if exchange in included else None)
-            if isinstance(included, dict) else included
-        )
-        exchange_excluded = (
-            (excluded[exchange] if exchange in excluded else None)
-            if isinstance(excluded, dict) else excluded
-        )
+        exchange_bases = exchange_value(exchange=exchange, values=bases)
+        exchange_quotes = exchange_value(exchange=exchange, values=quotes)
+        exchange_included = exchange_value(exchange=exchange, values=included)
+        exchange_excluded = exchange_value(exchange=exchange, values=excluded)
 
         caller = Caller(
             target=collector,
             kwargs=dict(
-                exchange=exchange,
+                exchange=saved_exchange,
                 separator=separator,
                 adjust=adjust,
                 quotes=exchange_quotes,
                 bases=exchange_bases,
                 included=exchange_included,
                 excluded=exchange_excluded
             )
```

### Comparing `crypto-screening-8.2.1/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.2.2/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.2.2/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/collect/market/orders.py` & `crypto-screening-8.2.2/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.2.2/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.2.2/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.2.2/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/collect/market/trades.py` & `crypto-screening-8.2.2/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/collect/screeners.py` & `crypto-screening-8.2.2/crypto_screening/collect/screeners.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Set, Union, Tuple, List
 )
 
 import pandas as pd
 from attrs import define
 
 from crypto_screening.symbols import symbol_to_pair, symbol_to_parts, adjust_symbol
+from crypto_screening.utils.process import string_in_values
 from crypto_screening.collect.symbols import (
     matching_symbol_pair, MarketSymbolSignature, exchanges_symbols
 )
 from crypto_screening.screeners import BaseScreener, BaseMarketScreener
 
 __all__ = [
     "matching_screener_signatures",
@@ -231,71 +232,71 @@
             )
         )
     }
 # end live_nonempty_screeners
 
 def structure_screeners(
         screeners: Iterable[BaseScreener]
-) -> Dict[str, Dict[str, List[BaseScreener]]]:
+) -> Dict[str, Dict[str, Set[BaseScreener]]]:
     """
     Structures the screener objects by exchanges and symbols
 
     :param screeners: The screeners to structure.
 
     :return: The structure of the screeners.
     """
 
-    structure: Dict[str, Dict[str, List[BaseScreener]]] = {}
+    structure: Dict[str, Dict[str, Set[BaseScreener]]] = {}
 
     for screener in screeners:
         (
             structure.
             setdefault(screener.exchange, {}).
-            setdefault(screener.symbol, [])
-        ).append(screener)
+            setdefault(screener.symbol, set())
+        ).add(screener)
     # end for
 
     return structure
 # end structure_screeners
 
 def find_screeners(
         screeners: Iterable[BaseScreener],
         exchange: Optional[str] = None,
         symbol: Optional[str] = None
-) -> List[BaseScreener]:
+) -> Set[BaseScreener]:
     """
     Finds all the screeners with the matching exchange and symbol key.
 
     :param screeners: The screeners to process.
     :param exchange: The exchange key for the symbol.
     :param symbol: The pair symbol to search its screeners.
 
     :return: The matching screeners.
     """
 
-    return [
+    return {
         screener for screener in screeners
         if (
             ((symbol is None) or (screener.symbol.lower() == symbol.lower())) and
             ((exchange is None) or (exchange.lower() == screener.exchange.lower()))
         )
-    ]
+    }
 # end find_screeners
 
-def remove_empty_screeners(screeners: Iterable[BaseScreener]) -> List[BaseScreener]:
+def remove_empty_screeners(screeners: Iterable[BaseScreener]) -> Set[BaseScreener]:
     """
     Removes the empty screeners.
 
     :param screeners: The screeners of the assets and exchanges.
     """
 
-    return [
+    return {
         screener for screener in screeners
         if len(screener.market) > 0
-    ]
+    }
 # end remove_empty_screeners
 
 def screeners_exchanges_symbols(screeners: Iterable[BaseScreener]) -> Dict[str, Set[str]]:
     """
     Collects the structure of the screeners exchanges and symbols.
 
     :param screeners: The screeners to process.
@@ -314,31 +315,31 @@
         for exchange, symbols in data.items()
         if symbols
     }
 # end screeners_exchanges_symbols
 
 def structure_exchanges_symbols_screeners(
         screeners: Iterable[BaseScreener]
-) -> Dict[str, Dict[str, List[BaseScreener]]]:
+) -> Dict[str, Dict[str, Set[BaseScreener]]]:
     """
     Structures the screener objects by exchanges and symbols
 
     :param screeners: The screeners to structure.
 
     :return: The structure of the screeners.
     """
 
-    structure: Dict[str, Dict[str, List[BaseScreener]]] = {}
+    structure: Dict[str, Dict[str, Set[BaseScreener]]] = {}
 
     for screener in screeners:
         (
             structure.
             setdefault(screener.exchange, {}).
-            setdefault(screener.symbol, [])
-        ).append(screener)
+            setdefault(screener.symbol, set())
+        ).add(screener)
     # end for
 
     return structure
 # end structure_exchanges_symbols_screeners
 
 def structure_exchanges_symbols_screener(
         screeners: Iterable[BaseScreener]
@@ -362,31 +363,31 @@
     # end for
 
     return structure
 # end structure_exchanges_symbols_screener
 
 def gather_screeners(
         screeners: Iterable[Union[BaseScreener, BaseMarketScreener]]
-) -> List[BaseScreener]:
+) -> Set[BaseScreener]:
     """
     Gathers the base screeners.
 
     :param screeners: The screeners to process.
 
     :return: The gathered base screeners.
     """
 
-    checked_screeners: List[BaseScreener] = []
+    checked_screeners: Set[BaseScreener] = set()
 
     for screener in screeners:
         if isinstance(screener, BaseScreener):
-            checked_screeners.append(screener)
+            checked_screeners.add(screener)
 
         elif isinstance(screener, BaseMarketScreener):
-            checked_screeners.extend(screener.screeners)
+            checked_screeners.update(screener.screeners)
         # end if
     # end for
 
     return checked_screeners
 # end gather_screeners
 
 def exchanges_symbols_screeners(
@@ -394,15 +395,15 @@
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
-) -> List[BaseScreener]:
+) -> Set[BaseScreener]:
     """
     Collects the symbols from the exchanges.
 
     :param screeners: The screeners to collect.
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
     :param excluded: The excluded symbols.
@@ -415,29 +416,35 @@
     """
 
     if exchanges is None:
         exchanges = {screener.exchange for screener in screeners}
     # end if
 
     if (not screeners) or (not exchanges):
-        return[]
+        return set()
     # end if
 
     found_exchanges_symbols = exchanges_symbols(
         exchanges=set(exchanges), adjust=adjust, separator=separator,
         bases=bases, quotes=quotes, included=included, excluded=excluded
     )
 
-    return [
+    return {
         screener for screener in screeners
         if (
-            (screener.exchange in found_exchanges_symbols) and
-            (screener.symbol in found_exchanges_symbols[screener.exchange])
+            string_in_values(
+                value=screener.exchange, values=found_exchanges_symbols
+            )
+            and
+            string_in_values(
+                value=screener.symbol,
+                values=found_exchanges_symbols[screener.exchange]
+            )
         )
-    ]
+    }
 # end exchanges_symbols_screeners
 
 def screeners_to_multiple_symbols_screeners(
         screeners: Iterable[BaseScreener]
 ) -> Dict[str, Dict[str, List[BaseScreener]]]:
     """
     Converts the datasets structure to the structure of the data rows.
```

### Comparing `crypto-screening-8.2.1/crypto_screening/collect/symbols.py` & `crypto-screening-8.2.2/crypto_screening/collect/assets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,645 +1,518 @@
-# symbols.py
+# assets.py
 
-import warnings
-from typing import (
-    Optional, Dict, Iterable,
-    Set, Union, Tuple
-)
-
-from attrs import define
-
-from represent import represent
+from typing import Optional, Dict, Iterable, Set, Union
 
-from multithreading import Caller, multi_threaded_call
-
-from crypto_screening.utils.process import (
-    find_string_value, upper_string_values,
-    mutual_string_values
-)
-from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
-from crypto_screening.symbols import (
-    symbol_to_parts, adjust_symbol, Separator
-)
-from crypto_screening.validate import validate_exchange
+from crypto_screening.utils.process import mutual_string_values
+from crypto_screening.symbols import symbol_to_parts, symbol_to_pair
 from crypto_screening.collect.exchanges import exchanges_data
+from crypto_screening.collect.symbols import (
+    all_exchange_symbols, exchange_symbols
+)
 
 __all__ = [
-    "exchanges_symbols",
-    "mutual_exchanges_symbols",
-    "include_symbols",
-    "exclude_symbols",
-    "exchange_symbols",
-    "all_exchange_symbols",
-    "matching_symbol_pair",
-    "matching_symbol_pairs",
-    "MarketSymbolSignature",
-    "matching_symbol_signatures",
-    "include_exchanges_symbols",
-    "exclude_exchanges_symbols",
-    "all_exchanges_symbols"
+    "exchanges_assets",
+    "mutual_exchanges_assets",
+    "exchange_assets",
+    "exchange_quote_assets",
+    "exchange_base_assets",
+    "all_exchange_assets",
+    "all_exchange_base_assets",
+    "all_exchange_quote_assets",
+    "exchanges_base_assets",
+    "exchanges_quote_assets",
+    "mutual_exchanges_base_assets",
+    "mutual_exchanges_quote_assets",
+    "exchanges_symbols_assets",
+    "exchanges_symbols_quote_assets",
+    "exchanges_symbols_base_assets"
 ]
 
-def include_symbols(
-        symbols: Iterable[str],
+def all_exchange_assets(
+        exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
-        bases: Optional[Iterable[str]] = None,
-        quotes: Optional[Iterable[str]] = None,
-        included: Optional[Iterable[str]] = None
 ) -> Set[str]:
     """
-    Removes all symbols with not matching base or quote.
+    Collects the symbols from the exchanges.
 
-    :param symbols: The symbols to filter.
-    :param separator: The separator for the symbols.
-    :param bases: The bases to include.
+    :param exchange: The name of the exchange.
     :param adjust: The value to adjust the invalid exchanges.
-    :param quotes: The quotes to include.
-    :param included: The symbols to include.
+    :param separator: The separator of the assets.
 
-    :return: The filtered symbols.
+    :return: The data of the exchanges.
     """
 
-    saved = []
+    symbols = all_exchange_symbols(
+        exchange=exchange, adjust=adjust, separator=separator
+    )
 
-    quotes = upper_string_values(quotes or [])
-    bases = upper_string_values(bases or [])
-    included = upper_string_values(included or [])
+    assets = set()
 
     for symbol in symbols:
-        if symbol in included:
-            saved.append(symbol)
+        assets.update(symbol_to_parts(symbol=symbol, separator=separator))
+    # end for
 
-            continue
-        # end if
+    return assets
+# end all_exchange_assets
 
-        try:
-            symbol = adjust_symbol(symbol=symbol, separator=separator)
+def all_exchange_base_assets(
+        exchange: str,
+        separator: Optional[str] = None,
+        adjust: Optional[bool] = True,
+) -> Set[str]:
+    """
+    Collects the symbols from the exchanges.
 
-        except ValueError as e:
-            if adjust:
-                continue
+    :param exchange: The name of the exchange.
+    :param adjust: The value to adjust the invalid exchanges.
+    :param separator: The separator of the assets.
 
-            else:
-                raise e
-            # end if
-        # end try
+    :return: The data of the exchanges.
+    """
 
-        if symbol in included:
-            saved.append(symbol)
+    symbols = all_exchange_symbols(
+        exchange=exchange, adjust=adjust, separator=separator
+    )
 
-            continue
-        # end if
+    assets = set()
 
-        base, quote = symbol_to_parts(
-            symbol=symbol, separator=separator
-        )
+    for symbol in symbols:
+        base, _ = symbol_to_parts(symbol=symbol, separator=separator)
 
-        if (
-            (find_string_value(value=base, values=bases) in bases) or
-            (find_string_value(value=quote, values=quotes) in quotes)
-        ):
-            saved.append(symbol)
-        # end if
+        assets.add(base)
     # end for
 
-    return set(saved)
-# end include_symbols
+    return assets
+# end all_exchange_base_assets
 
-def exclude_symbols(
-        symbols: Iterable[str],
+def all_exchange_quote_assets(
+        exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
-        bases: Optional[Iterable[str]] = None,
-        quotes: Optional[Iterable[str]] = None,
-        excluded: Optional[Iterable[str]] = None
 ) -> Set[str]:
     """
-    Removes all symbols with the matching base or quote.
+    Collects the symbols from the exchanges.
 
-    :param symbols: The symbols to filter.
-    :param separator: The separator for the symbols.
-    :param bases: The bases to exclude.
-    :param quotes: The quotes to exclude.
+    :param exchange: The name of the exchange.
     :param adjust: The value to adjust the invalid exchanges.
-    :param excluded: The symbols to exclude.
+    :param separator: The separator of the assets.
 
-    :return: The filtered symbols.
+    :return: The data of the exchanges.
     """
 
-    saved = []
+    symbols = all_exchange_symbols(
+        exchange=exchange, adjust=adjust, separator=separator
+    )
 
-    quotes = upper_string_values(quotes or [])
-    bases = upper_string_values(bases or [])
-    excluded = upper_string_values(excluded or [])
+    assets = set()
 
     for symbol in symbols:
-        if symbol in excluded:
-            continue
-        # end if
-
-        try:
-            symbol = adjust_symbol(symbol=symbol, separator=separator)
-
-        except ValueError as e:
-            if adjust:
-                continue
-
-            else:
-                raise e
-            # end if
-        # end try
-
-        if symbol in excluded:
-            continue
-        # end if
-
-        base, quote = symbol_to_parts(symbol=symbol, separator=separator)
-
-        if (
-            (find_string_value(value=base, values=bases) in bases) or
-            (find_string_value(value=quote, values=quotes) in quotes)
-        ):
-            continue
-        # end if
+        _, quote = symbol_to_parts(symbol=symbol, separator=separator)
 
-        saved.append(symbol)
+        assets.add(quote)
     # end for
 
-    return set(saved)
-# end exclude_symbols
+    return assets
+# end all_exchange_quote_assets
 
-def include_exchanges_symbols(
-        data: Dict[str, Iterable[str]],
-        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
-) -> Dict[str, Set[str]]:
+def exchange_assets(
+        exchange: str,
+        separator: Optional[str] = None,
+        adjust: Optional[bool] = True,
+        bases: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None,
+        included: Optional[Iterable[str]] = None,
+        excluded: Optional[Iterable[str]] = None
+) -> Set[str]:
     """
-    Removes all symbols with not matching base or quote.
+    Collects the assets from the exchanges.
 
-    :param data: The data to filter.
-    :param bases: The bases to include.
-    :param quotes: The quotes to include.
+    :param exchange: The name of the exchange.
+    :param bases: The bases of the asset pairs.
+    :param quotes: The quotes of the asset pairs.
+    :param adjust: The value to adjust the invalid exchanges.
+    :param separator: The separator for the symbols.
     :param included: The symbols to include.
+    :param excluded: The excluded symbols.
 
-    :return: The filtered symbols.
+    :return: The data of the exchanges.
     """
 
-    if all(value is None for value in (bases, quotes, included)):
-        return {exchange: set(symbols) for exchange, symbols in data.items()}
-    # end if
-
-    if not isinstance(quotes, dict):
-        saved_quotes = quotes
-        quotes = {exchange: saved_quotes for exchange in data}
-    # end if
-
-    if not isinstance(bases, dict):
-        saved_bases = bases
-        bases = {exchange: saved_bases for exchange in data}
-    # end if
-
-    if not isinstance(included, dict):
-        saved_included = included
-        included = {exchange: saved_included for exchange in data}
-    # end if
-
-    return {
-        exchange: saved for exchange, symbols in data.items()
-        if (
-            saved := include_symbols(
-                symbols=symbols,
-                bases=bases.get(exchange, None),
-                quotes=quotes.get(exchange, None),
-                included=included.get(exchange, None)
-            )
-        )
-    }
-# end include_exchanges_symbols
+    symbols = exchange_symbols(
+        exchange=exchange, separator=separator, bases=bases,
+        quotes=quotes, excluded=excluded, adjust=adjust, included=included
+    )
 
-def exclude_exchanges_symbols(
-        data: Dict[str, Iterable[str]],
-        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
-) -> Dict[str, Set[str]]:
-    """
-    Removes all symbols with the matching base or quote.
+    assets = set()
 
-    :param data: The data to filter.
-    :param bases: The bases to exclude.
-    :param quotes: The quotes to exclude.
-    :param excluded: The symbols to exclude.
-
-    :return: The filtered symbols.
-    """
-
-    if all(value is None for value in (bases, quotes, excluded)):
-        return {exchange: set(symbols) for exchange, symbols in data.items()}
-    # end if
-
-    if not isinstance(quotes, dict):
-        saved_quotes = quotes
-        quotes = {exchange: saved_quotes for exchange in data}
-    # end if
-
-    if not isinstance(bases, dict):
-        saved_bases = bases
-        bases = {exchange: saved_bases for exchange in data}
-    # end if
-
-    if not isinstance(excluded, dict):
-        saved_excluded = excluded
-        excluded = {exchange: saved_excluded for exchange in data}
-    # end if
+    for symbol in symbols:
+        assets.update(symbol_to_parts(symbol=symbol, separator=separator))
+    # end for
 
-    return {
-        exchange: saved for exchange, symbols in data.items()
-        if (
-            saved := exclude_symbols(
-                symbols=symbols,
-                bases=bases.get(exchange, None),
-                quotes=quotes.get(exchange, None),
-                excluded=excluded.get(exchange, None)
-            )
-        )
-    }
-# end exclude_exchanges_symbols
+    return assets
+# end exchange_assets
 
-def all_exchange_symbols(
+def exchange_base_assets(
         exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
-        test: Optional[bool] = False
+        bases: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None,
+        included: Optional[Iterable[str]] = None,
+        excluded: Optional[Iterable[str]] = None
 ) -> Set[str]:
     """
-    Collects the symbols from the exchanges.
+    Collects the assets from the exchanges.
 
     :param exchange: The name of the exchange.
+    :param bases: The bases of the asset pairs.
     :param adjust: The value to adjust the invalid exchanges.
-    :param separator: The separator of the assets.
-    :param test: Include test assets.
+    :param quotes: The quotes of the asset pairs.
+    :param separator: The separator for the symbols.
+    :param included: The symbols to include.
+    :param excluded: The excluded symbols.
 
     :return: The data of the exchanges.
     """
 
-    validate_exchange(exchange=exchange, exchanges=EXCHANGE_NAMES)
-
-    try:
-        found_symbols: Iterable[str] = EXCHANGES[exchange].symbols()
-
-    except Exception as e:
-        error_message = (
-            f"Cannot fetch symbols of '{exchange}' exchange: {str(e)}."
-        )
-
-        if not adjust:
-            raise RuntimeError(error_message)
-
-        else:
-            warnings.warn(error_message)
-
-            return set()
-        # end if
-    # end try
-
-    symbols = []
-
-    if separator is None:
-        separator = Separator.value
-    # end if
-
-    for symbol in found_symbols:
-        try:
-            symbol = adjust_symbol(symbol=symbol, separator=separator)
-
-            if symbol.count(separator) != 1:
-                raise ValueError(
-                    f"Invalid symbol structure: {symbol}. "
-                    f"Symbol must contain only one separator."
-                )
-            # end if
-
-        except ValueError as e:
-            if adjust:
-                continue
-
-            else:
-                raise e
-            # end if
-        # end try
+    symbols = exchange_symbols(
+        exchange=exchange, separator=separator, bases=bases,
+        quotes=quotes, excluded=excluded, adjust=adjust, included=included
+    )
 
-        base, quote = symbol_to_parts(symbol=symbol, separator=separator)
+    assets = set()
 
-        if (not test) and base.startswith("TEST") and quote.startswith("TEST"):
-            continue
-        # end if
+    for symbol in symbols:
+        base, _ = symbol_to_parts(symbol=symbol, separator=separator)
 
-        symbols.append(symbol)
+        assets.add(base)
     # end for
 
-    return set(symbols)
-# end all_exchange_symbols
+    return assets
+# end exchange_assets
 
-def all_exchanges_symbols(
-        exchanges: Iterable[str],
+def exchange_quote_assets(
+        exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
-        test: Optional[bool] = False
-) -> Dict[str, Set[str]]:
+        bases: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None,
+        included: Optional[Iterable[str]] = None,
+        excluded: Optional[Iterable[str]] = None
+) -> Set[str]:
     """
-    Collects the symbols from the exchanges.
+    Collects the assets from the exchanges.
 
-    :param exchanges: The name of the exchange.
+    :param exchange: The name of the exchange.
+    :param bases: The bases of the asset pairs.
     :param adjust: The value to adjust the invalid exchanges.
-    :param separator: The separator of the assets.
-    :param test: Include test assets.
+    :param quotes: The quotes of the asset pairs.
+    :param separator: The separator for the symbols.
+    :param included: The symbols to include.
+    :param excluded: The excluded symbols.
 
     :return: The data of the exchanges.
     """
 
-    results = multi_threaded_call(
-        [
-            Caller(
-                target=all_exchange_symbols, kwargs=dict(
-                    exchange=exchange, separator=separator,
-                    adjust=adjust, test=test
-                ), identifier=exchange
-            ) for exchange in exchanges
-        ]
+    symbols = exchange_symbols(
+        exchange=exchange, separator=separator, bases=bases,
+        quotes=quotes, excluded=excluded, adjust=adjust, included=included
     )
 
-    return {
-        exchange: results.results(exchange).returns
-        for exchange in exchanges
-    }
-# end all_exchanges_symbols
+    assets = set()
 
-def exchange_symbols(
-        exchange: Optional[str] = None,
-        separator: Optional[str] = None,
+    for symbol in symbols:
+        _, quote = symbol_to_parts(symbol=symbol, separator=separator)
+
+        assets.add(quote)
+    # end for
+
+    return assets
+# end exchange_assets
+
+def exchanges_assets(
+        exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
-        bases: Optional[Iterable[str]] = None,
-        quotes: Optional[Iterable[str]] = None,
-        included: Optional[Iterable[str]] = None,
-        excluded: Optional[Iterable[str]] = None
-) -> Set[str]:
+        separator: Optional[str] = None,
+        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
-    :param exchange: The name of the exchange.
+    :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
-    :param adjust: The value to adjust the invalid exchanges.
     :param bases: The bases of the asset pairs.
+    :param excluded: The excluded symbols.
+    :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
     :param included: The symbols to include.
-    :param excluded: The excluded symbols.
+    :param bases: The bases of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
-    symbols = all_exchange_symbols(
-        exchange=exchange, adjust=adjust, separator=separator
-    )
-
-    symbols = (
-        symbols if all(value is None for value in (included, bases, quotes)) else
-        include_symbols(
-            symbols=symbols, included=included,
-            bases=bases, quotes=quotes, separator=separator
-        )
-    )
-
-    return symbols if excluded is None else exclude_symbols(
-        symbols=symbols, excluded=excluded, separator=separator, adjust=adjust
+    return exchanges_data(
+        collector=exchange_assets,
+        exchanges=exchanges, quotes=quotes, excluded=excluded,
+        adjust=adjust, separator=separator, bases=bases, included=included
     )
-# end exchange_symbols
+# end exchanges_assets
 
-def exchanges_symbols(
+def exchanges_base_assets(
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
 ) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
+    :param bases: The bases of the asset pairs.
     :param excluded: The excluded symbols.
     :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
     :param included: The symbols to include.
     :param bases: The bases of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
     return exchanges_data(
-        collector=exchange_symbols,
+        collector=exchange_base_assets,
         exchanges=exchanges, quotes=quotes, excluded=excluded,
-        adjust=adjust, separator=separator, included=included, bases=bases
+        adjust=adjust, separator=separator, bases=bases, included=included
     )
-# end exchanges_symbols
+# end exchanges_assets
 
-def mutual_exchanges_symbols(
+def exchanges_quote_assets(
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        data: Optional[Dict[str, Iterable[str]]] = None
+        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
 ) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
+    :param bases: The bases of the asset pairs.
     :param excluded: The excluded symbols.
     :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
-    :param data: The data to search in.
     :param included: The symbols to include.
     :param bases: The bases of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
-    return mutual_string_values(
-        data=data or exchanges_symbols(
-            exchanges=exchanges, quotes=quotes, excluded=excluded,
-            adjust=adjust, separator=separator, included=included, bases=bases
-        )
+    return exchanges_data(
+        collector=exchange_quote_assets,
+        exchanges=exchanges, quotes=quotes, excluded=excluded,
+        adjust=adjust, separator=separator, bases=bases, included=included
     )
-# end mutual_exchanges_symbols
+# end exchanges_quote_assets
 
-AssetMatches = Iterable[Iterable[str]]
-
-def matching_symbol_pair(
-        symbol1: str,
-        symbol2: str, /, *,
-        matches: Optional[AssetMatches] = None,
+def exchanges_symbols_assets(
+        data: Dict[str, Iterable[str]],
         separator: Optional[str] = None
-) -> bool:
+) -> Dict[str, Set[str]]:
     """
-    Checks if the symbols are valid with the matching currencies.
+    Finds the currencies from the screeners.
 
-    :param symbol1: The first ticker.
-    :param symbol2: The second ticker.
-    :param matches: The currencies.
+    :param data: The data to process.
     :param separator: The separator of the assets.
 
-    :return: The validation value for the symbols.
+    :return: The currencies from the screeners.
     """
 
-    symbol1 = adjust_symbol(symbol=symbol1, separator=separator)
-    symbol2 = adjust_symbol(symbol=symbol2, separator=separator)
-
-    if symbol1 == symbol2:
-        return True
-    # end if
+    result = {}
 
-    asset1, currency1 = symbol_to_parts(symbol=symbol1, separator=separator)
-    asset2, currency2 = symbol_to_parts(symbol=symbol2, separator=separator)
+    for exchange, symbols in data.items():
+        result.setdefault(exchange, []).extend(symbols)
+    # end for
 
-    if asset1 != asset2:
-        return False
-    # end if
+    results = {}
 
-    matches = matches or []
+    for exchange, symbols in result.items():
+        assets = set()
 
-    for matches in matches:
-        if (currency1 in matches) and (currency2 in matches):
-            return True
-        # end if
+        for symbol in set(symbols):
+            assets.update(symbol_to_parts(symbol=symbol, separator=separator))
+        # end for
 
-        if (
-            ((currency1 in matches) and (currency2 not in matches)) or
-            ((currency1 not in matches) and (currency2 in matches))
-        ):
-            return False
-        # end if
+        results.setdefault(exchange, assets)
     # end for
 
-    return False
-# end matching_symbol_pair
+    return results
+# end exchanges_symbols_assets
 
-ExchangeSymbolPairs = Set[Tuple[Tuple[str, str], Tuple[str, str]]]
-ExchangesAssetMatches = Union[Dict[Iterable[str], AssetMatches], AssetMatches]
-
-def matching_symbol_pairs(
+def exchanges_symbols_base_assets(
         data: Dict[str, Iterable[str]],
-        matches: Optional[ExchangesAssetMatches] = None,
         separator: Optional[str] = None
-) -> ExchangeSymbolPairs:
+) -> Dict[str, Set[str]]:
     """
-    Checks if the symbols are valid with the matching currencies.
+    Finds the currencies from the screeners.
 
-    :param data: The symbols.
-    :param matches: The currencies.
+    :param data: The data to process.
     :param separator: The separator of the assets.
 
-    :return: The validation value for the symbols.
+    :return: The currencies from the screeners.
     """
 
-    pairs = []
-    exchange_symbol_pairs = []
+    result = {}
 
     for exchange, symbols in data.items():
-        exchange_symbol_pairs.extend([(exchange, symbol) for symbol in symbols])
+        result.setdefault(exchange, []).extend(symbols)
     # end for
 
-    for exchange1, symbol1 in exchange_symbol_pairs:
-        for exchange2, symbol2 in exchange_symbol_pairs:
-            exchanges_matches = (
-                matches if not isinstance(matches, dict) else
-                [*matches.get(exchange1, []), *matches.get(exchange2, [])]
+    return {
+        exchange: list(
+            set(
+                symbol_to_pair(symbol=symbol, separator=separator).base
+                for symbol in set(symbols)
             )
+        )
 
-            if (
-                (exchange1 != exchange2) and
-                matching_symbol_pair(
-                    symbol1, symbol2,
-                    matches=exchanges_matches or None,
-                    separator=separator
-                )
-            ):
-                pairs.append(
-                    ((exchange1, symbol1), (exchange2, symbol2))
-                )
-            # end if
-        # end for
+        for exchange, symbols in result.items()
+    }
+# end exchanges_symbols_base_assets
+
+def exchanges_symbols_quote_assets(
+        data: Dict[str, Iterable[str]],
+        separator: Optional[str] = None
+) -> Dict[str, Set[str]]:
+    """
+    Finds the currencies from the screeners.
+
+    :param data: The data to process.
+    :param separator: The separator of the assets.
+
+    :return: The currencies from the screeners.
+    """
+
+    result = {}
+
+    for exchange, symbols in data.items():
+        result.setdefault(exchange, []).extend(symbols)
     # end for
 
-    return set(pairs)
-# end matching_symbol_pairs
+    return {
+        exchange: list(
+            set(
+                symbol_to_pair(symbol=symbol, separator=separator).quote
+                for symbol in set(symbols)
+            )
+        )
+        for exchange, symbols in result.items()
+    }
+# end exchanges_symbols_quote_assets
 
-@define(repr=False, unsafe_hash=True)
-@represent
-class MarketSymbolSignature:
-    """A class to represent the data for the execution of a trade."""
-
-    asset: str
-    currency: str
-    exchange: str
-# end MarketPairSignature
-
-def matching_symbol_signatures(
-        pairs: Optional[ExchangeSymbolPairs] = None,
-        data: Optional[Dict[str, Iterable[str]]] = None,
-        matches: Optional[ExchangesAssetMatches] = None,
-        separator: Optional[str] = None
-) -> Set[Tuple[MarketSymbolSignature, MarketSymbolSignature]]:
+def mutual_exchanges_assets(
+        exchanges: Optional[Iterable[str]] = None,
+        adjust: Optional[bool] = True,
+        separator: Optional[str] = None,
+        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        data: Optional[Dict[str, Iterable[str]]] = None
+) -> Dict[str, Set[str]]:
     """
-    Checks if the screeners are valid with the matching currencies.
+    Collects the symbols from the exchanges.
 
-    :param data: The data for the pairs.
-    :param pairs: The pairs' data.
-    :param matches: The currencies.
+    :param exchanges: The exchanges.
+    :param quotes: The quotes of the asset pairs.
+    :param bases: The bases of the asset pairs.
+    :param excluded: The excluded symbols.
+    :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
+    :param data: The data to search in.
+    :param included: The symbols to include.
 
-    :return: The validation value for the symbols.
+    :return: The data of the exchanges.
     """
 
-    if (data is None) and (pairs is None):
-        raise ValueError(
-            f"One of 'pairs' and 'data' parameters must be given, "
-            f"when 'pairs' is superior to 'data'."
+    return mutual_string_values(
+        data=data or exchanges_assets(
+            exchanges=exchanges, quotes=quotes, bases=bases, included=included,
+            excluded=excluded, adjust=adjust, separator=separator
         )
+    )
+# end mutual_exchanges_assets
 
-    elif (not pairs) and (not data):
-        return set()
-    # end if
-
-    new_pairs = []
-
-    pairs = pairs or matching_symbol_pairs(
-        data=data, matches=matches, separator=separator
-    )
-
-    for (exchange1, symbol1), (exchange2, symbol2) in pairs:
-        asset1, currency1 = symbol_to_parts(adjust_symbol(symbol1))
-        asset2, currency2 = symbol_to_parts(adjust_symbol(symbol2))
-
-        new_pairs.append(
-            (
-                MarketSymbolSignature(
-                    asset=asset1, currency=currency1,
-                    exchange=exchange1
-                ),
-                MarketSymbolSignature(
-                    asset=asset2, currency=currency2,
-                    exchange=exchange2
-                )
-            )
+def mutual_exchanges_base_assets(
+        exchanges: Optional[Iterable[str]] = None,
+        adjust: Optional[bool] = True,
+        separator: Optional[str] = None,
+        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        data: Optional[Dict[str, Iterable[str]]] = None
+) -> Dict[str, Set[str]]:
+    """
+    Collects the symbols from the exchanges.
+
+    :param exchanges: The exchanges.
+    :param quotes: The quotes of the asset pairs.
+    :param bases: The bases of the asset pairs.
+    :param excluded: The excluded symbols.
+    :param adjust: The value to adjust the invalid exchanges.
+    :param separator: The separator of the assets.
+    :param data: The data to search in.
+    :param included: The symbols to include.
+
+    :return: The data of the exchanges.
+    """
+
+    return mutual_string_values(
+        data=data or exchanges_base_assets(
+            exchanges=exchanges, quotes=quotes, bases=bases, included=included,
+            excluded=excluded, adjust=adjust, separator=separator
         )
-    # end for
+    )
+# end mutual_exchanges_base_assets
+
+def mutual_exchanges_quote_assets(
+        exchanges: Optional[Iterable[str]] = None,
+        adjust: Optional[bool] = True,
+        separator: Optional[str] = None,
+        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        data: Optional[Dict[str, Iterable[str]]] = None
+) -> Dict[str, Set[str]]:
+    """
+    Collects the symbols from the exchanges.
 
-    return set(new_pairs)
-# end matching_symbol_signatures
+    :param exchanges: The exchanges.
+    :param quotes: The quotes of the asset pairs.
+    :param bases: The bases of the asset pairs.
+    :param excluded: The excluded symbols.
+    :param adjust: The value to adjust the invalid exchanges.
+    :param separator: The separator of the assets.
+    :param data: The data to search in.
+    :param included: The symbols to include.
+
+    :return: The data of the exchanges.
+    """
+
+    return mutual_string_values(
+        data=data or exchanges_quote_assets(
+            exchanges=exchanges, quotes=quotes, bases=bases, included=included,
+            excluded=excluded, adjust=adjust, separator=separator
+        )
+    )
+# end mutual_exchanges_quote_assets
```

### Comparing `crypto-screening-8.2.1/crypto_screening/dataset.py` & `crypto-screening-8.2.2/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/exchanges.py` & `crypto-screening-8.2.2/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/interval.py` & `crypto-screening-8.2.2/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/base.py` & `crypto-screening-8.2.2/crypto_screening/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/callbacks/base.py` & `crypto-screening-8.2.2/crypto_screening/screeners/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/callbacks/database.py` & `crypto-screening-8.2.2/crypto_screening/screeners/callbacks/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/callbacks/sockets.py` & `crypto-screening-8.2.2/crypto_screening/screeners/callbacks/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/collectors/base.py` & `crypto-screening-8.2.2/crypto_screening/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/collectors/database.py` & `crypto-screening-8.2.2/crypto_screening/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/collectors/sockets.py` & `crypto-screening-8.2.2/crypto_screening/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/combined.py` & `crypto-screening-8.2.2/crypto_screening/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/container.py` & `crypto-screening-8.2.2/crypto_screening/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/database.py` & `crypto-screening-8.2.2/crypto_screening/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/foundation/data.py` & `crypto-screening-8.2.2/crypto_screening/screeners/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/foundation/protocols.py` & `crypto-screening-8.2.2/crypto_screening/screeners/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/foundation/state.py` & `crypto-screening-8.2.2/crypto_screening/screeners/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/foundation/waiting.py` & `crypto-screening-8.2.2/crypto_screening/screeners/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/market.py` & `crypto-screening-8.2.2/crypto_screening/screeners/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/ohlcv.py` & `crypto-screening-8.2.2/crypto_screening/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/orderbook.py` & `crypto-screening-8.2.2/crypto_screening/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/orders.py` & `crypto-screening-8.2.2/crypto_screening/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/recorder.py` & `crypto-screening-8.2.2/crypto_screening/screeners/recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,36 +101,38 @@
 
     else:
         base_parameters = parameters or {}
         parameters = {}
     # end if
 
     for exchange, symbols in data.items():
+        saved_exchange = exchange
+
         exchange = find_string_value(value=exchange, values=EXCHANGE_NAMES)
 
         symbols = [adjust_symbol(symbol, separator='-') for symbol in symbols]
 
         if fixed:
-            parameters.setdefault(exchange, base_parameters)
+            parameters.setdefault(saved_exchange, base_parameters)
         # end if
 
         EXCHANGES[exchange]: Type[ExchangeFeed]
 
         groups = []
 
         for i in range(0, int(len(symbols) / amount) + len(symbols) % amount, amount):
             groups.append(symbols[i:])
         # end for
 
         for symbols_packet in groups:
             exchange_parameters = (
-                parameters[exchange]
+                parameters[saved_exchange]
                 if (
-                    (exchange in parameters) and
-                    isinstance(parameters[exchange], dict) and
+                    (saved_exchange in parameters) and
+                    isinstance(parameters[saved_exchange], dict) and
                     all(isinstance(key, str) for key in parameters)
                 ) else {}
             )
 
             feed = EXCHANGES[exchange](symbols=symbols_packet, **exchange_parameters)
 
             feed.start = partial(ExchangeFeed.start, feed)
```

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/trades.py` & `crypto-screening-8.2.2/crypto_screening/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/screeners/waiting.py` & `crypto-screening-8.2.2/crypto_screening/screeners/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.2.2/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/symbols.py` & `crypto-screening-8.2.2/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/utils/base.py` & `crypto-screening-8.2.2/crypto_screening/utils/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/crypto_screening/utils/process.py` & `crypto-screening-8.2.2/crypto_screening/utils/process.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from typing import Iterable, List, Set, Optional, Dict
 
 __all__ = [
     "find_string_value",
     "upper_string_values",
     "lower_string_values",
-    "mutual_string_values"
+    "mutual_string_values",
+    "string_in_values"
 ]
 
 def find_string_value(value: str, values: Iterable[str]) -> str:
     """
     Finds the exchange in the exchanges.
 
     :param value: The name of the exchange.
@@ -32,14 +33,27 @@
             return valid
         # end if
     # end for
 
     return value
 # end find_string_value
 
+def string_in_values(value: str, values: Iterable[str]) -> bool:
+    """
+    Finds the exchange in the exchanges.
+
+    :param value: The name of the exchange.
+    :param values: The exchanges to search in.
+
+    :return: The valid exchange name.
+    """
+
+    return find_string_value(value=value, values=values) in values
+# end string_in_values
+
 def upper_string_values(values: Iterable[str]) -> List[str]:
     """
     Converts all string values to upper case.
 
     :param values: The values to convert.
 
     :return: The converted values.
```

### Comparing `crypto-screening-8.2.1/crypto_screening/validate.py` & `crypto-screening-8.2.2/crypto_screening/validate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # validate.py
 
 from typing import Optional, Iterable, Any
 
-from crypto_screening.utils.process import find_string_value
+from crypto_screening.utils.process import string_in_values
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.interval import interval_to_total_time
 from crypto_screening.exchanges import EXCHANGE_NAMES
 
 __all__ = [
     "is_valid_symbol",
     "validate_exchange",
@@ -92,17 +92,15 @@
     :return: The validation value.
     """
 
     if exchanges is None:
         exchanges = EXCHANGE_NAMES
     # end if
 
-    exchange = find_string_value(value=exchange, values=exchanges)
-
-    return exchange in exchanges
+    return string_in_values(value=exchange, values=exchanges)
 # end is_valid_exchange
 
 def validate_exchange(
         exchange: str,
         exchanges: Optional[Iterable[str]] = None,
         provider: Optional[Any] = None
 ) -> str:
```

### Comparing `crypto-screening-8.2.1/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.2.2/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.2.1
+Version: 8.2.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.2.1/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.2.2/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.1/pyproject.toml` & `crypto-screening-8.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.2.1'
+version = '8.2.2'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.2.1/setup.py` & `crypto-screening-8.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='8.2.1',
+        version='8.2.2',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

