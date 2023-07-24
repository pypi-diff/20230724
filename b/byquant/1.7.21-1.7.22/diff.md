# Comparing `tmp/byquant-1.7.21.tar.gz` & `tmp/byquant-1.7.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byquant-1.7.21.tar", last modified: Mon Jul 24 03:06:38 2023, max compression
+gzip compressed data, was "byquant-1.7.22.tar", last modified: Mon Jul 24 03:23:33 2023, max compression
```

## Comparing `byquant-1.7.21.tar` & `byquant-1.7.22.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 03:06:38.530334 byquant-1.7.21/
--rw-rw-rw-   0        0        0     1484 2023-07-24 03:06:38.529333 byquant-1.7.21/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.7.21/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 03:06:37.564225 byquant-1.7.21/byquant/
--rw-rw-rw-   0        0        0    21865 2023-06-30 01:20:38.000000 byquant-1.7.21/byquant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 03:06:37.711830 byquant-1.7.21/byquant/crypto/
--rw-rw-rw-   0        0        0       63 2023-06-27 01:17:34.000000 byquant-1.7.21/byquant/crypto/__init__.py
--rw-rw-rw-   0        0        0    17167 2023-06-27 01:17:45.000000 byquant-1.7.21/byquant/crypto/broker.py
--rw-rw-rw-   0        0        0     8092 2023-06-27 01:17:57.000000 byquant-1.7.21/byquant/crypto/feed.py
--rw-rw-rw-   0        0        0     7942 2021-09-04 05:54:05.000000 byquant-1.7.21/byquant/crypto/store.py
-drwxrwxrwx   0        0        0        0 2023-07-24 03:06:37.724795 byquant-1.7.21/byquant/data/
--rw-rw-rw-   0        0        0      225 2023-07-24 02:18:22.000000 byquant-1.7.21/byquant/data/__init__.py
--rw-rw-rw-   0        0        0    25574 2023-07-24 03:05:56.000000 byquant-1.7.21/byquant/data/get.py
-drwxrwxrwx   0        0        0        0 2023-07-24 03:06:38.515405 byquant-1.7.21/byquant/exchange/
--rw-rw-rw-   0        0        0        0 2023-05-16 08:03:11.000000 byquant-1.7.21/byquant/exchange/__init__.py
--rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.7.21/byquant/exchange/ace.py
--rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/alpaca.py
--rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/ascendex.py
--rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bequant.py
--rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bigone.py
--rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/binance.py
--rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/binancecoinm.py
--rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/binanceus.py
--rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/binanceusdm.py
--rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bit2c.py
--rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitbank.py
--rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitbay.py
--rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitbns.py
--rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitcoincom.py
--rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitfinex.py
--rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitfinex2.py
--rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitflyer.py
--rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitforex.py
--rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitget.py
--rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bithumb.py
--rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitmart.py
--rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitmex.py
--rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitopro.py
--rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitpanda.py
--rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitrue.py
--rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitso.py
--rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitstamp.py
--rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitstamp1.py
--rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bittrex.py
--rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bitvavo.py
--rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bkex.py
--rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bl3p.py
--rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/blockchaincom.py
--rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/btcalpha.py
--rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/btcbox.py
--rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/btcex.py
--rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/btcmarkets.py
--rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/btctradeua.py
--rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/btcturk.py
--rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/buda.py
--rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/bybit.py
--rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/cex.py
--rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/coinbase.py
--rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/coinbaseprime.py
--rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/coinbasepro.py
--rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/coincheck.py
--rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/coinex.py
--rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/coinfalcon.py
--rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/coinmate.py
--rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/coinone.py
--rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/coinsph.py
--rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/coinspot.py
--rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/cryptocom.py
--rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/currencycom.py
--rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/delta.py
--rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/deribit.py
--rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/digifinex.py
--rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/exmo.py
--rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/flowbtc.py
--rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/fmfwio.py
--rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/gate.py
--rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/gateio.py
--rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/gemini.py
--rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/hitbtc.py
--rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/hitbtc3.py
--rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/hollaex.py
--rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/huobi.py
--rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/huobijp.py
--rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/huobipro.py
--rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/idex.py
--rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/independentreserve.py
--rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/indodax.py
--rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/itbit.py
--rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/kraken.py
--rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/krakenfutures.py
--rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/kucoin.py
--rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/kucoinfutures.py
--rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/kuna.py
--rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/latoken.py
--rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/lbank.py
--rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/lbank2.py
--rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/luno.py
--rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/lykke.py
--rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/mercado.py
--rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/mexc.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/mexc3.py
--rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/ndax.py
--rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/novadax.py
--rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/oceanex.py
--rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/okcoin.py
--rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/okex.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/okex5.py
--rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.7.21/byquant/exchange/okx.py
--rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/paymium.py
--rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/phemex.py
--rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/poloniex.py
--rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/poloniexfutures.py
--rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/probit.py
--rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/ripio.py
--rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/stex.py
--rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/tidex.py
--rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/timex.py
--rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/tokocrypto.py
--rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/upbit.py
--rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/wavesexchange.py
--rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/wazirx.py
--rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/whitebit.py
--rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/woo.py
--rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/xt.py
--rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/yobit.py
--rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/zaif.py
--rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/zb.py
--rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.7.21/byquant/exchange/zonda.py
-drwxrwxrwx   0        0        0        0 2023-07-24 03:06:38.526094 byquant-1.7.21/byquant/tool/
--rw-rw-rw-   0        0        0        0 2023-06-27 01:25:40.000000 byquant-1.7.21/byquant/tool/__init__.py
--rw-rw-rw-   0        0        0     3427 2023-02-15 05:30:28.000000 byquant-1.7.21/byquant/tool/tawPlus.py
-drwxrwxrwx   0        0        0        0 2023-07-24 03:06:37.674928 byquant-1.7.21/byquant.egg-info/
--rw-rw-rw-   0        0        0     1484 2023-07-24 03:06:37.000000 byquant-1.7.21/byquant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3606 2023-07-24 03:06:37.000000 byquant-1.7.21/byquant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 03:06:37.000000 byquant-1.7.21/byquant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-07-24 03:06:37.000000 byquant-1.7.21/byquant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-24 03:06:37.000000 byquant-1.7.21/byquant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.7.21/byquant.egg-info/zip-safe
--rw-rw-rw-   0        0        0      190 2023-07-24 03:06:06.000000 byquant-1.7.21/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 03:06:38.531332 byquant-1.7.21/setup.cfg
--rw-rw-rw-   0        0        0     2913 2023-07-24 03:06:10.000000 byquant-1.7.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 03:23:33.680846 byquant-1.7.22/
+-rw-rw-rw-   0        0        0     1484 2023-07-24 03:23:33.678851 byquant-1.7.22/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.7.22/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 03:23:32.870884 byquant-1.7.22/byquant/
+-rw-rw-rw-   0        0        0    21865 2023-06-30 01:20:38.000000 byquant-1.7.22/byquant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 03:23:32.912773 byquant-1.7.22/byquant/crypto/
+-rw-rw-rw-   0        0        0       63 2023-06-27 01:17:34.000000 byquant-1.7.22/byquant/crypto/__init__.py
+-rw-rw-rw-   0        0        0    17167 2023-06-27 01:17:45.000000 byquant-1.7.22/byquant/crypto/broker.py
+-rw-rw-rw-   0        0        0     8092 2023-06-27 01:17:57.000000 byquant-1.7.22/byquant/crypto/feed.py
+-rw-rw-rw-   0        0        0     7942 2021-09-04 05:54:05.000000 byquant-1.7.22/byquant/crypto/store.py
+drwxrwxrwx   0        0        0        0 2023-07-24 03:23:32.922746 byquant-1.7.22/byquant/data/
+-rw-rw-rw-   0        0        0      225 2023-07-24 03:15:51.000000 byquant-1.7.22/byquant/data/__init__.py
+-rw-rw-rw-   0        0        0    25709 2023-07-24 03:22:38.000000 byquant-1.7.22/byquant/data/get.py
+drwxrwxrwx   0        0        0        0 2023-07-24 03:23:33.665891 byquant-1.7.22/byquant/exchange/
+-rw-rw-rw-   0        0        0        0 2023-05-16 08:03:11.000000 byquant-1.7.22/byquant/exchange/__init__.py
+-rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.7.22/byquant/exchange/ace.py
+-rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/alpaca.py
+-rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/ascendex.py
+-rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bequant.py
+-rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bigone.py
+-rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/binance.py
+-rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/binancecoinm.py
+-rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/binanceus.py
+-rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/binanceusdm.py
+-rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bit2c.py
+-rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitbank.py
+-rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitbay.py
+-rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitbns.py
+-rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitcoincom.py
+-rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitfinex.py
+-rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitfinex2.py
+-rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitflyer.py
+-rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitforex.py
+-rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitget.py
+-rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bithumb.py
+-rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitmart.py
+-rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitmex.py
+-rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitopro.py
+-rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitpanda.py
+-rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitrue.py
+-rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitso.py
+-rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitstamp.py
+-rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitstamp1.py
+-rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bittrex.py
+-rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bitvavo.py
+-rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bkex.py
+-rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bl3p.py
+-rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/blockchaincom.py
+-rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/btcalpha.py
+-rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/btcbox.py
+-rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/btcex.py
+-rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/btcmarkets.py
+-rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/btctradeua.py
+-rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/btcturk.py
+-rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/buda.py
+-rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/bybit.py
+-rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/cex.py
+-rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/coinbase.py
+-rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/coinbaseprime.py
+-rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/coinbasepro.py
+-rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/coincheck.py
+-rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/coinex.py
+-rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/coinfalcon.py
+-rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/coinmate.py
+-rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/coinone.py
+-rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/coinsph.py
+-rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/coinspot.py
+-rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/cryptocom.py
+-rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/currencycom.py
+-rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/delta.py
+-rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/deribit.py
+-rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/digifinex.py
+-rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/exmo.py
+-rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/flowbtc.py
+-rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/fmfwio.py
+-rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/gate.py
+-rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/gateio.py
+-rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/gemini.py
+-rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/hitbtc.py
+-rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/hitbtc3.py
+-rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/hollaex.py
+-rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/huobi.py
+-rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/huobijp.py
+-rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/huobipro.py
+-rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/idex.py
+-rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/independentreserve.py
+-rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/indodax.py
+-rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/itbit.py
+-rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/kraken.py
+-rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/krakenfutures.py
+-rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/kucoin.py
+-rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/kucoinfutures.py
+-rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/kuna.py
+-rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/latoken.py
+-rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/lbank.py
+-rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/lbank2.py
+-rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/luno.py
+-rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/lykke.py
+-rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/mercado.py
+-rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/mexc.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/mexc3.py
+-rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/ndax.py
+-rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/novadax.py
+-rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/oceanex.py
+-rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/okcoin.py
+-rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/okex.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/okex5.py
+-rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.7.22/byquant/exchange/okx.py
+-rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/paymium.py
+-rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/phemex.py
+-rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/poloniex.py
+-rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/poloniexfutures.py
+-rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/probit.py
+-rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/ripio.py
+-rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/stex.py
+-rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/tidex.py
+-rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/timex.py
+-rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/tokocrypto.py
+-rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/upbit.py
+-rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/wavesexchange.py
+-rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/wazirx.py
+-rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/whitebit.py
+-rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/woo.py
+-rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/xt.py
+-rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/yobit.py
+-rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/zaif.py
+-rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/zb.py
+-rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.7.22/byquant/exchange/zonda.py
+drwxrwxrwx   0        0        0        0 2023-07-24 03:23:33.675861 byquant-1.7.22/byquant/tool/
+-rw-rw-rw-   0        0        0        0 2023-06-27 01:25:40.000000 byquant-1.7.22/byquant/tool/__init__.py
+-rw-rw-rw-   0        0        0     3427 2023-02-15 05:30:28.000000 byquant-1.7.22/byquant/tool/tawPlus.py
+drwxrwxrwx   0        0        0        0 2023-07-24 03:23:32.896815 byquant-1.7.22/byquant.egg-info/
+-rw-rw-rw-   0        0        0     1484 2023-07-24 03:23:32.000000 byquant-1.7.22/byquant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3606 2023-07-24 03:23:32.000000 byquant-1.7.22/byquant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 03:23:32.000000 byquant-1.7.22/byquant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-07-24 03:23:32.000000 byquant-1.7.22/byquant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-24 03:23:32.000000 byquant-1.7.22/byquant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.7.22/byquant.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      190 2023-07-24 03:22:58.000000 byquant-1.7.22/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 03:23:33.680846 byquant-1.7.22/setup.cfg
+-rw-rw-rw-   0        0        0     2913 2023-07-24 03:22:54.000000 byquant-1.7.22/setup.py
```

### Comparing `byquant-1.7.21/PKG-INFO` & `byquant-1.7.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.7.21
+Version: 1.7.22
 Summary: ByQuant.com is a Artificial Intelligence Quantitative Investment Trading Competition Learning Community
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
 License: MIT
 Project-URL: Homepage, https://byquant.com
 Keywords: quant,strategy,algorithmic,algotrading
```

### Comparing `byquant-1.7.21/byquant/__init__.py` & `byquant-1.7.22/byquant/__init__.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/crypto/broker.py` & `byquant-1.7.22/byquant/crypto/broker.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/crypto/feed.py` & `byquant-1.7.22/byquant/crypto/feed.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/crypto/store.py` & `byquant-1.7.22/byquant/crypto/store.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/data/get.py` & `byquant-1.7.22/byquant/data/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,18 @@
         self.freq = freq
         self.tawtime = tawtime
         self.renew = renew
         self.haskey = 'no'
         self.exchange = self.symbol.split('.')[-1]
         self.underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange, '')
         self.MARKET_DATA_PATH = '~/temp/%s/' % (self.ktype)
+        if not os.path.isdir('~/temp/'):
+            os.makedirs('~/temp/')
+            if not os.path.isdir(self.MARKET_DATA_PATH):
+                os.makedirs(self.MARKET_DATA_PATH)
         self.tushareKey = 'Your  API  Token'
         self.filepath = self.MARKET_DATA_PATH + '%s/%s/%s.csv' % (self.exchange, self.freq, self.symbol.replace('.' + self.exchange, ''))
 
         self.underlying_ex = self.underlying
         if self.exchange == 'SSE':
             self.underlying_ex = self.underlying_ex.replace('SH', '') + '.SH'
         elif self.exchange == 'SZSE':
@@ -512,15 +516,15 @@
     def alpacaStockApi(self):
         df = {}
         try:
             # underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange.upper(), '')
             # print([freq])
             # toDay = date.today()
             # toDay = format(toDay.strftime('%Y-%m-%d'))
-            client = StockHistoricalDataClient("PKCUWHUG8005XUTOYLZM", "BHWJiwEp4WW0VXBwqkEHL3cgJ4xWKrm1CsbuGlcD")
+            client = StockHistoricalDataClient("KEY", "KEYI")
             # strFreq = freq
             if self.freq == '1m':
                 # strFreq = '1m'
                 startTime = (date.today() + timedelta(days=-7)).strftime("%Y-%m-%d %H:%M:%S")
                 request_params = StockBarsRequest(
                     symbol_or_symbols=[self.underlying],
                     timeframe=TimeFrame.Minute,
```

### Comparing `byquant-1.7.21/byquant/exchange/ace.py` & `byquant-1.7.22/byquant/exchange/ace.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/alpaca.py` & `byquant-1.7.22/byquant/exchange/alpaca.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/ascendex.py` & `byquant-1.7.22/byquant/exchange/ascendex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bequant.py` & `byquant-1.7.22/byquant/exchange/bequant.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bigone.py` & `byquant-1.7.22/byquant/exchange/bigone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/binance.py` & `byquant-1.7.22/byquant/exchange/binance.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/binancecoinm.py` & `byquant-1.7.22/byquant/exchange/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/binanceus.py` & `byquant-1.7.22/byquant/exchange/binanceus.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/binanceusdm.py` & `byquant-1.7.22/byquant/exchange/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bit2c.py` & `byquant-1.7.22/byquant/exchange/bit2c.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitbank.py` & `byquant-1.7.22/byquant/exchange/bitbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitbns.py` & `byquant-1.7.22/byquant/exchange/bitbns.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitfinex.py` & `byquant-1.7.22/byquant/exchange/bitfinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitfinex2.py` & `byquant-1.7.22/byquant/exchange/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitflyer.py` & `byquant-1.7.22/byquant/exchange/bitflyer.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitforex.py` & `byquant-1.7.22/byquant/exchange/bitforex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitget.py` & `byquant-1.7.22/byquant/exchange/bitget.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bithumb.py` & `byquant-1.7.22/byquant/exchange/bithumb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitmart.py` & `byquant-1.7.22/byquant/exchange/bitmart.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitmex.py` & `byquant-1.7.22/byquant/exchange/bitmex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitopro.py` & `byquant-1.7.22/byquant/exchange/bitopro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitpanda.py` & `byquant-1.7.22/byquant/exchange/bitpanda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitrue.py` & `byquant-1.7.22/byquant/exchange/bitrue.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitso.py` & `byquant-1.7.22/byquant/exchange/bitso.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitstamp.py` & `byquant-1.7.22/byquant/exchange/bitstamp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitstamp1.py` & `byquant-1.7.22/byquant/exchange/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bittrex.py` & `byquant-1.7.22/byquant/exchange/bittrex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bitvavo.py` & `byquant-1.7.22/byquant/exchange/bitvavo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bkex.py` & `byquant-1.7.22/byquant/exchange/bkex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bl3p.py` & `byquant-1.7.22/byquant/exchange/bl3p.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/blockchaincom.py` & `byquant-1.7.22/byquant/exchange/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/btcalpha.py` & `byquant-1.7.22/byquant/exchange/btcalpha.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/btcbox.py` & `byquant-1.7.22/byquant/exchange/btcbox.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/btcex.py` & `byquant-1.7.22/byquant/exchange/btcex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/btcmarkets.py` & `byquant-1.7.22/byquant/exchange/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/btctradeua.py` & `byquant-1.7.22/byquant/exchange/btctradeua.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/btcturk.py` & `byquant-1.7.22/byquant/exchange/btcturk.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/buda.py` & `byquant-1.7.22/byquant/exchange/buda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/bybit.py` & `byquant-1.7.22/byquant/exchange/bybit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/cex.py` & `byquant-1.7.22/byquant/exchange/cex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/coinbase.py` & `byquant-1.7.22/byquant/exchange/coinbase.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/coinbaseprime.py` & `byquant-1.7.22/byquant/exchange/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/coinbasepro.py` & `byquant-1.7.22/byquant/exchange/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/coincheck.py` & `byquant-1.7.22/byquant/exchange/coincheck.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/coinex.py` & `byquant-1.7.22/byquant/exchange/coinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/coinfalcon.py` & `byquant-1.7.22/byquant/exchange/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/coinmate.py` & `byquant-1.7.22/byquant/exchange/coinmate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/coinone.py` & `byquant-1.7.22/byquant/exchange/coinone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/coinsph.py` & `byquant-1.7.22/byquant/exchange/coinsph.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/coinspot.py` & `byquant-1.7.22/byquant/exchange/coinspot.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/cryptocom.py` & `byquant-1.7.22/byquant/exchange/cryptocom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/currencycom.py` & `byquant-1.7.22/byquant/exchange/currencycom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/delta.py` & `byquant-1.7.22/byquant/exchange/delta.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/deribit.py` & `byquant-1.7.22/byquant/exchange/deribit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/digifinex.py` & `byquant-1.7.22/byquant/exchange/digifinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/exmo.py` & `byquant-1.7.22/byquant/exchange/exmo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/flowbtc.py` & `byquant-1.7.22/byquant/exchange/flowbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/fmfwio.py` & `byquant-1.7.22/byquant/exchange/fmfwio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/gate.py` & `byquant-1.7.22/byquant/exchange/gate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/gemini.py` & `byquant-1.7.22/byquant/exchange/gemini.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/hitbtc.py` & `byquant-1.7.22/byquant/exchange/hitbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/hitbtc3.py` & `byquant-1.7.22/byquant/exchange/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/hollaex.py` & `byquant-1.7.22/byquant/exchange/hollaex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/huobi.py` & `byquant-1.7.22/byquant/exchange/huobi.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/huobijp.py` & `byquant-1.7.22/byquant/exchange/huobijp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/huobipro.py` & `byquant-1.7.22/byquant/exchange/huobipro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/idex.py` & `byquant-1.7.22/byquant/exchange/idex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/independentreserve.py` & `byquant-1.7.22/byquant/exchange/independentreserve.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/indodax.py` & `byquant-1.7.22/byquant/exchange/indodax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/itbit.py` & `byquant-1.7.22/byquant/exchange/itbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/kraken.py` & `byquant-1.7.22/byquant/exchange/kraken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/krakenfutures.py` & `byquant-1.7.22/byquant/exchange/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/kucoin.py` & `byquant-1.7.22/byquant/exchange/kucoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/kucoinfutures.py` & `byquant-1.7.22/byquant/exchange/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/kuna.py` & `byquant-1.7.22/byquant/exchange/kuna.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/latoken.py` & `byquant-1.7.22/byquant/exchange/latoken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/lbank.py` & `byquant-1.7.22/byquant/exchange/lbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/lbank2.py` & `byquant-1.7.22/byquant/exchange/lbank2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/luno.py` & `byquant-1.7.22/byquant/exchange/luno.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/lykke.py` & `byquant-1.7.22/byquant/exchange/lykke.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/mercado.py` & `byquant-1.7.22/byquant/exchange/mercado.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/mexc.py` & `byquant-1.7.22/byquant/exchange/mexc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/ndax.py` & `byquant-1.7.22/byquant/exchange/ndax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/novadax.py` & `byquant-1.7.22/byquant/exchange/novadax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/oceanex.py` & `byquant-1.7.22/byquant/exchange/oceanex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/okcoin.py` & `byquant-1.7.22/byquant/exchange/okcoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/okx.py` & `byquant-1.7.22/byquant/exchange/okx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/paymium.py` & `byquant-1.7.22/byquant/exchange/paymium.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/phemex.py` & `byquant-1.7.22/byquant/exchange/phemex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/poloniex.py` & `byquant-1.7.22/byquant/exchange/poloniex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/poloniexfutures.py` & `byquant-1.7.22/byquant/exchange/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/probit.py` & `byquant-1.7.22/byquant/exchange/probit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/ripio.py` & `byquant-1.7.22/byquant/exchange/ripio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/stex.py` & `byquant-1.7.22/byquant/exchange/stex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/tidex.py` & `byquant-1.7.22/byquant/exchange/tidex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/timex.py` & `byquant-1.7.22/byquant/exchange/timex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/tokocrypto.py` & `byquant-1.7.22/byquant/exchange/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/upbit.py` & `byquant-1.7.22/byquant/exchange/upbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/wavesexchange.py` & `byquant-1.7.22/byquant/exchange/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/wazirx.py` & `byquant-1.7.22/byquant/exchange/wazirx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/whitebit.py` & `byquant-1.7.22/byquant/exchange/whitebit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/woo.py` & `byquant-1.7.22/byquant/exchange/woo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/xt.py` & `byquant-1.7.22/byquant/exchange/xt.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/yobit.py` & `byquant-1.7.22/byquant/exchange/yobit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/zaif.py` & `byquant-1.7.22/byquant/exchange/zaif.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/zb.py` & `byquant-1.7.22/byquant/exchange/zb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/exchange/zonda.py` & `byquant-1.7.22/byquant/exchange/zonda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant/tool/tawPlus.py` & `byquant-1.7.22/byquant/tool/tawPlus.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/byquant.egg-info/PKG-INFO` & `byquant-1.7.22/byquant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.7.21
+Version: 1.7.22
 Summary: ByQuant.com is a Artificial Intelligence Quantitative Investment Trading Competition Learning Community
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
 License: MIT
 Project-URL: Homepage, https://byquant.com
 Keywords: quant,strategy,algorithmic,algotrading
```

### Comparing `byquant-1.7.21/byquant.egg-info/SOURCES.txt` & `byquant-1.7.22/byquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `byquant-1.7.21/setup.py` & `byquant-1.7.22/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 here = path.abspath(path.dirname(__file__))
 root = path.dirname(here)
 
 readme = path.join(here, 'README.md')
 package = {
   "name": "byquant",
-  "version": "1.7.21",
+  "version": "1.7.22",
   "description": "ByQuant.com is a Artificial Intelligence Quantitative Investment Trading Competition Learning Community",
   "type": "module",
   "readme": "README.md",
   "package_json": "package.json",
   "author": {
     "name": "Uakeey",
     "email": "uakee@outlook.com",
```

