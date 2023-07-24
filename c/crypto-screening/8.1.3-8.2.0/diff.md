# Comparing `tmp/crypto-screening-8.1.3.tar.gz` & `tmp/crypto-screening-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.1.3.tar", last modified: Mon Jul 24 09:21:12 2023, max compression
+gzip compressed data, was "crypto-screening-8.2.0.tar", last modified: Mon Jul 24 09:53:55 2023, max compression
```

## Comparing `crypto-screening-8.1.3.tar` & `crypto-screening-8.2.0.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.915155 crypto-screening-8.1.3/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:21:11.000000 crypto-screening-8.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-24 09:21:12.915155 crypto-screening-8.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.1.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.1.3/build.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.700265 crypto-screening-8.1.3/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.737362 crypto-screening-8.1.3/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17733 2023-07-22 15:48:11.000000 crypto-screening-8.1.3/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4773 2023-07-22 15:47:32.000000 crypto-screening-8.1.3/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.764362 crypto-screening-8.1.3/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-8.1.3/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-8.1.3/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-8.1.3/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-8.1.3/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.786393 crypto-screening-8.1.3/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-8.1.3/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-8.1.3/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16580 2023-07-23 16:36:28.000000 crypto-screening-8.1.3/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-8.1.3/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-8.1.3/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    17755 2023-07-23 13:27:54.000000 crypto-screening-8.1.3/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19520 2023-07-22 15:47:21.000000 crypto-screening-8.1.3/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.1.3/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.1.3/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.1.3/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.797394 crypto-screening-8.1.3/crypto_screening/market/
--rw-rw-rw-   0        0        0    15126 2023-07-22 11:30:19.000000 crypto-screening-8.1.3/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.817394 crypto-screening-8.1.3/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10459 2023-07-22 14:33:35.000000 crypto-screening-8.1.3/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.1.3/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-8.1.3/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-8.1.3/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.874184 crypto-screening-8.1.3/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    23442 2023-07-22 14:11:45.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/base.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.881155 crypto-screening-8.1.3/crypto_screening/market/screeners/callbacks/
--rw-rw-rw-   0        0        0      214 2023-07-22 15:42:32.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/callbacks/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/callbacks/base.py
--rw-rw-rw-   0        0        0     4414 2023-07-24 09:18:59.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/callbacks/database.py
--rw-rw-rw-   0        0        0     5612 2023-07-24 09:18:59.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/callbacks/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.902155 crypto-screening-8.1.3/crypto_screening/market/screeners/collectors/
--rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6285 2023-07-22 14:19:31.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4055 2023-07-22 09:26:50.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6164 2023-07-22 15:50:07.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12308 2023-07-22 15:48:11.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    10848 2023-07-22 14:02:39.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    10983 2023-07-21 08:58:32.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/database.py
--rw-rw-rw-   0        0        0    22129 2023-07-22 15:48:53.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11829 2023-07-22 15:54:41.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11431 2023-07-22 15:49:37.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    16942 2023-07-22 15:49:37.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    11500 2023-07-22 15:50:19.000000 crypto-screening-8.1.3/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-8.1.3/crypto_screening/market/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.665270 crypto-screening-8.1.3/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.902155 crypto-screening-8.1.3/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.1.3/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-8.1.3/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.914184 crypto-screening-8.1.3/crypto_screening/utils/
--rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.1.3/crypto_screening/utils/base.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-8.1.3/crypto_screening/utils/process.py
--rw-rw-rw-   0        0        0     3605 2023-07-22 15:45:17.000000 crypto-screening-8.1.3/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:12.714391 crypto-screening-8.1.3/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-24 09:21:12.000000 crypto-screening-8.1.3/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2254 2023-07-24 09:21:12.000000 crypto-screening-8.1.3/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:21:12.000000 crypto-screening-8.1.3/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-24 09:21:12.000000 crypto-screening-8.1.3/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-24 09:21:12.000000 crypto-screening-8.1.3/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-24 09:21:11.000000 crypto-screening-8.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.1.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 09:21:12.915155 crypto-screening-8.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-24 09:20:54.000000 crypto-screening-8.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.916527 crypto-screening-8.2.0/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:53:55.000000 crypto-screening-8.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-24 09:53:55.916527 crypto-screening-8.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.2.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.2.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.883527 crypto-screening-8.2.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.891527 crypto-screening-8.2.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17733 2023-07-22 15:48:11.000000 crypto-screening-8.2.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4773 2023-07-22 15:47:32.000000 crypto-screening-8.2.0/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.894527 crypto-screening-8.2.0/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.2.0/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.2.0/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.897527 crypto-screening-8.2.0/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.2.0/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24665 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16516 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21653 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    17728 2023-07-24 09:40:24.000000 crypto-screening-8.2.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19520 2023-07-22 15:47:21.000000 crypto-screening-8.2.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.2.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.2.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.2.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.905527 crypto-screening-8.2.0/crypto_screening/screeners/
+-rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.2.0/crypto_screening/screeners/__init__.py
+-rw-rw-rw-   0        0        0    23312 2023-07-24 09:37:18.000000 crypto-screening-8.2.0/crypto_screening/screeners/base.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.908527 crypto-screening-8.2.0/crypto_screening/screeners/callbacks/
+-rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.2.0/crypto_screening/screeners/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.2.0/crypto_screening/screeners/callbacks/base.py
+-rw-rw-rw-   0        0        0     4400 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/screeners/callbacks/database.py
+-rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/screeners/callbacks/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.910527 crypto-screening-8.2.0/crypto_screening/screeners/collectors/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.2.0/crypto_screening/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6271 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.2.0/crypto_screening/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.2.0/crypto_screening/screeners/combined.py
+-rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.2.0/crypto_screening/screeners/container.py
+-rw-rw-rw-   0        0        0    10976 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/screeners/database.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.913525 crypto-screening-8.2.0/crypto_screening/screeners/foundation/
+-rw-rw-rw-   0        0        0    10462 2023-07-24 09:37:33.000000 crypto-screening-8.2.0/crypto_screening/screeners/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.2.0/crypto_screening/screeners/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.2.0/crypto_screening/screeners/foundation/state.py
+-rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.2.0/crypto_screening/screeners/foundation/waiting.py
+-rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.2.0/crypto_screening/screeners/market.py
+-rw-rw-rw-   0        0        0    22099 2023-07-24 09:38:59.000000 crypto-screening-8.2.0/crypto_screening/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11814 2023-07-24 09:39:14.000000 crypto-screening-8.2.0/crypto_screening/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11410 2023-07-24 09:39:34.000000 crypto-screening-8.2.0/crypto_screening/screeners/orders.py
+-rw-rw-rw-   0        0        0    16921 2023-07-24 09:39:41.000000 crypto-screening-8.2.0/crypto_screening/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11479 2023-07-24 09:39:59.000000 crypto-screening-8.2.0/crypto_screening/screeners/trades.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.2.0/crypto_screening/screeners/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.875518 crypto-screening-8.2.0/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.913525 crypto-screening-8.2.0/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.2.0/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-8.2.0/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.915526 crypto-screening-8.2.0/crypto_screening/utils/
+-rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.2.0/crypto_screening/utils/base.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-8.2.0/crypto_screening/utils/process.py
+-rw-rw-rw-   0        0        0     3605 2023-07-22 15:45:17.000000 crypto-screening-8.2.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:55.888527 crypto-screening-8.2.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-24 09:53:55.000000 crypto-screening-8.2.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-07-24 09:53:55.000000 crypto-screening-8.2.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 09:53:55.000000 crypto-screening-8.2.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-24 09:53:55.000000 crypto-screening-8.2.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-24 09:53:55.000000 crypto-screening-8.2.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-24 09:49:05.000000 crypto-screening-8.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.2.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 09:53:55.916527 crypto-screening-8.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-24 09:48:54.000000 crypto-screening-8.2.0/setup.py
```

### Comparing `crypto-screening-8.1.3/PKG-INFO` & `crypto-screening-8.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.1.3
+Version: 8.2.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.1.3/README.md` & `crypto-screening-8.2.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/build.py` & `crypto-screening-8.2.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/collect/assets.py` & `crypto-screening-8.2.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/collect/exchanges.py` & `crypto-screening-8.2.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.2.0/crypto_screening/collect/market/ohlcv.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from represent import represent, Modifiers
 
 import pandas as pd
 
 from crypto_screening.dataset import OPEN, HIGH, LOW, CLOSE, VOLUME
 
-from crypto_screening.market.screeners.base import BaseScreener
+from crypto_screening.screeners import BaseScreener
 from crypto_screening.collect.market.state import (
     MarketState, assets_market_values, SymbolsMarketState,
     is_symbol_in_assets_market_values, symbols_market_values,
     is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
     assets_to_symbols_data, assets_market_state_data,
     symbol_to_assets_data, symbols_market_state_data,
     merge_assets_market_states_data, AssetsMarketState
```

### Comparing `crypto-screening-8.1.3/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.2.0/crypto_screening/collect/market/orderbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 
 from attrs import define
 
 from represent import represent, Modifiers
 
 import pandas as pd
 
-from crypto_screening.market.screeners.base import BaseScreener
+from crypto_screening.screeners import BaseScreener
+from crypto_screening.collect.market.state.base import ORDERBOOK_ATTRIBUTES
 from crypto_screening.collect.market.state import (
-    MarketState, assets_market_values, ORDERBOOK_ATTRIBUTES,
+    MarketState, assets_market_values, AssetsMarketState,
     is_symbol_in_assets_market_values, symbols_market_values,
     is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
     assets_to_symbols_data, assets_market_state_data,
     symbol_to_assets_data, symbols_market_state_data,
-    merge_assets_market_states_data, SymbolsMarketState, AssetsMarketState
+    merge_assets_market_states_data, SymbolsMarketState
 )
 
 __all__ = [
     "symbols_orderbook_market_state",
     "merge_assets_orderbook_market_states",
     "merge_symbols_orderbook_market_states",
     "assets_orderbook_market_state",
```

### Comparing `crypto-screening-8.1.3/crypto_screening/collect/market/orders.py` & `crypto-screening-8.2.0/crypto_screening/collect/market/orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from represent import represent, Modifiers
 
 import pandas as pd
 
 from crypto_screening.dataset import BIDS, ASKS
 
-from crypto_screening.market.screeners.base import BaseScreener
+from crypto_screening.screeners import BaseScreener
 from crypto_screening.collect.market.state import (
     MarketState, assets_market_values, SymbolsMarketState,
     is_symbol_in_assets_market_values, symbols_market_values,
     is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
     assets_to_symbols_data, assets_market_state_data,
     symbol_to_assets_data, symbols_market_state_data,
     merge_assets_market_states_data, AssetsMarketState
```

### Comparing `crypto-screening-8.1.3/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.2.0/crypto_screening/collect/market/state/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 from represent import represent
 
 import numpy as np
 import pandas as pd
 
 from crypto_screening.dataset import create_dataset
-from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.orderbook import OrderbookScreener
-from crypto_screening.market.screeners.ohlcv import OHLCVScreener
-from crypto_screening.market.screeners.orders import OrdersScreener
-from crypto_screening.market.screeners.trades import TradesScreener
+from crypto_screening.screeners import BaseScreener
+from crypto_screening.screeners import OrderbookScreener
+from crypto_screening.screeners.ohlcv import OHLCVScreener
+from crypto_screening.screeners import OrdersScreener
+from crypto_screening.screeners import TradesScreener
 from crypto_screening.symbols import symbol_to_parts, parts_to_symbol
 from crypto_screening.collect.screeners import find_screeners
 from crypto_screening.collect.market.state.base import (
     is_exchange_in_market_data, get_last_value, MarketState,
     dataset_to_data_rows, add_data_to_screeners, data_from_dataset,
     minimum_common_dataset_length, screener_dataset,
     add_data_to_symbols_screeners, index_to_datetime,
```

### Comparing `crypto-screening-8.1.3/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.2.0/crypto_screening/collect/market/state/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
 import numpy as np
 import pandas as pd
 
 from crypto_screening.dataset import (
     BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, bid_ask_to_ohlcv
 )
-from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.orderbook import OrderbookScreener
-from crypto_screening.market.screeners.ohlcv import OHLCVScreener
-from crypto_screening.market.screeners.orders import OrdersScreener
-from crypto_screening.market.screeners.trades import TradesScreener
+from crypto_screening.screeners import BaseScreener
+from crypto_screening.screeners import OrderbookScreener
+from crypto_screening.screeners.ohlcv import OHLCVScreener
+from crypto_screening.screeners import OrdersScreener
+from crypto_screening.screeners import TradesScreener
 from crypto_screening.dataset import dataset_to_json
 from crypto_screening.collect.screeners import find_screeners
 
 __all__ = [
     "is_exchange_in_market_data",
     "dataset_to_data_rows",
     "MarketState",
```

### Comparing `crypto-screening-8.1.3/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.2.0/crypto_screening/collect/market/state/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 from represent import represent
 
 import numpy as np
 import pandas as pd
 
 from crypto_screening.dataset import create_dataset
-from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.orderbook import OrderbookScreener
-from crypto_screening.market.screeners.ohlcv import OHLCVScreener
-from crypto_screening.market.screeners.orders import OrdersScreener
-from crypto_screening.market.screeners.trades import TradesScreener
+from crypto_screening.screeners import BaseScreener
+from crypto_screening.screeners import OrderbookScreener
+from crypto_screening.screeners.ohlcv import OHLCVScreener
+from crypto_screening.screeners import OrdersScreener
+from crypto_screening.screeners import TradesScreener
 from crypto_screening.symbols import symbol_to_parts
 from crypto_screening.collect.screeners import find_screeners
 from crypto_screening.collect.market.state.base import (
     is_exchange_in_market_data, get_last_value, MarketState,
     dataset_to_data_rows, add_data_to_screeners, adjusted_dataset_length,
     minimum_common_dataset_length, screener_dataset, set_screener_dataset,
     add_data_to_symbols_screeners, index_to_datetime, data_from_dataset,
```

### Comparing `crypto-screening-8.1.3/crypto_screening/collect/market/trades.py` & `crypto-screening-8.2.0/crypto_screening/collect/market/trades.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from represent import represent, Modifiers
 
 import pandas as pd
 
 from crypto_screening.dataset import PRICE, AMOUNT, SIDE
 
-from crypto_screening.market.screeners.base import BaseScreener
+from crypto_screening.screeners import BaseScreener
 from crypto_screening.collect.market.state import (
     MarketState, assets_market_values, SymbolsMarketState,
     is_symbol_in_assets_market_values, symbols_market_values,
     is_symbol_in_symbols_market_values, merge_symbols_market_states_data,
     assets_to_symbols_data, assets_market_state_data,
     symbol_to_assets_data, symbols_market_state_data,
     merge_assets_market_states_data, AssetsMarketState
```

### Comparing `crypto-screening-8.1.3/crypto_screening/collect/screeners.py` & `crypto-screening-8.2.0/crypto_screening/collect/screeners.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,17 @@
 )
 
 import pandas as pd
 from attrs import define
 
 from crypto_screening.symbols import symbol_to_pair, symbol_to_parts
 from crypto_screening.collect.symbols import (
-    matching_symbol_pair, MarketSymbolSignature,
-    exchanges_symbols
-)
-from crypto_screening.market.screeners.base import (
-    BaseScreener, BaseMarketScreener
+    matching_symbol_pair, MarketSymbolSignature, exchanges_symbols
 )
+from crypto_screening.screeners import BaseScreener, BaseMarketScreener
 
 __all__ = [
     "matching_screener_signatures",
     "matching_screener_pair",
     "matching_screener_pairs",
     "MarketScreenerSignature",
     "find_screeners",
```

### Comparing `crypto-screening-8.1.3/crypto_screening/collect/symbols.py` & `crypto-screening-8.2.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/dataset.py` & `crypto-screening-8.2.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/exchanges.py` & `crypto-screening-8.2.0/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/interval.py` & `crypto-screening-8.2.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/market/dynamic.py` & `crypto-screening-8.2.0/crypto_screening/screeners/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# dynamic.py
+# market.py
 
 from typing import Optional, Iterable, Union, Dict
 
 from crypto_screening.collect.screeners import exchanges_symbols_screeners
 from crypto_screening.collect.market.orderbook import (
     assets_orderbook_market_state, symbols_orderbook_market_state,
     SymbolsOrderbookMarketState, AssetsOrderbookMarketState
@@ -15,21 +15,21 @@
     assets_orders_market_state, symbols_orders_market_state,
     SymbolsOrdersMarketState, AssetsOrdersMarketState
 )
 from crypto_screening.collect.market.trades import (
     assets_trades_market_state, symbols_trades_market_state,
     SymbolsTradesMarketState, AssetsTradesMarketState
 )
-from crypto_screening.market.screeners.container import (
-    ScreenersContainer, FrozenScreenersContainer
+from crypto_screening.screeners.container import (
+    FrozenScreenersContainer, ScreenersContainer
 )
 
 __all__ = [
-    "ScreenersMarket",
-    "FrozenScreenersMarket"
+    "FrozenScreenersMarket",
+    "ScreenersMarket"
 ]
 
 ExchangesData = Union[Dict[str, Iterable[str]], Iterable[str]]
 
 class FrozenScreenersMarket(FrozenScreenersContainer):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
@@ -37,16 +37,16 @@
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
         The screener objects to form a market.
 
-    >>> from crypto_screening.market.dynamic import FrozenScreenersMarket
-    >>> from crypto_screening.market.screeners.base import BaseScreener
+    >>> from crypto_screening.screeners.market import FrozenScreenersMarket
+    >>> from crypto_screening.screeners import BaseScreener
     >>>
     >>> market = FrozenScreenersMarket(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     >>>
     >>> market.find_screener(exchange="binance", symbol="BTC/USDT"))
     """
@@ -367,16 +367,16 @@
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
         The screener objects to form a market.
 
-    >>> from crypto_screening.market.dynamic import ScreenersMarket
-    >>> from crypto_screening.market.screeners.base import BaseScreener
+    >>> from crypto_screening.screeners.market import ScreenersMarket
+    >>> from crypto_screening.screeners import BaseScreener
     >>>
     >>> market = ScreenersMarket(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     >>>
     >>> market.find_screener(exchange="binance", symbol="BTC/USDT"))
     """
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/foundation/data.py` & `crypto-screening-8.2.0/crypto_screening/screeners/foundation/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from abc import ABCMeta, abstractmethod
 import threading
 from typing import Optional, Union, Dict, Any
 
 from represent import represent
 
 
-from crypto_screening.market.foundation.state import WaitingState
+from crypto_screening.screeners.foundation.state import WaitingState
 
 __all__ = [
     "DataCollector"
 ]
 
 @represent
 class DataCollector(metaclass=ABCMeta):
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/foundation/protocols.py` & `crypto-screening-8.2.0/crypto_screening/screeners/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/market/foundation/state.py` & `crypto-screening-8.2.0/crypto_screening/screeners/foundation/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Optional, Union, Iterable, ClassVar, TypeVar, Generic
 )
 
 from attrs import define
 
 from represent import represent, Modifiers
 
-from crypto_screening.market.foundation.protocols import (
+from crypto_screening.screeners.foundation.protocols import (
     BaseScreenerProtocol, BaseMarketScreenerProtocol
 )
 
 __all__ = [
     "WaitingState"
 ]
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/foundation/waiting.py` & `crypto-screening-8.2.0/crypto_screening/screeners/foundation/waiting.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import datetime as dt
 import time
 from typing import (
     Optional, Union, Iterable, Callable, TypeVar
 )
 
-from crypto_screening.market.foundation.data import DataCollector
-from crypto_screening.market.foundation.state import WaitingState
-from crypto_screening.market.foundation.protocols import (
+from crypto_screening.screeners.foundation.data import DataCollector
+from crypto_screening.screeners.foundation.state import WaitingState
+from crypto_screening.screeners.foundation.protocols import (
     BaseScreenerProtocol, BaseMarketScreenerProtocol
 )
 
 __all__ = [
     "base_await_update",
     "base_await_initialization",
     "base_await_dynamic_update",
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/base.py` & `crypto-screening-8.2.0/crypto_screening/screeners/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 from multithreading import Caller, multi_threaded_call
 
 from crypto_screening.dataset import save_dataset, load_dataset, create_dataset
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.validate import validate_exchange, validate_symbol
 from crypto_screening.collect.symbols import all_exchange_symbols
-from crypto_screening.market.foundation.state import WaitingState
-from crypto_screening.market.foundation.data import DataCollector
-from crypto_screening.market.foundation.protocols import BaseScreenerProtocol
-from crypto_screening.market.foundation.waiting import (
+from crypto_screening.screeners.foundation.state import WaitingState
+from crypto_screening.screeners.foundation.data import DataCollector
+from crypto_screening.screeners.foundation.protocols import BaseScreenerProtocol
+from crypto_screening.screeners.foundation.waiting import (
     base_await_initialization, base_await_dynamic_initialization,
     base_await_dynamic_update, base_await_update
 )
 
 __all__ = [
     "BaseScreener",
     "BaseMarketScreener",
@@ -386,16 +386,15 @@
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
         The screener objects to form a market.
 
-    >>> from crypto_screening.market.screeners.base import BaseFrozenScreenersContainer
-    >>> from crypto_screening.market.screeners.base import BaseScreener
+    >>> from crypto_screening.screeners import BaseFrozenScreenersContainer, BaseScreener
     >>>
     >>> container = BaseFrozenScreenersContainer(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     """
 
     def __init__(self, screeners: Iterable[BaseScreener]) -> None:
@@ -552,16 +551,15 @@
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
         The screener objects to form a market.
 
-    >>> from crypto_screening.market.screeners.base import BaseScreenersContainer
-    >>> from crypto_screening.market.screeners.base import BaseScreener
+    >>> from crypto_screening.screeners import BaseScreenersContainer, BaseScreener
     >>>
     >>> container = BaseScreenersContainer(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     """
 
     def update_screeners(self) -> None:
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/callbacks/base.py` & `crypto-screening-8.2.0/crypto_screening/screeners/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/callbacks/database.py` & `crypto-screening-8.2.0/crypto_screening/screeners/callbacks/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import datetime as dt
 from typing import Optional, Any, Dict, List, Tuple
 
 from sqlalchemy import Engine, text, inspect
 from sqlalchemy.orm import sessionmaker
 
 from crypto_screening.dataset import DATE_TIME
-from crypto_screening.market.screeners.database import (
+from crypto_screening.screeners.database import (
     create_engine, parts_to_database_table_name
 )
-from crypto_screening.market.screeners.callbacks.base import BaseCallback
+from crypto_screening.screeners.callbacks.base import BaseCallback
 
 __all__ = [
     "DatabaseCallback"
 ]
 
 class DatabaseCallback(BaseCallback):
     """A class to represent a callback."""
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/callbacks/sockets.py` & `crypto-screening-8.2.0/crypto_screening/screeners/callbacks/sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 from typing import Optional, Any, Union, Dict, Callable
 import asyncio
 from textwrap import wrap
 
 from cryptofeed.backends.socket import UDPProtocol
 
-from crypto_screening.market.screeners.callbacks.base import BaseCallback
+from crypto_screening.screeners.callbacks.base import BaseCallback
 
 __all__ = [
     "SocketCallback"
 ]
 
 Connection = Union[asyncio.StreamWriter, asyncio.DatagramTransport]
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/collectors/base.py` & `crypto-screening-8.2.0/crypto_screening/screeners/collectors/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # base.py
 
 import threading
 import datetime as dt
 import time
 from typing import List, Tuple, Optional, Iterable, Union, Dict, Any
 
-from crypto_screening.market.screeners.container import ScreenersContainer
-from crypto_screening.market.screeners.base import BaseScreener, BaseMarketScreener
+from crypto_screening.screeners.container import ScreenersContainer
+from crypto_screening.screeners.base import BaseScreener, BaseMarketScreener
 from crypto_screening.collect.market.state.base import index_to_datetime
 
 __all__ = [
     "ScreenersDataCollector"
 ]
 
 Data = List[Tuple[Union[str, float, dt.datetime], Dict[str, Optional[Union[str, float, bool]]]]]
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/collectors/database.py` & `crypto-screening-8.2.0/crypto_screening/screeners/collectors/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# data.py
+# database.py
 
 import datetime as dt
 from typing import Optional, Union, Iterable, Dict, Tuple, List
 
 from sqlalchemy import Engine
 
-from crypto_screening.market.screeners.callbacks import DatabaseCallback
-from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.database import (
+from crypto_screening.screeners.base import BaseScreener
+from crypto_screening.screeners.database import (
     extract_database_table_parts, extract_database_table_record,
-    create_engine, extract_database_tables
+    create_engine, extract_database_table_names, screeners_tables_names
 )
-from crypto_screening.market.screeners.collectors.base import ScreenersDataCollector
+from crypto_screening.screeners.collectors.base import ScreenersDataCollector
 
 __all__ = [
-    "DatabaseScreenersDataCollector",
-    "DatabaseCallback"
+    "DatabaseScreenersDataCollector"
 ]
 
 Data = List[Tuple[Union[str, float, dt.datetime], Dict[str, Optional[Union[str, float, bool]]]]]
 
 class DatabaseScreenersDataCollector(ScreenersDataCollector):
     """
     A class to represent an asset price screener.
@@ -83,17 +81,24 @@
 
         if isinstance(self.engine, Engine):
             self._connected = True
         # end if
 
         self._session: Optional = None
 
+        all_tables = extract_database_table_names(self.engine)
+
         self.tables = (
-            extract_database_table_parts(tables) or
-            extract_database_tables(self.engine)
+            extract_database_table_parts(
+                tables or [
+                    table for table in
+                    screeners_tables_names(self.screeners).values()
+                    if table in all_tables
+                ]
+            )
         )
 
         self.failed_tables: Dict[str, List[Exception]] = {}
     # end __init__
 
     def screening_loop(self) -> None:
         """Runs the process of the price screening."""
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/collectors/sockets.py` & `crypto-screening-8.2.0/crypto_screening/screeners/collectors/sockets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # sockets.py
 
 import json
 import asyncio
 import datetime as dt
 from typing import Dict, Any, Optional, Union, Iterable, List, Tuple
 
-from crypto_screening.market.screeners.callbacks import SocketCallback, BaseCallback
-from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.collectors.base import ScreenersDataCollector
+from crypto_screening.screeners.callbacks import SocketCallback, BaseCallback
+from crypto_screening.screeners.base import BaseScreener
+from crypto_screening.screeners.collectors.base import ScreenersDataCollector
 
 __all__ = [
     "SocketScreenersDataCollector",
     "SocketCallback"
 ]
 
 ScreenersTable = Dict[str, Dict[str, Dict[str, Dict[Optional[str], List[BaseScreener]]]]]
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/combined.py` & `crypto-screening-8.2.0/crypto_screening/screeners/combined.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # combined.py
 
 import datetime as dt
 from typing import (
     Dict, Optional, Iterable, Any, Union, List, Type, Callable
 )
 
-from crypto_screening.market.screeners.orderbook import (
+from crypto_screening.screeners.orderbook import (
     orderbook_market_screener
 )
-from crypto_screening.market.screeners.ohlcv import (
+from crypto_screening.screeners.ohlcv import (
     ohlcv_market_screener
 )
-from crypto_screening.market.screeners.trades import (
+from crypto_screening.screeners.trades import (
     trades_market_screener
 )
-from crypto_screening.market.screeners.orders import (
+from crypto_screening.screeners.orders import (
     orders_market_screener
 )
-from crypto_screening.market.screeners.container import ScreenersContainer
-from crypto_screening.market.screeners.callbacks.base import BaseCallback
-from crypto_screening.market.screeners.recorder import (
+from crypto_screening.screeners.container import ScreenersContainer
+from crypto_screening.screeners.callbacks.base import BaseCallback
+from crypto_screening.screeners.recorder import (
     MarketScreener, MarketRecorder, MarketHandler
 )
 
 __all__ = [
     "CombinedMarketRecorder",
     "CombinedMarketScreener",
     "combined_market_screener",
@@ -117,15 +117,15 @@
     the data fetched by the handler.
 
     Parameters:
 
     - recorders:
         The Recorder objects to contron and collect data from, into the markets.
 
-    >>> from crypto_screening.market.screeners import CombinedMarketRecorder
+    >>> from crypto_screening.screeners.combined import CombinedMarketRecorder
     >>>
     >>> recorder = CombinedMarketRecorder(...)
     """
 
     def __init__(self, recorders: Iterable[MarketRecorder]) -> None:
         """
         Defines the class attributes.
@@ -240,15 +240,15 @@
 
     - amount:
         The amount of symbols for each symbols group for an exchange.
 
     - limited:
         The value to limit the running screeners to active exchanges.
 
-    >>> from crypto_screening.market.screeners import combined_market_screener
+    >>> from crypto_screening.screeners.combined import combined_market_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> screener = combined_market_screener(data=structure)
     >>> screener.run()
     """
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/container.py` & `crypto-screening-8.2.0/crypto_screening/screeners/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # container.py
 
-from typing import List, Optional
+from typing import Optional, List
 
-from crypto_screening.market.screeners.ohlcv import OHLCVScreener
-from crypto_screening.market.screeners.orderbook import OrderbookScreener
-from crypto_screening.market.screeners.trades import TradesScreener
-from crypto_screening.market.screeners.orders import OrdersScreener
-from crypto_screening.market.screeners.base import (
+from crypto_screening.screeners.ohlcv import OHLCVScreener
+from crypto_screening.screeners.orderbook import OrderbookScreener
+from crypto_screening.screeners.trades import TradesScreener
+from crypto_screening.screeners.orders import OrdersScreener
+from crypto_screening.screeners.base import (
     BaseFrozenScreenersContainer, BaseScreenersContainer
 )
 
 __all__ = [
     "FrozenScreenersContainer",
     "ScreenersContainer"
 ]
@@ -22,16 +22,16 @@
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
         The screener objects to form a market.
 
-    >>> from crypto_screening.market.screeners.container import FrozenScreenersContainer
-    >>> from crypto_screening.market.screeners.base import BaseScreener
+    >>> from crypto_screening.screeners.container import FrozenScreenersContainer
+    >>> from crypto_screening.screeners import BaseScreener
     >>>
     >>> container = FrozenScreenersContainer(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     """
 
     @property
@@ -350,15 +350,15 @@
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
         The screener objects to form a market.
 
-    >>> from crypto_screening.market.screeners.container import ScreenersContainer
-    >>> from crypto_screening.market.screeners.base import BaseScreener
+    >>> from crypto_screening.screeners.container import ScreenersContainer
+    >>> from crypto_screening.screeners import BaseScreener
     >>>
     >>> container = ScreenersContainer(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     """
 # end ScreenersContainer
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/database.py` & `crypto-screening-8.2.0/crypto_screening/screeners/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from multithreading import Caller, multi_threaded_call
 
 from crypto_screening.dataset import DATE_TIME
 from crypto_screening.symbols import (
     symbol_to_parts, adjust_symbol, parts_to_symbol
 )
-from crypto_screening.market.screeners.base import BaseScreener
+from crypto_screening.screeners.base import BaseScreener
 
 __all__ = [
     "insert_database_record",
     "extract_database_record",
     "validate_database_engines",
     "parts_to_database_table_name",
     "database_table_name_to_parts",
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-8.2.0/crypto_screening/screeners/ohlcv.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 from crypto_screening.interval import interval_to_total_time
 from crypto_screening.dataset import (
     OHLCV_COLUMNS, bid_ask_to_ohlcv,
     load_dataset, save_dataset, create_dataset
 )
 from crypto_screening.validate import validate_interval
 from crypto_screening.symbols import adjust_symbol
-from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.callbacks.base import (
+from crypto_screening.screeners.base import BaseScreener
+from crypto_screening.screeners.callbacks.base import (
     BaseCallback, callback_data
 )
-from crypto_screening.market.screeners.recorder import (
+from crypto_screening.screeners.recorder import (
     MarketScreener, MarketRecorder, MarketHandler
 )
-from crypto_screening.market.screeners.orderbook import (
+from crypto_screening.screeners.orderbook import (
     OrderbookScreener, record_orderbook, create_orderbook_screeners
 )
 
 __all__ = [
     "OHLCVMarketScreener",
     "OHLCVMarketRecorder",
     "OHLCVScreener",
@@ -390,15 +390,15 @@
 
     - screeners:
         The screeners to record data into their market datasets.
 
     - callbacks:
         The callbacks to run when collecting new data.
 
-    >>> from crypto_screening.market.screeners import OHLCVMarketRecorder
+    >>> from crypto_screening.screeners.ohlcv import OHLCVMarketRecorder
     >>>
     >>> recorder = OHLCVMarketRecorder(...)
     """
 
     COLUMNS = OHLCVScreener.COLUMNS
 
     def __init__(
@@ -525,15 +525,15 @@
 
     - amount:
         The amount of symbols for each symbols group for an exchange.
 
     - limited:
         The value to limit the running screeners to active exchanges.
 
-    >>> from crypto_screening.market.screeners import ohlcv_market_screener
+    >>> from crypto_screening.screeners.ohlcv import ohlcv_market_screener
     >>>
     >>> structure = {'1m': {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}}
     >>>
     >>> screener = ohlcv_market_screener(data=structure)
     >>> screener.run()
     """
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-8.2.0/crypto_screening/screeners/orderbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from cryptofeed.types import OrderBook
 from cryptofeed.defines import L2_BOOK
 
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.dataset import (
     BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, create_dataset, ORDERBOOK_COLUMNS
 )
-from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.callbacks import (
+from crypto_screening.screeners.base import BaseScreener
+from crypto_screening.screeners.callbacks import (
     BaseCallback, callback_data
 )
-from crypto_screening.market.screeners.recorder import (
+from crypto_screening.screeners.recorder import (
     MarketScreener, MarketRecorder, MarketHandler
 )
 
 __all__ = [
     "OrderbookMarketScreener",
     "OrderbookMarketRecorder",
     "OrderbookScreener",
@@ -166,15 +166,15 @@
 
     - screeners:
         The screeners to record data into their market datasets.
 
     - callbacks:
         The callbacks to run when collecting new data.
 
-    >>> from crypto_screening.market.screeners import OrderbookMarketRecorder
+    >>> from crypto_screening.screeners.orderbook import OrderbookMarketRecorder
     >>>
     >>> recorder = OrderbookMarketRecorder(...)
     """
 
     COLUMNS = OrderbookScreener.COLUMNS
 
     @property
@@ -254,15 +254,15 @@
 
     - amount:
         The amount of symbols for each symbols group for an exchange.
 
     - limited:
         The value to limit the running screeners to active exchanges.
 
-    >>> from crypto_screening.market.screeners import orderbook_market_screener
+    >>> from crypto_screening.screeners.orderbook import orderbook_market_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> screener = orderbook_market_screener(data=structure)
     >>> screener.run()
     """
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/orders.py` & `crypto-screening-8.2.0/crypto_screening/screeners/orders.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from cryptofeed.types import Ticker
 from cryptofeed.defines import TICKER
 
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.dataset import (
     BIDS, ASKS, ORDERS_COLUMNS, create_dataset
 )
-from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.callbacks import (
+from crypto_screening.screeners.base import BaseScreener
+from crypto_screening.screeners.callbacks import (
     BaseCallback, callback_data
 )
-from crypto_screening.market.screeners.recorder import (
+from crypto_screening.screeners.recorder import (
     MarketScreener, MarketRecorder, MarketHandler
 )
 __all__ = [
     "OrdersMarketScreener",
     "OrdersMarketRecorder",
     "OrdersScreener",
     "orders_market_screener",
@@ -160,15 +160,15 @@
 
     - screeners:
         The screeners to record data into their market datasets.
 
     - callbacks:
         The callbacks to run when collecting new data.
 
-    >>> from crypto_screening.market.screeners import OrdersMarketRecorder
+    >>> from crypto_screening.screeners.orders import OrdersMarketRecorder
     >>>
     >>> recorder = OrdersMarketRecorder(...)
     """
 
     COLUMNS = OrdersScreener.COLUMNS
 
     @property
@@ -248,15 +248,15 @@
 
     - amount:
         The amount of symbols for each symbols group for an exchange.
 
     - limited:
         The value to limit the running screeners to active exchanges.
 
-    >>> from crypto_screening.market.screeners import orders_market_screener
+    >>> from crypto_screening.screeners.orders import orders_market_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> screener = orders_market_screener(data=structure)
     >>> screener.run()
     """
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/recorder.py` & `crypto-screening-8.2.0/crypto_screening/screeners/recorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 from cryptofeed import FeedHandler
 from cryptofeed.feed import Feed
 
 from crypto_screening.utils.process import find_string_value
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.symbols import adjust_symbol
-from crypto_screening.market.screeners.base import (
+from crypto_screening.screeners.base import (
     BaseMarketScreener, BaseScreener, BaseScreenersContainer
 )
-from crypto_screening.market.screeners.callbacks.base import BaseCallback
+from crypto_screening.screeners.callbacks.base import BaseCallback
 
 __all__ = [
     "MarketHandler",
     "ExchangeFeed",
     "FEED_GROUP_SIZE",
     "add_feeds",
     "MarketScreener",
@@ -154,15 +154,15 @@
 
     - screeners:
         The screeners to record data into their market datasets.
 
     - callbacks:
         The callbacks to run when collecting new data.
 
-    >>> from crypto_screening.market.screeners.recorder import MarketRecorder
+    >>> from crypto_screening.screeners.recorder import MarketRecorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = MarketRecorder(data=market)
 
     """
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/screeners/trades.py` & `crypto-screening-8.2.0/crypto_screening/screeners/trades.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from cryptofeed.types import Trade
 from cryptofeed.defines import TRADES
 
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.dataset import (
     TRADES_COLUMNS, create_dataset, AMOUNT, PRICE, SIDE
 )
-from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.callbacks import BaseCallback, callback_data
-from crypto_screening.market.screeners.recorder import (
+from crypto_screening.screeners.base import BaseScreener
+from crypto_screening.screeners.callbacks import BaseCallback, callback_data
+from crypto_screening.screeners.recorder import (
     MarketScreener, MarketRecorder, MarketHandler
 )
 
 __all__ = [
     "TradesMarketScreener",
     "TradesMarketRecorder",
     "TradesScreener",
@@ -160,15 +160,15 @@
 
     - screeners:
         The screeners to record data into their market datasets.
 
     - callbacks:
         The callbacks to run when collecting new data.
 
-    >>> from crypto_screening.market.screeners import TradesMarketRecorder
+    >>> from crypto_screening.screeners.trades import TradesMarketRecorder
     >>>
     >>> recorder = TradesMarketRecorder(...)
     """
 
     COLUMNS = TradesScreener.COLUMNS
 
     @property
@@ -250,15 +250,15 @@
 
     - amount:
         The amount of symbols for each symbols group for an exchange.
 
     - limited:
         The value to limit the running screeners to active exchanges.
 
-    >>> from crypto_screening.market.screeners import trades_market_screener
+    >>> from crypto_screening.screeners.trades import trades_market_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> screener = trades_market_screener(data=structure)
     >>> screener.run()
     """
```

### Comparing `crypto-screening-8.1.3/crypto_screening/market/waiting.py` & `crypto-screening-8.2.0/crypto_screening/screeners/waiting.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import datetime as dt
 from typing import (
     Optional, Union, Iterable
 )
 
 from crypto_screening.collect.screeners import gather_screeners
-from crypto_screening.market.screeners import BaseScreener, BaseMarketScreener
-from crypto_screening.market.foundation.state import WaitingState
-from crypto_screening.market.foundation.waiting import (
+from crypto_screening.screeners import BaseScreener, BaseMarketScreener
+from crypto_screening.screeners.foundation.state import WaitingState
+from crypto_screening.screeners.foundation.waiting import (
     base_await_update, base_await_dynamic_initialization,
     base_await_initialization, base_await_dynamic_update
 )
 
 __all__ = [
     "await_dynamic_initialization",
     "await_update",
```

### Comparing `crypto-screening-8.1.3/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.2.0/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/symbols.py` & `crypto-screening-8.2.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/utils/base.py` & `crypto-screening-8.2.0/crypto_screening/utils/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/utils/process.py` & `crypto-screening-8.2.0/crypto_screening/utils/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening/validate.py` & `crypto-screening-8.2.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.1.3/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.2.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.1.3
+Version: 8.2.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.1.3/pyproject.toml` & `crypto-screening-8.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.1.3'
+version = '8.2.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.1.3/setup.py` & `crypto-screening-8.2.0/setup.py`

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
-        version='8.1.3',
+        version='8.2.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

