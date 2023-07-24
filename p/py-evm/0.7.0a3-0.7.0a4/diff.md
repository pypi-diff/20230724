# Comparing `tmp/py-evm-0.7.0a3.tar.gz` & `tmp/py-evm-0.7.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-evm-0.7.0a3.tar", last modified: Thu Jun  8 20:25:34 2023, max compression
+gzip compressed data, was "py-evm-0.7.0a4.tar", last modified: Mon Jul 24 21:05:51 2023, max compression
```

## Comparing `py-evm-0.7.0a3.tar` & `py-evm-0.7.0a4.tar`

### file list

```diff
@@ -1,337 +1,337 @@
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.271456 py-evm-0.7.0a3/
--rw-r--r--   0 eve        (501) staff       (20)     1095 2023-05-01 17:23:48.000000 py-evm-0.7.0a3/LICENSE
--rw-r--r--   0 eve        (501) staff       (20)      141 2023-05-01 17:23:48.000000 py-evm-0.7.0a3/MANIFEST.in
--rw-r--r--   0 eve        (501) staff       (20)     2977 2023-06-08 20:25:34.271158 py-evm-0.7.0a3/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     2157 2023-05-01 17:23:48.000000 py-evm-0.7.0a3/README.md
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.239643 py-evm-0.7.0a3/eth/
--rw-r--r--   0 eve        (501) staff       (20)      368 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.241667 py-evm-0.7.0a3/eth/_utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      687 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/address.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.242049 py-evm-0.7.0a3/eth/_utils/blake2/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 18:37:56.000000 py-evm-0.7.0a3/eth/_utils/blake2/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1841 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/blake2/coders.py
--rwxr-xr-x   0 eve        (501) staff       (20)     5793 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/blake2/compression.py
--rw-r--r--   0 eve        (501) staff       (20)      980 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/bn128.py
--rw-r--r--   0 eve        (501) staff       (20)     3924 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/datatypes.py
--rw-r--r--   0 eve        (501) staff       (20)     1013 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/db.py
--rw-r--r--   0 eve        (501) staff       (20)       40 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/_utils/empty.py
--rw-r--r--   0 eve        (501) staff       (20)     8124 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/env.py
--rw-r--r--   0 eve        (501) staff       (20)      612 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/generator.py
--rw-r--r--   0 eve        (501) staff       (20)     5024 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/headers.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 18:37:56.000000 py-evm-0.7.0a3/eth/_utils/logging.py
--rw-r--r--   0 eve        (501) staff       (20)     1540 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/module_loading.py
--rw-r--r--   0 eve        (501) staff       (20)     2671 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/numeric.py
--rw-r--r--   0 eve        (501) staff       (20)      337 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/padding.py
--rw-r--r--   0 eve        (501) staff       (20)     3284 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/rlp.py
--rw-r--r--   0 eve        (501) staff       (20)     1749 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/spoof.py
--rw-r--r--   0 eve        (501) staff       (20)     1343 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/state.py
--rw-r--r--   0 eve        (501) staff       (20)     3379 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)      385 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/version.py
--rw-r--r--   0 eve        (501) staff       (20)      364 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_warnings.py
--rw-r--r--   0 eve        (501) staff       (20)   117181 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/abc.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.242397 py-evm-0.7.0a3/eth/chains/
--rw-r--r--   0 eve        (501) staff       (20)      223 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/chains/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    25965 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/base.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.242652 py-evm-0.7.0a3/eth/chains/goerli/
--rw-r--r--   0 eve        (501) staff       (20)     1305 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/goerli/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      270 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/goerli/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     2554 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/header.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.242876 py-evm-0.7.0a3/eth/chains/mainnet/
--rw-r--r--   0 eve        (501) staff       (20)     4409 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/mainnet/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1199 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/mainnet/constants.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.243084 py-evm-0.7.0a3/eth/chains/ropsten/
--rw-r--r--   0 eve        (501) staff       (20)     2131 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/ropsten/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      847 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/ropsten/constants.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.243193 py-evm-0.7.0a3/eth/chains/tester/
--rw-r--r--   0 eve        (501) staff       (20)     5919 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/tester/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.243864 py-evm-0.7.0a3/eth/consensus/
--rw-r--r--   0 eve        (501) staff       (20)      313 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/consensus/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      968 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/applier.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.244690 py-evm-0.7.0a3/eth/consensus/clique/
--rw-r--r--   0 eve        (501) staff       (20)      271 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5208 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)     5383 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/clique.py
--rw-r--r--   0 eve        (501) staff       (20)      486 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     3368 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/datatypes.py
--rw-r--r--   0 eve        (501) staff       (20)     2949 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/encoding.py
--rw-r--r--   0 eve        (501) staff       (20)      158 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)    11157 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/snapshot_manager.py
--rw-r--r--   0 eve        (501) staff       (20)      187 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/context.py
--rw-r--r--   0 eve        (501) staff       (20)      683 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/noproof.py
--rw-r--r--   0 eve        (501) staff       (20)      819 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/pos.py
--rw-r--r--   0 eve        (501) staff       (20)     4024 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/pow.py
--rw-r--r--   0 eve        (501) staff       (20)     3921 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/constants.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.246821 py-evm-0.7.0a3/eth/db/
--rw-r--r--   0 eve        (501) staff       (20)      714 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/db/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3460 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/accesslog.py
--rw-r--r--   0 eve        (501) staff       (20)    24411 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/account.py
--rw-r--r--   0 eve        (501) staff       (20)     4277 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/atomic.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.247220 py-evm-0.7.0a3/eth/db/backends/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/db/backends/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2513 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/backends/base.py
--rw-r--r--   0 eve        (501) staff       (20)     4496 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/backends/level.py
--rw-r--r--   0 eve        (501) staff       (20)      890 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/db/backends/memory.py
--rw-r--r--   0 eve        (501) staff       (20)     2874 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/batch.py
--rw-r--r--   0 eve        (501) staff       (20)      971 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/cache.py
--rw-r--r--   0 eve        (501) staff       (20)    19206 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/db/chain.py
--rw-r--r--   0 eve        (501) staff       (20)     5873 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/chain_gaps.py
--rw-r--r--   0 eve        (501) staff       (20)     7394 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/diff.py
--rw-r--r--   0 eve        (501) staff       (20)      506 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/hash_trie.py
--rw-r--r--   0 eve        (501) staff       (20)    24129 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/header.py
--rw-r--r--   0 eve        (501) staff       (20)    17008 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/journal.py
--rw-r--r--   0 eve        (501) staff       (20)     1306 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/keymap.py
--rw-r--r--   0 eve        (501) staff       (20)     1354 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/schema.py
--rw-r--r--   0 eve        (501) staff       (20)    16562 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/slow_journal.py
--rw-r--r--   0 eve        (501) staff       (20)    16442 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/storage.py
--rw-r--r--   0 eve        (501) staff       (20)     1393 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/trie.py
--rw-r--r--   0 eve        (501) staff       (20)     1660 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/witness.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.247428 py-evm-0.7.0a3/eth/estimators/
--rw-r--r--   0 eve        (501) staff       (20)      514 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/estimators/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3427 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/estimators/gas.py
--rw-r--r--   0 eve        (501) staff       (20)     4115 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/exceptions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.248574 py-evm-0.7.0a3/eth/precompiles/
--rw-r--r--   0 eve        (501) staff       (20)      398 2021-02-26 19:54:17.000000 py-evm-0.7.0a3/eth/precompiles/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      962 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/blake2.py
--rw-r--r--   0 eve        (501) staff       (20)     1502 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/ecadd.py
--rw-r--r--   0 eve        (501) staff       (20)     1390 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/ecmul.py
--rw-r--r--   0 eve        (501) staff       (20)     3257 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/ecpairing.py
--rw-r--r--   0 eve        (501) staff       (20)     1512 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/ecrecover.py
--rw-r--r--   0 eve        (501) staff       (20)      472 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/identity.py
--rw-r--r--   0 eve        (501) staff       (20)     3934 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/modexp.py
--rw-r--r--   0 eve        (501) staff       (20)      670 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/ripemd160.py
--rw-r--r--   0 eve        (501) staff       (20)      541 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/sha256.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/py.typed
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.249432 py-evm-0.7.0a3/eth/rlp/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/rlp/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1022 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/accounts.py
--rw-r--r--   0 eve        (501) staff       (20)      904 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     5417 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      603 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/logs.py
--rw-r--r--   0 eve        (501) staff       (20)     1285 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/receipts.py
--rw-r--r--   0 eve        (501) staff       (20)      387 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/sedes.py
--rw-r--r--   0 eve        (501) staff       (20)     3611 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.249735 py-evm-0.7.0a3/eth/tools/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/tools/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.250875 py-evm-0.7.0a3/eth/tools/_utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/tools/_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      662 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/tools/_utils/deprecation.py
--rw-r--r--   0 eve        (501) staff       (20)      190 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/_utils/git.py
--rw-r--r--   0 eve        (501) staff       (20)      556 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/_utils/hashing.py
--rw-r--r--   0 eve        (501) staff       (20)     1564 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/_utils/mappings.py
--rw-r--r--   0 eve        (501) staff       (20)    18084 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/_utils/normalization.py
--rw-r--r--   0 eve        (501) staff       (20)     4410 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/_utils/slow_code_stream.py
--rw-r--r--   0 eve        (501) staff       (20)      903 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/_utils/vyper.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.250983 py-evm-0.7.0a3/eth/tools/builder/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/tools/builder/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.251175 py-evm-0.7.0a3/eth/tools/builder/chain/
--rw-r--r--   0 eve        (501) staff       (20)     2936 2023-04-28 21:07:47.000000 py-evm-0.7.0a3/eth/tools/builder/chain/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    15254 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/builder/chain/builders.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.251502 py-evm-0.7.0a3/eth/tools/db/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/tools/db/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5191 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/tools/db/atomic.py
--rw-r--r--   0 eve        (501) staff       (20)     2269 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/db/base.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.252087 py-evm-0.7.0a3/eth/tools/fixtures/
--rw-r--r--   0 eve        (501) staff       (20)      615 2021-08-19 20:42:01.000000 py-evm-0.7.0a3/eth/tools/fixtures/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      887 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/_utils.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.252838 py-evm-0.7.0a3/eth/tools/fixtures/fillers/
--rw-r--r--   0 eve        (501) staff       (20)      282 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2456 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)    12716 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/common.py
--rw-r--r--   0 eve        (501) staff       (20)     3461 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/formatters.py
--rw-r--r--   0 eve        (501) staff       (20)     1307 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/main.py
--rw-r--r--   0 eve        (501) staff       (20)     2758 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1737 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/vm.py
--rw-r--r--   0 eve        (501) staff       (20)     2079 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/generation.py
--rw-r--r--   0 eve        (501) staff       (20)     9361 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/helpers.py
--rw-r--r--   0 eve        (501) staff       (20)     3068 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/loading.py
--rw-r--r--   0 eve        (501) staff       (20)      791 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/mining.py
--rw-r--r--   0 eve        (501) staff       (20)      476 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/rlp.py
--rw-r--r--   0 eve        (501) staff       (20)     2693 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/typing.py
--rw-r--r--   0 eve        (501) staff       (20)     8548 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.254784 py-evm-0.7.0a3/eth/vm/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/vm/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    26238 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/base.py
--rw-r--r--   0 eve        (501) staff       (20)      632 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/chain_context.py
--rw-r--r--   0 eve        (501) staff       (20)     4438 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/vm/code_stream.py
--rw-r--r--   0 eve        (501) staff       (20)    19222 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/computation.py
--rw-r--r--   0 eve        (501) staff       (20)     2124 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/execution_context.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.254878 py-evm-0.7.0a3/eth/vm/forks/
--rw-r--r--   0 eve        (501) staff       (20)      899 2023-04-28 21:07:47.000000 py-evm-0.7.0a3/eth/vm/forks/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.255545 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/
--rw-r--r--   0 eve        (501) staff       (20)      856 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      993 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      287 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/computation.py
--rw-r--r--   0 eve        (501) staff       (20)     1084 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      523 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1134 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.256618 py-evm-0.7.0a3/eth/vm/forks/berlin/
--rw-r--r--   0 eve        (501) staff       (20)      772 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      784 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     2441 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      327 2021-08-30 21:22:29.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      374 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     6417 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/logic.py
--rw-r--r--   0 eve        (501) staff       (20)     2922 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)     4606 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/receipts.py
--rw-r--r--   0 eve        (501) staff       (20)     1187 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/state.py
--rw-r--r--   0 eve        (501) staff       (20)    15395 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.257581 py-evm-0.7.0a3/eth/vm/forks/byzantium/
--rw-r--r--   0 eve        (501) staff       (20)     3584 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      485 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     1016 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      235 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     3368 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     3526 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      222 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1231 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.258580 py-evm-0.7.0a3/eth/vm/forks/constantinople/
--rw-r--r--   0 eve        (501) staff       (20)     1106 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      484 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      757 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      329 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      406 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     1574 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      221 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/state.py
--rw-r--r--   0 eve        (501) staff       (20)      334 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/storage.py
--rw-r--r--   0 eve        (501) staff       (20)     1235 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.259676 py-evm-0.7.0a3/eth/vm/forks/frontier/
--rw-r--r--   0 eve        (501) staff       (20)     3732 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3412 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     3715 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/computation.py
--rw-r--r--   0 eve        (501) staff       (20)       96 2021-09-20 20:47:49.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     3529 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/headers.py
--rw-r--r--   0 eve        (501) staff       (20)    20228 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)     7686 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/state.py
--rw-r--r--   0 eve        (501) staff       (20)      140 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/transaction_context.py
--rw-r--r--   0 eve        (501) staff       (20)     5868 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)     1603 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.260335 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/
--rw-r--r--   0 eve        (501) staff       (20)      855 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1068 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      317 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/computation.py
--rw-r--r--   0 eve        (501) staff       (20)     1119 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      556 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1170 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.261524 py-evm-0.7.0a3/eth/vm/forks/homestead/
--rw-r--r--   0 eve        (501) staff       (20)     1250 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      466 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     2289 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/computation.py
--rw-r--r--   0 eve        (501) staff       (20)       61 2021-09-03 20:35:50.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     9656 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      637 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      640 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/state.py
--rw-r--r--   0 eve        (501) staff       (20)     2197 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)      518 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.262617 py-evm-0.7.0a3/eth/vm/forks/istanbul/
--rw-r--r--   0 eve        (501) staff       (20)      817 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      469 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     1421 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      316 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      384 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     1664 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      206 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/state.py
--rw-r--r--   0 eve        (501) staff       (20)      909 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/storage.py
--rw-r--r--   0 eve        (501) staff       (20)     1798 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.263788 py-evm-0.7.0a3/eth/vm/forks/london/
--rw-r--r--   0 eve        (501) staff       (20)     2260 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5828 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      810 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      470 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     5618 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      895 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      629 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/receipts.py
--rw-r--r--   0 eve        (501) staff       (20)     4881 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/state.py
--rw-r--r--   0 eve        (501) staff       (20)      544 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/storage.py
--rw-r--r--   0 eve        (501) staff       (20)     9486 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)      855 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.264476 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/
--rw-r--r--   0 eve        (501) staff       (20)      842 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      472 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      537 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      443 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      137 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      209 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1212 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.265183 py-evm-0.7.0a3/eth/vm/forks/paris/
--rw-r--r--   0 eve        (501) staff       (20)     2117 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1039 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      379 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/computation.py
--rw-r--r--   0 eve        (501) staff       (20)     2284 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      686 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      666 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1121 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.265991 py-evm-0.7.0a3/eth/vm/forks/petersburg/
--rw-r--r--   0 eve        (501) staff       (20)     1036 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      472 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      531 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      110 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      386 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     1399 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      209 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1211 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.267033 py-evm-0.7.0a3/eth/vm/forks/shanghai/
--rw-r--r--   0 eve        (501) staff       (20)      667 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     9048 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     1655 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      196 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      824 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      821 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/logic.py
--rw-r--r--   0 eve        (501) staff       (20)     1531 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      751 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1099 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)     1515 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/withdrawals.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.267886 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/
--rw-r--r--   0 eve        (501) staff       (20)      429 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2145 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)      484 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     3322 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      169 2023-04-28 21:07:47.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     1221 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)     1465 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/state.py
--rw-r--r--   0 eve        (501) staff       (20)     2866 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.268364 py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/
--rw-r--r--   0 eve        (501) staff       (20)      469 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      428 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      225 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     2106 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      227 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/state.py
--rw-r--r--   0 eve        (501) staff       (20)     2626 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/gas_meter.py
--rw-r--r--   0 eve        (501) staff       (20)      540 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/header.py
--rw-r--r--   0 eve        (501) staff       (20)     3425 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/interrupt.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.270147 py-evm-0.7.0a3/eth/vm/logic/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/vm/logic/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     4805 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/arithmetic.py
--rw-r--r--   0 eve        (501) staff       (20)     1113 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/block.py
--rw-r--r--   0 eve        (501) staff       (20)    13394 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/call.py
--rw-r--r--   0 eve        (501) staff       (20)     2824 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/comparison.py
--rw-r--r--   0 eve        (501) staff       (20)     6418 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/context.py
--rw-r--r--   0 eve        (501) staff       (20)      944 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/duplication.py
--rw-r--r--   0 eve        (501) staff       (20)     1508 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/flow.py
--rw-r--r--   0 eve        (501) staff       (20)      507 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/invalid.py
--rw-r--r--   0 eve        (501) staff       (20)     1355 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/logging.py
--rw-r--r--   0 eve        (501) staff       (20)     1102 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/memory.py
--rw-r--r--   0 eve        (501) staff       (20)      640 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/sha3.py
--rw-r--r--   0 eve        (501) staff       (20)     2176 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/stack.py
--rw-r--r--   0 eve        (501) staff       (20)     3939 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/storage.py
--rw-r--r--   0 eve        (501) staff       (20)      974 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/swap.py
--rw-r--r--   0 eve        (501) staff       (20)     9727 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/system.py
--rw-r--r--   0 eve        (501) staff       (20)     2134 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/memory.py
--rw-r--r--   0 eve        (501) staff       (20)     3214 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/message.py
--rw-r--r--   0 eve        (501) staff       (20)     2785 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/mnemonics.py
--rw-r--r--   0 eve        (501) staff       (20)     1864 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/opcode.py
--rw-r--r--   0 eve        (501) staff       (20)     2432 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/opcode_values.py
--rw-r--r--   0 eve        (501) staff       (20)      416 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/spoof.py
--rw-r--r--   0 eve        (501) staff       (20)     7713 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/stack.py
--rw-r--r--   0 eve        (501) staff       (20)    10406 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/state.py
--rw-r--r--   0 eve        (501) staff       (20)      875 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/transaction_context.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.270971 py-evm-0.7.0a3/py_evm.egg-info/
--rw-r--r--   0 eve        (501) staff       (20)     2977 2023-06-08 20:25:31.000000 py-evm-0.7.0a3/py_evm.egg-info/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     8485 2023-06-08 20:25:34.000000 py-evm-0.7.0a3/py_evm.egg-info/SOURCES.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-06-08 20:25:31.000000 py-evm-0.7.0a3/py_evm.egg-info/dependency_links.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2021-02-24 18:15:32.000000 py-evm-0.7.0a3/py_evm.egg-info/not-zip-safe
--rw-r--r--   0 eve        (501) staff       (20)     2144 2023-06-08 20:25:32.000000 py-evm-0.7.0a3/py_evm.egg-info/requires.txt
--rw-r--r--   0 eve        (501) staff       (20)        4 2023-06-08 20:25:32.000000 py-evm-0.7.0a3/py_evm.egg-info/top_level.txt
--rw-r--r--   0 eve        (501) staff       (20)     1117 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/pyproject.toml
--rw-r--r--   0 eve        (501) staff       (20)       38 2023-06-08 20:25:34.271501 py-evm-0.7.0a3/setup.cfg
--rw-r--r--   0 eve        (501) staff       (20)     4043 2023-06-08 20:25:28.000000 py-evm-0.7.0a3/setup.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.135735 py-evm-0.7.0a4/
+-rw-r--r--   0 eve        (501) staff       (20)     1095 2023-05-01 17:23:48.000000 py-evm-0.7.0a4/LICENSE
+-rw-r--r--   0 eve        (501) staff       (20)      141 2023-05-01 17:23:48.000000 py-evm-0.7.0a4/MANIFEST.in
+-rw-r--r--   0 eve        (501) staff       (20)     2997 2023-07-24 21:05:51.135587 py-evm-0.7.0a4/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     2157 2023-05-01 17:23:48.000000 py-evm-0.7.0a4/README.md
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.105367 py-evm-0.7.0a4/eth/
+-rw-r--r--   0 eve        (501) staff       (20)      368 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.107335 py-evm-0.7.0a4/eth/_utils/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/_utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      687 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/address.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.107637 py-evm-0.7.0a4/eth/_utils/blake2/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 18:37:56.000000 py-evm-0.7.0a4/eth/_utils/blake2/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1841 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/blake2/coders.py
+-rwxr-xr-x   0 eve        (501) staff       (20)     5793 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/blake2/compression.py
+-rw-r--r--   0 eve        (501) staff       (20)      980 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/bn128.py
+-rw-r--r--   0 eve        (501) staff       (20)     3924 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/datatypes.py
+-rw-r--r--   0 eve        (501) staff       (20)     1013 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/db.py
+-rw-r--r--   0 eve        (501) staff       (20)       40 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/_utils/empty.py
+-rw-r--r--   0 eve        (501) staff       (20)     8124 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/env.py
+-rw-r--r--   0 eve        (501) staff       (20)      612 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/generator.py
+-rw-r--r--   0 eve        (501) staff       (20)     5042 2023-07-24 21:02:16.000000 py-evm-0.7.0a4/eth/_utils/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 18:37:56.000000 py-evm-0.7.0a4/eth/_utils/logging.py
+-rw-r--r--   0 eve        (501) staff       (20)     1540 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/module_loading.py
+-rw-r--r--   0 eve        (501) staff       (20)     2671 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/numeric.py
+-rw-r--r--   0 eve        (501) staff       (20)      337 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/padding.py
+-rw-r--r--   0 eve        (501) staff       (20)     3284 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/rlp.py
+-rw-r--r--   0 eve        (501) staff       (20)     1749 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/spoof.py
+-rw-r--r--   0 eve        (501) staff       (20)     1343 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     3379 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)      385 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_utils/version.py
+-rw-r--r--   0 eve        (501) staff       (20)      364 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/_warnings.py
+-rw-r--r--   0 eve        (501) staff       (20)   117213 2023-07-20 19:47:13.000000 py-evm-0.7.0a4/eth/abc.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.107967 py-evm-0.7.0a4/eth/chains/
+-rw-r--r--   0 eve        (501) staff       (20)      223 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/chains/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    25965 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/chains/base.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.108228 py-evm-0.7.0a4/eth/chains/goerli/
+-rw-r--r--   0 eve        (501) staff       (20)     1305 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/chains/goerli/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      270 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/chains/goerli/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     2554 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/chains/header.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.108466 py-evm-0.7.0a4/eth/chains/mainnet/
+-rw-r--r--   0 eve        (501) staff       (20)     4409 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/chains/mainnet/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1199 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/chains/mainnet/constants.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.108687 py-evm-0.7.0a4/eth/chains/ropsten/
+-rw-r--r--   0 eve        (501) staff       (20)     2131 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/chains/ropsten/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      847 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/chains/ropsten/constants.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.108785 py-evm-0.7.0a4/eth/chains/tester/
+-rw-r--r--   0 eve        (501) staff       (20)     5919 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/chains/tester/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.109413 py-evm-0.7.0a4/eth/consensus/
+-rw-r--r--   0 eve        (501) staff       (20)      313 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/consensus/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      968 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/applier.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.110274 py-evm-0.7.0a4/eth/consensus/clique/
+-rw-r--r--   0 eve        (501) staff       (20)      271 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/clique/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     5208 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/clique/_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     5383 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/clique/clique.py
+-rw-r--r--   0 eve        (501) staff       (20)      486 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/clique/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     3368 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/clique/datatypes.py
+-rw-r--r--   0 eve        (501) staff       (20)     2949 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/clique/encoding.py
+-rw-r--r--   0 eve        (501) staff       (20)      158 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/clique/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)    11157 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/clique/snapshot_manager.py
+-rw-r--r--   0 eve        (501) staff       (20)      187 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/context.py
+-rw-r--r--   0 eve        (501) staff       (20)      683 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/noproof.py
+-rw-r--r--   0 eve        (501) staff       (20)      819 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/pos.py
+-rw-r--r--   0 eve        (501) staff       (20)     4024 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/consensus/pow.py
+-rw-r--r--   0 eve        (501) staff       (20)     3921 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/constants.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.112598 py-evm-0.7.0a4/eth/db/
+-rw-r--r--   0 eve        (501) staff       (20)      714 2023-06-08 20:21:10.000000 py-evm-0.7.0a4/eth/db/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3460 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/accesslog.py
+-rw-r--r--   0 eve        (501) staff       (20)    24411 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/account.py
+-rw-r--r--   0 eve        (501) staff       (20)     4277 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/atomic.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.112961 py-evm-0.7.0a4/eth/db/backends/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/db/backends/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2497 2023-07-20 19:47:13.000000 py-evm-0.7.0a4/eth/db/backends/base.py
+-rw-r--r--   0 eve        (501) staff       (20)     4496 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/backends/level.py
+-rw-r--r--   0 eve        (501) staff       (20)      890 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/db/backends/memory.py
+-rw-r--r--   0 eve        (501) staff       (20)     2874 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/batch.py
+-rw-r--r--   0 eve        (501) staff       (20)      971 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/cache.py
+-rw-r--r--   0 eve        (501) staff       (20)    19206 2023-06-08 20:21:10.000000 py-evm-0.7.0a4/eth/db/chain.py
+-rw-r--r--   0 eve        (501) staff       (20)     5873 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/chain_gaps.py
+-rw-r--r--   0 eve        (501) staff       (20)     7394 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/diff.py
+-rw-r--r--   0 eve        (501) staff       (20)      506 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/hash_trie.py
+-rw-r--r--   0 eve        (501) staff       (20)    24129 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/header.py
+-rw-r--r--   0 eve        (501) staff       (20)    17008 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/journal.py
+-rw-r--r--   0 eve        (501) staff       (20)     1306 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/keymap.py
+-rw-r--r--   0 eve        (501) staff       (20)     1354 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/schema.py
+-rw-r--r--   0 eve        (501) staff       (20)    16562 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/slow_journal.py
+-rw-r--r--   0 eve        (501) staff       (20)    16442 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)     1393 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/trie.py
+-rw-r--r--   0 eve        (501) staff       (20)     1660 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/db/witness.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.113148 py-evm-0.7.0a4/eth/estimators/
+-rw-r--r--   0 eve        (501) staff       (20)      514 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/estimators/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3427 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/estimators/gas.py
+-rw-r--r--   0 eve        (501) staff       (20)     4115 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/exceptions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.114245 py-evm-0.7.0a4/eth/precompiles/
+-rw-r--r--   0 eve        (501) staff       (20)      398 2021-02-26 19:54:17.000000 py-evm-0.7.0a4/eth/precompiles/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      962 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/precompiles/blake2.py
+-rw-r--r--   0 eve        (501) staff       (20)     1502 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/precompiles/ecadd.py
+-rw-r--r--   0 eve        (501) staff       (20)     1390 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/precompiles/ecmul.py
+-rw-r--r--   0 eve        (501) staff       (20)     3257 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/precompiles/ecpairing.py
+-rw-r--r--   0 eve        (501) staff       (20)     1512 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/precompiles/ecrecover.py
+-rw-r--r--   0 eve        (501) staff       (20)      472 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/precompiles/identity.py
+-rw-r--r--   0 eve        (501) staff       (20)     3934 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/precompiles/modexp.py
+-rw-r--r--   0 eve        (501) staff       (20)      670 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/precompiles/ripemd160.py
+-rw-r--r--   0 eve        (501) staff       (20)      541 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/precompiles/sha256.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/py.typed
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.114975 py-evm-0.7.0a4/eth/rlp/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/rlp/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1022 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/rlp/accounts.py
+-rw-r--r--   0 eve        (501) staff       (20)      904 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/rlp/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     5417 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/rlp/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      603 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/rlp/logs.py
+-rw-r--r--   0 eve        (501) staff       (20)     1285 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/rlp/receipts.py
+-rw-r--r--   0 eve        (501) staff       (20)      387 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/rlp/sedes.py
+-rw-r--r--   0 eve        (501) staff       (20)     3611 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/rlp/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.115238 py-evm-0.7.0a4/eth/tools/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/tools/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.116184 py-evm-0.7.0a4/eth/tools/_utils/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/tools/_utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      662 2023-06-08 20:21:10.000000 py-evm-0.7.0a4/eth/tools/_utils/deprecation.py
+-rw-r--r--   0 eve        (501) staff       (20)      190 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/_utils/git.py
+-rw-r--r--   0 eve        (501) staff       (20)      556 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/_utils/hashing.py
+-rw-r--r--   0 eve        (501) staff       (20)     1564 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/_utils/mappings.py
+-rw-r--r--   0 eve        (501) staff       (20)    18084 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/_utils/normalization.py
+-rw-r--r--   0 eve        (501) staff       (20)     4410 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/_utils/slow_code_stream.py
+-rw-r--r--   0 eve        (501) staff       (20)      903 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/_utils/vyper.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.116277 py-evm-0.7.0a4/eth/tools/builder/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/tools/builder/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.116446 py-evm-0.7.0a4/eth/tools/builder/chain/
+-rw-r--r--   0 eve        (501) staff       (20)     2936 2023-04-28 21:07:47.000000 py-evm-0.7.0a4/eth/tools/builder/chain/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    15254 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/builder/chain/builders.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.116747 py-evm-0.7.0a4/eth/tools/db/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/tools/db/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     5191 2023-06-08 20:21:10.000000 py-evm-0.7.0a4/eth/tools/db/atomic.py
+-rw-r--r--   0 eve        (501) staff       (20)     2269 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/db/base.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.118045 py-evm-0.7.0a4/eth/tools/fixtures/
+-rw-r--r--   0 eve        (501) staff       (20)      615 2021-08-19 20:42:01.000000 py-evm-0.7.0a4/eth/tools/fixtures/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      887 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/fixtures/_utils.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.118718 py-evm-0.7.0a4/eth/tools/fixtures/fillers/
+-rw-r--r--   0 eve        (501) staff       (20)      282 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/tools/fixtures/fillers/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2456 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/fixtures/fillers/_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)    12716 2023-06-08 20:21:10.000000 py-evm-0.7.0a4/eth/tools/fixtures/fillers/common.py
+-rw-r--r--   0 eve        (501) staff       (20)     3461 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/fixtures/fillers/formatters.py
+-rw-r--r--   0 eve        (501) staff       (20)     1307 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/fixtures/fillers/main.py
+-rw-r--r--   0 eve        (501) staff       (20)     2758 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/fixtures/fillers/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1737 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/fixtures/fillers/vm.py
+-rw-r--r--   0 eve        (501) staff       (20)     2079 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/fixtures/generation.py
+-rw-r--r--   0 eve        (501) staff       (20)     9361 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/fixtures/helpers.py
+-rw-r--r--   0 eve        (501) staff       (20)     3068 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/fixtures/loading.py
+-rw-r--r--   0 eve        (501) staff       (20)      791 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/mining.py
+-rw-r--r--   0 eve        (501) staff       (20)      476 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/tools/rlp.py
+-rw-r--r--   0 eve        (501) staff       (20)     2693 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/typing.py
+-rw-r--r--   0 eve        (501) staff       (20)     8548 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.120411 py-evm-0.7.0a4/eth/vm/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/vm/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    26238 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/base.py
+-rw-r--r--   0 eve        (501) staff       (20)      632 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/chain_context.py
+-rw-r--r--   0 eve        (501) staff       (20)     4438 2023-06-08 20:21:10.000000 py-evm-0.7.0a4/eth/vm/code_stream.py
+-rw-r--r--   0 eve        (501) staff       (20)    19222 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)     2124 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/execution_context.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.120511 py-evm-0.7.0a4/eth/vm/forks/
+-rw-r--r--   0 eve        (501) staff       (20)      899 2023-04-28 21:07:47.000000 py-evm-0.7.0a4/eth/vm/forks/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.121070 py-evm-0.7.0a4/eth/vm/forks/arrow_glacier/
+-rw-r--r--   0 eve        (501) staff       (20)      856 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/arrow_glacier/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      993 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/arrow_glacier/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      287 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/arrow_glacier/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)     1084 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/arrow_glacier/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      523 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/arrow_glacier/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1134 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/arrow_glacier/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.122004 py-evm-0.7.0a4/eth/vm/forks/berlin/
+-rw-r--r--   0 eve        (501) staff       (20)      772 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/berlin/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      784 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/berlin/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     2441 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/berlin/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      327 2021-08-30 21:22:29.000000 py-evm-0.7.0a4/eth/vm/forks/berlin/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      374 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/berlin/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     6417 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/berlin/logic.py
+-rw-r--r--   0 eve        (501) staff       (20)     2922 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/berlin/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)     4606 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/berlin/receipts.py
+-rw-r--r--   0 eve        (501) staff       (20)     1187 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/berlin/state.py
+-rw-r--r--   0 eve        (501) staff       (20)    15395 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/berlin/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.122744 py-evm-0.7.0a4/eth/vm/forks/byzantium/
+-rw-r--r--   0 eve        (501) staff       (20)     3584 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/byzantium/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      485 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/byzantium/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     1016 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/byzantium/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      235 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/byzantium/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     3368 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/byzantium/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     3526 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/byzantium/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      222 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/byzantium/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1231 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/byzantium/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.123575 py-evm-0.7.0a4/eth/vm/forks/constantinople/
+-rw-r--r--   0 eve        (501) staff       (20)     1106 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/constantinople/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      484 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/constantinople/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      757 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/constantinople/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      329 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/constantinople/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      406 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/constantinople/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     1574 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/constantinople/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      221 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/constantinople/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      334 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/constantinople/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)     1235 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/constantinople/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.124555 py-evm-0.7.0a4/eth/vm/forks/frontier/
+-rw-r--r--   0 eve        (501) staff       (20)     3732 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/frontier/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3412 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/frontier/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     3715 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/frontier/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)       96 2021-09-20 20:47:49.000000 py-evm-0.7.0a4/eth/vm/forks/frontier/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     3529 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/frontier/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)    20228 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/frontier/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)     7686 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/frontier/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      140 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/frontier/transaction_context.py
+-rw-r--r--   0 eve        (501) staff       (20)     5952 2023-07-20 19:47:13.000000 py-evm-0.7.0a4/eth/vm/forks/frontier/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)     1603 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/frontier/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.125323 py-evm-0.7.0a4/eth/vm/forks/gray_glacier/
+-rw-r--r--   0 eve        (501) staff       (20)      855 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/gray_glacier/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1068 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/gray_glacier/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      317 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/gray_glacier/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)     1119 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/gray_glacier/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      556 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/gray_glacier/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1170 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/gray_glacier/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.126383 py-evm-0.7.0a4/eth/vm/forks/homestead/
+-rw-r--r--   0 eve        (501) staff       (20)     1250 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/homestead/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      466 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/homestead/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     2289 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/homestead/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)       61 2021-09-03 20:35:50.000000 py-evm-0.7.0a4/eth/vm/forks/homestead/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     9656 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/homestead/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      637 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/homestead/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      640 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/homestead/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     2281 2023-07-20 19:47:13.000000 py-evm-0.7.0a4/eth/vm/forks/homestead/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)      518 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/homestead/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.127376 py-evm-0.7.0a4/eth/vm/forks/istanbul/
+-rw-r--r--   0 eve        (501) staff       (20)      817 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/istanbul/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      469 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/istanbul/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     1421 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/istanbul/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      316 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/vm/forks/istanbul/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      384 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/istanbul/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     1664 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/istanbul/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      206 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/istanbul/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      909 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/istanbul/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)     1798 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/istanbul/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.128532 py-evm-0.7.0a4/eth/vm/forks/london/
+-rw-r--r--   0 eve        (501) staff       (20)     2260 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/london/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     5828 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/london/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      810 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/london/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      470 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/london/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     5618 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/london/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      895 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/london/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      629 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/london/receipts.py
+-rw-r--r--   0 eve        (501) staff       (20)     4881 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/london/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      544 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/london/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)     9486 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/london/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)      855 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/london/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.129197 py-evm-0.7.0a4/eth/vm/forks/muir_glacier/
+-rw-r--r--   0 eve        (501) staff       (20)      842 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/muir_glacier/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      472 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/muir_glacier/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      537 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/muir_glacier/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      443 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/muir_glacier/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      137 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/muir_glacier/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      209 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/muir_glacier/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1212 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/muir_glacier/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.129865 py-evm-0.7.0a4/eth/vm/forks/paris/
+-rw-r--r--   0 eve        (501) staff       (20)     2117 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/paris/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1039 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/paris/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      379 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/paris/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)     2284 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/paris/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      686 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/paris/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      666 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/paris/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1121 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/paris/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.130769 py-evm-0.7.0a4/eth/vm/forks/petersburg/
+-rw-r--r--   0 eve        (501) staff       (20)     1036 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/petersburg/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      472 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/petersburg/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      531 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/petersburg/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      110 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/petersburg/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      386 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/petersburg/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     1399 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/petersburg/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      209 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/petersburg/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1211 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/petersburg/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.131838 py-evm-0.7.0a4/eth/vm/forks/shanghai/
+-rw-r--r--   0 eve        (501) staff       (20)      667 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/shanghai/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     9048 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/shanghai/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     1655 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/shanghai/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      196 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/shanghai/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      824 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/shanghai/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      821 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/shanghai/logic.py
+-rw-r--r--   0 eve        (501) staff       (20)     1531 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/shanghai/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      751 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/shanghai/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1099 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/shanghai/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)     1515 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/shanghai/withdrawals.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.132624 py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/
+-rw-r--r--   0 eve        (501) staff       (20)      429 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2145 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)      484 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     3322 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      169 2023-04-28 21:07:47.000000 py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     1221 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)     1465 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     2866 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.133109 py-evm-0.7.0a4/eth/vm/forks/tangerine_whistle/
+-rw-r--r--   0 eve        (501) staff       (20)      469 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/tangerine_whistle/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      428 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/tangerine_whistle/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      225 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/vm/forks/tangerine_whistle/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     2106 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/tangerine_whistle/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      227 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/forks/tangerine_whistle/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     2626 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/gas_meter.py
+-rw-r--r--   0 eve        (501) staff       (20)      540 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/header.py
+-rw-r--r--   0 eve        (501) staff       (20)     3425 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/interrupt.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.134637 py-evm-0.7.0a4/eth/vm/logic/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a4/eth/vm/logic/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     4805 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/arithmetic.py
+-rw-r--r--   0 eve        (501) staff       (20)     1113 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/block.py
+-rw-r--r--   0 eve        (501) staff       (20)    13394 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/call.py
+-rw-r--r--   0 eve        (501) staff       (20)     2824 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/comparison.py
+-rw-r--r--   0 eve        (501) staff       (20)     6418 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/context.py
+-rw-r--r--   0 eve        (501) staff       (20)      944 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/duplication.py
+-rw-r--r--   0 eve        (501) staff       (20)     1508 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/flow.py
+-rw-r--r--   0 eve        (501) staff       (20)      507 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/invalid.py
+-rw-r--r--   0 eve        (501) staff       (20)     1355 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/logging.py
+-rw-r--r--   0 eve        (501) staff       (20)     1102 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/memory.py
+-rw-r--r--   0 eve        (501) staff       (20)      640 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/sha3.py
+-rw-r--r--   0 eve        (501) staff       (20)     2176 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/stack.py
+-rw-r--r--   0 eve        (501) staff       (20)     3939 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)      974 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/swap.py
+-rw-r--r--   0 eve        (501) staff       (20)     9727 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/logic/system.py
+-rw-r--r--   0 eve        (501) staff       (20)     2134 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/memory.py
+-rw-r--r--   0 eve        (501) staff       (20)     3214 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/message.py
+-rw-r--r--   0 eve        (501) staff       (20)     2785 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/mnemonics.py
+-rw-r--r--   0 eve        (501) staff       (20)     1864 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/opcode.py
+-rw-r--r--   0 eve        (501) staff       (20)     2432 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/opcode_values.py
+-rw-r--r--   0 eve        (501) staff       (20)      416 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/spoof.py
+-rw-r--r--   0 eve        (501) staff       (20)     7713 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/stack.py
+-rw-r--r--   0 eve        (501) staff       (20)    10406 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      875 2023-06-02 21:07:53.000000 py-evm-0.7.0a4/eth/vm/transaction_context.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-24 21:05:51.135409 py-evm-0.7.0a4/py_evm.egg-info/
+-rw-r--r--   0 eve        (501) staff       (20)     2997 2023-07-24 21:05:48.000000 py-evm-0.7.0a4/py_evm.egg-info/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     8485 2023-07-24 21:05:51.000000 py-evm-0.7.0a4/py_evm.egg-info/SOURCES.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-07-24 21:05:48.000000 py-evm-0.7.0a4/py_evm.egg-info/dependency_links.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2021-02-24 18:15:32.000000 py-evm-0.7.0a4/py_evm.egg-info/not-zip-safe
+-rw-r--r--   0 eve        (501) staff       (20)     2146 2023-07-24 21:05:48.000000 py-evm-0.7.0a4/py_evm.egg-info/requires.txt
+-rw-r--r--   0 eve        (501) staff       (20)        4 2023-07-24 21:05:48.000000 py-evm-0.7.0a4/py_evm.egg-info/top_level.txt
+-rw-r--r--   0 eve        (501) staff       (20)     1117 2023-06-08 20:21:10.000000 py-evm-0.7.0a4/pyproject.toml
+-rw-r--r--   0 eve        (501) staff       (20)       38 2023-07-24 21:05:51.135771 py-evm-0.7.0a4/setup.cfg
+-rw-r--r--   0 eve        (501) staff       (20)     4036 2023-07-24 21:05:42.000000 py-evm-0.7.0a4/setup.py
```

### Comparing `py-evm-0.7.0a3/LICENSE` & `py-evm-0.7.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/PKG-INFO` & `py-evm-0.7.0a4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: py-evm
-Version: 0.7.0a3
+Version: 0.7.0a4
 Summary: Python implementation of the Ethereum Virtual Machine
 Home-page: https://github.com/ethereum/py-evm
 Author: Ethereum Foundation
 Author-email: piper@pipermerriam.com
 License: MIT
 Keywords: ethereum blockchain evm
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -67,7 +68,9 @@
 
 Check out the [documentation on our official website](https://py-evm.readthedocs.io/en/latest/)
 
 ## Want to help?
 
 Want to file a bug, contribute some code, or improve documentation? Excellent! Read up on our
 guidelines for [contributing](https://py-evm.readthedocs.io/en/latest/contributing.html) and then check out one of our issues that are labeled [Good First Issue](https://github.com/ethereum/py-evm/issues?q=is%3Aissue+is%3Aopen+label%3A%22Good+First+Issue%22).
+
+
```

### Comparing `py-evm-0.7.0a3/README.md` & `py-evm-0.7.0a4/README.md`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/address.py` & `py-evm-0.7.0a4/eth/_utils/address.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/blake2/coders.py` & `py-evm-0.7.0a4/eth/_utils/blake2/coders.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/blake2/compression.py` & `py-evm-0.7.0a4/eth/_utils/blake2/compression.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/bn128.py` & `py-evm-0.7.0a4/eth/_utils/bn128.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/datatypes.py` & `py-evm-0.7.0a4/eth/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/db.py` & `py-evm-0.7.0a4/eth/_utils/db.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/env.py` & `py-evm-0.7.0a4/eth/_utils/env.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/generator.py` & `py-evm-0.7.0a4/eth/_utils/generator.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/headers.py` & `py-evm-0.7.0a4/eth/_utils/headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 )
 
 
 def eth_now() -> int:
     """
     The timestamp is in UTC.
     """
-    return int(datetime.datetime.utcnow().timestamp())
+    return int(datetime.datetime.now(datetime.timezone.utc).timestamp())
 
 
 def new_timestamp_from_parent(parent: Optional[BlockHeaderAPI]) -> int:
     """
     Generate a timestamp to use on a new header.
 
     Generally, attempt to use the current time. If timestamp is too old (equal
```

### Comparing `py-evm-0.7.0a3/eth/_utils/module_loading.py` & `py-evm-0.7.0a4/eth/_utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/numeric.py` & `py-evm-0.7.0a4/eth/_utils/numeric.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/rlp.py` & `py-evm-0.7.0a4/eth/_utils/rlp.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/spoof.py` & `py-evm-0.7.0a4/eth/_utils/spoof.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/state.py` & `py-evm-0.7.0a4/eth/_utils/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/_utils/transactions.py` & `py-evm-0.7.0a4/eth/_utils/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/abc.py` & `py-evm-0.7.0a4/eth/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -483,15 +483,17 @@
     value: int
     data: bytes
 
     #
     # API that must be implemented by all Transaction subclasses.
     #
     @abstractmethod
-    def as_signed_transaction(self, private_key: PrivateKey) -> "SignedTransactionAPI":
+    def as_signed_transaction(
+        self, private_key: PrivateKey, chain_id: int = None
+    ) -> "SignedTransactionAPI":
         """
         Return a version of this transaction which has been signed using the
         provided `private_key`
         """
         ...
 
 
@@ -3763,15 +3765,15 @@
         Validate the given ``receipt``.
         """
         ...
 
     @abstractmethod
     def validate_block(self, block: BlockAPI) -> None:
         """
-        Validate the the given block.
+        Validate the given block.
         """
         ...
 
     @classmethod
     @abstractmethod
     def validate_header(
         self, header: BlockHeaderAPI, parent_header: BlockHeaderAPI
```

### Comparing `py-evm-0.7.0a3/eth/chains/base.py` & `py-evm-0.7.0a4/eth/chains/base.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/chains/goerli/__init__.py` & `py-evm-0.7.0a4/eth/chains/goerli/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/chains/header.py` & `py-evm-0.7.0a4/eth/chains/header.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/chains/mainnet/__init__.py` & `py-evm-0.7.0a4/eth/chains/mainnet/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/chains/mainnet/constants.py` & `py-evm-0.7.0a4/eth/chains/mainnet/constants.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/chains/ropsten/__init__.py` & `py-evm-0.7.0a4/eth/chains/ropsten/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/chains/ropsten/constants.py` & `py-evm-0.7.0a4/eth/chains/ropsten/constants.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/chains/tester/__init__.py` & `py-evm-0.7.0a4/eth/chains/tester/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/consensus/applier.py` & `py-evm-0.7.0a4/eth/consensus/applier.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/consensus/clique/_utils.py` & `py-evm-0.7.0a4/eth/consensus/clique/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/consensus/clique/clique.py` & `py-evm-0.7.0a4/eth/consensus/clique/clique.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/consensus/clique/datatypes.py` & `py-evm-0.7.0a4/eth/consensus/clique/datatypes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/consensus/clique/encoding.py` & `py-evm-0.7.0a4/eth/consensus/clique/encoding.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/consensus/clique/snapshot_manager.py` & `py-evm-0.7.0a4/eth/consensus/clique/snapshot_manager.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/consensus/noproof.py` & `py-evm-0.7.0a4/eth/consensus/noproof.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/consensus/pos.py` & `py-evm-0.7.0a4/eth/consensus/pos.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/consensus/pow.py` & `py-evm-0.7.0a4/eth/consensus/pow.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/constants.py` & `py-evm-0.7.0a4/eth/constants.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/__init__.py` & `py-evm-0.7.0a4/eth/db/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/accesslog.py` & `py-evm-0.7.0a4/eth/db/accesslog.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/account.py` & `py-evm-0.7.0a4/eth/db/account.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/atomic.py` & `py-evm-0.7.0a4/eth/db/atomic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/backends/base.py` & `py-evm-0.7.0a4/eth/db/backends/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def exists(self, key: bytes) -> bool:
         return self.__contains__(key)
 
     def __contains__(self, key: bytes) -> bool:  # type: ignore # Breaks LSP
         if hasattr(self, "_exists"):
             # Classes which inherit this class would have `_exists` attr
-            return self._exists(key)  # type: ignore
+            return self._exists(key)
         else:
             return super().__contains__(key)
 
     def delete(self, key: bytes) -> None:
         try:
             del self[key]
         except KeyError:
```

### Comparing `py-evm-0.7.0a3/eth/db/backends/level.py` & `py-evm-0.7.0a4/eth/db/backends/level.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/backends/memory.py` & `py-evm-0.7.0a4/eth/db/backends/memory.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/batch.py` & `py-evm-0.7.0a4/eth/db/batch.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/cache.py` & `py-evm-0.7.0a4/eth/db/cache.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/chain.py` & `py-evm-0.7.0a4/eth/db/chain.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/chain_gaps.py` & `py-evm-0.7.0a4/eth/db/chain_gaps.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/diff.py` & `py-evm-0.7.0a4/eth/db/diff.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/header.py` & `py-evm-0.7.0a4/eth/db/header.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/journal.py` & `py-evm-0.7.0a4/eth/db/journal.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/keymap.py` & `py-evm-0.7.0a4/eth/db/keymap.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/schema.py` & `py-evm-0.7.0a4/eth/db/schema.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/slow_journal.py` & `py-evm-0.7.0a4/eth/db/slow_journal.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/storage.py` & `py-evm-0.7.0a4/eth/db/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/trie.py` & `py-evm-0.7.0a4/eth/db/trie.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/db/witness.py` & `py-evm-0.7.0a4/eth/db/witness.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/estimators/__init__.py` & `py-evm-0.7.0a4/eth/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/estimators/gas.py` & `py-evm-0.7.0a4/eth/estimators/gas.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/exceptions.py` & `py-evm-0.7.0a4/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/precompiles/blake2.py` & `py-evm-0.7.0a4/eth/precompiles/blake2.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/precompiles/ecadd.py` & `py-evm-0.7.0a4/eth/precompiles/ecadd.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/precompiles/ecmul.py` & `py-evm-0.7.0a4/eth/precompiles/ecmul.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/precompiles/ecpairing.py` & `py-evm-0.7.0a4/eth/precompiles/ecpairing.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/precompiles/ecrecover.py` & `py-evm-0.7.0a4/eth/precompiles/ecrecover.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/precompiles/modexp.py` & `py-evm-0.7.0a4/eth/precompiles/modexp.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/precompiles/ripemd160.py` & `py-evm-0.7.0a4/eth/precompiles/ripemd160.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/precompiles/sha256.py` & `py-evm-0.7.0a4/eth/precompiles/sha256.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/rlp/accounts.py` & `py-evm-0.7.0a4/eth/rlp/accounts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/rlp/blocks.py` & `py-evm-0.7.0a4/eth/rlp/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/rlp/headers.py` & `py-evm-0.7.0a4/eth/rlp/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/rlp/logs.py` & `py-evm-0.7.0a4/eth/rlp/logs.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/rlp/receipts.py` & `py-evm-0.7.0a4/eth/rlp/receipts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/rlp/transactions.py` & `py-evm-0.7.0a4/eth/rlp/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/_utils/deprecation.py` & `py-evm-0.7.0a4/eth/tools/_utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/_utils/hashing.py` & `py-evm-0.7.0a4/eth/tools/_utils/hashing.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/_utils/mappings.py` & `py-evm-0.7.0a4/eth/tools/_utils/mappings.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/_utils/normalization.py` & `py-evm-0.7.0a4/eth/tools/_utils/normalization.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/_utils/slow_code_stream.py` & `py-evm-0.7.0a4/eth/tools/_utils/slow_code_stream.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/_utils/vyper.py` & `py-evm-0.7.0a4/eth/tools/_utils/vyper.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/builder/chain/__init__.py` & `py-evm-0.7.0a4/eth/tools/builder/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/builder/chain/builders.py` & `py-evm-0.7.0a4/eth/tools/builder/chain/builders.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/db/atomic.py` & `py-evm-0.7.0a4/eth/tools/db/atomic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/db/base.py` & `py-evm-0.7.0a4/eth/tools/db/base.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/fixtures/__init__.py` & `py-evm-0.7.0a4/eth/tools/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/fixtures/_utils.py` & `py-evm-0.7.0a4/eth/tools/fixtures/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/fixtures/fillers/_utils.py` & `py-evm-0.7.0a4/eth/tools/fixtures/fillers/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/fixtures/fillers/common.py` & `py-evm-0.7.0a4/eth/tools/fixtures/fillers/common.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/fixtures/fillers/formatters.py` & `py-evm-0.7.0a4/eth/tools/fixtures/fillers/formatters.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/fixtures/fillers/main.py` & `py-evm-0.7.0a4/eth/tools/fixtures/fillers/main.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/fixtures/fillers/state.py` & `py-evm-0.7.0a4/eth/tools/fixtures/fillers/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/fixtures/fillers/vm.py` & `py-evm-0.7.0a4/eth/tools/fixtures/fillers/vm.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/fixtures/generation.py` & `py-evm-0.7.0a4/eth/tools/fixtures/generation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/fixtures/helpers.py` & `py-evm-0.7.0a4/eth/tools/fixtures/helpers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/fixtures/loading.py` & `py-evm-0.7.0a4/eth/tools/fixtures/loading.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/tools/mining.py` & `py-evm-0.7.0a4/eth/tools/mining.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/typing.py` & `py-evm-0.7.0a4/eth/typing.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/validation.py` & `py-evm-0.7.0a4/eth/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/base.py` & `py-evm-0.7.0a4/eth/vm/base.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/chain_context.py` & `py-evm-0.7.0a4/eth/vm/chain_context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/code_stream.py` & `py-evm-0.7.0a4/eth/vm/code_stream.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/computation.py` & `py-evm-0.7.0a4/eth/vm/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/execution_context.py` & `py-evm-0.7.0a4/eth/vm/execution_context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/arrow_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/blocks.py` & `py-evm-0.7.0a4/eth/vm/forks/arrow_glacier/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/headers.py` & `py-evm-0.7.0a4/eth/vm/forks/arrow_glacier/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/state.py` & `py-evm-0.7.0a4/eth/vm/forks/arrow_glacier/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/arrow_glacier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/berlin/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/berlin/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/berlin/blocks.py` & `py-evm-0.7.0a4/eth/vm/forks/berlin/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/berlin/computation.py` & `py-evm-0.7.0a4/eth/vm/forks/berlin/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/berlin/logic.py` & `py-evm-0.7.0a4/eth/vm/forks/berlin/logic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/berlin/opcodes.py` & `py-evm-0.7.0a4/eth/vm/forks/berlin/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/berlin/receipts.py` & `py-evm-0.7.0a4/eth/vm/forks/berlin/receipts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/berlin/state.py` & `py-evm-0.7.0a4/eth/vm/forks/berlin/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/berlin/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/berlin/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/byzantium/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/byzantium/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/byzantium/computation.py` & `py-evm-0.7.0a4/eth/vm/forks/byzantium/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/byzantium/headers.py` & `py-evm-0.7.0a4/eth/vm/forks/byzantium/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/byzantium/opcodes.py` & `py-evm-0.7.0a4/eth/vm/forks/byzantium/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/byzantium/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/byzantium/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/constantinople/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/constantinople/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/constantinople/computation.py` & `py-evm-0.7.0a4/eth/vm/forks/constantinople/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/constantinople/opcodes.py` & `py-evm-0.7.0a4/eth/vm/forks/constantinople/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/constantinople/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/constantinople/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/frontier/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/frontier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/frontier/blocks.py` & `py-evm-0.7.0a4/eth/vm/forks/frontier/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/frontier/computation.py` & `py-evm-0.7.0a4/eth/vm/forks/frontier/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/frontier/headers.py` & `py-evm-0.7.0a4/eth/vm/forks/frontier/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/frontier/opcodes.py` & `py-evm-0.7.0a4/eth/vm/forks/frontier/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/frontier/state.py` & `py-evm-0.7.0a4/eth/vm/forks/frontier/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/frontier/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/frontier/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,19 @@
         validate_uint256(self.gas, title="Transaction.gas")
         if self.to != CREATE_CONTRACT_ADDRESS:
             validate_canonical_address(self.to, title="Transaction.to")
         validate_uint256(self.value, title="Transaction.value")
         validate_is_bytes(self.data, title="Transaction.data")
         super().validate()
 
-    def as_signed_transaction(self, private_key: PrivateKey) -> FrontierTransaction:
+    def as_signed_transaction(
+        self,
+        private_key: PrivateKey,
+        chain_id: int = None,  # unused until SpuriousDragon
+    ) -> FrontierTransaction:
         v, r, s = create_transaction_signature(self, private_key)
         return FrontierTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
             value=self.value,
```

### Comparing `py-evm-0.7.0a3/eth/vm/forks/frontier/validation.py` & `py-evm-0.7.0a4/eth/vm/forks/frontier/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/gray_glacier/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/gray_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/gray_glacier/blocks.py` & `py-evm-0.7.0a4/eth/vm/forks/gray_glacier/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/gray_glacier/headers.py` & `py-evm-0.7.0a4/eth/vm/forks/gray_glacier/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/gray_glacier/state.py` & `py-evm-0.7.0a4/eth/vm/forks/gray_glacier/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/gray_glacier/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/gray_glacier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/homestead/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/homestead/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/homestead/computation.py` & `py-evm-0.7.0a4/eth/vm/forks/homestead/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/homestead/headers.py` & `py-evm-0.7.0a4/eth/vm/forks/homestead/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/homestead/opcodes.py` & `py-evm-0.7.0a4/eth/vm/forks/homestead/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/homestead/state.py` & `py-evm-0.7.0a4/eth/vm/forks/homestead/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/homestead/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/homestead/transactions.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,19 @@
         value: int,
         data: bytes
     ) -> "HomesteadUnsignedTransaction":
         return HomesteadUnsignedTransaction(nonce, gas_price, gas, to, value, data)
 
 
 class HomesteadUnsignedTransaction(FrontierUnsignedTransaction):
-    def as_signed_transaction(self, private_key: PrivateKey) -> HomesteadTransaction:
+    def as_signed_transaction(
+        self,
+        private_key: PrivateKey,
+        chain_id: int = None,  # unused until SpuriousDragon
+    ) -> HomesteadTransaction:
         v, r, s = create_transaction_signature(self, private_key)
         return HomesteadTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
             value=self.value,
```

### Comparing `py-evm-0.7.0a3/eth/vm/forks/homestead/validation.py` & `py-evm-0.7.0a4/eth/vm/forks/homestead/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/istanbul/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/istanbul/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/istanbul/computation.py` & `py-evm-0.7.0a4/eth/vm/forks/istanbul/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/istanbul/opcodes.py` & `py-evm-0.7.0a4/eth/vm/forks/istanbul/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/istanbul/storage.py` & `py-evm-0.7.0a4/eth/vm/forks/istanbul/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/istanbul/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/istanbul/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/london/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/london/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/london/blocks.py` & `py-evm-0.7.0a4/eth/vm/forks/london/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/london/computation.py` & `py-evm-0.7.0a4/eth/vm/forks/london/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/london/headers.py` & `py-evm-0.7.0a4/eth/vm/forks/london/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/london/opcodes.py` & `py-evm-0.7.0a4/eth/vm/forks/london/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/london/receipts.py` & `py-evm-0.7.0a4/eth/vm/forks/london/receipts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/london/state.py` & `py-evm-0.7.0a4/eth/vm/forks/london/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/london/storage.py` & `py-evm-0.7.0a4/eth/vm/forks/london/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/london/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/london/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/london/validation.py` & `py-evm-0.7.0a4/eth/vm/forks/london/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/muir_glacier/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/muir_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/muir_glacier/computation.py` & `py-evm-0.7.0a4/eth/vm/forks/muir_glacier/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/muir_glacier/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/muir_glacier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/paris/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/paris/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/paris/blocks.py` & `py-evm-0.7.0a4/eth/vm/forks/paris/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/paris/headers.py` & `py-evm-0.7.0a4/eth/vm/forks/paris/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/paris/opcodes.py` & `py-evm-0.7.0a4/eth/vm/forks/paris/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/paris/state.py` & `py-evm-0.7.0a4/eth/vm/forks/paris/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/paris/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/paris/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/petersburg/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/petersburg/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/petersburg/computation.py` & `py-evm-0.7.0a4/eth/vm/forks/petersburg/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/petersburg/opcodes.py` & `py-evm-0.7.0a4/eth/vm/forks/petersburg/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/petersburg/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/petersburg/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/shanghai/__init__.py` & `py-evm-0.7.0a4/eth/vm/forks/shanghai/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/shanghai/blocks.py` & `py-evm-0.7.0a4/eth/vm/forks/shanghai/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/shanghai/computation.py` & `py-evm-0.7.0a4/eth/vm/forks/shanghai/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/shanghai/headers.py` & `py-evm-0.7.0a4/eth/vm/forks/shanghai/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/shanghai/logic.py` & `py-evm-0.7.0a4/eth/vm/forks/shanghai/logic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/shanghai/opcodes.py` & `py-evm-0.7.0a4/eth/vm/forks/shanghai/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/shanghai/state.py` & `py-evm-0.7.0a4/eth/vm/forks/shanghai/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/shanghai/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/shanghai/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/shanghai/withdrawals.py` & `py-evm-0.7.0a4/eth/vm/forks/shanghai/withdrawals.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/_utils.py` & `py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/computation.py` & `py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/opcodes.py` & `py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/state.py` & `py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/transactions.py` & `py-evm-0.7.0a4/eth/vm/forks/spurious_dragon/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/opcodes.py` & `py-evm-0.7.0a4/eth/vm/forks/tangerine_whistle/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/gas_meter.py` & `py-evm-0.7.0a4/eth/vm/gas_meter.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/header.py` & `py-evm-0.7.0a4/eth/vm/header.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/interrupt.py` & `py-evm-0.7.0a4/eth/vm/interrupt.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/arithmetic.py` & `py-evm-0.7.0a4/eth/vm/logic/arithmetic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/block.py` & `py-evm-0.7.0a4/eth/vm/logic/block.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/call.py` & `py-evm-0.7.0a4/eth/vm/logic/call.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/comparison.py` & `py-evm-0.7.0a4/eth/vm/logic/comparison.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/context.py` & `py-evm-0.7.0a4/eth/vm/logic/context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/duplication.py` & `py-evm-0.7.0a4/eth/vm/logic/duplication.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/flow.py` & `py-evm-0.7.0a4/eth/vm/logic/flow.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/logging.py` & `py-evm-0.7.0a4/eth/vm/logic/logging.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/memory.py` & `py-evm-0.7.0a4/eth/vm/logic/memory.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/sha3.py` & `py-evm-0.7.0a4/eth/vm/logic/sha3.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/stack.py` & `py-evm-0.7.0a4/eth/vm/logic/stack.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/storage.py` & `py-evm-0.7.0a4/eth/vm/logic/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/swap.py` & `py-evm-0.7.0a4/eth/vm/logic/swap.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/logic/system.py` & `py-evm-0.7.0a4/eth/vm/logic/system.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/memory.py` & `py-evm-0.7.0a4/eth/vm/memory.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/message.py` & `py-evm-0.7.0a4/eth/vm/message.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/mnemonics.py` & `py-evm-0.7.0a4/eth/vm/mnemonics.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/opcode.py` & `py-evm-0.7.0a4/eth/vm/opcode.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/opcode_values.py` & `py-evm-0.7.0a4/eth/vm/opcode_values.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/stack.py` & `py-evm-0.7.0a4/eth/vm/stack.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/state.py` & `py-evm-0.7.0a4/eth/vm/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/eth/vm/transaction_context.py` & `py-evm-0.7.0a4/eth/vm/transaction_context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/py_evm.egg-info/PKG-INFO` & `py-evm-0.7.0a4/py_evm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: py-evm
-Version: 0.7.0a3
+Version: 0.7.0a4
 Summary: Python implementation of the Ethereum Virtual Machine
 Home-page: https://github.com/ethereum/py-evm
 Author: Ethereum Foundation
 Author-email: piper@pipermerriam.com
 License: MIT
 Keywords: ethereum blockchain evm
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -67,7 +68,9 @@
 
 Check out the [documentation on our official website](https://py-evm.readthedocs.io/en/latest/)
 
 ## Want to help?
 
 Want to file a bug, contribute some code, or improve documentation? Excellent! Read up on our
 guidelines for [contributing](https://py-evm.readthedocs.io/en/latest/contributing.html) and then check out one of our issues that are labeled [Good First Issue](https://github.com/ethereum/py-evm/issues?q=is%3Aissue+is%3Aopen+label%3A%22Good+First+Issue%22).
+
+
```

### Comparing `py-evm-0.7.0a3/py_evm.egg-info/SOURCES.txt` & `py-evm-0.7.0a4/py_evm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/py_evm.egg-info/requires.txt` & `py-evm-0.7.0a4/py_evm.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 cached-property<2,>=1.5.1
 eth-bloom>=1.0.3
 eth-keys<0.5.0,>=0.4.0
 eth-typing<4.0.0,>=3.3.0
 eth-utils<3.0.0,>=2.0.0
 lru-dict>=1.1.6
-mypy_extensions<1.0.0,>=0.4.1
+mypy-extensions>=1.0.0
 py-ecc<7.0.0,>=1.4.7
 pyethash<1.0.0,>=0.1.27
 rlp<4,>=3
 trie<3,>=2.0.0
 
 [benchmark]
 termcolor<2.0.0,>=1.1.0
@@ -24,15 +24,15 @@
 twine
 cached-property<2,>=1.5.1
 eth-bloom>=1.0.3
 eth-keys<0.5.0,>=0.4.0
 eth-typing<4.0.0,>=3.3.0
 eth-utils<3.0.0,>=2.0.0
 lru-dict>=1.1.6
-mypy_extensions<1.0.0,>=0.4.1
+mypy-extensions>=1.0.0
 py-ecc<7.0.0,>=1.4.7
 pyethash<1.0.0,>=0.1.27
 rlp<4,>=3
 trie<3,>=2.0.0
 factory-boy==2.11.1
 hypothesis<6,>=5
 pexpect<5,>=4.6
@@ -41,28 +41,29 @@
 pytest-cov==2.5.1
 pytest-timeout<2,>=1.4.2
 pytest-watch<5,>=4.1.0
 pytest-xdist==2.3.0
 flake8==6.0.0
 flake8-bugbear==23.3.23
 isort>=5.10.1
-mypy==0.971
+mypy==1.4.0
 pydocstyle>=6.0.0
 black>=23
 types-setuptools
 py-evm>=0.2.0-a.14
 pysha3<2.0.0,>=1.0.0
 Sphinx<2,>=1.5.5
 jinja2<3.1.0,>=3.0.0
 sphinx_rtd_theme>=0.1.9
 sphinxcontrib-asyncio<0.4,>=0.2.0
 towncrier<22,>=21
 
 [dev:python_version < "3.8"]
 importlib-metadata<5.0
+importlib-metadata<5.0
 
 [docs]
 py-evm>=0.2.0-a.14
 pysha3<2.0.0,>=1.0.0
 Sphinx<2,>=1.5.5
 jinja2<3.1.0,>=3.0.0
 sphinx_rtd_theme>=0.1.9
@@ -72,15 +73,15 @@
 [eth]
 cached-property<2,>=1.5.1
 eth-bloom>=1.0.3
 eth-keys<0.5.0,>=0.4.0
 eth-typing<4.0.0,>=3.3.0
 eth-utils<3.0.0,>=2.0.0
 lru-dict>=1.1.6
-mypy_extensions<1.0.0,>=0.4.1
+mypy-extensions>=1.0.0
 py-ecc<7.0.0,>=1.4.7
 pyethash<1.0.0,>=0.1.27
 rlp<4,>=3
 trie<3,>=2.0.0
 
 [eth-extra]
 blake2b-py<0.2,>=0.1.4
@@ -93,15 +94,15 @@
 [eth-extra:implementation_name == "pypy"]
 eth-hash[pycryptodome]
 
 [lint]
 flake8==6.0.0
 flake8-bugbear==23.3.23
 isort>=5.10.1
-mypy==0.971
+mypy==1.4.0
 pydocstyle>=6.0.0
 black>=23
 types-setuptools
 
 [lint:python_version < "3.8"]
 importlib-metadata<5.0
```

### Comparing `py-evm-0.7.0a3/pyproject.toml` & `py-evm-0.7.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a3/setup.py` & `py-evm-0.7.0a4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "eth": [
         "cached-property>=1.5.1,<2",
         "eth-bloom>=1.0.3",
         "eth-keys>=0.4.0,<0.5.0",
         "eth-typing>=3.3.0,<4.0.0",
         "eth-utils>=2.0.0,<3.0.0",
         "lru-dict>=1.1.6",
-        "mypy_extensions>=0.4.1,<1.0.0",
+        "mypy-extensions>=1.0.0",
         "py-ecc>=1.4.7,<7.0.0",
         "pyethash>=0.1.27,<1.0.0",
         "rlp>=3,<4",
         "trie>=2.0.0,<3",
     ],
     # The eth-extra sections is for libraries that the evm does not
     # explicitly need to function and hence should not depend on.
@@ -43,15 +43,15 @@
         "pytest-xdist==2.3.0",
         "importlib-metadata<5.0;python_version<'3.8'",
     ],
     "lint": [
         "flake8==6.0.0",  # flake8 claims semver but adds new warnings at minor releases, leave it pinned.
         "flake8-bugbear==23.3.23",  # flake8-bugbear does not follow semver, leave it pinned.
         "isort>=5.10.1",
-        "mypy==0.971",  # mypy does not follow semver, leave it pinned.
+        "mypy==1.4.0",  # mypy does not follow semver, leave it pinned.
         "pydocstyle>=6.0.0",
         "black>=23",
         "types-setuptools",
         "importlib-metadata<5.0;python_version<'3.8'",
     ],
     "benchmark": [
         "termcolor>=1.1.0,<2.0.0",
@@ -94,15 +94,15 @@
 
 with open("README.md") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="py-evm",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="0.7.0-alpha.3",
+    version="0.7.0-alpha.4",
     description="Python implementation of the Ethereum Virtual Machine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ethereum Foundation",
     author_email="piper@pipermerriam.com",
     url="https://github.com/ethereum/py-evm",
     include_package_data=True,
```

