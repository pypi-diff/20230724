# Comparing `tmp/xrpl-py-2.1.0.tar.gz` & `tmp/xrpl_py-2.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrpl-py-2.1.0.tar", max compression
+gzip compressed data, was "xrpl_py-2.1.0b0.tar", max compression
```

## Comparing `xrpl-py-2.1.0.tar` & `xrpl_py-2.1.0b0.tar`

### file list

```diff
@@ -1,223 +1,241 @@
--rw-r--r--   0        0        0      740 2022-08-01 22:16:55.908732 xrpl-py-2.1.0/LICENSE
--rw-r--r--   0        0        0    16775 2023-07-24 20:26:49.639685 xrpl-py-2.1.0/README.md
--rw-r--r--   0        0        0     2227 2023-07-24 20:34:13.683234 xrpl-py-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      348 2022-08-01 22:16:55.925560 xrpl-py-2.1.0/xrpl/__init__.py
--rw-r--r--   0        0        0      393 2023-07-24 20:26:49.657432 xrpl-py-2.1.0/xrpl/account/__init__.py
--rw-r--r--   0        0        0     3376 2023-07-24 20:26:49.657694 xrpl-py-2.1.0/xrpl/account/main.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.925802 xrpl-py-2.1.0/xrpl/account/py.typed
--rw-r--r--   0        0        0      776 2023-07-24 20:26:49.657917 xrpl-py-2.1.0/xrpl/account/transaction_history.py
--rw-r--r--   0        0        0      189 2022-08-01 22:16:55.926006 xrpl-py-2.1.0/xrpl/asyncio/__init__.py
--rw-r--r--   0        0        0      415 2023-07-24 20:26:49.658170 xrpl-py-2.1.0/xrpl/asyncio/account/__init__.py
--rw-r--r--   0        0        0     4245 2023-07-24 20:26:49.658423 xrpl-py-2.1.0/xrpl/asyncio/account/main.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.926233 xrpl-py-2.1.0/xrpl/asyncio/account/py.typed
--rw-r--r--   0        0        0     1170 2023-07-24 20:26:49.658635 xrpl-py-2.1.0/xrpl/asyncio/account/transaction_history.py
--rw-r--r--   0        0        0      705 2022-08-01 22:16:55.926434 xrpl-py-2.1.0/xrpl/asyncio/clients/__init__.py
--rw-r--r--   0        0        0      692 2022-11-29 16:02:23.639409 xrpl-py-2.1.0/xrpl/asyncio/clients/async_client.py
--rw-r--r--   0        0        0      315 2022-08-01 22:16:55.926591 xrpl-py-2.1.0/xrpl/asyncio/clients/async_json_rpc_client.py
--rw-r--r--   0        0        0     7149 2023-07-24 20:26:49.658891 xrpl-py-2.1.0/xrpl/asyncio/clients/async_websocket_client.py
--rw-r--r--   0        0        0     1189 2023-07-24 20:26:49.659060 xrpl-py-2.1.0/xrpl/asyncio/clients/client.py
--rw-r--r--   0        0        0     1083 2022-08-01 22:16:55.926861 xrpl-py-2.1.0/xrpl/asyncio/clients/exceptions.py
--rw-r--r--   0        0        0     1612 2022-11-29 16:02:23.640386 xrpl-py-2.1.0/xrpl/asyncio/clients/json_rpc_base.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.927017 xrpl-py-2.1.0/xrpl/asyncio/clients/py.typed
--rw-r--r--   0        0        0     3341 2022-08-01 22:16:55.927137 xrpl-py-2.1.0/xrpl/asyncio/clients/utils.py
--rw-r--r--   0        0        0     8173 2023-07-24 20:26:49.659506 xrpl-py-2.1.0/xrpl/asyncio/clients/websocket_base.py
--rw-r--r--   0        0        0      328 2022-08-01 22:16:55.927359 xrpl-py-2.1.0/xrpl/asyncio/ledger/__init__.py
--rw-r--r--   0        0        0     3443 2022-11-29 16:02:23.640820 xrpl-py-2.1.0/xrpl/asyncio/ledger/main.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.927497 xrpl-py-2.1.0/xrpl/asyncio/ledger/py.typed
--rw-r--r--   0        0        0     2353 2022-08-01 22:16:55.927585 xrpl-py-2.1.0/xrpl/asyncio/ledger/utils.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.927614 xrpl-py-2.1.0/xrpl/asyncio/py.typed
--rw-r--r--   0        0        0      569 2023-07-24 20:26:49.659796 xrpl-py-2.1.0/xrpl/asyncio/transaction/__init__.py
--rw-r--r--   0        0        0    17821 2023-07-24 20:26:49.660149 xrpl-py-2.1.0/xrpl/asyncio/transaction/main.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.927988 xrpl-py-2.1.0/xrpl/asyncio/transaction/py.typed
--rw-r--r--   0        0        0     8210 2023-07-24 20:26:49.660490 xrpl-py-2.1.0/xrpl/asyncio/transaction/reliable_submission.py
--rw-r--r--   0        0        0      219 2022-08-01 22:16:55.928190 xrpl-py-2.1.0/xrpl/asyncio/wallet/__init__.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.928216 xrpl-py-2.1.0/xrpl/asyncio/wallet/py.typed
--rw-r--r--   0        0        0     6614 2023-07-24 20:26:49.660740 xrpl-py-2.1.0/xrpl/asyncio/wallet/wallet_generation.py
--rw-r--r--   0        0        0      656 2022-08-01 22:16:55.928444 xrpl-py-2.1.0/xrpl/clients/__init__.py
--rw-r--r--   0        0        0      295 2022-08-01 22:16:55.928509 xrpl-py-2.1.0/xrpl/clients/json_rpc_client.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.928539 xrpl-py-2.1.0/xrpl/clients/py.typed
--rw-r--r--   0        0        0      705 2022-11-29 16:02:23.642203 xrpl-py-2.1.0/xrpl/clients/sync_client.py
--rw-r--r--   0        0        0     8893 2023-07-24 20:26:49.660994 xrpl-py-2.1.0/xrpl/clients/websocket_client.py
--rw-r--r--   0        0        0     1414 2022-08-01 22:16:55.928802 xrpl-py-2.1.0/xrpl/constants.py
--rw-r--r--   0        0        0      171 2022-08-01 22:16:55.928894 xrpl-py-2.1.0/xrpl/core/__init__.py
--rw-r--r--   0        0        0     1131 2023-07-24 20:26:49.661293 xrpl-py-2.1.0/xrpl/core/addresscodec/__init__.py
--rw-r--r--   0        0        0     7175 2022-08-01 22:16:55.929068 xrpl-py-2.1.0/xrpl/core/addresscodec/codec.py
--rw-r--r--   0        0        0      194 2022-08-01 22:16:55.929135 xrpl-py-2.1.0/xrpl/core/addresscodec/exceptions.py
--rw-r--r--   0        0        0     5735 2023-07-24 20:26:49.661564 xrpl-py-2.1.0/xrpl/core/addresscodec/main.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.929237 xrpl-py-2.1.0/xrpl/core/addresscodec/py.typed
--rw-r--r--   0        0        0      235 2022-08-01 22:16:55.929319 xrpl-py-2.1.0/xrpl/core/addresscodec/utils.py
--rw-r--r--   0        0        0      488 2022-08-01 22:16:55.929451 xrpl-py-2.1.0/xrpl/core/binarycodec/__init__.py
--rw-r--r--   0        0        0      296 2022-08-01 22:16:55.929545 xrpl-py-2.1.0/xrpl/core/binarycodec/binary_wrappers/__init__.py
--rw-r--r--   0        0        0     9076 2022-08-01 22:16:55.929653 xrpl-py-2.1.0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py
--rw-r--r--   0        0        0     4650 2022-08-01 22:16:55.929750 xrpl-py-2.1.0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py
--rw-r--r--   0        0        0     1025 2022-08-01 22:16:55.929856 xrpl-py-2.1.0/xrpl/core/binarycodec/definitions/__init__.py
--rw-r--r--   0        0        0    45270 2023-07-24 20:26:49.661930 xrpl-py-2.1.0/xrpl/core/binarycodec/definitions/definitions.json
--rw-r--r--   0        0        0     8431 2022-08-01 22:16:55.930103 xrpl-py-2.1.0/xrpl/core/binarycodec/definitions/definitions.py
--rw-r--r--   0        0        0     1870 2022-08-01 22:16:55.930170 xrpl-py-2.1.0/xrpl/core/binarycodec/definitions/field_header.py
--rw-r--r--   0        0        0     1192 2022-08-01 22:16:55.930230 xrpl-py-2.1.0/xrpl/core/binarycodec/definitions/field_info.py
--rw-r--r--   0        0        0     1931 2022-08-01 22:16:55.930297 xrpl-py-2.1.0/xrpl/core/binarycodec/definitions/field_instance.py
--rw-r--r--   0        0        0      191 2022-08-01 22:16:55.930360 xrpl-py-2.1.0/xrpl/core/binarycodec/exceptions.py
--rw-r--r--   0        0        0     3942 2022-08-01 22:16:55.930429 xrpl-py-2.1.0/xrpl/core/binarycodec/field_id_codec.py
--rw-r--r--   0        0        0     3708 2022-08-01 22:16:55.930501 xrpl-py-2.1.0/xrpl/core/binarycodec/main.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.930524 xrpl-py-2.1.0/xrpl/core/binarycodec/py.typed
--rw-r--r--   0        0        0     1255 2022-08-01 22:16:55.930618 xrpl-py-2.1.0/xrpl/core/binarycodec/types/__init__.py
--rw-r--r--   0        0        0     2956 2022-08-01 22:16:55.930695 xrpl-py-2.1.0/xrpl/core/binarycodec/types/account_id.py
--rw-r--r--   0        0        0    11513 2023-07-24 20:26:49.662253 xrpl-py-2.1.0/xrpl/core/binarycodec/types/amount.py
--rw-r--r--   0        0        0     1950 2022-08-01 22:16:55.930876 xrpl-py-2.1.0/xrpl/core/binarycodec/types/blob.py
--rw-r--r--   0        0        0     4347 2022-08-01 22:16:55.930970 xrpl-py-2.1.0/xrpl/core/binarycodec/types/currency.py
--rw-r--r--   0        0        0     2640 2022-08-01 22:16:55.931038 xrpl-py-2.1.0/xrpl/core/binarycodec/types/hash.py
--rw-r--r--   0        0        0     1494 2023-07-24 20:26:49.662615 xrpl-py-2.1.0/xrpl/core/binarycodec/types/hash128.py
--rw-r--r--   0        0        0      571 2022-08-01 22:16:55.931169 xrpl-py-2.1.0/xrpl/core/binarycodec/types/hash160.py
--rw-r--r--   0        0        0      572 2022-08-01 22:16:55.931223 xrpl-py-2.1.0/xrpl/core/binarycodec/types/hash256.py
--rw-r--r--   0        0        0     9067 2022-08-01 22:16:55.931310 xrpl-py-2.1.0/xrpl/core/binarycodec/types/path_set.py
--rw-r--r--   0        0        0     2493 2022-08-01 22:16:55.931542 xrpl-py-2.1.0/xrpl/core/binarycodec/types/serialized_type.py
--rw-r--r--   0        0        0     3301 2022-08-01 22:16:55.931629 xrpl-py-2.1.0/xrpl/core/binarycodec/types/st_array.py
--rw-r--r--   0        0        0     8392 2023-07-24 20:26:49.662876 xrpl-py-2.1.0/xrpl/core/binarycodec/types/st_object.py
--rw-r--r--   0        0        0     3383 2022-08-01 22:16:55.931813 xrpl-py-2.1.0/xrpl/core/binarycodec/types/uint.py
--rw-r--r--   0        0        0     2063 2022-08-01 22:16:55.931884 xrpl-py-2.1.0/xrpl/core/binarycodec/types/uint16.py
--rw-r--r--   0        0        0     2283 2022-08-01 22:16:55.931986 xrpl-py-2.1.0/xrpl/core/binarycodec/types/uint32.py
--rw-r--r--   0        0        0     2854 2022-08-01 22:16:55.932060 xrpl-py-2.1.0/xrpl/core/binarycodec/types/uint64.py
--rw-r--r--   0        0        0     1994 2022-08-01 22:16:55.932114 xrpl-py-2.1.0/xrpl/core/binarycodec/types/uint8.py
--rw-r--r--   0        0        0     2905 2022-08-01 22:16:55.932184 xrpl-py-2.1.0/xrpl/core/binarycodec/types/vector256.py
--rw-r--r--   0        0        0      447 2023-01-25 22:21:10.654220 xrpl-py-2.1.0/xrpl/core/keypairs/__init__.py
--rw-r--r--   0        0        0     1275 2022-08-01 22:16:55.932344 xrpl-py-2.1.0/xrpl/core/keypairs/crypto_implementation.py
--rw-r--r--   0        0        0     3662 2023-07-24 20:26:49.663141 xrpl-py-2.1.0/xrpl/core/keypairs/ed25519.py
--rw-r--r--   0        0        0      182 2022-08-01 22:16:55.932515 xrpl-py-2.1.0/xrpl/core/keypairs/exceptions.py
--rw-r--r--   0        0        0      893 2023-01-25 22:21:10.654542 xrpl-py-2.1.0/xrpl/core/keypairs/helpers.py
--rw-r--r--   0        0        0     4881 2023-07-24 20:26:49.663410 xrpl-py-2.1.0/xrpl/core/keypairs/main.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.933087 xrpl-py-2.1.0/xrpl/core/keypairs/py.typed
--rw-r--r--   0        0        0     7480 2022-08-01 22:16:55.933179 xrpl-py-2.1.0/xrpl/core/keypairs/secp256k1.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.933211 xrpl-py-2.1.0/xrpl/core/py.typed
--rw-r--r--   0        0        0      314 2022-08-01 22:16:55.933335 xrpl-py-2.1.0/xrpl/ledger/__init__.py
--rw-r--r--   0        0        0     2283 2022-08-01 22:16:55.933419 xrpl-py-2.1.0/xrpl/ledger/main.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.933450 xrpl-py-2.1.0/xrpl/ledger/py.typed
--rw-r--r--   0        0        0      858 2022-08-01 22:16:55.933578 xrpl-py-2.1.0/xrpl/models/__init__.py
--rw-r--r--   0        0        0      497 2022-08-01 22:16:55.933689 xrpl-py-2.1.0/xrpl/models/amounts/__init__.py
--rw-r--r--   0        0        0     1377 2022-08-01 22:16:55.933762 xrpl-py-2.1.0/xrpl/models/amounts/amount.py
--rw-r--r--   0        0        0     1349 2022-08-01 22:16:55.933853 xrpl-py-2.1.0/xrpl/models/amounts/issued_currency_amount.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.933882 xrpl-py-2.1.0/xrpl/models/amounts/py.typed
--rw-r--r--   0        0        0    10682 2023-07-24 20:26:49.663721 xrpl-py-2.1.0/xrpl/models/base_model.py
--rw-r--r--   0        0        0      371 2022-08-01 22:16:55.934139 xrpl-py-2.1.0/xrpl/models/currencies/__init__.py
--rw-r--r--   0        0        0      319 2022-08-01 22:16:55.934218 xrpl-py-2.1.0/xrpl/models/currencies/currency.py
--rw-r--r--   0        0        0     2237 2022-08-01 22:16:55.934282 xrpl-py-2.1.0/xrpl/models/currencies/issued_currency.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.934313 xrpl-py-2.1.0/xrpl/models/currencies/py.typed
--rw-r--r--   0        0        0     2716 2023-07-24 20:26:49.664163 xrpl-py-2.1.0/xrpl/models/currencies/xrp.py
--rw-r--r--   0        0        0      171 2022-08-01 22:16:55.934477 xrpl-py-2.1.0/xrpl/models/exceptions.py
--rw-r--r--   0        0        0     4126 2023-07-24 20:26:49.664434 xrpl-py-2.1.0/xrpl/models/flags.py
--rw-r--r--   0        0        0     2462 2022-11-29 16:02:23.642809 xrpl-py-2.1.0/xrpl/models/nested_model.py
--rw-r--r--   0        0        0     2088 2022-08-01 22:16:55.934640 xrpl-py-2.1.0/xrpl/models/path.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.934669 xrpl-py-2.1.0/xrpl/models/py.typed
--rw-r--r--   0        0        0     3607 2023-07-24 20:26:49.664763 xrpl-py-2.1.0/xrpl/models/requests/__init__.py
--rw-r--r--   0        0        0     1549 2023-07-24 20:26:49.665001 xrpl-py-2.1.0/xrpl/models/requests/account_channels.py
--rw-r--r--   0        0        0     1134 2023-07-24 20:26:49.665324 xrpl-py-2.1.0/xrpl/models/requests/account_currencies.py
--rw-r--r--   0        0        0     1088 2023-07-24 20:26:49.665607 xrpl-py-2.1.0/xrpl/models/requests/account_info.py
--rw-r--r--   0        0        0     1323 2023-07-24 20:26:49.665868 xrpl-py-2.1.0/xrpl/models/requests/account_lines.py
--rw-r--r--   0        0        0     1216 2023-07-24 20:26:49.666188 xrpl-py-2.1.0/xrpl/models/requests/account_nfts.py
--rw-r--r--   0        0        0     1738 2023-07-24 20:26:49.666467 xrpl-py-2.1.0/xrpl/models/requests/account_objects.py
--rw-r--r--   0        0        0     1161 2023-07-24 20:26:49.666705 xrpl-py-2.1.0/xrpl/models/requests/account_offers.py
--rw-r--r--   0        0        0     1207 2023-07-24 20:26:49.666991 xrpl-py-2.1.0/xrpl/models/requests/account_tx.py
--rw-r--r--   0        0        0     1024 2023-07-24 20:26:49.667535 xrpl-py-2.1.0/xrpl/models/requests/book_offers.py
--rw-r--r--   0        0        0     3020 2022-08-01 22:16:55.935564 xrpl-py-2.1.0/xrpl/models/requests/channel_authorize.py
--rw-r--r--   0        0        0     1130 2022-08-01 22:16:55.935628 xrpl-py-2.1.0/xrpl/models/requests/channel_verify.py
--rw-r--r--   0        0        0     1145 2023-07-24 20:26:49.667815 xrpl-py-2.1.0/xrpl/models/requests/deposit_authorized.py
--rw-r--r--   0        0        0      775 2022-08-01 22:16:55.935848 xrpl-py-2.1.0/xrpl/models/requests/fee.py
--rw-r--r--   0        0        0     1076 2023-07-24 20:26:49.668034 xrpl-py-2.1.0/xrpl/models/requests/gateway_balances.py
--rw-r--r--   0        0        0     3068 2022-08-01 22:16:55.936012 xrpl-py-2.1.0/xrpl/models/requests/generic_request.py
--rw-r--r--   0        0        0      887 2023-07-24 20:26:49.668331 xrpl-py-2.1.0/xrpl/models/requests/ledger.py
--rw-r--r--   0        0        0      944 2022-08-01 22:16:55.936538 xrpl-py-2.1.0/xrpl/models/requests/ledger_closed.py
--rw-r--r--   0        0        0      726 2022-08-01 22:16:55.936605 xrpl-py-2.1.0/xrpl/models/requests/ledger_current.py
--rw-r--r--   0        0        0     1190 2023-07-24 20:26:49.668568 xrpl-py-2.1.0/xrpl/models/requests/ledger_data.py
--rw-r--r--   0        0        0     5171 2023-07-24 20:26:49.668759 xrpl-py-2.1.0/xrpl/models/requests/ledger_entry.py
--rw-r--r--   0        0        0      853 2022-08-01 22:16:55.936843 xrpl-py-2.1.0/xrpl/models/requests/manifest.py
--rw-r--r--   0        0        0      809 2023-07-24 20:26:49.668941 xrpl-py-2.1.0/xrpl/models/requests/nft_buy_offers.py
--rw-r--r--   0        0        0     1184 2023-07-24 20:26:49.669038 xrpl-py-2.1.0/xrpl/models/requests/nft_history.py
--rw-r--r--   0        0        0      772 2023-07-24 20:26:49.669140 xrpl-py-2.1.0/xrpl/models/requests/nft_info.py
--rw-r--r--   0        0        0      816 2023-07-24 20:26:49.669340 xrpl-py-2.1.0/xrpl/models/requests/nft_sell_offers.py
--rw-r--r--   0        0        0     1446 2023-07-24 20:26:49.669532 xrpl-py-2.1.0/xrpl/models/requests/no_ripple_check.py
--rw-r--r--   0        0        0     4347 2022-08-01 22:16:55.937130 xrpl-py-2.1.0/xrpl/models/requests/path_find.py
--rw-r--r--   0        0        0      547 2022-08-01 22:16:55.937198 xrpl-py-2.1.0/xrpl/models/requests/ping.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.937221 xrpl-py-2.1.0/xrpl/models/requests/py.typed
--rw-r--r--   0        0        0      579 2022-08-01 22:16:55.937291 xrpl-py-2.1.0/xrpl/models/requests/random.py
--rw-r--r--   0        0        0     6234 2023-07-24 20:26:49.669750 xrpl-py-2.1.0/xrpl/models/requests/request.py
--rw-r--r--   0        0        0     2280 2023-07-24 20:26:49.669926 xrpl-py-2.1.0/xrpl/models/requests/ripple_path_find.py
--rw-r--r--   0        0        0      618 2022-08-01 22:16:55.937526 xrpl-py-2.1.0/xrpl/models/requests/server_info.py
--rw-r--r--   0        0        0     1194 2022-08-01 22:16:55.937596 xrpl-py-2.1.0/xrpl/models/requests/server_state.py
--rw-r--r--   0        0        0     4034 2022-08-01 22:16:55.937691 xrpl-py-2.1.0/xrpl/models/requests/sign.py
--rw-r--r--   0        0        0     5062 2022-08-01 22:16:55.937746 xrpl-py-2.1.0/xrpl/models/requests/sign_and_submit.py
--rw-r--r--   0        0        0     3274 2022-08-01 22:16:55.937819 xrpl-py-2.1.0/xrpl/models/requests/sign_for.py
--rw-r--r--   0        0        0     3758 2022-08-01 22:16:55.937885 xrpl-py-2.1.0/xrpl/models/requests/submit.py
--rw-r--r--   0        0        0     2478 2022-08-01 22:16:55.937960 xrpl-py-2.1.0/xrpl/models/requests/submit_multisigned.py
--rw-r--r--   0        0        0     2842 2022-08-01 22:16:55.938038 xrpl-py-2.1.0/xrpl/models/requests/submit_only.py
--rw-r--r--   0        0        0     2103 2022-08-01 22:16:55.938116 xrpl-py-2.1.0/xrpl/models/requests/subscribe.py
--rw-r--r--   0        0        0     1200 2023-07-24 20:26:49.670099 xrpl-py-2.1.0/xrpl/models/requests/transaction_entry.py
--rw-r--r--   0        0        0      817 2022-08-01 22:16:55.938266 xrpl-py-2.1.0/xrpl/models/requests/tx.py
--rw-r--r--   0        0        0     1595 2022-08-01 22:16:55.938326 xrpl-py-2.1.0/xrpl/models/requests/unsubscribe.py
--rw-r--r--   0        0        0      251 2022-08-01 22:16:55.938395 xrpl-py-2.1.0/xrpl/models/required.py
--rw-r--r--   0        0        0     3617 2022-08-01 22:16:55.938480 xrpl-py-2.1.0/xrpl/models/response.py
--rw-r--r--   0        0        0     3341 2023-07-24 20:26:49.670297 xrpl-py-2.1.0/xrpl/models/transactions/__init__.py
--rw-r--r--   0        0        0     1333 2022-08-01 22:16:55.938722 xrpl-py-2.1.0/xrpl/models/transactions/account_delete.py
--rw-r--r--   0        0        0     9705 2023-07-24 20:26:49.670485 xrpl-py-2.1.0/xrpl/models/transactions/account_set.py
--rw-r--r--   0        0        0     1101 2022-08-01 22:16:55.938922 xrpl-py-2.1.0/xrpl/models/transactions/check_cancel.py
--rw-r--r--   0        0        0     1993 2022-08-01 22:16:55.939008 xrpl-py-2.1.0/xrpl/models/transactions/check_cash.py
--rw-r--r--   0        0        0     1934 2022-08-01 22:16:55.939102 xrpl-py-2.1.0/xrpl/models/transactions/check_create.py
--rw-r--r--   0        0        0     1598 2022-08-01 22:16:55.939172 xrpl-py-2.1.0/xrpl/models/transactions/deposit_preauth.py
--rw-r--r--   0        0        0     1069 2022-08-01 22:16:55.939246 xrpl-py-2.1.0/xrpl/models/transactions/escrow_cancel.py
--rw-r--r--   0        0        0     2617 2022-08-01 22:16:55.939319 xrpl-py-2.1.0/xrpl/models/transactions/escrow_create.py
--rw-r--r--   0        0        0     2114 2022-08-01 22:16:55.939385 xrpl-py-2.1.0/xrpl/models/transactions/escrow_finish.py
--rw-r--r--   0        0        0     3163 2023-07-24 20:26:49.670644 xrpl-py-2.1.0/xrpl/models/transactions/metadata.py
--rw-r--r--   0        0        0     4537 2022-08-01 22:16:55.939537 xrpl-py-2.1.0/xrpl/models/transactions/nftoken_accept_offer.py
--rw-r--r--   0        0        0     1769 2022-08-01 22:16:55.939607 xrpl-py-2.1.0/xrpl/models/transactions/nftoken_burn.py
--rw-r--r--   0        0        0     2015 2022-08-01 22:16:55.939682 xrpl-py-2.1.0/xrpl/models/transactions/nftoken_cancel_offer.py
--rw-r--r--   0        0        0     4324 2022-08-01 22:16:55.939756 xrpl-py-2.1.0/xrpl/models/transactions/nftoken_create_offer.py
--rw-r--r--   0        0        0     4762 2022-08-01 22:16:55.939836 xrpl-py-2.1.0/xrpl/models/transactions/nftoken_mint.py
--rw-r--r--   0        0        0     1045 2022-08-01 22:16:55.939899 xrpl-py-2.1.0/xrpl/models/transactions/offer_cancel.py
--rw-r--r--   0        0        0     3866 2022-08-01 22:16:55.939972 xrpl-py-2.1.0/xrpl/models/transactions/offer_create.py
--rw-r--r--   0        0        0     5861 2022-08-01 22:16:55.940059 xrpl-py-2.1.0/xrpl/models/transactions/payment.py
--rw-r--r--   0        0        0     3917 2022-08-01 22:16:55.940128 xrpl-py-2.1.0/xrpl/models/transactions/payment_channel_claim.py
--rw-r--r--   0        0        0     2367 2022-08-01 22:16:55.940199 xrpl-py-2.1.0/xrpl/models/transactions/payment_channel_create.py
--rw-r--r--   0        0        0     1614 2022-08-01 22:16:55.940264 xrpl-py-2.1.0/xrpl/models/transactions/payment_channel_fund.py
--rw-r--r--   0        0        0      575 2022-08-01 22:16:55.940361 xrpl-py-2.1.0/xrpl/models/transactions/pseudo_transactions/__init__.py
--rw-r--r--   0        0        0     3651 2022-08-01 22:16:55.940443 xrpl-py-2.1.0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py
--rw-r--r--   0        0        0     1366 2022-08-01 22:16:55.940509 xrpl-py-2.1.0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py
--rw-r--r--   0        0        0     1874 2022-08-01 22:16:55.940572 xrpl-py-2.1.0/xrpl/models/transactions/pseudo_transactions/set_fee.py
--rw-r--r--   0        0        0     2262 2022-08-01 22:16:55.940627 xrpl-py-2.1.0/xrpl/models/transactions/pseudo_transactions/unl_modify.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.940651 xrpl-py-2.1.0/xrpl/models/transactions/py.typed
--rw-r--r--   0        0        0      959 2022-08-01 22:16:55.940741 xrpl-py-2.1.0/xrpl/models/transactions/set_regular_key.py
--rw-r--r--   0        0        0     5113 2023-07-24 20:26:49.670805 xrpl-py-2.1.0/xrpl/models/transactions/signer_list_set.py
--rw-r--r--   0        0        0      959 2022-08-01 22:16:55.940881 xrpl-py-2.1.0/xrpl/models/transactions/ticket_create.py
--rw-r--r--   0        0        0    15851 2023-07-24 20:26:49.671083 xrpl-py-2.1.0/xrpl/models/transactions/transaction.py
--rw-r--r--   0        0        0     2425 2022-08-01 22:16:55.941131 xrpl-py-2.1.0/xrpl/models/transactions/trust_set.py
--rw-r--r--   0        0        0      275 2022-08-01 22:16:55.941220 xrpl-py-2.1.0/xrpl/models/transactions/types/__init__.py
--rw-r--r--   0        0        0      287 2022-08-01 22:16:55.941278 xrpl-py-2.1.0/xrpl/models/transactions/types/pseudo_transaction_type.py
--rw-r--r--   0        0        0     1069 2022-08-01 22:16:55.941341 xrpl-py-2.1.0/xrpl/models/transactions/types/transaction_type.py
--rw-r--r--   0        0        0      749 2022-08-01 22:16:55.941399 xrpl-py-2.1.0/xrpl/models/types.py
--rw-r--r--   0        0        0     2196 2023-07-24 20:26:49.671313 xrpl-py-2.1.0/xrpl/models/utils.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.941490 xrpl-py-2.1.0/xrpl/py.typed
--rw-r--r--   0        0        0      645 2023-07-24 20:26:49.671536 xrpl-py-2.1.0/xrpl/transaction/__init__.py
--rw-r--r--   0        0        0     3614 2023-07-24 20:26:49.671847 xrpl-py-2.1.0/xrpl/transaction/main.py
--rw-r--r--   0        0        0     1216 2023-07-24 20:26:49.672055 xrpl-py-2.1.0/xrpl/transaction/multisign.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.941727 xrpl-py-2.1.0/xrpl/transaction/py.typed
--rw-r--r--   0        0        0     2092 2023-07-24 20:26:49.672267 xrpl-py-2.1.0/xrpl/transaction/reliable_submission.py
--rw-r--r--   0        0        0      839 2023-07-24 20:26:49.672471 xrpl-py-2.1.0/xrpl/utils/__init__.py
--rw-r--r--   0        0        0     4220 2023-07-24 20:26:49.672580 xrpl-py-2.1.0/xrpl/utils/get_nftoken_id.py
--rw-r--r--   0        0        0     3412 2022-08-01 22:16:55.941978 xrpl-py-2.1.0/xrpl/utils/parse_nftoken_id.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.942004 xrpl-py-2.1.0/xrpl/utils/py.typed
--rw-r--r--   0        0        0      788 2022-08-01 22:16:55.942166 xrpl-py-2.1.0/xrpl/utils/str_conversions.py
--rw-r--r--   0        0        0     4202 2022-08-01 22:16:55.942235 xrpl-py-2.1.0/xrpl/utils/time_conversions.py
--rw-r--r--   0        0        0      350 2022-08-01 22:16:55.942317 xrpl-py-2.1.0/xrpl/utils/txn_parser/__init__.py
--rw-r--r--   0        0        0     1717 2022-08-01 22:16:55.942378 xrpl-py-2.1.0/xrpl/utils/txn_parser/get_balance_changes.py
--rw-r--r--   0        0        0     1446 2022-08-01 22:16:55.942431 xrpl-py-2.1.0/xrpl/utils/txn_parser/get_final_balances.py
--rw-r--r--   0        0        0      641 2022-08-01 22:16:55.942490 xrpl-py-2.1.0/xrpl/utils/txn_parser/get_order_book_changes.py
--rw-r--r--   0        0        0      627 2022-08-01 22:16:55.942573 xrpl-py-2.1.0/xrpl/utils/txn_parser/utils/__init__.py
--rw-r--r--   0        0        0     5218 2022-08-01 22:16:55.942661 xrpl-py-2.1.0/xrpl/utils/txn_parser/utils/balance_parser.py
--rw-r--r--   0        0        0     2518 2023-01-25 22:21:10.656015 xrpl-py-2.1.0/xrpl/utils/txn_parser/utils/nodes.py
--rw-r--r--   0        0        0     6191 2022-08-01 22:16:55.942800 xrpl-py-2.1.0/xrpl/utils/txn_parser/utils/order_book_parser.py
--rw-r--r--   0        0        0     1192 2022-08-01 22:16:55.942856 xrpl-py-2.1.0/xrpl/utils/txn_parser/utils/parser.py
--rw-r--r--   0        0        0     1404 2023-01-25 22:21:10.656234 xrpl-py-2.1.0/xrpl/utils/txn_parser/utils/types.py
--rw-r--r--   0        0        0     3476 2022-08-01 22:16:55.942981 xrpl-py-2.1.0/xrpl/utils/xrp_conversions.py
--rw-r--r--   0        0        0      269 2022-08-01 22:16:55.943073 xrpl-py-2.1.0/xrpl/wallet/__init__.py
--rw-r--r--   0        0        0     9439 2023-07-24 20:26:49.672779 xrpl-py-2.1.0/xrpl/wallet/main.py
--rw-r--r--   0        0        0        0 2022-08-01 22:16:55.943167 xrpl-py-2.1.0/xrpl/wallet/py.typed
--rw-r--r--   0        0        0     1639 2023-07-24 20:26:49.672948 xrpl-py-2.1.0/xrpl/wallet/wallet_generation.py
--rw-r--r--   0        0        0    19064 2023-07-24 20:34:27.741794 xrpl-py-2.1.0/setup.py
--rw-r--r--   0        0        0    18010 2023-07-24 20:34:27.742501 xrpl-py-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      740 2022-08-01 03:07:06.902817 xrpl_py-2.1.0b0/LICENSE
+-rw-r--r--   0        0        0    16001 2023-07-10 17:12:46.149667 xrpl_py-2.1.0b0/README.md
+-rw-r--r--   0        0        0     2229 2023-07-10 17:42:47.452415 xrpl_py-2.1.0b0/pyproject.toml
+-rw-r--r--   0        0        0      348 2022-08-01 03:07:06.915966 xrpl_py-2.1.0b0/xrpl/__init__.py
+-rw-r--r--   0        0        0      393 2023-07-10 17:12:46.163012 xrpl_py-2.1.0b0/xrpl/account/__init__.py
+-rw-r--r--   0        0        0     3376 2023-07-10 17:12:46.163184 xrpl_py-2.1.0b0/xrpl/account/main.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.916219 xrpl_py-2.1.0b0/xrpl/account/py.typed
+-rw-r--r--   0        0        0      776 2023-07-10 17:12:46.163338 xrpl_py-2.1.0b0/xrpl/account/transaction_history.py
+-rw-r--r--   0        0        0      189 2022-08-01 03:07:06.916458 xrpl_py-2.1.0b0/xrpl/asyncio/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-10 17:12:46.163581 xrpl_py-2.1.0b0/xrpl/asyncio/account/__init__.py
+-rw-r--r--   0        0        0     4245 2023-07-10 17:12:46.163782 xrpl_py-2.1.0b0/xrpl/asyncio/account/main.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.916659 xrpl_py-2.1.0b0/xrpl/asyncio/account/py.typed
+-rw-r--r--   0        0        0     1170 2023-07-10 17:12:46.163955 xrpl_py-2.1.0b0/xrpl/asyncio/account/transaction_history.py
+-rw-r--r--   0        0        0      705 2022-08-01 03:07:06.916816 xrpl_py-2.1.0b0/xrpl/asyncio/clients/__init__.py
+-rw-r--r--   0        0        0      692 2023-01-09 23:03:27.485595 xrpl_py-2.1.0b0/xrpl/asyncio/clients/async_client.py
+-rw-r--r--   0        0        0      315 2022-08-01 03:07:06.916941 xrpl_py-2.1.0b0/xrpl/asyncio/clients/async_json_rpc_client.py
+-rw-r--r--   0        0        0     7149 2023-05-23 16:51:49.263971 xrpl_py-2.1.0b0/xrpl/asyncio/clients/async_websocket_client.py
+-rw-r--r--   0        0        0     1189 2023-07-10 17:12:46.164105 xrpl_py-2.1.0b0/xrpl/asyncio/clients/client.py
+-rw-r--r--   0        0        0     1083 2022-08-01 03:07:06.917148 xrpl_py-2.1.0b0/xrpl/asyncio/clients/exceptions.py
+-rw-r--r--   0        0        0     1612 2023-01-09 23:03:27.486437 xrpl_py-2.1.0b0/xrpl/asyncio/clients/json_rpc_base.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.917264 xrpl_py-2.1.0b0/xrpl/asyncio/clients/py.typed
+-rw-r--r--   0        0        0     3341 2022-08-01 03:07:06.917343 xrpl_py-2.1.0b0/xrpl/asyncio/clients/utils.py
+-rw-r--r--   0        0        0     8173 2023-05-23 16:51:49.264461 xrpl_py-2.1.0b0/xrpl/asyncio/clients/websocket_base.py
+-rw-r--r--   0        0        0      328 2022-08-01 03:07:06.917510 xrpl_py-2.1.0b0/xrpl/asyncio/ledger/__init__.py
+-rw-r--r--   0        0        0     3443 2023-01-09 23:03:27.487487 xrpl_py-2.1.0b0/xrpl/asyncio/ledger/main.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.917612 xrpl_py-2.1.0b0/xrpl/asyncio/ledger/py.typed
+-rw-r--r--   0        0        0     2353 2022-08-01 03:07:06.917676 xrpl_py-2.1.0b0/xrpl/asyncio/ledger/utils.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.917699 xrpl_py-2.1.0b0/xrpl/asyncio/py.typed
+-rw-r--r--   0        0        0      569 2023-07-10 17:12:46.164296 xrpl_py-2.1.0b0/xrpl/asyncio/transaction/__init__.py
+-rw-r--r--   0        0        0    17903 2023-07-10 17:12:46.164855 xrpl_py-2.1.0b0/xrpl/asyncio/transaction/main.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.917997 xrpl_py-2.1.0b0/xrpl/asyncio/transaction/py.typed
+-rw-r--r--   0        0        0     8210 2023-07-10 17:12:46.165121 xrpl_py-2.1.0b0/xrpl/asyncio/transaction/reliable_submission.py
+-rw-r--r--   0        0        0      219 2022-08-01 03:07:06.918169 xrpl_py-2.1.0b0/xrpl/asyncio/wallet/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.918193 xrpl_py-2.1.0b0/xrpl/asyncio/wallet/py.typed
+-rw-r--r--   0        0        0     6614 2023-07-10 17:12:46.165310 xrpl_py-2.1.0b0/xrpl/asyncio/wallet/wallet_generation.py
+-rw-r--r--   0        0        0      656 2022-08-01 03:07:06.918352 xrpl_py-2.1.0b0/xrpl/clients/__init__.py
+-rw-r--r--   0        0        0      295 2022-08-01 03:07:06.918414 xrpl_py-2.1.0b0/xrpl/clients/json_rpc_client.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.918443 xrpl_py-2.1.0b0/xrpl/clients/py.typed
+-rw-r--r--   0        0        0      705 2023-01-09 23:03:27.488832 xrpl_py-2.1.0b0/xrpl/clients/sync_client.py
+-rw-r--r--   0        0        0     8893 2023-05-23 16:51:49.266224 xrpl_py-2.1.0b0/xrpl/clients/websocket_client.py
+-rw-r--r--   0        0        0     1414 2022-08-01 03:07:06.918722 xrpl_py-2.1.0b0/xrpl/constants.py
+-rw-r--r--   0        0        0      171 2022-08-01 03:07:06.918808 xrpl_py-2.1.0b0/xrpl/core/__init__.py
+-rw-r--r--   0        0        0     1131 2023-07-10 17:12:46.165519 xrpl_py-2.1.0b0/xrpl/core/addresscodec/__init__.py
+-rw-r--r--   0        0        0     7175 2022-08-01 03:07:06.918953 xrpl_py-2.1.0b0/xrpl/core/addresscodec/codec.py
+-rw-r--r--   0        0        0      194 2022-08-01 03:07:06.919006 xrpl_py-2.1.0b0/xrpl/core/addresscodec/exceptions.py
+-rw-r--r--   0        0        0     5735 2023-07-10 17:12:46.165893 xrpl_py-2.1.0b0/xrpl/core/addresscodec/main.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.919094 xrpl_py-2.1.0b0/xrpl/core/addresscodec/py.typed
+-rw-r--r--   0        0        0      235 2022-08-01 03:07:06.919150 xrpl_py-2.1.0b0/xrpl/core/addresscodec/utils.py
+-rw-r--r--   0        0        0      488 2022-08-01 03:07:06.919229 xrpl_py-2.1.0b0/xrpl/core/binarycodec/__init__.py
+-rw-r--r--   0        0        0      296 2022-08-01 03:07:06.919308 xrpl_py-2.1.0b0/xrpl/core/binarycodec/binary_wrappers/__init__.py
+-rw-r--r--   0        0        0     9076 2022-08-01 03:07:06.919401 xrpl_py-2.1.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py
+-rw-r--r--   0        0        0     4650 2022-08-01 03:07:06.919480 xrpl_py-2.1.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py
+-rw-r--r--   0        0        0     1025 2022-08-01 03:07:06.919564 xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/__init__.py
+-rw-r--r--   0        0        0    56327 2023-07-10 16:48:55.570924 xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/definitions.json
+-rw-r--r--   0        0        0     8431 2022-08-01 03:07:06.919791 xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/definitions.py
+-rw-r--r--   0        0        0     2060 2023-07-10 16:48:55.571160 xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_header.py
+-rw-r--r--   0        0        0     1192 2022-08-01 03:07:06.919903 xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_info.py
+-rw-r--r--   0        0        0     1931 2022-08-01 03:07:06.919964 xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_instance.py
+-rw-r--r--   0        0        0      191 2022-08-01 03:07:06.920016 xrpl_py-2.1.0b0/xrpl/core/binarycodec/exceptions.py
+-rw-r--r--   0        0        0     3942 2022-08-01 03:07:06.920077 xrpl_py-2.1.0b0/xrpl/core/binarycodec/field_id_codec.py
+-rw-r--r--   0        0        0     3898 2023-07-10 16:48:55.571442 xrpl_py-2.1.0b0/xrpl/core/binarycodec/main.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.920169 xrpl_py-2.1.0b0/xrpl/core/binarycodec/py.typed
+-rw-r--r--   0        0        0     1407 2023-07-10 16:48:55.571638 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/__init__.py
+-rw-r--r--   0        0        0     2956 2022-08-01 03:07:06.920334 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/account_id.py
+-rw-r--r--   0        0        0    11513 2023-05-23 16:51:49.266730 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/amount.py
+-rw-r--r--   0        0        0     1950 2022-08-01 03:07:06.920520 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/blob.py
+-rw-r--r--   0        0        0     4347 2022-08-01 03:07:06.920602 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/currency.py
+-rw-r--r--   0        0        0     2640 2022-08-01 03:07:06.920654 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash.py
+-rw-r--r--   0        0        0     1494 2023-02-15 23:24:27.094208 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash128.py
+-rw-r--r--   0        0        0      571 2022-08-01 03:07:06.920764 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash160.py
+-rw-r--r--   0        0        0      572 2022-08-01 03:07:06.920890 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash256.py
+-rw-r--r--   0        0        0     3325 2023-07-10 16:48:55.572074 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/issue.py
+-rw-r--r--   0        0        0     3335 2023-07-10 16:48:55.572315 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/issued_currency.py
+-rw-r--r--   0        0        0     9067 2022-08-01 03:07:06.921018 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/path_set.py
+-rw-r--r--   0        0        0     2493 2022-08-01 03:07:06.921099 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/serialized_type.py
+-rw-r--r--   0        0        0     3301 2022-08-01 03:07:06.921166 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/st_array.py
+-rw-r--r--   0        0        0     8392 2023-05-23 16:51:49.267029 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/st_object.py
+-rw-r--r--   0        0        0     3383 2022-08-01 03:07:06.921335 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint.py
+-rw-r--r--   0        0        0     2063 2022-08-01 03:07:06.921397 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint16.py
+-rw-r--r--   0        0        0     2283 2022-08-01 03:07:06.921488 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint32.py
+-rw-r--r--   0        0        0     2854 2022-08-01 03:07:06.921562 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint64.py
+-rw-r--r--   0        0        0     1994 2022-08-01 03:07:06.921617 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint8.py
+-rw-r--r--   0        0        0     2905 2022-08-01 03:07:06.921683 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/vector256.py
+-rw-r--r--   0        0        0     3407 2023-07-10 16:48:55.572418 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/xchain_bridge.py
+-rw-r--r--   0        0        0      447 2023-01-09 23:03:27.489834 xrpl_py-2.1.0b0/xrpl/core/keypairs/__init__.py
+-rw-r--r--   0        0        0     1275 2022-08-01 03:07:06.921836 xrpl_py-2.1.0b0/xrpl/core/keypairs/crypto_implementation.py
+-rw-r--r--   0        0        0     3662 2023-07-10 17:12:46.166050 xrpl_py-2.1.0b0/xrpl/core/keypairs/ed25519.py
+-rw-r--r--   0        0        0      182 2022-08-01 03:07:06.921991 xrpl_py-2.1.0b0/xrpl/core/keypairs/exceptions.py
+-rw-r--r--   0        0        0      893 2023-01-09 23:03:27.490087 xrpl_py-2.1.0b0/xrpl/core/keypairs/helpers.py
+-rw-r--r--   0        0        0     4881 2023-07-10 17:12:46.166195 xrpl_py-2.1.0b0/xrpl/core/keypairs/main.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.922143 xrpl_py-2.1.0b0/xrpl/core/keypairs/py.typed
+-rw-r--r--   0        0        0     7480 2022-08-01 03:07:06.922211 xrpl_py-2.1.0b0/xrpl/core/keypairs/secp256k1.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.922235 xrpl_py-2.1.0b0/xrpl/core/py.typed
+-rw-r--r--   0        0        0      314 2022-08-01 03:07:06.922326 xrpl_py-2.1.0b0/xrpl/ledger/__init__.py
+-rw-r--r--   0        0        0     2283 2022-08-01 03:07:06.922387 xrpl_py-2.1.0b0/xrpl/ledger/main.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.922410 xrpl_py-2.1.0b0/xrpl/ledger/py.typed
+-rw-r--r--   0        0        0      997 2023-07-10 16:48:55.573510 xrpl_py-2.1.0b0/xrpl/models/__init__.py
+-rw-r--r--   0        0        0      497 2022-08-01 03:07:06.922581 xrpl_py-2.1.0b0/xrpl/models/amounts/__init__.py
+-rw-r--r--   0        0        0     1377 2022-08-01 03:07:06.922638 xrpl_py-2.1.0b0/xrpl/models/amounts/amount.py
+-rw-r--r--   0        0        0     1349 2022-09-14 22:10:28.650164 xrpl_py-2.1.0b0/xrpl/models/amounts/issued_currency_amount.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.922737 xrpl_py-2.1.0b0/xrpl/models/amounts/py.typed
+-rw-r--r--   0        0        0     2319 2023-07-10 16:48:55.573804 xrpl_py-2.1.0b0/xrpl/models/auth_account.py
+-rw-r--r--   0        0        0    11037 2023-07-10 16:48:55.574109 xrpl_py-2.1.0b0/xrpl/models/base_model.py
+-rw-r--r--   0        0        0      371 2023-02-23 18:51:59.114959 xrpl_py-2.1.0b0/xrpl/models/currencies/__init__.py
+-rw-r--r--   0        0        0      319 2022-11-17 15:10:10.681283 xrpl_py-2.1.0b0/xrpl/models/currencies/currency.py
+-rw-r--r--   0        0        0     2237 2022-08-01 03:07:06.923061 xrpl_py-2.1.0b0/xrpl/models/currencies/issued_currency.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.923083 xrpl_py-2.1.0b0/xrpl/models/currencies/py.typed
+-rw-r--r--   0        0        0     2918 2023-07-10 17:12:46.166342 xrpl_py-2.1.0b0/xrpl/models/currencies/xrp.py
+-rw-r--r--   0        0        0      171 2022-08-01 03:07:06.923203 xrpl_py-2.1.0b0/xrpl/models/exceptions.py
+-rw-r--r--   0        0        0     4661 2023-07-10 17:12:46.166725 xrpl_py-2.1.0b0/xrpl/models/flags.py
+-rw-r--r--   0        0        0     2462 2023-01-09 23:03:27.490815 xrpl_py-2.1.0b0/xrpl/models/nested_model.py
+-rw-r--r--   0        0        0     2088 2022-09-15 01:11:48.323392 xrpl_py-2.1.0b0/xrpl/models/path.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.923353 xrpl_py-2.1.0b0/xrpl/models/py.typed
+-rw-r--r--   0        0        0     3740 2023-07-10 16:48:55.575204 xrpl_py-2.1.0b0/xrpl/models/requests/__init__.py
+-rw-r--r--   0        0        0     1549 2023-07-10 17:12:46.166921 xrpl_py-2.1.0b0/xrpl/models/requests/account_channels.py
+-rw-r--r--   0        0        0     1134 2023-07-10 17:12:46.167126 xrpl_py-2.1.0b0/xrpl/models/requests/account_currencies.py
+-rw-r--r--   0        0        0     1088 2023-07-10 17:12:46.167293 xrpl_py-2.1.0b0/xrpl/models/requests/account_info.py
+-rw-r--r--   0        0        0     1323 2023-07-10 17:12:46.167456 xrpl_py-2.1.0b0/xrpl/models/requests/account_lines.py
+-rw-r--r--   0        0        0     1216 2023-07-10 17:12:46.167656 xrpl_py-2.1.0b0/xrpl/models/requests/account_nfts.py
+-rw-r--r--   0        0        0     1894 2023-07-10 17:12:46.168085 xrpl_py-2.1.0b0/xrpl/models/requests/account_objects.py
+-rw-r--r--   0        0        0     1161 2023-07-10 17:12:46.168281 xrpl_py-2.1.0b0/xrpl/models/requests/account_offers.py
+-rw-r--r--   0        0        0     1207 2023-07-10 17:12:46.168502 xrpl_py-2.1.0b0/xrpl/models/requests/account_tx.py
+-rw-r--r--   0        0        0     1017 2023-07-10 16:48:55.577338 xrpl_py-2.1.0b0/xrpl/models/requests/amm_info.py
+-rw-r--r--   0        0        0     1024 2023-07-10 17:12:46.168659 xrpl_py-2.1.0b0/xrpl/models/requests/book_offers.py
+-rw-r--r--   0        0        0     3048 2023-07-10 16:48:55.577739 xrpl_py-2.1.0b0/xrpl/models/requests/channel_authorize.py
+-rw-r--r--   0        0        0     1158 2023-07-10 16:48:55.578010 xrpl_py-2.1.0b0/xrpl/models/requests/channel_verify.py
+-rw-r--r--   0        0        0     1145 2023-07-10 17:12:46.168920 xrpl_py-2.1.0b0/xrpl/models/requests/deposit_authorized.py
+-rw-r--r--   0        0        0      775 2022-08-01 03:07:06.924306 xrpl_py-2.1.0b0/xrpl/models/requests/fee.py
+-rw-r--r--   0        0        0     1076 2023-07-10 17:12:46.169151 xrpl_py-2.1.0b0/xrpl/models/requests/gateway_balances.py
+-rw-r--r--   0        0        0     3068 2022-08-01 03:07:06.924450 xrpl_py-2.1.0b0/xrpl/models/requests/generic_request.py
+-rw-r--r--   0        0        0      887 2023-07-10 17:12:46.169383 xrpl_py-2.1.0b0/xrpl/models/requests/ledger.py
+-rw-r--r--   0        0        0      944 2022-08-01 03:07:06.924563 xrpl_py-2.1.0b0/xrpl/models/requests/ledger_closed.py
+-rw-r--r--   0        0        0      726 2022-08-01 03:07:06.924621 xrpl_py-2.1.0b0/xrpl/models/requests/ledger_current.py
+-rw-r--r--   0        0        0     1190 2023-07-10 17:12:46.169752 xrpl_py-2.1.0b0/xrpl/models/requests/ledger_data.py
+-rw-r--r--   0        0        0     6160 2023-07-10 17:12:46.170014 xrpl_py-2.1.0b0/xrpl/models/requests/ledger_entry.py
+-rw-r--r--   0        0        0      853 2022-08-01 03:07:06.924810 xrpl_py-2.1.0b0/xrpl/models/requests/manifest.py
+-rw-r--r--   0        0        0      809 2023-07-10 17:12:46.170217 xrpl_py-2.1.0b0/xrpl/models/requests/nft_buy_offers.py
+-rw-r--r--   0        0        0     1184 2023-07-10 17:12:46.170408 xrpl_py-2.1.0b0/xrpl/models/requests/nft_history.py
+-rw-r--r--   0        0        0      772 2023-07-10 17:12:46.170596 xrpl_py-2.1.0b0/xrpl/models/requests/nft_info.py
+-rw-r--r--   0        0        0      816 2023-07-10 17:12:46.170821 xrpl_py-2.1.0b0/xrpl/models/requests/nft_sell_offers.py
+-rw-r--r--   0        0        0     1446 2023-07-10 17:12:46.171216 xrpl_py-2.1.0b0/xrpl/models/requests/no_ripple_check.py
+-rw-r--r--   0        0        0     4347 2022-08-01 03:07:06.925088 xrpl_py-2.1.0b0/xrpl/models/requests/path_find.py
+-rw-r--r--   0        0        0      547 2022-08-01 03:07:06.925142 xrpl_py-2.1.0b0/xrpl/models/requests/ping.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.925165 xrpl_py-2.1.0b0/xrpl/models/requests/py.typed
+-rw-r--r--   0        0        0      579 2022-08-01 03:07:06.925223 xrpl_py-2.1.0b0/xrpl/models/requests/random.py
+-rw-r--r--   0        0        0     6279 2023-07-10 17:12:46.171586 xrpl_py-2.1.0b0/xrpl/models/requests/request.py
+-rw-r--r--   0        0        0     2280 2023-07-10 17:12:46.171767 xrpl_py-2.1.0b0/xrpl/models/requests/ripple_path_find.py
+-rw-r--r--   0        0        0      618 2022-08-01 03:07:06.925432 xrpl_py-2.1.0b0/xrpl/models/requests/server_info.py
+-rw-r--r--   0        0        0     1194 2022-08-01 03:07:06.925493 xrpl_py-2.1.0b0/xrpl/models/requests/server_state.py
+-rw-r--r--   0        0        0     4034 2022-08-01 03:07:06.925582 xrpl_py-2.1.0b0/xrpl/models/requests/sign.py
+-rw-r--r--   0        0        0     5062 2022-08-01 03:07:06.925632 xrpl_py-2.1.0b0/xrpl/models/requests/sign_and_submit.py
+-rw-r--r--   0        0        0     3274 2022-08-01 03:07:06.925686 xrpl_py-2.1.0b0/xrpl/models/requests/sign_for.py
+-rw-r--r--   0        0        0     3758 2022-08-01 03:07:06.925767 xrpl_py-2.1.0b0/xrpl/models/requests/submit.py
+-rw-r--r--   0        0        0     2478 2022-08-01 03:07:06.925860 xrpl_py-2.1.0b0/xrpl/models/requests/submit_multisigned.py
+-rw-r--r--   0        0        0     2842 2022-08-01 03:07:06.925936 xrpl_py-2.1.0b0/xrpl/models/requests/submit_only.py
+-rw-r--r--   0        0        0     2103 2022-08-01 03:07:06.926016 xrpl_py-2.1.0b0/xrpl/models/requests/subscribe.py
+-rw-r--r--   0        0        0     1200 2023-07-10 17:12:46.171975 xrpl_py-2.1.0b0/xrpl/models/requests/transaction_entry.py
+-rw-r--r--   0        0        0      817 2022-08-01 03:07:06.926139 xrpl_py-2.1.0b0/xrpl/models/requests/tx.py
+-rw-r--r--   0        0        0     1595 2022-08-01 03:07:06.926195 xrpl_py-2.1.0b0/xrpl/models/requests/unsubscribe.py
+-rw-r--r--   0        0        0      251 2022-08-01 03:07:06.926255 xrpl_py-2.1.0b0/xrpl/models/required.py
+-rw-r--r--   0        0        0     3617 2022-08-01 03:07:06.926326 xrpl_py-2.1.0b0/xrpl/models/response.py
+-rw-r--r--   0        0        0     5016 2023-07-10 17:12:46.172406 xrpl_py-2.1.0b0/xrpl/models/transactions/__init__.py
+-rw-r--r--   0        0        0     1333 2022-08-01 03:07:06.926509 xrpl_py-2.1.0b0/xrpl/models/transactions/account_delete.py
+-rw-r--r--   0        0        0     9705 2023-07-10 17:12:46.172625 xrpl_py-2.1.0b0/xrpl/models/transactions/account_set.py
+-rw-r--r--   0        0        0     2644 2023-07-10 16:48:55.581988 xrpl_py-2.1.0b0/xrpl/models/transactions/amm_bid.py
+-rw-r--r--   0        0        0     2135 2023-07-10 16:48:55.582269 xrpl_py-2.1.0b0/xrpl/models/transactions/amm_create.py
+-rw-r--r--   0        0        0     3164 2023-07-10 16:48:55.582630 xrpl_py-2.1.0b0/xrpl/models/transactions/amm_deposit.py
+-rw-r--r--   0        0        0     1984 2023-07-10 16:48:55.582934 xrpl_py-2.1.0b0/xrpl/models/transactions/amm_vote.py
+-rw-r--r--   0        0        0     3286 2023-07-10 16:48:55.583236 xrpl_py-2.1.0b0/xrpl/models/transactions/amm_withdraw.py
+-rw-r--r--   0        0        0     1101 2022-08-01 03:07:06.926693 xrpl_py-2.1.0b0/xrpl/models/transactions/check_cancel.py
+-rw-r--r--   0        0        0     1993 2022-08-01 03:07:06.926771 xrpl_py-2.1.0b0/xrpl/models/transactions/check_cash.py
+-rw-r--r--   0        0        0     1934 2022-08-01 03:07:06.926860 xrpl_py-2.1.0b0/xrpl/models/transactions/check_create.py
+-rw-r--r--   0        0        0     1598 2022-08-01 03:07:06.926937 xrpl_py-2.1.0b0/xrpl/models/transactions/deposit_preauth.py
+-rw-r--r--   0        0        0     1072 2023-07-10 16:48:55.583461 xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_cancel.py
+-rw-r--r--   0        0        0     2751 2023-07-10 16:48:55.583638 xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_create.py
+-rw-r--r--   0        0        0     2114 2022-08-01 03:07:06.927180 xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_finish.py
+-rw-r--r--   0        0        0     3163 2023-05-23 16:51:49.269564 xrpl_py-2.1.0b0/xrpl/models/transactions/metadata.py
+-rw-r--r--   0        0        0     4537 2022-08-01 03:07:06.927331 xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_accept_offer.py
+-rw-r--r--   0        0        0     1769 2022-08-01 03:07:06.927408 xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_burn.py
+-rw-r--r--   0        0        0     2015 2022-08-01 03:07:06.927486 xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_cancel_offer.py
+-rw-r--r--   0        0        0     4324 2022-08-01 03:07:06.927560 xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_create_offer.py
+-rw-r--r--   0        0        0     4762 2022-08-09 19:51:34.686117 xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_mint.py
+-rw-r--r--   0        0        0     1045 2022-08-01 03:07:06.927715 xrpl_py-2.1.0b0/xrpl/models/transactions/offer_cancel.py
+-rw-r--r--   0        0        0     3866 2022-08-01 03:07:06.927795 xrpl_py-2.1.0b0/xrpl/models/transactions/offer_create.py
+-rw-r--r--   0        0        0     5861 2022-08-01 03:07:06.927880 xrpl_py-2.1.0b0/xrpl/models/transactions/payment.py
+-rw-r--r--   0        0        0     4227 2023-07-10 16:48:55.583810 xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_claim.py
+-rw-r--r--   0        0        0     2569 2023-07-10 16:48:55.583967 xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_create.py
+-rw-r--r--   0        0        0     1660 2023-07-10 16:48:55.584128 xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_fund.py
+-rw-r--r--   0        0        0      575 2022-08-01 03:07:06.928228 xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py
+-rw-r--r--   0        0        0     3651 2022-08-01 03:07:06.928326 xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py
+-rw-r--r--   0        0        0     1366 2022-08-01 03:07:06.928402 xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py
+-rw-r--r--   0        0        0     1874 2022-08-01 03:07:06.928467 xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py
+-rw-r--r--   0        0        0     2262 2022-08-01 03:07:06.928526 xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.928554 xrpl_py-2.1.0b0/xrpl/models/transactions/py.typed
+-rw-r--r--   0        0        0      959 2022-08-01 03:07:06.928643 xrpl_py-2.1.0b0/xrpl/models/transactions/set_regular_key.py
+-rw-r--r--   0        0        0     5113 2023-06-07 18:37:48.861498 xrpl_py-2.1.0b0/xrpl/models/transactions/signer_list_set.py
+-rw-r--r--   0        0        0      959 2022-08-01 03:07:06.928817 xrpl_py-2.1.0b0/xrpl/models/transactions/ticket_create.py
+-rw-r--r--   0        0        0    15955 2023-07-10 17:12:46.173127 xrpl_py-2.1.0b0/xrpl/models/transactions/transaction.py
+-rw-r--r--   0        0        0     2425 2022-08-01 03:07:06.929079 xrpl_py-2.1.0b0/xrpl/models/transactions/trust_set.py
+-rw-r--r--   0        0        0      275 2022-08-01 03:07:06.929186 xrpl_py-2.1.0b0/xrpl/models/transactions/types/__init__.py
+-rw-r--r--   0        0        0      287 2022-08-01 03:07:06.929265 xrpl_py-2.1.0b0/xrpl/models/transactions/types/pseudo_transaction_type.py
+-rw-r--r--   0        0        0     1631 2023-07-10 16:48:55.584619 xrpl_py-2.1.0b0/xrpl/models/transactions/types/transaction_type.py
+-rw-r--r--   0        0        0     2236 2023-07-10 16:48:55.584718 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_account_create_commit.py
+-rw-r--r--   0        0        0     3283 2023-07-10 16:48:55.584824 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_add_account_create_attestation.py
+-rw-r--r--   0        0        0     3011 2023-07-10 16:48:55.584928 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_add_claim_attestation.py
+-rw-r--r--   0        0        0     2690 2023-07-10 16:48:55.585019 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_claim.py
+-rw-r--r--   0        0        0     2235 2023-07-10 16:48:55.585114 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_commit.py
+-rw-r--r--   0        0        0     3225 2023-07-10 16:48:55.585229 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_create_bridge.py
+-rw-r--r--   0        0        0     2169 2023-07-10 16:48:55.585329 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_create_claim_id.py
+-rw-r--r--   0        0        0     3388 2023-07-10 16:48:55.585409 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_modify_bridge.py
+-rw-r--r--   0        0        0      749 2022-08-01 03:07:06.929418 xrpl_py-2.1.0b0/xrpl/models/types.py
+-rw-r--r--   0        0        0     2196 2023-05-23 16:51:49.272002 xrpl_py-2.1.0b0/xrpl/models/utils.py
+-rw-r--r--   0        0        0     1097 2023-07-10 16:48:55.585500 xrpl_py-2.1.0b0/xrpl/models/xchain_bridge.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.929533 xrpl_py-2.1.0b0/xrpl/py.typed
+-rw-r--r--   0        0        0      645 2023-07-10 17:12:46.173358 xrpl_py-2.1.0b0/xrpl/transaction/__init__.py
+-rw-r--r--   0        0        0     3614 2023-07-10 17:12:46.173633 xrpl_py-2.1.0b0/xrpl/transaction/main.py
+-rw-r--r--   0        0        0     1216 2023-07-10 17:12:46.173829 xrpl_py-2.1.0b0/xrpl/transaction/multisign.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.929779 xrpl_py-2.1.0b0/xrpl/transaction/py.typed
+-rw-r--r--   0        0        0     2092 2023-07-10 17:12:46.174053 xrpl_py-2.1.0b0/xrpl/transaction/reliable_submission.py
+-rw-r--r--   0        0        0      839 2023-05-23 16:51:49.273697 xrpl_py-2.1.0b0/xrpl/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2023-05-23 16:51:49.273844 xrpl_py-2.1.0b0/xrpl/utils/get_nftoken_id.py
+-rw-r--r--   0        0        0     3412 2022-08-01 03:07:06.930042 xrpl_py-2.1.0b0/xrpl/utils/parse_nftoken_id.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.930069 xrpl_py-2.1.0b0/xrpl/utils/py.typed
+-rw-r--r--   0        0        0      788 2022-08-01 03:07:06.930218 xrpl_py-2.1.0b0/xrpl/utils/str_conversions.py
+-rw-r--r--   0        0        0     4202 2022-08-01 03:07:06.930296 xrpl_py-2.1.0b0/xrpl/utils/time_conversions.py
+-rw-r--r--   0        0        0      350 2022-08-01 03:07:06.930405 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/__init__.py
+-rw-r--r--   0        0        0     1717 2022-08-01 03:07:06.930477 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_balance_changes.py
+-rw-r--r--   0        0        0     1446 2022-08-01 03:07:06.930538 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_final_balances.py
+-rw-r--r--   0        0        0      641 2022-08-01 03:07:06.930603 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_order_book_changes.py
+-rw-r--r--   0        0        0      627 2022-08-01 03:07:06.930692 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/__init__.py
+-rw-r--r--   0        0        0     5218 2022-08-01 03:07:06.930789 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/balance_parser.py
+-rw-r--r--   0        0        0     2518 2023-01-09 23:03:27.494325 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/nodes.py
+-rw-r--r--   0        0        0     6191 2022-08-01 03:07:06.930936 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py
+-rw-r--r--   0        0        0     1192 2022-08-01 03:07:06.931006 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/parser.py
+-rw-r--r--   0        0        0     1404 2023-01-09 23:03:27.494567 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/types.py
+-rw-r--r--   0        0        0     3476 2022-08-01 03:07:06.931171 xrpl_py-2.1.0b0/xrpl/utils/xrp_conversions.py
+-rw-r--r--   0        0        0      269 2022-08-01 03:07:06.931262 xrpl_py-2.1.0b0/xrpl/wallet/__init__.py
+-rw-r--r--   0        0        0     9439 2023-07-10 17:12:46.174332 xrpl_py-2.1.0b0/xrpl/wallet/main.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:07:06.931385 xrpl_py-2.1.0b0/xrpl/wallet/py.typed
+-rw-r--r--   0        0        0     1639 2023-07-10 17:12:46.174580 xrpl_py-2.1.0b0/xrpl/wallet/wallet_generation.py
+-rw-r--r--   0        0        0    17291 1970-01-01 00:00:00.000000 xrpl_py-2.1.0b0/PKG-INFO
```

### Comparing `xrpl-py-2.1.0/LICENSE` & `xrpl_py-2.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/README.md` & `xrpl_py-2.1.0b0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,81 @@
+Metadata-Version: 2.1
+Name: xrpl-py
+Version: 2.1.0b0
+Summary: A complete Python library for interacting with the XRP ledger
+Home-page: https://github.com/XRPLF/xrpl-py
+License: ISC
+Keywords: xrp,xrpl,cryptocurrency
+Author: Mayukha Vadari
+Author-email: mvadari@ripple.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Deprecated (>=1.2.13,<2.0.0)
+Requires-Dist: ECPy (>=1.2.5,<2.0.0)
+Requires-Dist: base58 (>=2.1.0,<3.0.0)
+Requires-Dist: httpx (>=0.18.1,<0.25.0)
+Requires-Dist: pycryptodome (>=3.16.0,<4.0.0)
+Requires-Dist: types-Deprecated (>=1.2.9,<2.0.0)
+Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
+Requires-Dist: websockets (>=10.0,<11.0) ; python_version >= "3.10" and python_version < "4.0"
+Requires-Dist: websockets (>=9.0.1,<11.0) ; python_version >= "3.7" and python_version < "3.10"
+Project-URL: Documentation, https://xrpl-py.readthedocs.io
+Project-URL: Repository, https://github.com/XRPLF/xrpl-py
+Description-Content-Type: text/markdown
+
 [![Documentation Status](https://readthedocs.org/projects/xrpl-py/badge)](https://xrpl-py.readthedocs.io/)
 
 # xrpl-py
 
-A pure Python implementation for interacting with the [XRP Ledger](https://xrpl.org/). 
+A pure Python implementation for interacting with the XRP Ledger, the `xrpl-py` library simplifies the hardest parts of XRP Ledger interaction, like serialization and transaction signing, by providing native Python methods and models for [XRP Ledger transactions](https://xrpl.org/transaction-formats.html) and core server [API](https://xrpl.org/api-conventions.html) ([`rippled`](https://github.com/ripple/rippled)) objects.
 
-The `xrpl-py` library simplifies the hardest parts of XRP Ledger interaction, like serialization and transaction signing. It also provides native Python methods and models for [XRP Ledger transactions](https://xrpl.org/transaction-formats.html) and core server [API](https://xrpl.org/api-conventions.html) ([`rippled`](https://github.com/ripple/rippled)) objects.
 
-As an example, this is how you would use this library to send a payment on testnet:
 
 ```py
-from xrpl.account import get_balance
+# create a network client
 from xrpl.clients import JsonRpcClient
-from xrpl.models import Payment, Tx
-from xrpl.transaction import submit_and_wait
-from xrpl.wallet import generate_faucet_wallet
-
-# Create a client to connect to the test network
 client = JsonRpcClient("https://s.altnet.rippletest.net:51234")
 
-# Create two wallets to send money between on the test network
-wallet1 = generate_faucet_wallet(client, debug=True)
-wallet2 = generate_faucet_wallet(client, debug=True)
-
-# Both balances should be zero since nothing has been sent yet
-print("Balances of wallets before Payment tx")
-print(get_balance(wallet1.address, client))
-print(get_balance(wallet2.address, client))
-
-# Create a Payment transaction from wallet1 to wallet2
-payment_tx = Payment(
-    account=wallet1.address,
-    amount="1000",
-    destination=wallet2.address,
+# create a wallet on the testnet
+from xrpl.wallet import generate_faucet_wallet
+test_wallet = generate_faucet_wallet(client)
+print(test_wallet)
+public_key: ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56
+private_key: -HIDDEN-
+address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo
+
+# look up account info
+from xrpl.models import AccountInfo
+acct_info = AccountInfo(
+    account="rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",
+    ledger_index="current",
+    queue=True,
+    strict=True,
 )
-
-# Submit the payment to the network and wait to see a response
-#   Behind the scenes, this fills in fields which can be looked up automatically like the fee.
-#   It also signs the transaction with wallet1 to prove you own the account you're paying from.
-payment_response = submit_and_wait(payment_tx, client, wallet1)
-print("Transaction was submitted")
-
-# Create a "Tx" request to look up the transaction on the ledger
-tx_response = client.request(Tx(transaction=payment_response.result["hash"]))
-
-# Check whether the transaction was actually validated on ledger
-print("Validated:", tx_response.result["validated"])
-
-# Check balances after 1000 drops (.001 XRP) was sent from wallet1 to wallet2
-print("Balances of wallets after Payment tx:")
-print(get_balance(wallet1.address, client))
-print(get_balance(wallet2.address, client))
+response = client.request(acct_info)
+result = response.result
+import json
+print(json.dumps(result["account_data"], indent=4, sort_keys=True))
+# {
+#     "Account": "rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",
+#     "Balance": "1000000000",
+#     "Flags": 0,
+#     "LedgerEntryType": "AccountRoot",
+#     "OwnerCount": 0,
+#     "PreviousTxnID": "73CD4A37537A992270AAC8472F6681F44E400CBDE04EC8983C34B519F56AB107",
+#     "PreviousTxnLgrSeq": 16233962,
+#     "Sequence": 16233962,
+#     "index": "FD66EC588B52712DCE74831DCB08B24157DC3198C29A0116AA64D310A58512D7"
+# }
 ```
 
 [![Downloads](https://pepy.tech/badge/xrpl-py/month)](https://pepy.tech/project/xrpl-py/month)
 [![Contributors](https://img.shields.io/github/contributors/xpring-eng/xrpl-py.svg)](https://github.com/xpring-eng/xrpl-py/graphs/contributors)
 
 ## Installation and supported versions
 
@@ -324,17 +346,14 @@
         is_test_network=True,
     )
 )
 print(testnet_xaddress)
 # T7QDemmxnuN7a52A62nx2fxGPWcRahLCf3qaswfrsNW9Lps
 ```
 
-## Migrating
-
-If you're currently using `xrpl-py` version 1, you can use [this guide to migrate to v2](https://xrpl.org/blog/2023/xrpl-py-2.0-release.html).
 
 ## Contributing
 
 If you want to contribute to this project, see [CONTRIBUTING.md].
 
 ### Mailing Lists
 
@@ -358,7 +377,8 @@
 
 The `xrpl-py` library is licensed under the ISC License. See [LICENSE] for more information.
 
 
 
 [CONTRIBUTING.md]: CONTRIBUTING.md
 [LICENSE]: LICENSE
+
```

### Comparing `xrpl-py-2.1.0/pyproject.toml` & `xrpl_py-2.1.0b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xrpl-py"
-version = "2.1.0"
+version = "2.1.0b0"
 description = "A complete Python library for interacting with the XRP ledger"
 readme = "README.md"
 repository = "https://github.com/XRPLF/xrpl-py"
 authors = [
   "Mayukha Vadari <mvadari@ripple.com>",
   "Greg Weisbrod <gweisbrod@ripple.com>",
   "Amie Corso <acorso@ripple.com>",
```

### Comparing `xrpl-py-2.1.0/xrpl/account/main.py` & `xrpl_py-2.1.0b0/xrpl/account/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/account/transaction_history.py` & `xrpl_py-2.1.0b0/xrpl/account/transaction_history.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/account/main.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/account/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/account/transaction_history.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/account/transaction_history.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/clients/__init__.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/clients/async_client.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/async_client.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/clients/async_websocket_client.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/async_websocket_client.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/clients/client.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/client.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/clients/exceptions.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/clients/json_rpc_base.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/json_rpc_base.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/clients/utils.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/clients/websocket_base.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/websocket_base.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/ledger/main.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/ledger/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/ledger/utils.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/ledger/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/transaction/__init__.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/transaction/main.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/transaction/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # accurate NetworkID field in every transaction to that chain to prevent replay attacks.
 # Mainnet and testnet are exceptions.
 # More context: https://github.com/XRPLF/rippled/pull/4370
 _RESTRICTED_NETWORKS = 1024
 _REQUIRED_NETWORKID_VERSION = "1.11.0"
 _HOOKS_TESTNET_ID = 21338
 # TODO: make this dynamic based on the current ledger fee
-_ACCOUNT_DELETE_FEE: Final[int] = int(xrp_to_drops(2))
+_OWNER_RESERVE_FEE: Final[int] = int(xrp_to_drops(2))
 
 
 async def sign_and_submit(
     transaction: Transaction,
     client: Client,
     wallet: Wallet,
     autofill: bool = True,
@@ -463,25 +463,28 @@
         escrow_finish = cast(EscrowFinish, transaction)
         if escrow_finish.fulfillment is not None:
             fulfillment_bytes = escrow_finish.fulfillment.encode("ascii")
             # 10 drops × (33 + (Fulfillment size in bytes / 16))
             base_fee = math.ceil(net_fee * (33 + (len(fulfillment_bytes) / 16)))
 
     # AccountDelete Transaction
-    if transaction.transaction_type == TransactionType.ACCOUNT_DELETE:
+    if (
+        transaction.transaction_type == TransactionType.ACCOUNT_DELETE
+        or transaction.transaction_type == TransactionType.AMM_CREATE
+    ):
         if client is None:
-            base_fee = _ACCOUNT_DELETE_FEE
+            base_fee = _OWNER_RESERVE_FEE
         else:
-            base_fee = await _fetch_account_delete_fee(client)
+            base_fee = await _fetch_owner_reserve_fee(client)
 
     # Multi-signed Transaction
     # 10 drops × (1 + Number of Signatures Provided)
     if signers_count is not None and signers_count > 0:
         base_fee += net_fee * (1 + signers_count)
     # Round Up base_fee and return it as a String
     return str(math.ceil(base_fee))
 
 
-async def _fetch_account_delete_fee(client: Client) -> int:
+async def _fetch_owner_reserve_fee(client: Client) -> int:
     server_state = await client._request_impl(ServerState())
     fee = server_state.result["state"]["validated_ledger"]["reserve_inc"]
     return int(fee)
```

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/transaction/reliable_submission.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/transaction/reliable_submission.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/asyncio/wallet/wallet_generation.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/wallet/wallet_generation.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/clients/__init__.py` & `xrpl_py-2.1.0b0/xrpl/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/clients/sync_client.py` & `xrpl_py-2.1.0b0/xrpl/clients/sync_client.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/clients/websocket_client.py` & `xrpl_py-2.1.0b0/xrpl/clients/websocket_client.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/constants.py` & `xrpl_py-2.1.0b0/xrpl/constants.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/addresscodec/__init__.py` & `xrpl_py-2.1.0b0/xrpl/core/addresscodec/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/addresscodec/codec.py` & `xrpl_py-2.1.0b0/xrpl/core/addresscodec/codec.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/addresscodec/main.py` & `xrpl_py-2.1.0b0/xrpl/core/addresscodec/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/definitions/__init__.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/definitions/definitions.json` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/definitions.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9107572631710564%*

 * *Differences: {"'FIELDS'": "{insert: [(18, ['WasLockingChainSend', OrderedDict([('nth', 19), ('isVLEncoded', "*

 * *             "False), ('isSerialized', True), ('isSigningField', True), ('type', 'UInt8')])]), "*

 * *             "(23, ['TradingFee', OrderedDict([('nth', 5), ('isVLEncoded', False), "*

 * *             "('isSerialized', True), ('isSigningField', True), ('type', 'UInt16')])]), (24, "*

 * *             "['DiscountedFee', OrderedDict([('nth', 6), ('isVLEncoded', False), ('isSerialized', "*

 * *             "True), ('isSigningField' […]*

```diff
@@ -177,14 +177,24 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 18,
                 "type": "UInt8"
             }
         ],
         [
+            "WasLockingChainSend",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 19,
+                "type": "UInt8"
+            }
+        ],
+        [
             "LedgerEntryType",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 1,
                 "type": "UInt16"
@@ -217,14 +227,34 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 4,
                 "type": "UInt16"
             }
         ],
         [
+            "TradingFee",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 5,
+                "type": "UInt16"
+            }
+        ],
+        [
+            "DiscountedFee",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 6,
+                "type": "UInt16"
+            }
+        ],
+        [
             "Version",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 16,
                 "type": "UInt16"
@@ -717,14 +747,54 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 46,
                 "type": "UInt32"
             }
         ],
         [
+            "LockCount",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 47,
+                "type": "UInt32"
+            }
+        ],
+        [
+            "VoteWeight",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 48,
+                "type": "UInt32"
+            }
+        ],
+        [
+            "FirstNFTokenSequence",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 50,
+                "type": "UInt32"
+            }
+        ],
+        [
+            "LockCount",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 49,
+                "type": "UInt32"
+            }
+        ],
+        [
             "IndexNext",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 1,
                 "type": "UInt64"
@@ -887,14 +957,44 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 19,
                 "type": "UInt64"
             }
         ],
         [
+            "XChainClaimID",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 20,
+                "type": "UInt64"
+            }
+        ],
+        [
+            "XChainAccountCreateCount",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 21,
+                "type": "UInt64"
+            }
+        ],
+        [
+            "XChainAccountClaimCount",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 22,
+                "type": "UInt64"
+            }
+        ],
+        [
             "EmailHash",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 1,
                 "type": "Hash128"
@@ -1067,14 +1167,24 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 13,
                 "type": "Hash256"
             }
         ],
         [
+            "AMMID",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 14,
+                "type": "Hash256"
+            }
+        ],
+        [
             "BookDirectory",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 16,
                 "type": "Hash256"
@@ -1337,14 +1447,44 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 10,
                 "type": "Amount"
             }
         ],
         [
+            "Amount2",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 11,
+                "type": "Amount"
+            }
+        ],
+        [
+            "BidMin",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 12,
+                "type": "Amount"
+            }
+        ],
+        [
+            "BidMax",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 13,
+                "type": "Amount"
+            }
+        ],
+        [
             "MinimumOffer",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 16,
                 "type": "Amount"
@@ -1377,14 +1517,124 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 19,
                 "type": "Amount"
             }
         ],
         [
+            "LockedBalance",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 21,
+                "type": "Amount"
+            }
+        ],
+        [
+            "BaseFeeDrops",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 22,
+                "type": "Amount"
+            }
+        ],
+        [
+            "ReserveBaseDrops",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 23,
+                "type": "Amount"
+            }
+        ],
+        [
+            "ReserveIncrementDrops",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 24,
+                "type": "Amount"
+            }
+        ],
+        [
+            "LPTokenOut",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 25,
+                "type": "Amount"
+            }
+        ],
+        [
+            "LPTokenIn",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 26,
+                "type": "Amount"
+            }
+        ],
+        [
+            "EPrice",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 27,
+                "type": "Amount"
+            }
+        ],
+        [
+            "Price",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 28,
+                "type": "Amount"
+            }
+        ],
+        [
+            "SignatureReward",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 29,
+                "type": "Amount"
+            }
+        ],
+        [
+            "MinAccountCreateAmount",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 30,
+                "type": "Amount"
+            }
+        ],
+        [
+            "LPTokenBalance",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 31,
+                "type": "Amount"
+            }
+        ],
+        [
             "PublicKey",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": true,
                 "nth": 1,
                 "type": "Blob"
@@ -1717,14 +1967,74 @@
                 "isSigningField": true,
                 "isVLEncoded": true,
                 "nth": 16,
                 "type": "AccountID"
             }
         ],
         [
+            "OtherChainSource",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": true,
+                "nth": 18,
+                "type": "AccountID"
+            }
+        ],
+        [
+            "OtherChainDestination",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": true,
+                "nth": 19,
+                "type": "AccountID"
+            }
+        ],
+        [
+            "AttestationSignerAccount",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": true,
+                "nth": 20,
+                "type": "AccountID"
+            }
+        ],
+        [
+            "AttestationRewardAccount",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": true,
+                "nth": 21,
+                "type": "AccountID"
+            }
+        ],
+        [
+            "LockingChainDoor",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": true,
+                "nth": 22,
+                "type": "AccountID"
+            }
+        ],
+        [
+            "IssuingChainDoor",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": true,
+                "nth": 23,
+                "type": "AccountID"
+            }
+        ],
+        [
             "Indexes",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": true,
                 "nth": 1,
                 "type": "Vector256"
@@ -1767,14 +2077,64 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 1,
                 "type": "PathSet"
             }
         ],
         [
+            "LockingChainIssue",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 1,
+                "type": "Issue"
+            }
+        ],
+        [
+            "IssuingChainIssue",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 2,
+                "type": "Issue"
+            }
+        ],
+        [
+            "Asset",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 3,
+                "type": "Issue"
+            }
+        ],
+        [
+            "Asset2",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 4,
+                "type": "Issue"
+            }
+        ],
+        [
+            "XChainBridge",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 1,
+                "type": "XChainBridge"
+            }
+        ],
+        [
             "TransactionMetaData",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 2,
                 "type": "STObject"
@@ -1977,14 +2337,84 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 24,
                 "type": "STObject"
             }
         ],
         [
+            "VoteEntry",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 25,
+                "type": "STObject"
+            }
+        ],
+        [
+            "AuctionSlot",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 26,
+                "type": "STObject"
+            }
+        ],
+        [
+            "AuthAccount",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 27,
+                "type": "STObject"
+            }
+        ],
+        [
+            "XChainClaimProofSig",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 32,
+                "type": "STObject"
+            }
+        ],
+        [
+            "XChainCreateAccountProofSig",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 33,
+                "type": "STObject"
+            }
+        ],
+        [
+            "XChainClaimAttestationBatchElement",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 34,
+                "type": "STObject"
+            }
+        ],
+        [
+            "XChainCreateAccountAttestationBatchElement",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 35,
+                "type": "STObject"
+            }
+        ],
+        [
             "Signers",
             {
                 "isSerialized": true,
                 "isSigningField": false,
                 "isVLEncoded": false,
                 "nth": 3,
                 "type": "STArray"
@@ -2067,14 +2497,24 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 11,
                 "type": "STArray"
             }
         ],
         [
+            "VoteSlots",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 12,
+                "type": "STArray"
+            }
+        ],
+        [
             "Majorities",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 16,
                 "type": "STArray"
@@ -2115,20 +2555,72 @@
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 20,
                 "type": "STArray"
             }
+        ],
+        [
+            "XChainClaimAttestationBatch",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 21,
+                "type": "STArray"
+            }
+        ],
+        [
+            "XChainCreateAccountAttestationBatch",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 22,
+                "type": "STArray"
+            }
+        ],
+        [
+            "XChainClaimAttestations",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 23,
+                "type": "STArray"
+            }
+        ],
+        [
+            "XChainCreateAccountAttestations",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 24,
+                "type": "STArray"
+            }
+        ],
+        [
+            "AuthAccounts",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 25,
+                "type": "STArray"
+            }
         ]
     ],
     "LEDGER_ENTRY_TYPES": {
+        "AMM": 121,
         "AccountRoot": 97,
         "Amendments": 102,
         "Any": -3,
+        "Bridge": 105,
         "Check": 67,
         "Child": -2,
         "Contract": 99,
         "DepositPreauth": 112,
         "DirectoryNode": 100,
         "Escrow": 117,
         "FeeSettings": 115,
@@ -2139,17 +2631,23 @@
         "NFTokenPage": 80,
         "NegativeUNL": 78,
         "Nickname": 110,
         "Offer": 111,
         "PayChannel": 120,
         "RippleState": 114,
         "SignerList": 83,
-        "Ticket": 84
+        "Ticket": 84,
+        "XChainClaimID": 113,
+        "XChainCreateAccountClaimID": 116
     },
     "TRANSACTION_RESULTS": {
+        "tecAMM_BALANCE": 163,
+        "tecAMM_FAILED": 164,
+        "tecAMM_INVALID_TOKENS": 165,
+        "tecBAD_XCHAIN_TRANSFER_ISSUE": 171,
         "tecCANT_ACCEPT_OWN_NFTOKEN_OFFER": 158,
         "tecCLAIM": 100,
         "tecCRYPTOCONDITION_ERROR": 146,
         "tecDIR_FULL": 121,
         "tecDST_TAG_NEEDED": 143,
         "tecDUPLICATE": 149,
         "tecEXPIRED": 148,
@@ -2183,19 +2681,37 @@
         "tecNO_SUITABLE_NFTOKEN_PAGE": 155,
         "tecNO_TARGET": 138,
         "tecOBJECT_NOT_FOUND": 160,
         "tecOVERSIZE": 145,
         "tecOWNERS": 132,
         "tecPATH_DRY": 128,
         "tecPATH_PARTIAL": 101,
+        "tecPRECISION_LOSS": 188,
+        "tecREQUIRES_FLAG": 187,
         "tecTOO_SOON": 152,
         "tecUNFUNDED": 129,
         "tecUNFUNDED_ADD": 102,
+        "tecUNFUNDED_AMM": 162,
         "tecUNFUNDED_OFFER": 103,
         "tecUNFUNDED_PAYMENT": 104,
+        "tecXCHAIN_ACCOUNT_CREATE_PAST": 182,
+        "tecXCHAIN_ACCOUNT_CREATE_TOO_MANY": 183,
+        "tecXCHAIN_BAD_CLAIM_ID": 173,
+        "tecXCHAIN_BAD_PUBLIC_KEY_ACCOUNT_PAIR": 186,
+        "tecXCHAIN_CLAIM_NO_QUORUM": 174,
+        "tecXCHAIN_CREATE_ACCOUNT_NONXRP_ISSUE": 176,
+        "tecXCHAIN_INSUFF_CREATE_AMOUNT": 181,
+        "tecXCHAIN_NO_CLAIM_ID": 172,
+        "tecXCHAIN_NO_SIGNERS_LIST": 179,
+        "tecXCHAIN_PAYMENT_FAILED": 184,
+        "tecXCHAIN_PROOF_UNKNOWN_KEY": 175,
+        "tecXCHAIN_REWARD_MISMATCH": 178,
+        "tecXCHAIN_SELF_COMMIT": 185,
+        "tecXCHAIN_SENDING_ACCOUNT_MISMATCH": 180,
+        "tecXCHAIN_WRONG_CHAIN": 177,
         "tefALREADY": -198,
         "tefBAD_ADD_AUTH": -197,
         "tefBAD_AUTH": -196,
         "tefBAD_AUTH_MASTER": -183,
         "tefBAD_LEDGER": -195,
         "tefBAD_QUORUM": -185,
         "tefBAD_SIGNATURE": -186,
@@ -2225,14 +2741,15 @@
         "telFAILED_PROCESSING": -395,
         "telINSUF_FEE_P": -394,
         "telLOCAL_ERROR": -399,
         "telNETWORK_ID_MAKES_TX_NON_CANONICAL": -384,
         "telNO_DST_PARTIAL": -393,
         "telREQUIRES_NETWORK_ID": -385,
         "telWRONG_NETWORK": -386,
+        "temBAD_AMM_TOKENS": -261,
         "temBAD_AMOUNT": -298,
         "temBAD_CURRENCY": -297,
         "temBAD_EXPIRATION": -296,
         "temBAD_FEE": -295,
         "temBAD_ISSUER": -294,
         "temBAD_LIMIT": -293,
         "temBAD_NFTOKEN_TRANSFER_FEE": -262,
@@ -2249,43 +2766,56 @@
         "temBAD_SEQUENCE": -283,
         "temBAD_SIGNATURE": -282,
         "temBAD_SIGNER": -272,
         "temBAD_SRC_ACCOUNT": -281,
         "temBAD_TICK_SIZE": -269,
         "temBAD_TRANSFER_RATE": -280,
         "temBAD_WEIGHT": -270,
+        "temBAD_XCHAIN_PROOF": -258,
         "temCANNOT_PREAUTH_SELF": -267,
         "temDISABLED": -273,
         "temDST_IS_SRC": -279,
         "temDST_NEEDED": -278,
+        "temEQUAL_DOOR_ACCOUNTS": -259,
         "temINVALID": -277,
         "temINVALID_ACCOUNT_ID": -268,
         "temINVALID_COUNT": -266,
         "temINVALID_FLAG": -276,
         "temMALFORMED": -299,
         "temREDUNDANT": -275,
         "temRIPPLE_EMPTY": -274,
         "temSEQ_AND_TICKET": -263,
+        "temSIDECHAIN_BAD_ISSUES": -257,
+        "temSIDECHAIN_NONDOOR_OWNER": -256,
         "temUNCERTAIN": -265,
         "temUNKNOWN": -264,
+        "temXCHAIN_BRIDGE_BAD_MIN_ACCOUNT_CREATE_AMOUNT": -255,
+        "temXCHAIN_BRIDGE_BAD_REWARD_AMOUNT": -254,
+        "temXCHAIN_TOO_MANY_ATTESTATIONS": -253,
         "terFUNDS_SPENT": -98,
         "terINSUF_FEE_B": -97,
         "terLAST": -91,
         "terNO_ACCOUNT": -96,
+        "terNO_AMM": -87,
         "terNO_AUTH": -95,
         "terNO_LINE": -94,
         "terNO_RIPPLE": -90,
         "terOWNERS": -93,
         "terPRE_SEQ": -92,
         "terPRE_TICKET": -88,
         "terQUEUED": -89,
         "terRETRY": -99,
         "tesSUCCESS": 0
     },
     "TRANSACTION_TYPES": {
+        "AMMBid": 39,
+        "AMMCreate": 35,
+        "AMMDeposit": 36,
+        "AMMVote": 38,
+        "AMMWithdraw": 37,
         "AccountDelete": 21,
         "AccountSet": 3,
         "CheckCancel": 18,
         "CheckCash": 17,
         "CheckCreate": 16,
         "Contract": 9,
         "DepositPreauth": 19,
@@ -2309,24 +2839,33 @@
         "SetFee": 101,
         "SetHook": 22,
         "SetRegularKey": 5,
         "SignerListSet": 12,
         "TicketCancel": 11,
         "TicketCreate": 10,
         "TrustSet": 20,
-        "UNLModify": 102
+        "UNLModify": 102,
+        "XChainAccountCreateCommit": 44,
+        "XChainAddAccountCreateAttestation": 46,
+        "XChainAddClaimAttestation": 45,
+        "XChainClaim": 43,
+        "XChainCommit": 42,
+        "XChainCreateBridge": 40,
+        "XChainCreateClaimID": 41,
+        "XChainModifyBridge": 47
     },
     "TYPES": {
         "AccountID": 8,
         "Amount": 6,
         "Blob": 7,
         "Done": -1,
         "Hash128": 4,
         "Hash160": 17,
         "Hash256": 5,
+        "Issue": 24,
         "LedgerEntry": 10002,
         "Metadata": 10004,
         "NotPresent": 0,
         "PathSet": 18,
         "STArray": 15,
         "STObject": 14,
         "Transaction": 10001,
@@ -2336,10 +2875,11 @@
         "UInt384": 22,
         "UInt512": 23,
         "UInt64": 3,
         "UInt8": 16,
         "UInt96": 20,
         "Unknown": -2,
         "Validation": 10003,
-        "Vector256": 19
+        "Vector256": 19,
+        "XChainBridge": 25
     }
 }
```

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/definitions/definitions.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/definitions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/definitions/field_header.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_header.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,7 +44,11 @@
                 header.append(self.field_code)
         elif self.field_code < 16:
             header += [self.field_code, self.type_code]
         else:
             header += [0, self.type_code, self.field_code]
 
         return bytes(header)
+
+    def __repr__(self: FieldHeader) -> str:
+        """Print a string representation of a FieldHeader (for debugging)."""
+        return f"FieldHeader({self.type_code}, {self.field_code})"
```

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/definitions/field_info.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_info.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/definitions/field_instance.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_instance.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/field_id_codec.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/field_id_codec.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/main.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Codec for encoding objects into the XRP Ledger's canonical binary format and
 decoding them.
 """
 
-from typing import Any, Dict, Optional, cast
+from typing import Any, Dict, Optional, Union, cast
 
 from typing_extensions import Final
 
 from xrpl.core.binarycodec.binary_wrappers.binary_parser import BinaryParser
 from xrpl.core.binarycodec.types.account_id import AccountID
+from xrpl.core.binarycodec.types.amount import Amount
 from xrpl.core.binarycodec.types.hash256 import Hash256
 from xrpl.core.binarycodec.types.st_object import STObject
 from xrpl.core.binarycodec.types.uint64 import UInt64
 
 
 def _num_to_bytes(num: int) -> bytes:
     return (num).to_bytes(4, byteorder="big", signed=False)
@@ -63,15 +64,19 @@
         json: A JSON-like dictionary representation of a Claim.
 
     Returns:
         The binary-encoded claim, ready to be signed.
     """
     prefix = _PAYMENT_CHANNEL_CLAIM_PREFIX
     channel = Hash256.from_value(json["channel"])
-    amount = UInt64.from_value(int(json["amount"]))
+
+    if isinstance(json["amount"], str):
+        amount: Union[Amount, UInt64] = UInt64.from_value(int(json["amount"]))
+    else:
+        amount = Amount.from_value(json["amount"])
 
     buffer = prefix + bytes(channel) + bytes(amount)
     return buffer.hex().upper()
 
 
 def encode_for_multisigning(json: Dict[str, Any], signing_account: str) -> str:
     """
```

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/__init__.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,36 +3,40 @@
 from xrpl.core.binarycodec.types.amount import Amount
 from xrpl.core.binarycodec.types.blob import Blob
 from xrpl.core.binarycodec.types.currency import Currency
 from xrpl.core.binarycodec.types.hash import Hash
 from xrpl.core.binarycodec.types.hash128 import Hash128
 from xrpl.core.binarycodec.types.hash160 import Hash160
 from xrpl.core.binarycodec.types.hash256 import Hash256
+from xrpl.core.binarycodec.types.issue import Issue
 from xrpl.core.binarycodec.types.path_set import PathSet
 from xrpl.core.binarycodec.types.st_array import STArray
 from xrpl.core.binarycodec.types.st_object import STObject
 from xrpl.core.binarycodec.types.uint import UInt
 from xrpl.core.binarycodec.types.uint8 import UInt8
 from xrpl.core.binarycodec.types.uint16 import UInt16
 from xrpl.core.binarycodec.types.uint32 import UInt32
 from xrpl.core.binarycodec.types.uint64 import UInt64
 from xrpl.core.binarycodec.types.vector256 import Vector256
+from xrpl.core.binarycodec.types.xchain_bridge import XChainBridge
 
 __all__ = [
     "AccountID",
     "Amount",
     "Blob",
     "Currency",
     "Hash",
     "Hash128",
     "Hash160",
     "Hash256",
+    "Issue",
     "PathSet",
     "STObject",
     "STArray",
     "UInt",
     "UInt8",
     "UInt16",
     "UInt32",
     "UInt64",
     "Vector256",
+    "XChainBridge",
 ]
```

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/account_id.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/account_id.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/amount.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/amount.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/blob.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/blob.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/currency.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/currency.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/hash.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/hash128.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash128.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/hash160.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash160.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/hash256.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash256.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/path_set.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/path_set.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/serialized_type.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/serialized_type.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/st_array.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/st_array.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/st_object.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/st_object.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/uint.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/uint16.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint16.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/uint32.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint32.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/uint64.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint64.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/uint8.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint8.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/binarycodec/types/vector256.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/vector256.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/keypairs/crypto_implementation.py` & `xrpl_py-2.1.0b0/xrpl/core/keypairs/crypto_implementation.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/keypairs/ed25519.py` & `xrpl_py-2.1.0b0/xrpl/core/keypairs/ed25519.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/keypairs/helpers.py` & `xrpl_py-2.1.0b0/xrpl/core/keypairs/helpers.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/keypairs/main.py` & `xrpl_py-2.1.0b0/xrpl/core/keypairs/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/core/keypairs/secp256k1.py` & `xrpl_py-2.1.0b0/xrpl/core/keypairs/secp256k1.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/ledger/main.py` & `xrpl_py-2.1.0b0/xrpl/ledger/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/__init__.py` & `xrpl_py-2.1.0b0/xrpl/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """Top-level exports for the models package."""
 from xrpl.models import amounts, currencies, requests, transactions
 from xrpl.models.amounts import *  # noqa: F401, F403
+from xrpl.models.auth_account import AuthAccount
 from xrpl.models.currencies import *  # noqa: F401, F403
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.path import Path, PathStep
 from xrpl.models.requests import *  # noqa: F401, F403
 from xrpl.models.response import Response
 from xrpl.models.transactions import *  # noqa: F401, F403
 from xrpl.models.transactions.pseudo_transactions import *  # noqa: F401, F403
+from xrpl.models.xchain_bridge import XChainBridge
 
 __all__ = [
     "XRPLModelException",
     "amounts",
     *amounts.__all__,
+    "AuthAccount",
     "currencies",
     *currencies.__all__,
     "requests",
     *requests.__all__,
     "transactions",
     *transactions.__all__,
     *transactions.pseudo_transactions.__all__,
     "Path",
     "PathStep",
     "Response",
+    "XChainBridge",
 ]
```

### Comparing `xrpl-py-2.1.0/xrpl/models/amounts/amount.py` & `xrpl_py-2.1.0b0/xrpl/models/amounts/amount.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/amounts/issued_currency_amount.py` & `xrpl_py-2.1.0b0/xrpl/models/amounts/issued_currency_amount.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/base_model.py` & `xrpl_py-2.1.0b0/xrpl/models/base_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import json
 import re
 from abc import ABC
 from dataclasses import dataclass, fields
 from enum import Enum
 from typing import Any, Dict, List, Pattern, Type, TypeVar, Union, cast, get_type_hints
 
-from typing_extensions import Final, get_args, get_origin
+from typing_extensions import Final, Literal, get_args, get_origin
 
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.required import REQUIRED
 from xrpl.models.types import XRPL_VALUE_TYPE
 
 # this regex splits words based on one of three cases:
 #
@@ -28,29 +28,39 @@
 # PascalCase like "Amount"
 _CAMEL_CASE_TYPICAL: Final[str] = "[A-Z][^A-Z]*"
 #
 # combining the above together into one regex:
 _CAMEL_TO_SNAKE_CASE_REGEX: Final[Pattern[str]] = re.compile(
     f"(?:{_CAMEL_CASE_LEADING_LOWER}|{_CAMEL_CASE_ABBREVIATION}|{_CAMEL_CASE_TYPICAL})"
 )
-# used for converting special substrings inside CamelCase fields
-SPECIAL_CAMELCASE_STRINGS = ["NFToken"]
+
+# This is used to make exceptions when converting dictionary keys to xrpl JSON
+# keys. We snake case keys, but some keys are abbreviations.
+ABBREVIATIONS: Final[Dict[str, str]] = {
+    "amm": "AMM",
+    "id": "ID",
+    "lp": "LP",
+    "nftoken": "NFToken",
+    "unl": "UNL",
+    "uri": "URI",
+    "xchain": "XChain",
+}
 
 BM = TypeVar("BM", bound="BaseModel")  # any type inherited from BaseModel
 
 
 def _key_to_json(field: str) -> str:
     """
     Transforms camelCase or PascalCase to snake_case. For example:
         1. 'TransactionType' becomes 'transaction_type'
         2. 'value' remains 'value'
         3. 'URI' becomes 'uri'
     """
     # convert all special CamelCase substrings to capitalized strings
-    for spec_str in SPECIAL_CAMELCASE_STRINGS:
+    for spec_str in ABBREVIATIONS.values():
         if spec_str in field:
             field = field.replace(spec_str, spec_str.capitalize())
 
     return "_".join(
         [word.lower() for word in _CAMEL_TO_SNAKE_CASE_REGEX.findall(field)]
     )
 
@@ -164,14 +174,18 @@
             # param_type is Any (e.g. will accept anything)
             return param_value
 
         if isinstance(param_type, type) and isinstance(param_value, param_type):
             # expected an object, received the correct object
             return param_value
 
+        if get_origin(param_type) == Literal:
+            if param_value in get_args(param_type):
+                return param_value
+
         if (
             isinstance(param_type, type)
             and issubclass(param_type, Enum)
             and param_value in list(param_type)
         ):
             # expected an Enum and received a valid value for it.
             # for some reason required for string enums.
```

### Comparing `xrpl-py-2.1.0/xrpl/models/currencies/issued_currency.py` & `xrpl_py-2.1.0b0/xrpl/models/currencies/issued_currency.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/currencies/xrp.py` & `xrpl_py-2.1.0b0/xrpl/models/currencies/xrp.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,7 +73,16 @@
         """
         # import needed here to avoid circular dependency
         from xrpl.utils.xrp_conversions import xrp_to_drops
 
         if isinstance(value, str):
             return xrp_to_drops(float(value))
         return xrp_to_drops(value)
+
+    def __repr__(self: XRP) -> str:
+        """
+        Generate string representation of XRP.
+
+        Returns:
+            A string representation of XRP currency.
+        """
+        return "XRP()"
```

### Comparing `xrpl-py-2.1.0/xrpl/models/flags.py` & `xrpl_py-2.1.0b0/xrpl/models/flags.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,30 @@
         "tf_require_dest_tag": 0x00010000,
         "tf_optional_dest_tag": 0x00020000,
         "tf_require_auth": 0x00040000,
         "tf_optional_auth": 0x00080000,
         "tf_disallow_xrp": 0x00100000,
         "tf_allow_xrp": 0x00200000,
     },
+    "AMMDeposit": {
+        "tf_lp_token": 0x00010000,
+        "tf_single_asset": 0x00080000,
+        "tf_two_asset": 0x00100000,
+        "tf_one_asset_lp_token": 0x00200000,
+        "tf_limit_lp_token": 0x00400000,
+    },
+    "AMMWithdraw": {
+        "tf_lp_token": 0x00010000,
+        "tf_withdraw_all": 0x00020000,
+        "tf_one_asset_withdraw_all": 0x00040000,
+        "tf_single_asset": 0x00080000,
+        "tf_two_asset": 0x00100000,
+        "tf_one_asset_lp_token": 0x00200000,
+        "tf_limit_lp_token": 0x00400000,
+    },
     "NFTokenCreateOffer": {
         "tf_sell_token": 0x00000001,
     },
     "NFTokenMint": {
         "tf_burnable": 0x00000001,
         "tf_only_xrp": 0x00000002,
         "tf_trustline": 0x00000004,
```

### Comparing `xrpl-py-2.1.0/xrpl/models/nested_model.py` & `xrpl_py-2.1.0b0/xrpl/models/nested_model.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/path.py` & `xrpl_py-2.1.0b0/xrpl/models/path.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/__init__.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Request models."""
+from xrpl.models.auth_account import AuthAccount
 from xrpl.models.path import PathStep
 from xrpl.models.requests.account_channels import AccountChannels
 from xrpl.models.requests.account_currencies import AccountCurrencies
 from xrpl.models.requests.account_info import AccountInfo
 from xrpl.models.requests.account_lines import AccountLines
 from xrpl.models.requests.account_nfts import AccountNFTs
 from xrpl.models.requests.account_objects import AccountObjects, AccountObjectType
 from xrpl.models.requests.account_offers import AccountOffers
 from xrpl.models.requests.account_tx import AccountTx
+from xrpl.models.requests.amm_info import AMMInfo
 from xrpl.models.requests.book_offers import BookOffers
 from xrpl.models.requests.channel_authorize import ChannelAuthorize
 from xrpl.models.requests.channel_verify import ChannelVerify
 from xrpl.models.requests.deposit_authorized import DepositAuthorized
 from xrpl.models.requests.fee import Fee
 from xrpl.models.requests.gateway_balances import GatewayBalances
 from xrpl.models.requests.generic_request import GenericRequest
@@ -50,14 +52,16 @@
     "AccountInfo",
     "AccountLines",
     "AccountNFTs",
     "AccountObjects",
     "AccountObjectType",
     "AccountOffers",
     "AccountTx",
+    "AMMInfo",
+    "AuthAccount",
     "BookOffers",
     "ChannelAuthorize",
     "ChannelVerify",
     "DepositAuthorized",
     "Fee",
     "GatewayBalances",
     "GenericRequest",
```

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/account_channels.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_channels.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/account_currencies.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_currencies.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/account_info.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_info.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/account_lines.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_lines.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/account_nfts.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_nfts.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/account_objects.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,26 @@
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 class AccountObjectType(str, Enum):
     """Represents the object types that an AccountObjectsRequest can ask for."""
 
+    BRIDGE = "bridge"
     CHECK = "check"
     DEPOSIT_PREAUTH = "deposit_preauth"
     ESCROW = "escrow"
+    NFT_OFFER = "nft_offer"
     OFFER = "offer"
     PAYMENT_CHANNEL = "payment_channel"
     SIGNER_LIST = "signer_list"
     STATE = "state"
     TICKET = "ticket"
-    NFT_OFFER = "nft_offer"
+    XCHAIN_OWNED_CREATE_ACCOUNT_CLAIM_ID = "xchain_owned_create_account_claim_id"
+    XCHAIN_OWNED_CLAIM_ID = "xchain_owned_claim_id"
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class AccountObjects(Request, LookupByLedgerRequest):
     """
     This request returns the raw ledger format for all objects owned by an account.
```

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/account_offers.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_offers.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/account_tx.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_tx.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/book_offers.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/book_offers.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/channel_authorize.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/channel_authorize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 The channel_authorize method creates a signature that can
-be used to redeem a specific amount of XRP from a payment channel.
+be used to redeem a specific amount from a payment channel.
 
 Warning: Do not send secret keys to untrusted servers or through unsecured network
 connections. (This includes the secret, seed, seed_hex, or passphrase fields of this
 request.) You should only use this method on a secure, encrypted network connection to
 a server you run or fully trust with your funds. Otherwise, eavesdroppers could use
 your secret key to sign claims and take all the money from this payment channel and
 anything else using the same key pair. See
@@ -14,25 +14,26 @@
 """
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Dict, Optional
 
 from xrpl.constants import CryptoAlgorithm
+from xrpl.models.amounts import Amount
 from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class ChannelAuthorize(Request):
     """
     The channel_authorize method creates a signature that can
-    be used to redeem a specific amount of XRP from a payment channel.
+    be used to redeem a specific amount from a payment channel.
 
     Warning: Do not send secret keys to untrusted servers or through unsecured network
     connections. (This includes the secret, seed, seed_hex, or passphrase fields of
     this request.) You should only use this method on a secure, encrypted network
     connection to a server you run or fully trust with your funds. Otherwise,
     eavesdroppers could use your secret key to sign claims and take all the money from
     this payment channel and anything else using the same key pair. See
@@ -46,15 +47,15 @@
     channel_id: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
-    amount: str = REQUIRED  # type: ignore
+    amount: Amount = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
     secret: Optional[str] = None
```

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/channel_verify.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/unsubscribe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 """
-The channel_verify method checks the validity of a
-signature that can be used to redeem a specific amount of
-XRP from a payment channel.
+The unsubscribe command tells the server to stop sending
+messages for a particular subscription or set of subscriptions.
+
+WebSocket API only.
+
+`See unsubscribe <https://xrpl.org/unsubscribe.html>`_
 """
 from dataclasses import dataclass, field
+from typing import List, Optional
 
+from xrpl.models.base_model import BaseModel
+from xrpl.models.currencies import Currency
 from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.subscribe import StreamParameter
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class ChannelVerify(Request):
-    """
-    The channel_verify method checks the validity of a
-    signature that can be used to redeem a specific amount of
-    XRP from a payment channel.
-    """
+class UnsubscribeBook(BaseModel):
+    """Format for elements in the ``books`` array for Unsubscribe only."""
 
-    method: RequestMethod = field(default=RequestMethod.CHANNEL_VERIFY, init=False)
-    channel_id: str = REQUIRED  # type: ignore
+    taker_gets: Currency = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
-    amount: str = REQUIRED  # type: ignore
+    taker_pays: Currency = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
-    public_key: str = REQUIRED  # type: ignore
-    """
-    This field is required.
+    both: bool = False
 
-    :meta hide-value:
-    """
 
-    signature: str = REQUIRED  # type: ignore
+@require_kwargs_on_init
+@dataclass(frozen=True)
+class Unsubscribe(Request):
     """
-    This field is required.
+    The unsubscribe command tells the server to stop sending
+    messages for a particular subscription or set of subscriptions.
 
-    :meta hide-value:
+    WebSocket API only.
+
+    `See unsubscribe <https://xrpl.org/unsubscribe.html>`_
     """
+
+    method: RequestMethod = field(default=RequestMethod.UNSUBSCRIBE, init=False)
+    streams: Optional[List[StreamParameter]] = None
+    accounts: Optional[List[str]] = None
+    accounts_proposed: Optional[List[str]] = None
+    books: Optional[List[UnsubscribeBook]] = None
```

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/deposit_authorized.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/deposit_authorized.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/fee.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/fee.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/gateway_balances.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/gateway_balances.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/generic_request.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/generic_request.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/ledger.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ledger.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/ledger_closed.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ledger_closed.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/ledger_current.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ledger_current.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/ledger_data.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ledger_data.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/ledger_entry.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ledger_entry.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Dict, List, Optional, Union
 
 from xrpl.models.base_model import BaseModel
+from xrpl.models.currencies import Currency
 from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 class LedgerEntryType(str, Enum):
     """Identifiers for on-ledger objects."""
@@ -128,15 +129,15 @@
     :meta hide-value:
     """
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class RippleState(BaseModel):
-    """Required fields for requesting a RippleState."""
+    """Required fields for requesting a RippleState if not querying by object ID."""
 
     accounts: List[str] = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
@@ -148,18 +149,15 @@
     :meta hide-value:
     """
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class Ticket(BaseModel):
-    """
-    Required fields for requesting a Ticket, if not querying by
-    object ID.
-    """
+    """Required fields for requesting a Ticket if not querying by object ID."""
 
     owner: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
@@ -170,14 +168,41 @@
 
     :meta hide-value:
     """
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
+class XChainClaimID(BaseModel):
+    """Required fields for requesting an XChainClaimID if not querying by object ID."""
+
+    locking_chain_door: str
+    locking_chain_issue: Currency
+    issuing_chain_door: str
+    issuing_chain_issue: Currency
+    xchain_claim_id: Union[int, str]
+
+
+@require_kwargs_on_init
+@dataclass(frozen=True)
+class XChainCreateAccountClaimID(BaseModel):
+    """
+    Required fields for requesting an XChainCreateAccountClaimID if not querying by
+    object ID.
+    """
+
+    locking_chain_door: str
+    locking_chain_issue: Currency
+    issuing_chain_door: str
+    issuing_chain_issue: Currency
+    xchain_create_account_claim_id: Union[int, str]
+
+
+@require_kwargs_on_init
+@dataclass(frozen=True)
 class LedgerEntry(Request, LookupByLedgerRequest):
     """
     The ledger_entry method returns a single ledger
     object from the XRP Ledger in its raw format.
     See ledger format for information on the
     different types of objects you can retrieve.
     `See ledger entry <https://xrpl.org/ledger_entry.html>`_
@@ -190,14 +215,20 @@
     deposit_preauth: Optional[Union[str, DepositPreauth]] = None
     directory: Optional[Union[str, Directory]] = None
     escrow: Optional[Union[str, Escrow]] = None
     offer: Optional[Union[str, Offer]] = None
     payment_channel: Optional[str] = None
     ripple_state: Optional[RippleState] = None
     ticket: Optional[Union[str, Ticket]] = None
+    bridge_account: Optional[str] = None
+    xchain_claim_id: Optional[Union[str, XChainClaimID]] = None
+    xchain_create_account_claim_id: Optional[
+        Union[str, XChainCreateAccountClaimID]
+    ] = None
+
     binary: bool = False
     nft_page: Optional[str] = None
     """Must be the object ID of the NFToken page, as hexadecimal"""
 
     def _get_errors(self: LedgerEntry) -> Dict[str, str]:
         errors = super()._get_errors()
         query_params = [
```

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/manifest.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/manifest.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/nft_buy_offers.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/nft_buy_offers.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/nft_history.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/nft_history.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/nft_info.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/nft_info.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/nft_sell_offers.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/nft_sell_offers.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/no_ripple_check.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/no_ripple_check.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/path_find.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/path_find.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/ping.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ping.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/random.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/random.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/request.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,17 @@
     SERVER_INFO = "server_info"
     SERVER_STATE = "server_state"
 
     # utility methods
     PING = "ping"
     RANDOM = "random"
 
+    # amm methods
+    AMM_INFO = "amm_info"
+
     # generic unknown/unsupported request
     # (there is no XRPL analog, this model is specific to xrpl-py)
     GENERIC_REQUEST = "zzgeneric_request"
 
 
 R = TypeVar("R", bound="Request")
```

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/ripple_path_find.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ripple_path_find.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/server_info.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/server_info.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/server_state.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/server_state.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/sign.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/sign.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/sign_and_submit.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/sign_and_submit.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/sign_for.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/sign_for.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/submit.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/submit.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/submit_multisigned.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/submit_multisigned.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/submit_only.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/submit_only.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/subscribe.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/subscribe.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/transaction_entry.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/transaction_entry.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/tx.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/tx.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/requests/unsubscribe.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_fund.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,49 @@
-"""
-The unsubscribe command tells the server to stop sending
-messages for a particular subscription or set of subscriptions.
-
-WebSocket API only.
-
-`See unsubscribe <https://xrpl.org/unsubscribe.html>`_
-"""
+"""Model for a PaymentChannelFund transaction type."""
 from dataclasses import dataclass, field
-from typing import List, Optional
+from typing import Optional
 
-from xrpl.models.base_model import BaseModel
-from xrpl.models.currencies import Currency
-from xrpl.models.requests.request import Request, RequestMethod
-from xrpl.models.requests.subscribe import StreamParameter
+from xrpl.models.amounts import Amount
 from xrpl.models.required import REQUIRED
+from xrpl.models.transactions.transaction import Transaction
+from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class UnsubscribeBook(BaseModel):
-    """Format for elements in the ``books`` array for Unsubscribe only."""
+class PaymentChannelFund(Transaction):
+    """
+    Represents a `PaymentChannelFund <https://xrpl.org/paymentchannelfund.html>`_
+    transaction, adds additional amount to an open `payment channel
+    <https://xrpl.org/payment-channels.html>`_, and optionally updates the
+    expiration time of the channel. Only the source address
+    of the channel can use this transaction.
+    """
 
-    taker_gets: Currency = REQUIRED  # type: ignore
+    channel: str = REQUIRED  # type: ignore
     """
-    This field is required.
+    The unique ID of the payment channel, as a 64-character hexadecimal
+    string. This field is required.
 
     :meta hide-value:
     """
 
-    taker_pays: Currency = REQUIRED  # type: ignore
+    amount: Amount = REQUIRED  # type: ignore
     """
-    This field is required.
+    Amount to add to the channel. Must be a positive amount. This field is required.
 
     :meta hide-value:
     """
 
-    both: bool = False
-
-
-@require_kwargs_on_init
-@dataclass(frozen=True)
-class Unsubscribe(Request):
+    expiration: Optional[int] = None
     """
-    The unsubscribe command tells the server to stop sending
-    messages for a particular subscription or set of subscriptions.
-
-    WebSocket API only.
-
-    `See unsubscribe <https://xrpl.org/unsubscribe.html>`_
+    A new mutable expiration time to set for the channel, in seconds since the
+    Ripple Epoch. This must be later than the existing expiration time of the
+    channel or later than the current time plus the settle delay of the channel.
+    This is separate from the immutable ``cancel_after`` time.
     """
 
-    method: RequestMethod = field(default=RequestMethod.UNSUBSCRIBE, init=False)
-    streams: Optional[List[StreamParameter]] = None
-    accounts: Optional[List[str]] = None
-    accounts_proposed: Optional[List[str]] = None
-    books: Optional[List[UnsubscribeBook]] = None
+    transaction_type: TransactionType = field(
+        default=TransactionType.PAYMENT_CHANNEL_FUND,
+        init=False,
+    )
```

### Comparing `xrpl-py-2.1.0/xrpl/models/response.py` & `xrpl_py-2.1.0b0/xrpl/models/response.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/account_delete.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/account_delete.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/account_set.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/account_set.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/check_cancel.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/check_cancel.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/check_cash.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/check_cash.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/check_create.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/check_create.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/deposit_preauth.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/deposit_preauth.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/escrow_cancel.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_cancel.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class EscrowCancel(Transaction):
     """
     Represents an `EscrowCancel <https://xrpl.org/escrowcancel.html>`_
-    transaction, which returns escrowed XRP to the sender after the Escrow has
+    transaction, which returns escrowed amount to the sender after the Escrow has
     expired.
     """
 
     owner: str = REQUIRED  # type: ignore
     """
     The address of the account that funded the Escrow. This field is required.
```

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/escrow_create.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_create_claim_id.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,68 @@
-"""Model for EscrowCreate transaction type."""
-from __future__ import annotations  # Requires Python 3.7+
+"""Model for a XChainCreateClaimID transaction type."""
+
+from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Dict, Optional
+from typing import Dict
 
-from xrpl.models.amounts import Amount
+from xrpl.core.addresscodec import is_valid_classic_address
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
+from xrpl.models.xchain_bridge import XChainBridge
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class EscrowCreate(Transaction):
+class XChainCreateClaimID(Transaction):
     """
-    Represents an `EscrowCreate <https://xrpl.org/escrowcreate.html>`_
-    transaction, which locks up XRP until a specific time or condition is met.
+    Represents a XChainCreateClaimID transaction.
+    The XChainCreateClaimID transaction creates a new cross-chain claim ID that
+    is used for a cross-chain transfer. A cross-chain claim ID represents one
+    cross-chain transfer of value.
     """
 
-    amount: Amount = REQUIRED  # type: ignore
+    xchain_bridge: XChainBridge = REQUIRED  # type: ignore
     """
-    Amount of XRP, in drops, to deduct from the sender's balance and set
-    aside in escrow. This field is required.
+    The bridge to create the claim ID for. This field is required.
 
     :meta hide-value:
     """
 
-    destination: str = REQUIRED  # type: ignore
+    signature_reward: str = REQUIRED  # type: ignore
     """
-    The address that should receive the escrowed XRP when the time or
-    condition is met. This field is required.
+    The amount, in XRP, to reward the witness servers for providing signatures.
+    This must match the amount on the ``Bridge`` ledger object. This field is
+    required.
 
     :meta hide-value:
     """
 
-    destination_tag: Optional[int] = None
-    """
-    An arbitrary `destination tag
-    <https://xrpl.org/source-and-destination-tags.html>`_ that
-    identifies the reason for the Escrow, or a hosted recipient to pay.
-    """
-
-    cancel_after: Optional[int] = None
-    """
-    The time, in seconds since the Ripple Epoch, when this escrow expires.
-    This value is immutable; the funds can only be returned the sender after
-    this time.
-    """
-
-    finish_after: Optional[int] = None
-    """
-    The time, in seconds since the Ripple Epoch, when the escrowed XRP can
-    be released to the recipient. This value is immutable; the funds cannot
-    move until this time is reached.
+    other_chain_source: str = REQUIRED  # type: ignore
     """
+    The account that must send the corresponding ``XChainCommit`` transaction
+    on the source chain. This field is required.
 
-    condition: Optional[str] = None
-    """
-    Hex value representing a `PREIMAGE-SHA-256 crypto-condition
-    <https://tools.ietf.org/html/draft-thomas-crypto-conditions-04#section-8.1.>`_
-    The funds can only be delivered to the recipient if this condition is
-    fulfilled.
+    :meta hide-value:
     """
 
     transaction_type: TransactionType = field(
-        default=TransactionType.ESCROW_CREATE,
+        default=TransactionType.XCHAIN_CREATE_CLAIM_ID,
         init=False,
     )
 
-    def _get_errors(self: EscrowCreate) -> Dict[str, str]:
+    def _get_errors(self: XChainCreateClaimID) -> Dict[str, str]:
         errors = super()._get_errors()
-        if (
-            self.cancel_after is not None
-            and self.finish_after is not None
-            and self.finish_after >= self.cancel_after
+
+        if self.signature_reward != REQUIRED and not self.signature_reward.isnumeric():
+            errors["signature_reward"] = "`signature_reward` must be numeric."
+
+        if self.other_chain_source != REQUIRED and not is_valid_classic_address(
+            self.other_chain_source
         ):
             errors[
-                "EscrowCreate"
-            ] = "The finish_after time must be before the cancel_after time."
+                "other_chain_source"
+            ] = "`other_chain_source` must be a valid XRPL address."
 
         return errors
```

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/escrow_finish.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_finish.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/metadata.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/metadata.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/nftoken_accept_offer.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_accept_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/nftoken_burn.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_burn.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/nftoken_cancel_offer.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_cancel_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/nftoken_create_offer.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_create_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/nftoken_mint.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_mint.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/offer_cancel.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/offer_cancel.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/offer_create.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/offer_create.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/payment.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/payment.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/payment_channel_claim.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_claim.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Model for PaymentChannelClaim transaction type."""
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Optional
 
+from xrpl.models.amounts import Amount
 from xrpl.models.flags import FlagInterface
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
@@ -26,22 +27,22 @@
     channel can use this flag.
     """
 
     TF_CLOSE = 0x00020000
     """
     Request to close the channel. Only the channel source and destination addresses
     can use this flag. This flag closes the channel immediately if it has no more
-    XRP allocated to it after processing the current claim, or if the destination
+    funds allocated to it after processing the current claim, or if the destination
     address uses it. If the source address uses this flag when the channel still
-    holds XRP, this schedules the channel to close after `SettleDelay` seconds have
+    holds a value, this schedules the channel to close after `SettleDelay` seconds have
     passed. (Specifically, this sets the `Expiration` of the channel to the close
     time of the previous ledger plus the channel's `SettleDelay` time, unless the
     channel already has an earlier `Expiration` time.) If the destination address
-    uses this flag when the channel still holds XRP, any XRP that remains after
-    processing the claim is returned to the source address.
+    uses this flag when the channel still holds an amount, any amount that remains
+    after processing the claim is returned to the source address.
     """
 
 
 class PaymentChannelClaimFlagInterface(FlagInterface):
     """
     Transactions of the PaymentChannelClaim type support additional values in the Flags
     field. This TypedDict represents those options.
@@ -55,38 +56,41 @@
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class PaymentChannelClaim(Transaction):
     """
     Represents a `PaymentChannelClaim <https://xrpl.org/paymentchannelclaim.html>`_
-    transaction, which claims XRP from a `payment channel
+    transaction, which claims an amount from a `payment channel
     <https://xrpl.org/payment-channels.html>`_, adjusts
     channel's expiration, or both. This transaction can be used differently
     depending on the transaction sender's role in the specified channel.
     """
 
     channel: str = REQUIRED  # type: ignore
     """
     The unique ID of the payment channel, as a 64-character hexadecimal
     string. This field is required.
 
     :meta hide-value:
     """
 
-    balance: Optional[str] = None
+    balance: Optional[Amount] = None
     """
-    The cumulative amount of XRP to have delivered through this channel after
-    processing this claim. Required unless closing the channel.
+    Total amount delivered by this channel after processing this claim. Required
+    to deliver amount. Must be more than the total amount delivered by the channel
+    so far, but not greater than the Amount of the signed claim. Must be provided
+    except when closing the channel.
     """
 
-    amount: Optional[str] = None
+    amount: Optional[Amount] = None
     """
-    The cumulative amount of XRP that has been authorized to deliver by the
-    attached claim signature. Required unless closing the channel.
+    The amount authorized by the Signature. This must match the amount in the signed
+    message. This is the cumulative amount that can be dispensed by the channel,
+    including amounts previously redeemed. Required unless closing the channel.
     """
 
     signature: Optional[str] = None
     """
     The signature of the claim, as hexadecimal. This signature must be
     verifiable for the this channel and the given ``public_key`` and ``amount``
     values. May be omitted if closing the channel or if the sender of this
```

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/payment_channel_create.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_create.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,29 +12,31 @@
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class PaymentChannelCreate(Transaction):
     """
     Represents a `PaymentChannelCreate
     <https://xrpl.org/paymentchannelcreate.html>`_ transaction, which creates a
     `payment channel <https://xrpl.org/payment-channels.html>`_ and funds it with
-    XRP. The sender of this transaction is the "source address" of the payment
+    an amount. The sender of this transaction is the "source address" of the payment
     channel.
     """
 
     amount: Amount = REQUIRED  # type: ignore
     """
-    The amount of XRP, in drops, to set aside in this channel. This field is
-    required.
+    Amount to deduct from the sender's balance and set aside in this channel.
+    While the channel is open, the amount can only go to the Destination address.
+    When the channel closes, any unclaimed amount is returned to the source
+    address's balance. This field is required.
 
     :meta hide-value:
     """
 
     destination: str = REQUIRED  # type: ignore
     """
-    The account that can receive XRP from this channel, also known as the
+    The account that can receive amounts from this channel, also known as the
     "destination address" of the channel. Cannot be the same as the sender.
     This field is required.
 
     :meta hide-value:
     """
 
     settle_delay: int = REQUIRED  # type: ignore
```

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/payment_channel_fund.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,63 @@
-"""Model for a PaymentChannelFund transaction type."""
+"""Model for SetFee pseudo-transaction type."""
+
 from dataclasses import dataclass, field
 from typing import Optional
 
 from xrpl.models.required import REQUIRED
-from xrpl.models.transactions.transaction import Transaction
-from xrpl.models.transactions.types import TransactionType
+from xrpl.models.transactions.pseudo_transactions.pseudo_transaction import (
+    PseudoTransaction,
+)
+from xrpl.models.transactions.types import PseudoTransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class PaymentChannelFund(Transaction):
+class SetFee(PseudoTransaction):
+    """
+    A SetFee pseudo-transaction marks a change in `transaction cost
+    <https://xrpl.org/transaction-cost.html>`_ or `reserve requirements
+    <https://xrpl.org/reserves.html>`_ as a result of `Fee Voting
+    <https://xrpl.org/fee-voting.html>`_.
+    """
+
+    base_fee: str = REQUIRED  # type: ignore
     """
-    Represents a `PaymentChannelFund <https://xrpl.org/paymentchannelfund.html>`_
-    transaction, adds additional XRP to an open `payment channel
-    <https://xrpl.org/payment-channels.html>`_, and optionally updates the
-    expiration time of the channel. Only the source address
-    of the channel can use this transaction.
+    The charge, in drops of XRP, for the reference transaction, as hex. (This is the
+    transaction cost before scaling for load.) This field is required.
+
+    :meta hide-value:
+    """
+
+    reference_fee_units: int = REQUIRED  # type: ignore
+    """
+    The cost, in fee units, of the reference transaction. This field is required.
+
+    :meta hide-value:
     """
 
-    channel: str = REQUIRED  # type: ignore
+    reserve_base: int = REQUIRED  # type: ignore
     """
-    The unique ID of the payment channel, as a 64-character hexadecimal
-    string. This field is required.
+    The base reserve, in drops. This field is required.
 
     :meta hide-value:
     """
 
-    amount: str = REQUIRED  # type: ignore
+    reserve_increment: int = REQUIRED  # type: ignore
     """
-    The amount of XRP, in drops, to add to the channel. This field is
-    required.
+    The incremental reserve, in drops. This field is required.
 
     :meta hide-value:
     """
 
-    expiration: Optional[int] = None
+    ledger_sequence: Optional[int] = None
     """
-    A new mutable expiration time to set for the channel, in seconds since the
-    Ripple Epoch. This must be later than the existing expiration time of the
-    channel or later than the current time plus the settle delay of the channel.
-    This is separate from the immutable ``cancel_after`` time.
+    The index of the ledger version where this pseudo-transaction appears. This
+    distinguishes the pseudo-transaction from other occurrences of the same change.
+    This field is omitted for some historical SetFee pseudo-transactions.
     """
 
-    transaction_type: TransactionType = field(
-        default=TransactionType.PAYMENT_CHANNEL_FUND,
+    transaction_type: PseudoTransactionType = field(
+        default=PseudoTransactionType.SET_FEE,
         init=False,
     )
```

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/pseudo_transactions/__init__.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/pseudo_transactions/set_fee.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,71 @@
-"""Model for SetFee pseudo-transaction type."""
+"""Model for UNLModify pseudo-transaction type."""
+
+from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Optional
+from typing import Dict
 
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.pseudo_transactions.pseudo_transaction import (
     PseudoTransaction,
 )
 from xrpl.models.transactions.types import PseudoTransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class SetFee(PseudoTransaction):
-    """
-    A SetFee pseudo-transaction marks a change in `transaction cost
-    <https://xrpl.org/transaction-cost.html>`_ or `reserve requirements
-    <https://xrpl.org/reserves.html>`_ as a result of `Fee Voting
-    <https://xrpl.org/fee-voting.html>`_.
-    """
-
-    base_fee: str = REQUIRED  # type: ignore
+class UNLModify(PseudoTransaction):
     """
-    The charge, in drops of XRP, for the reference transaction, as hex. (This is the
-    transaction cost before scaling for load.) This field is required.
-
-    :meta hide-value:
+    A UNLModify pseudo-transaction marks a change to the `Negative UNL
+    <https://xrpl.org/negative-unl.html>`_, indicating that a trusted validator has
+    gone offline or come back online.
     """
 
-    reference_fee_units: int = REQUIRED  # type: ignore
+    ledger_sequence: int = REQUIRED  # type: ignore
     """
-    The cost, in fee units, of the reference transaction. This field is required.
+    The ledger index where this pseudo-transaction appears. This distinguishes the
+    pseudo-transaction from other occurrences of the same change.
+    This field is required.
 
     :meta hide-value:
     """
 
-    reserve_base: int = REQUIRED  # type: ignore
+    unl_modify_disabling: int = REQUIRED  # type: ignore
     """
-    The base reserve, in drops. This field is required.
+    If 1, this change represents adding a validator to the Negative UNL. If 0, this
+    change represents removing a validator from the Negative UNL. (No other values
+    are allowed.) This field is required.
 
     :meta hide-value:
     """
 
-    reserve_increment: int = REQUIRED  # type: ignore
+    unl_modify_validator: str = REQUIRED  # type: ignore
     """
-    The incremental reserve, in drops. This field is required.
+    The validator to add or remove, as identified by its master public key.
+    This field is required.
 
     :meta hide-value:
     """
 
-    ledger_sequence: Optional[int] = None
-    """
-    The index of the ledger version where this pseudo-transaction appears. This
-    distinguishes the pseudo-transaction from other occurrences of the same change.
-    This field is omitted for some historical SetFee pseudo-transactions.
-    """
-
     transaction_type: PseudoTransactionType = field(
-        default=PseudoTransactionType.SET_FEE,
+        default=PseudoTransactionType.UNL_MODIFY,
         init=False,
     )
+
+    flags: int = 0
+    """
+    The Flags value of the EnableAmendment pseudo-transaction indicates the status
+    of the amendment at the time of the ledger including the pseudo-transaction.
+    A Flags value of 0 (no flags) or an omitted Flags field indicates that the
+    amendment has been enabled, and applies to all ledgers afterward.
+    """
+
+    def _get_errors(self: UNLModify) -> Dict[str, str]:
+        errors = super()._get_errors()
+        if self.unl_modify_disabling not in {0, 1}:
+            errors[
+                "unl_modify_disabling"
+            ] = "`unl_modify_disabling` is not equal to 0 or 1."
+
+        return errors
```

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/pseudo_transactions/unl_modify.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_claim.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,87 @@
-"""Model for UNLModify pseudo-transaction type."""
+"""Model for a XChainClaim transaction type."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Dict
+from typing import Dict, Optional, Union
 
+from xrpl.models.amounts import Amount
+from xrpl.models.currencies import XRP
 from xrpl.models.required import REQUIRED
-from xrpl.models.transactions.pseudo_transactions.pseudo_transaction import (
-    PseudoTransaction,
-)
-from xrpl.models.transactions.types import PseudoTransactionType
+from xrpl.models.transactions.transaction import Transaction
+from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
+from xrpl.models.xchain_bridge import XChainBridge
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class UNLModify(PseudoTransaction):
+class XChainClaim(Transaction):
     """
-    A UNLModify pseudo-transaction marks a change to the `Negative UNL
-    <https://xrpl.org/negative-unl.html>`_, indicating that a trusted validator has
-    gone offline or come back online.
+    Represents a XChainClaim transaction.
+    The ``XChainClaim`` transaction completes a cross-chain transfer of value.
+    It allows a user to claim the value on the destination chain - the
+    equivalent of the value locked on the source chain.
     """
 
-    ledger_sequence: int = REQUIRED  # type: ignore
+    xchain_bridge: XChainBridge = REQUIRED  # type: ignore
     """
-    The ledger index where this pseudo-transaction appears. This distinguishes the
-    pseudo-transaction from other occurrences of the same change.
-    This field is required.
+    The bridge to use for the transfer. This field is required.
 
     :meta hide-value:
     """
 
-    unl_modify_disabling: int = REQUIRED  # type: ignore
+    xchain_claim_id: Union[int, str] = REQUIRED  # type: ignore
     """
-    If 1, this change represents adding a validator to the Negative UNL. If 0, this
-    change represents removing a validator from the Negative UNL. (No other values
-    are allowed.) This field is required.
+    The unique integer ID for the cross-chain transfer that was referenced in
+    the corresponding ``XChainCommit`` transaction. This field is required.
 
     :meta hide-value:
     """
 
-    unl_modify_validator: str = REQUIRED  # type: ignore
+    destination: str = REQUIRED  # type: ignore
     """
-    The validator to add or remove, as identified by its master public key.
-    This field is required.
+    The destination account on the destination chain. It must exist or the
+    transaction will fail. However, if the transaction fails in this case, the
+    sequence number and collected signatures won't be destroyed, and the
+    transaction can be rerun with a different destination. This field is
+    required.
 
     :meta hide-value:
     """
 
-    transaction_type: PseudoTransactionType = field(
-        default=PseudoTransactionType.UNL_MODIFY,
-        init=False,
-    )
+    destination_tag: Optional[int] = None
+    """
+    An integer destination tag.
 
-    flags: int = 0
+    :meta hide-value:
     """
-    The Flags value of the EnableAmendment pseudo-transaction indicates the status
-    of the amendment at the time of the ledger including the pseudo-transaction.
-    A Flags value of 0 (no flags) or an omitted Flags field indicates that the
-    amendment has been enabled, and applies to all ledgers afterward.
+
+    amount: Amount = REQUIRED  # type: ignore
     """
+    The amount to claim on the destination chain. This must match the amount
+    attested to on the attestations associated with this ``XChainClaimID``.
+    This field is required.
 
-    def _get_errors(self: UNLModify) -> Dict[str, str]:
+    :meta hide-value:
+    """
+
+    transaction_type: TransactionType = field(
+        default=TransactionType.XCHAIN_CLAIM,
+        init=False,
+    )
+
+    def _get_errors(self: XChainClaim) -> Dict[str, str]:
         errors = super()._get_errors()
-        if self.unl_modify_disabling not in {0, 1}:
+
+        bridge = self.xchain_bridge
+        currency = XRP() if isinstance(self.amount, str) else self.amount.to_currency()
+        if (
+            currency != bridge.locking_chain_issue
+            and currency != bridge.issuing_chain_issue
+        ):
             errors[
-                "unl_modify_disabling"
-            ] = "`unl_modify_disabling` is not equal to 0 or 1."
+                "amount"
+            ] = "Amount must match either locking chain issue or issuing chain issue."
 
         return errors
```

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/set_regular_key.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/set_regular_key.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/signer_list_set.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/signer_list_set.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/ticket_create.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/ticket_create.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/transaction.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,31 @@
 from hashlib import sha512
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 from typing_extensions import Final
 
 from xrpl.core.binarycodec import decode, encode
 from xrpl.models.amounts import IssuedCurrencyAmount
-from xrpl.models.base_model import BaseModel
+from xrpl.models.base_model import ABBREVIATIONS, BaseModel
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.flags import check_false_flag_definition, interface_to_flag_list
 from xrpl.models.nested_model import NestedModel
 from xrpl.models.requests import PathStep
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.types import PseudoTransactionType, TransactionType
 from xrpl.models.types import XRPL_VALUE_TYPE
 from xrpl.models.utils import require_kwargs_on_init
 
 _TRANSACTION_HASH_PREFIX: Final[int] = 0x54584E00
-# This is used to make exceptions when converting dictionary keys to xrpl JSON
-# keys. We snake case keys, but some keys are abbreviations.
-_ABBREVIATIONS: Final[Dict[str, str]] = {
-    "unl": "UNL",
-    "id": "ID",
-    "uri": "URI",
-    "nftoken": "NFToken",
-}
+
+# special cases that should not be snake cased and only contain primitive members
+_LOWER_CASE_MODELS: List[Type[BaseModel]] = [
+    IssuedCurrencyAmount,
+    PathStep,
+]
 
 
 def transaction_json_to_binary_codec_form(
     dictionary: Dict[str, XRPL_VALUE_TYPE]
 ) -> Dict[str, XRPL_VALUE_TYPE]:
     """
     Returns a new dictionary in which the keys have been formatted as CamelCase and
@@ -52,36 +50,43 @@
 
 def _key_to_tx_json(key: str) -> str:
     """
     Transforms snake_case to PascalCase. For example:
         1. 'transaction_type' becomes 'TransactionType'
         2. 'URI' becomes 'uri'
 
-    Known abbreviations (example 2 above) need to be enumerated in _ABBREVIATIONS.
+    Known abbreviations (example 2 above) need to be enumerated in ABBREVIATIONS.
     """
     return "".join(
         [
-            _ABBREVIATIONS[word] if word in _ABBREVIATIONS else word.capitalize()
+            ABBREVIATIONS[word] if word in ABBREVIATIONS else word.capitalize()
             for word in key.split("_")
         ]
     )
 
 
 def _value_to_tx_json(value: XRPL_VALUE_TYPE) -> XRPL_VALUE_TYPE:
-    # IssuedCurrencyAmount and PathStep are special cases and should not be snake cased
-    # and only contain primitive members
-    if IssuedCurrencyAmount.is_dict_of_model(value) or PathStep.is_dict_of_model(value):
+    if isinstance(value, dict) and "auth_account" in value:
+        return _auth_account_value_to_tx_json(value)
+    if any([model.is_dict_of_model(value) for model in _LOWER_CASE_MODELS]):
         return value
     if isinstance(value, dict):
         return transaction_json_to_binary_codec_form(value)
     if isinstance(value, list):
         return [_value_to_tx_json(sub_value) for sub_value in value]
     return value
 
 
+def _auth_account_value_to_tx_json(value: Dict[str, Any]) -> Dict[str, Any]:
+    return {
+        _key_to_tx_json(key): transaction_json_to_binary_codec_form(val)
+        for (key, val) in value.items()
+    }
+
+
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class Memo(NestedModel):
     """
     An arbitrary piece of data attached to a transaction. A transaction can
     have multiple Memo objects as an array in the Memos field.
     Must contain one or more of ``memo_data``, ``memo_format``, and
```

### Comparing `xrpl-py-2.1.0/xrpl/models/transactions/trust_set.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/trust_set.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/types.py` & `xrpl_py-2.1.0b0/xrpl/models/types.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/models/utils.py` & `xrpl_py-2.1.0b0/xrpl/models/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/transaction/__init__.py` & `xrpl_py-2.1.0b0/xrpl/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/transaction/main.py` & `xrpl_py-2.1.0b0/xrpl/transaction/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/transaction/multisign.py` & `xrpl_py-2.1.0b0/xrpl/transaction/multisign.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/transaction/reliable_submission.py` & `xrpl_py-2.1.0b0/xrpl/transaction/reliable_submission.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/__init__.py` & `xrpl_py-2.1.0b0/xrpl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/get_nftoken_id.py` & `xrpl_py-2.1.0b0/xrpl/utils/get_nftoken_id.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/parse_nftoken_id.py` & `xrpl_py-2.1.0b0/xrpl/utils/parse_nftoken_id.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/str_conversions.py` & `xrpl_py-2.1.0b0/xrpl/utils/str_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/time_conversions.py` & `xrpl_py-2.1.0b0/xrpl/utils/time_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/txn_parser/get_balance_changes.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_balance_changes.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/txn_parser/get_final_balances.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_final_balances.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/txn_parser/get_order_book_changes.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_order_book_changes.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/txn_parser/utils/__init__.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/txn_parser/utils/balance_parser.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/balance_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/txn_parser/utils/nodes.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/nodes.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/txn_parser/utils/order_book_parser.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/txn_parser/utils/parser.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/parser.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/txn_parser/utils/types.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/types.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/utils/xrp_conversions.py` & `xrpl_py-2.1.0b0/xrpl/utils/xrp_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/wallet/main.py` & `xrpl_py-2.1.0b0/xrpl/wallet/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/xrpl/wallet/wallet_generation.py` & `xrpl_py-2.1.0b0/xrpl/wallet/wallet_generation.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.1.0/setup.py` & `xrpl_py-2.1.0b0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,353 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+[![Documentation Status](https://readthedocs.org/projects/xrpl-py/badge)](https://xrpl-py.readthedocs.io/)
 
-packages = \
-['xrpl',
- 'xrpl.account',
- 'xrpl.asyncio',
- 'xrpl.asyncio.account',
- 'xrpl.asyncio.clients',
- 'xrpl.asyncio.ledger',
- 'xrpl.asyncio.transaction',
- 'xrpl.asyncio.wallet',
- 'xrpl.clients',
- 'xrpl.core',
- 'xrpl.core.addresscodec',
- 'xrpl.core.binarycodec',
- 'xrpl.core.binarycodec.binary_wrappers',
- 'xrpl.core.binarycodec.definitions',
- 'xrpl.core.binarycodec.types',
- 'xrpl.core.keypairs',
- 'xrpl.ledger',
- 'xrpl.models',
- 'xrpl.models.amounts',
- 'xrpl.models.currencies',
- 'xrpl.models.requests',
- 'xrpl.models.transactions',
- 'xrpl.models.transactions.pseudo_transactions',
- 'xrpl.models.transactions.types',
- 'xrpl.transaction',
- 'xrpl.utils',
- 'xrpl.utils.txn_parser',
- 'xrpl.utils.txn_parser.utils',
- 'xrpl.wallet']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Deprecated>=1.2.13,<2.0.0',
- 'ECPy>=1.2.5,<2.0.0',
- 'base58>=2.1.0,<3.0.0',
- 'httpx>=0.18.1,<0.25.0',
- 'pycryptodome>=3.16.0,<4.0.0',
- 'types-Deprecated>=1.2.9,<2.0.0',
- 'typing-extensions>=4.2.0,<5.0.0']
-
-extras_require = \
-{':python_version >= "3.10" and python_version < "4.0"': ['websockets>=10.0,<11.0'],
- ':python_version >= "3.7" and python_version < "3.10"': ['websockets>=9.0.1,<11.0']}
-
-setup_kwargs = {
-    'name': 'xrpl-py',
-    'version': '2.1.0',
-    'description': 'A complete Python library for interacting with the XRP ledger',
-    'long_description': '[![Documentation Status](https://readthedocs.org/projects/xrpl-py/badge)](https://xrpl-py.readthedocs.io/)\n\n# xrpl-py\n\nA pure Python implementation for interacting with the [XRP Ledger](https://xrpl.org/). \n\nThe `xrpl-py` library simplifies the hardest parts of XRP Ledger interaction, like serialization and transaction signing. It also provides native Python methods and models for [XRP Ledger transactions](https://xrpl.org/transaction-formats.html) and core server [API](https://xrpl.org/api-conventions.html) ([`rippled`](https://github.com/ripple/rippled)) objects.\n\nAs an example, this is how you would use this library to send a payment on testnet:\n\n```py\nfrom xrpl.account import get_balance\nfrom xrpl.clients import JsonRpcClient\nfrom xrpl.models import Payment, Tx\nfrom xrpl.transaction import submit_and_wait\nfrom xrpl.wallet import generate_faucet_wallet\n\n# Create a client to connect to the test network\nclient = JsonRpcClient("https://s.altnet.rippletest.net:51234")\n\n# Create two wallets to send money between on the test network\nwallet1 = generate_faucet_wallet(client, debug=True)\nwallet2 = generate_faucet_wallet(client, debug=True)\n\n# Both balances should be zero since nothing has been sent yet\nprint("Balances of wallets before Payment tx")\nprint(get_balance(wallet1.address, client))\nprint(get_balance(wallet2.address, client))\n\n# Create a Payment transaction from wallet1 to wallet2\npayment_tx = Payment(\n    account=wallet1.address,\n    amount="1000",\n    destination=wallet2.address,\n)\n\n# Submit the payment to the network and wait to see a response\n#   Behind the scenes, this fills in fields which can be looked up automatically like the fee.\n#   It also signs the transaction with wallet1 to prove you own the account you\'re paying from.\npayment_response = submit_and_wait(payment_tx, client, wallet1)\nprint("Transaction was submitted")\n\n# Create a "Tx" request to look up the transaction on the ledger\ntx_response = client.request(Tx(transaction=payment_response.result["hash"]))\n\n# Check whether the transaction was actually validated on ledger\nprint("Validated:", tx_response.result["validated"])\n\n# Check balances after 1000 drops (.001 XRP) was sent from wallet1 to wallet2\nprint("Balances of wallets after Payment tx:")\nprint(get_balance(wallet1.address, client))\nprint(get_balance(wallet2.address, client))\n```\n\n[![Downloads](https://pepy.tech/badge/xrpl-py/month)](https://pepy.tech/project/xrpl-py/month)\n[![Contributors](https://img.shields.io/github/contributors/xpring-eng/xrpl-py.svg)](https://github.com/xpring-eng/xrpl-py/graphs/contributors)\n\n## Installation and supported versions\n\nThe `xrpl-py` library is available on [PyPI](https://pypi.org/). Install with `pip`:\n\n\n```\npip3 install xrpl-py\n```\n\nThe library supports [Python 3.7](https://www.python.org/downloads/) and later.\n\n[![Supported Versions](https://img.shields.io/pypi/pyversions/xrpl-py.svg)](https://pypi.org/project/xrpl-py)\n\n\n## Features\n\nUse `xrpl-py` to build Python applications that leverage the [XRP Ledger](https://xrpl.org/). The library helps with all aspects of interacting with the XRP Ledger, including:\n\n* Key and wallet management\n* Serialization\n* Transaction Signing\n\n`xrpl-py` also provides:\n\n* A network client — See [`xrpl.clients`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.clients.html) for more information.\n* Methods for inspecting accounts — See [XRPL Account Methods](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.account.html) for more information.\n* Codecs for encoding and decoding addresses and other objects — See [Core Codecs](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.html) for more information.\n\n## [➡️ Reference Documentation](https://xrpl-py.readthedocs.io/en/stable/)\n\nSee the complete [`xrpl-py` reference documentation on Read the Docs](https://xrpl-py.readthedocs.io/en/stable/index.html).\n\n\n## Usage\n\nThe following sections describe some of the most commonly used modules in the `xrpl-py` library and provide sample code.\n\n### Network client\n\nUse the `xrpl.clients` library to create a network client for connecting to the XRP Ledger.\n\n```py\nfrom xrpl.clients import JsonRpcClient\nJSON_RPC_URL = "https://s.altnet.rippletest.net:51234"\nclient = JsonRpcClient(JSON_RPC_URL)\n```\n\n### Manage keys and wallets\n\n#### `xrpl.wallet`\n\nUse the [`xrpl.wallet`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.wallet.html) module to create a wallet from a given seed or or via a [Testnet faucet](https://xrpl.org/xrp-testnet-faucet.html).\n\nTo create a wallet from a seed (in this case, the value generated using [`xrpl.keypairs`](#xrpl-keypairs)):\n\n```py\nwallet_from_seed = xrpl.wallet.Wallet.from_seed(seed)\nprint(wallet_from_seed)\n# pub_key: ED46949E414A3D6D758D347BAEC9340DC78F7397FEE893132AAF5D56E4D7DE77B0\n# priv_key: -HIDDEN-\n# address: rG5ZvYsK5BPi9f1Nb8mhFGDTNMJhEhufn6\n```\n\nTo create a wallet from a Testnet faucet:\n\n```py\ntest_wallet = generate_faucet_wallet(client)\ntest_account = test_wallet.address\nprint("Classic address:", test_account)\n# Classic address: rEQB2hhp3rg7sHj6L8YyR4GG47Cb7pfcuw\n```\n\n#### `xrpl.core.keypairs`\n\nUse the [`xrpl.core.keypairs`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html#module-xrpl.core.keypairs) module to generate seeds and derive keypairs and addresses from those seed values.\n\nHere\'s an example of how to generate a `seed` value and derive an [XRP Ledger "classic" address](https://xrpl.org/cryptographic-keys.html#account-id-and-address) from that seed.\n\n\n```py\nfrom xrpl.core import keypairs\nseed = keypairs.generate_seed()\npublic, private = keypairs.derive_keypair(seed)\ntest_account = keypairs.derive_classic_address(public)\nprint("Here\'s the public key:")\nprint(public)\nprint("Here\'s the private key:")\nprint(private)\nprint("Store this in a secure place!")\n# Here\'s the public key:\n# ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56\n# Here\'s the private key:\n# EDE65EE7882847EF5345A43BFB8E6F5EEC60F45461696C384639B99B26AAA7A5CD\n# Store this in a secure place!\n```\n\n**Note:** You can use `xrpl.core.keypairs.sign` to sign transactions but `xrpl-py` also provides explicit methods for safely signing and submitting transactions. See [Transaction Signing](#transaction-signing) and [XRPL Transaction Methods](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#module-xrpl.transaction) for more information.\n\n\n### Serialize and sign transactions\n\nTo securely submit transactions to the XRP Ledger, you need to first serialize data from JSON and other formats into the [XRP Ledger\'s canonical format](https://xrpl.org/serialization.html), then to [authorize the transaction](https://xrpl.org/transaction-basics.html#authorizing-transactions) by digitally [signing it](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html?highlight=sign#xrpl.core.keypairs.sign) with the account\'s private key. The `xrpl-py` library provides several methods to simplify this process.\n\n\nUse the [`xrpl.transaction`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html) module to sign and submit transactions. The module offers three ways to do this:\n\n* [`sign_and_submit`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign_and_submit) — Signs a transaction locally, then submits it to the XRP Ledger. This method does not implement [reliable transaction submission](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission) best practices, so only use it for development or testing purposes.\n\n* [`sign`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign) — Signs a transaction locally. This method **does  not** submit the transaction to the XRP Ledger.\n\n* [`submit_and_wait`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.submit_and_wait) — An implementation of the [reliable transaction submission guidelines](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission), this method submits a signed transaction to the XRP Ledger and then verifies that it has been included in a validated ledger (or has failed to do so). Use this method to submit transactions for production purposes.\n\n\n```py\nfrom xrpl.models.transactions import Payment\nfrom xrpl.transaction import sign, submit_and_wait\nfrom xrpl.ledger import get_latest_validated_ledger_sequence\nfrom xrpl.account import get_next_valid_seq_number\n\ncurrent_validated_ledger = get_latest_validated_ledger_sequence(client)\n\n# prepare the transaction\n# the amount is expressed in drops, not XRP\n# see https://xrpl.org/basic-data-types.html#specifying-currency-amounts\nmy_tx_payment = Payment(\n    account=test_wallet.address,\n    amount="2200000",\n    destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",\n    last_ledger_sequence=current_validated_ledger + 20,\n    sequence=get_next_valid_seq_number(test_wallet.address, client),\n    fee="10",\n)\n# sign the transaction\nmy_tx_payment_signed = sign(my_tx_payment,test_wallet)\n\n# submit the transaction\ntx_response = submit_and_wait(my_tx_payment_signed, client)\n```\n\n#### Get fee from the XRP Ledger\n\n\nIn most cases, you can specify the minimum [transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) of `"10"` for the `fee` field unless you have a strong reason not to. But if you want to get the [current load-balanced transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) from the network, you can use the `get_fee` function:\n\n```py\nfrom xrpl.ledger import get_fee\nfee = get_fee(client)\nprint(fee)\n# 10\n```\n\n#### Auto-filled fields\n\nThe `xrpl-py` library automatically populates the `fee`, `sequence` and `last_ledger_sequence` fields when you create transactions. In the example above, you could omit those fields and let the library fill them in for you.\n\n```py\nfrom xrpl.models.transactions import Payment\nfrom xrpl.transaction import submit_and_wait, autofill_and_sign\n# prepare the transaction\n# the amount is expressed in drops, not XRP\n# see https://xrpl.org/basic-data-types.html#specifying-currency-amounts\nmy_tx_payment = Payment(\n    account=test_wallet.address,\n    amount="2200000",\n    destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe"\n)\n\n# sign the transaction with the autofill method\n# (this will auto-populate the fee, sequence, and last_ledger_sequence)\nmy_tx_payment_signed = autofill_and_sign(my_tx_payment, client, test_wallet)\nprint(my_tx_payment_signed)\n# Payment(\n#     account=\'rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz\',\n#     transaction_type=<TransactionType.PAYMENT: \'Payment\'>,\n#     fee=\'10\',\n#     sequence=16034065,\n#     account_txn_id=None,\n#     flags=0,\n#     last_ledger_sequence=10268600,\n#     memos=None,\n#     signers=None,\n#     source_tag=None,\n#     signing_pub_key=\'EDD9540FA398915F0BCBD6E65579C03BE5424836CB68B7EB1D6573F2382156B444\',\n#     txn_signature=\'938FB22AE7FE76CF26FD11F8F97668E175DFAABD2977BCA397233117E7E1C4A1E39681091CC4D6DF21403682803AB54CC21DC4FA2F6848811DEE10FFEF74D809\',\n#     amount=\'2200000\',\n#     destination=\'rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe\',\n#     destination_tag=None,\n#     invoice_id=None,\n#     paths=None,\n#     send_max=None,\n#     deliver_min=None\n# )\n\n# submit the transaction\ntx_response = submit_and_wait(my_tx_payment_signed, client)\n```\n\n\n### Subscribe to ledger updates\n\nYou can send `subscribe` and `unsubscribe` requests only using the WebSocket network client. These request methods allow you to be alerted of certain situations as they occur, such as when a new ledger is declared.\n\n```py\nfrom xrpl.clients import WebsocketClient\nurl = "wss://s.altnet.rippletest.net/"\nfrom xrpl.models import Subscribe, StreamParameter\nreq = Subscribe(streams=[StreamParameter.LEDGER])\n# NOTE: this code will run forever without a timeout, until the process is killed\nwith WebsocketClient(url) as client:\n    client.send(req)\n    for message in client:\n        print(message)\n# {\'result\': {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'7CD50477F23FF158B430772D8E82A961376A7B40E13C695AA849811EDF66C5C0\', \'ledger_index\': 18183504, \'ledger_time\': 676412962, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'validated_ledgers\': \'17469391-18183504\'}, \'status\': \'success\', \'type\': \'response\'}\n# {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'BAA743DABD168BD434804416C8087B7BDEF7E6D7EAD412B9102281DD83B10D00\', \'ledger_index\': 18183505, \'ledger_time\': 676412970, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'txn_count\': 0, \'type\': \'ledgerClosed\', \'validated_ledgers\': \'17469391-18183505\'}\n# {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'D8227DAF8F745AE3F907B251D40B4081E019D013ABC23B68C0B1431DBADA1A46\', \'ledger_index\': 18183506, \'ledger_time\': 676412971, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'txn_count\': 0, \'type\': \'ledgerClosed\', \'validated_ledgers\': \'17469391-18183506\'}\n# {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'CFC412B6DDB9A402662832A781C23F0F2E842EAE6CFC539FEEB287318092C0DE\', \'ledger_index\': 18183507, \'ledger_time\': 676412972, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'txn_count\': 0, \'type\': \'ledgerClosed\', \'validated_ledgers\': \'17469391-18183507\'}\n```\n\n\n### Asynchronous Code\n\nThis library supports Python\'s [`asyncio`](https://docs.python.org/3/library/asyncio.html) package, which is used to run asynchronous code. All the async code is in [`xrpl.asyncio`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.asyncio.html) If you are writing asynchronous code, please note that you will not be able to use any synchronous sugar functions, due to how event loops are handled. However, every synchronous method has a corresponding asynchronous method that you can use.\n\nThis sample code is the asynchronous equivalent of the above section on submitting a transaction.\n\n```py\nimport asyncio\nfrom xrpl.models.transactions import Payment\nfrom xrpl.asyncio.transaction import sign, submit_and_wait\nfrom xrpl.asyncio.ledger import get_latest_validated_ledger_sequence\nfrom xrpl.asyncio.account import get_next_valid_seq_number\nfrom xrpl.asyncio.clients import AsyncJsonRpcClient\n\nasync_client = AsyncJsonRpcClient(JSON_RPC_URL)\n\nasync def submit_sample_transaction():\n    current_validated_ledger = await get_latest_validated_ledger_sequence(async_client)\n\n    # prepare the transaction\n    # the amount is expressed in drops, not XRP\n    # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts\n    my_tx_payment = Payment(\n        account=test_wallet.address,\n        amount="2200000",\n        destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",\n        last_ledger_sequence=current_validated_ledger + 20,\n        sequence=await get_next_valid_seq_number(test_wallet.address, async_client),\n        fee="10",\n    )\n    # sign and submit the transaction\n    tx_response = await submit_and_wait(my_tx_payment_signed, async_client, test_wallet)\n\nasyncio.run(submit_sample_transaction())\n```\n\n### Encode addresses\n\nUse [`xrpl.core.addresscodec`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.addresscodec.html) to encode and decode addresses into and from the ["classic" and X-address formats](https://xrpl.org/accounts.html#addresses).\n\n```py\n# convert classic address to x-address\nfrom xrpl.core import addresscodec\ntestnet_xaddress = (\n    addresscodec.classic_address_to_xaddress(\n        "rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz",\n        tag=0,\n        is_test_network=True,\n    )\n)\nprint(testnet_xaddress)\n# T7QDemmxnuN7a52A62nx2fxGPWcRahLCf3qaswfrsNW9Lps\n```\n\n## Migrating\n\nIf you\'re currently using `xrpl-py` version 1, you can use [this guide to migrate to v2](https://xrpl.org/blog/2023/xrpl-py-2.0-release.html).\n\n## Contributing\n\nIf you want to contribute to this project, see [CONTRIBUTING.md].\n\n### Mailing Lists\n\nWe have a low-traffic mailing list for announcements of new `xrpl-py` releases. (About 1 email per week)\n\n+ [Subscribe to xrpl-announce](https://groups.google.com/g/xrpl-announce)\n\nIf you\'re using the XRP Ledger in production, you should run a [rippled server](https://github.com/ripple/rippled) and subscribe to the ripple-server mailing list as well.\n\n+ [Subscribe to ripple-server](https://groups.google.com/g/ripple-server)\n\n### Code Samples\n- For samples of common use cases, see the [XRPL.org Code Samples](https://xrpl.org/code-samples.html) page.\n- You can also browse those samples [directly on GitHub](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples).\n\n### Report an issue\n\nExperienced an issue? Report it [here](https://github.com/XRPLF/xrpl-py/issues/new).\n\n## License\n\nThe `xrpl-py` library is licensed under the ISC License. See [LICENSE] for more information.\n\n\n\n[CONTRIBUTING.md]: CONTRIBUTING.md\n[LICENSE]: LICENSE\n',
-    'author': 'Mayukha Vadari',
-    'author_email': 'mvadari@ripple.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/XRPLF/xrpl-py',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+# xrpl-py
 
+A pure Python implementation for interacting with the XRP Ledger, the `xrpl-py` library simplifies the hardest parts of XRP Ledger interaction, like serialization and transaction signing, by providing native Python methods and models for [XRP Ledger transactions](https://xrpl.org/transaction-formats.html) and core server [API](https://xrpl.org/api-conventions.html) ([`rippled`](https://github.com/ripple/rippled)) objects.
 
-setup(**setup_kwargs)
+
+
+```py
+# create a network client
+from xrpl.clients import JsonRpcClient
+client = JsonRpcClient("https://s.altnet.rippletest.net:51234")
+
+# create a wallet on the testnet
+from xrpl.wallet import generate_faucet_wallet
+test_wallet = generate_faucet_wallet(client)
+print(test_wallet)
+public_key: ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56
+private_key: -HIDDEN-
+address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo
+
+# look up account info
+from xrpl.models import AccountInfo
+acct_info = AccountInfo(
+    account="rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",
+    ledger_index="current",
+    queue=True,
+    strict=True,
+)
+response = client.request(acct_info)
+result = response.result
+import json
+print(json.dumps(result["account_data"], indent=4, sort_keys=True))
+# {
+#     "Account": "rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",
+#     "Balance": "1000000000",
+#     "Flags": 0,
+#     "LedgerEntryType": "AccountRoot",
+#     "OwnerCount": 0,
+#     "PreviousTxnID": "73CD4A37537A992270AAC8472F6681F44E400CBDE04EC8983C34B519F56AB107",
+#     "PreviousTxnLgrSeq": 16233962,
+#     "Sequence": 16233962,
+#     "index": "FD66EC588B52712DCE74831DCB08B24157DC3198C29A0116AA64D310A58512D7"
+# }
+```
+
+[![Downloads](https://pepy.tech/badge/xrpl-py/month)](https://pepy.tech/project/xrpl-py/month)
+[![Contributors](https://img.shields.io/github/contributors/xpring-eng/xrpl-py.svg)](https://github.com/xpring-eng/xrpl-py/graphs/contributors)
+
+## Installation and supported versions
+
+The `xrpl-py` library is available on [PyPI](https://pypi.org/). Install with `pip`:
+
+
+```
+pip3 install xrpl-py
+```
+
+The library supports [Python 3.7](https://www.python.org/downloads/) and later.
+
+[![Supported Versions](https://img.shields.io/pypi/pyversions/xrpl-py.svg)](https://pypi.org/project/xrpl-py)
+
+
+## Features
+
+Use `xrpl-py` to build Python applications that leverage the [XRP Ledger](https://xrpl.org/). The library helps with all aspects of interacting with the XRP Ledger, including:
+
+* Key and wallet management
+* Serialization
+* Transaction Signing
+
+`xrpl-py` also provides:
+
+* A network client — See [`xrpl.clients`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.clients.html) for more information.
+* Methods for inspecting accounts — See [XRPL Account Methods](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.account.html) for more information.
+* Codecs for encoding and decoding addresses and other objects — See [Core Codecs](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.html) for more information.
+
+## [➡️ Reference Documentation](https://xrpl-py.readthedocs.io/en/stable/)
+
+See the complete [`xrpl-py` reference documentation on Read the Docs](https://xrpl-py.readthedocs.io/en/stable/index.html).
+
+
+## Usage
+
+The following sections describe some of the most commonly used modules in the `xrpl-py` library and provide sample code.
+
+### Network client
+
+Use the `xrpl.clients` library to create a network client for connecting to the XRP Ledger.
+
+```py
+from xrpl.clients import JsonRpcClient
+JSON_RPC_URL = "https://s.altnet.rippletest.net:51234"
+client = JsonRpcClient(JSON_RPC_URL)
+```
+
+### Manage keys and wallets
+
+#### `xrpl.wallet`
+
+Use the [`xrpl.wallet`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.wallet.html) module to create a wallet from a given seed or or via a [Testnet faucet](https://xrpl.org/xrp-testnet-faucet.html).
+
+To create a wallet from a seed (in this case, the value generated using [`xrpl.keypairs`](#xrpl-keypairs)):
+
+```py
+wallet_from_seed = xrpl.wallet.Wallet.from_seed(seed)
+print(wallet_from_seed)
+# pub_key: ED46949E414A3D6D758D347BAEC9340DC78F7397FEE893132AAF5D56E4D7DE77B0
+# priv_key: -HIDDEN-
+# address: rG5ZvYsK5BPi9f1Nb8mhFGDTNMJhEhufn6
+```
+
+To create a wallet from a Testnet faucet:
+
+```py
+test_wallet = generate_faucet_wallet(client)
+test_account = test_wallet.address
+print("Classic address:", test_account)
+# Classic address: rEQB2hhp3rg7sHj6L8YyR4GG47Cb7pfcuw
+```
+
+#### `xrpl.core.keypairs`
+
+Use the [`xrpl.core.keypairs`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html#module-xrpl.core.keypairs) module to generate seeds and derive keypairs and addresses from those seed values.
+
+Here's an example of how to generate a `seed` value and derive an [XRP Ledger "classic" address](https://xrpl.org/cryptographic-keys.html#account-id-and-address) from that seed.
+
+
+```py
+from xrpl.core import keypairs
+seed = keypairs.generate_seed()
+public, private = keypairs.derive_keypair(seed)
+test_account = keypairs.derive_classic_address(public)
+print("Here's the public key:")
+print(public)
+print("Here's the private key:")
+print(private)
+print("Store this in a secure place!")
+# Here's the public key:
+# ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56
+# Here's the private key:
+# EDE65EE7882847EF5345A43BFB8E6F5EEC60F45461696C384639B99B26AAA7A5CD
+# Store this in a secure place!
+```
+
+**Note:** You can use `xrpl.core.keypairs.sign` to sign transactions but `xrpl-py` also provides explicit methods for safely signing and submitting transactions. See [Transaction Signing](#transaction-signing) and [XRPL Transaction Methods](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#module-xrpl.transaction) for more information.
+
+
+### Serialize and sign transactions
+
+To securely submit transactions to the XRP Ledger, you need to first serialize data from JSON and other formats into the [XRP Ledger's canonical format](https://xrpl.org/serialization.html), then to [authorize the transaction](https://xrpl.org/transaction-basics.html#authorizing-transactions) by digitally [signing it](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html?highlight=sign#xrpl.core.keypairs.sign) with the account's private key. The `xrpl-py` library provides several methods to simplify this process.
+
+
+Use the [`xrpl.transaction`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html) module to sign and submit transactions. The module offers three ways to do this:
+
+* [`sign_and_submit`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign_and_submit) — Signs a transaction locally, then submits it to the XRP Ledger. This method does not implement [reliable transaction submission](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission) best practices, so only use it for development or testing purposes.
+
+* [`sign`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign) — Signs a transaction locally. This method **does  not** submit the transaction to the XRP Ledger.
+
+* [`submit_and_wait`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.submit_and_wait) — An implementation of the [reliable transaction submission guidelines](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission), this method submits a signed transaction to the XRP Ledger and then verifies that it has been included in a validated ledger (or has failed to do so). Use this method to submit transactions for production purposes.
+
+
+```py
+from xrpl.models.transactions import Payment
+from xrpl.transaction import sign, submit_and_wait
+from xrpl.ledger import get_latest_validated_ledger_sequence
+from xrpl.account import get_next_valid_seq_number
+
+current_validated_ledger = get_latest_validated_ledger_sequence(client)
+
+# prepare the transaction
+# the amount is expressed in drops, not XRP
+# see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
+my_tx_payment = Payment(
+    account=test_wallet.address,
+    amount="2200000",
+    destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",
+    last_ledger_sequence=current_validated_ledger + 20,
+    sequence=get_next_valid_seq_number(test_wallet.address, client),
+    fee="10",
+)
+# sign the transaction
+my_tx_payment_signed = sign(my_tx_payment,test_wallet)
+
+# submit the transaction
+tx_response = submit_and_wait(my_tx_payment_signed, client)
+```
+
+#### Get fee from the XRP Ledger
+
+
+In most cases, you can specify the minimum [transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) of `"10"` for the `fee` field unless you have a strong reason not to. But if you want to get the [current load-balanced transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) from the network, you can use the `get_fee` function:
+
+```py
+from xrpl.ledger import get_fee
+fee = get_fee(client)
+print(fee)
+# 10
+```
+
+#### Auto-filled fields
+
+The `xrpl-py` library automatically populates the `fee`, `sequence` and `last_ledger_sequence` fields when you create transactions. In the example above, you could omit those fields and let the library fill them in for you.
+
+```py
+from xrpl.models.transactions import Payment
+from xrpl.transaction import submit_and_wait, autofill_and_sign
+# prepare the transaction
+# the amount is expressed in drops, not XRP
+# see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
+my_tx_payment = Payment(
+    account=test_wallet.address,
+    amount="2200000",
+    destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe"
+)
+
+# sign the transaction with the autofill method
+# (this will auto-populate the fee, sequence, and last_ledger_sequence)
+my_tx_payment_signed = autofill_and_sign(my_tx_payment, client, test_wallet)
+print(my_tx_payment_signed)
+# Payment(
+#     account='rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz',
+#     transaction_type=<TransactionType.PAYMENT: 'Payment'>,
+#     fee='10',
+#     sequence=16034065,
+#     account_txn_id=None,
+#     flags=0,
+#     last_ledger_sequence=10268600,
+#     memos=None,
+#     signers=None,
+#     source_tag=None,
+#     signing_pub_key='EDD9540FA398915F0BCBD6E65579C03BE5424836CB68B7EB1D6573F2382156B444',
+#     txn_signature='938FB22AE7FE76CF26FD11F8F97668E175DFAABD2977BCA397233117E7E1C4A1E39681091CC4D6DF21403682803AB54CC21DC4FA2F6848811DEE10FFEF74D809',
+#     amount='2200000',
+#     destination='rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe',
+#     destination_tag=None,
+#     invoice_id=None,
+#     paths=None,
+#     send_max=None,
+#     deliver_min=None
+# )
+
+# submit the transaction
+tx_response = submit_and_wait(my_tx_payment_signed, client)
+```
+
+
+### Subscribe to ledger updates
+
+You can send `subscribe` and `unsubscribe` requests only using the WebSocket network client. These request methods allow you to be alerted of certain situations as they occur, such as when a new ledger is declared.
+
+```py
+from xrpl.clients import WebsocketClient
+url = "wss://s.altnet.rippletest.net/"
+from xrpl.models import Subscribe, StreamParameter
+req = Subscribe(streams=[StreamParameter.LEDGER])
+# NOTE: this code will run forever without a timeout, until the process is killed
+with WebsocketClient(url) as client:
+    client.send(req)
+    for message in client:
+        print(message)
+# {'result': {'fee_base': 10, 'fee_ref': 10, 'ledger_hash': '7CD50477F23FF158B430772D8E82A961376A7B40E13C695AA849811EDF66C5C0', 'ledger_index': 18183504, 'ledger_time': 676412962, 'reserve_base': 20000000, 'reserve_inc': 5000000, 'validated_ledgers': '17469391-18183504'}, 'status': 'success', 'type': 'response'}
+# {'fee_base': 10, 'fee_ref': 10, 'ledger_hash': 'BAA743DABD168BD434804416C8087B7BDEF7E6D7EAD412B9102281DD83B10D00', 'ledger_index': 18183505, 'ledger_time': 676412970, 'reserve_base': 20000000, 'reserve_inc': 5000000, 'txn_count': 0, 'type': 'ledgerClosed', 'validated_ledgers': '17469391-18183505'}
+# {'fee_base': 10, 'fee_ref': 10, 'ledger_hash': 'D8227DAF8F745AE3F907B251D40B4081E019D013ABC23B68C0B1431DBADA1A46', 'ledger_index': 18183506, 'ledger_time': 676412971, 'reserve_base': 20000000, 'reserve_inc': 5000000, 'txn_count': 0, 'type': 'ledgerClosed', 'validated_ledgers': '17469391-18183506'}
+# {'fee_base': 10, 'fee_ref': 10, 'ledger_hash': 'CFC412B6DDB9A402662832A781C23F0F2E842EAE6CFC539FEEB287318092C0DE', 'ledger_index': 18183507, 'ledger_time': 676412972, 'reserve_base': 20000000, 'reserve_inc': 5000000, 'txn_count': 0, 'type': 'ledgerClosed', 'validated_ledgers': '17469391-18183507'}
+```
+
+
+### Asynchronous Code
+
+This library supports Python's [`asyncio`](https://docs.python.org/3/library/asyncio.html) package, which is used to run asynchronous code. All the async code is in [`xrpl.asyncio`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.asyncio.html) If you are writing asynchronous code, please note that you will not be able to use any synchronous sugar functions, due to how event loops are handled. However, every synchronous method has a corresponding asynchronous method that you can use.
+
+This sample code is the asynchronous equivalent of the above section on submitting a transaction.
+
+```py
+import asyncio
+from xrpl.models.transactions import Payment
+from xrpl.asyncio.transaction import sign, submit_and_wait
+from xrpl.asyncio.ledger import get_latest_validated_ledger_sequence
+from xrpl.asyncio.account import get_next_valid_seq_number
+from xrpl.asyncio.clients import AsyncJsonRpcClient
+
+async_client = AsyncJsonRpcClient(JSON_RPC_URL)
+
+async def submit_sample_transaction():
+    current_validated_ledger = await get_latest_validated_ledger_sequence(async_client)
+
+    # prepare the transaction
+    # the amount is expressed in drops, not XRP
+    # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
+    my_tx_payment = Payment(
+        account=test_wallet.address,
+        amount="2200000",
+        destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",
+        last_ledger_sequence=current_validated_ledger + 20,
+        sequence=await get_next_valid_seq_number(test_wallet.address, async_client),
+        fee="10",
+    )
+    # sign and submit the transaction
+    tx_response = await submit_and_wait(my_tx_payment_signed, async_client, test_wallet)
+
+asyncio.run(submit_sample_transaction())
+```
+
+### Encode addresses
+
+Use [`xrpl.core.addresscodec`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.addresscodec.html) to encode and decode addresses into and from the ["classic" and X-address formats](https://xrpl.org/accounts.html#addresses).
+
+```py
+# convert classic address to x-address
+from xrpl.core import addresscodec
+testnet_xaddress = (
+    addresscodec.classic_address_to_xaddress(
+        "rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz",
+        tag=0,
+        is_test_network=True,
+    )
+)
+print(testnet_xaddress)
+# T7QDemmxnuN7a52A62nx2fxGPWcRahLCf3qaswfrsNW9Lps
+```
+
+
+## Contributing
+
+If you want to contribute to this project, see [CONTRIBUTING.md].
+
+### Mailing Lists
+
+We have a low-traffic mailing list for announcements of new `xrpl-py` releases. (About 1 email per week)
+
++ [Subscribe to xrpl-announce](https://groups.google.com/g/xrpl-announce)
+
+If you're using the XRP Ledger in production, you should run a [rippled server](https://github.com/ripple/rippled) and subscribe to the ripple-server mailing list as well.
+
++ [Subscribe to ripple-server](https://groups.google.com/g/ripple-server)
+
+### Code Samples
+- For samples of common use cases, see the [XRPL.org Code Samples](https://xrpl.org/code-samples.html) page.
+- You can also browse those samples [directly on GitHub](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples).
+
+### Report an issue
+
+Experienced an issue? Report it [here](https://github.com/XRPLF/xrpl-py/issues/new).
+
+## License
+
+The `xrpl-py` library is licensed under the ISC License. See [LICENSE] for more information.
+
+
+
+[CONTRIBUTING.md]: CONTRIBUTING.md
+[LICENSE]: LICENSE
```

