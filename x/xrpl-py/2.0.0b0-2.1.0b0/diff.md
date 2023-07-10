# Comparing `tmp/xrpl-py-2.0.0b0.tar.gz` & `tmp/xrpl_py-2.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrpl-py-2.0.0b0.tar", max compression
+gzip compressed data, was "xrpl_py-2.1.0b0.tar", max compression
```

## Comparing `xrpl-py-2.0.0b0.tar` & `xrpl_py-2.1.0b0.tar`

### file list

```diff
@@ -1,223 +1,241 @@
--rw-r--r--   0        0        0      740 2021-07-28 20:35:08.759607 xrpl-py-2.0.0b0/LICENSE
--rw-r--r--   0        0        0    15971 2022-12-15 20:10:31.004701 xrpl-py-2.0.0b0/README.md
--rw-r--r--   0        0        0     2234 2022-12-15 20:19:30.899020 xrpl-py-2.0.0b0/pyproject.toml
--rw-r--r--   0        0        0      348 2021-07-28 20:35:08.796326 xrpl-py-2.0.0b0/xrpl/__init__.py
--rw-r--r--   0        0        0      588 2022-09-15 21:17:14.712442 xrpl-py-2.0.0b0/xrpl/account/__init__.py
--rw-r--r--   0        0        0     4410 2022-12-15 20:10:31.050399 xrpl-py-2.0.0b0/xrpl/account/main.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.923644 xrpl-py-2.0.0b0/xrpl/account/py.typed
--rw-r--r--   0        0        0     2692 2022-12-15 20:10:31.051202 xrpl-py-2.0.0b0/xrpl/account/transaction_history.py
--rw-r--r--   0        0        0      189 2021-07-28 20:35:08.798278 xrpl-py-2.0.0b0/xrpl/asyncio/__init__.py
--rw-r--r--   0        0        0      610 2021-07-28 20:35:08.798757 xrpl-py-2.0.0b0/xrpl/asyncio/account/__init__.py
--rw-r--r--   0        0        0     5885 2022-12-15 20:10:31.052617 xrpl-py-2.0.0b0/xrpl/asyncio/account/main.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.923758 xrpl-py-2.0.0b0/xrpl/asyncio/account/py.typed
--rw-r--r--   0        0        0     3432 2022-12-15 20:10:31.053536 xrpl-py-2.0.0b0/xrpl/asyncio/account/transaction_history.py
--rw-r--r--   0        0        0      705 2022-04-05 18:02:24.758557 xrpl-py-2.0.0b0/xrpl/asyncio/clients/__init__.py
--rw-r--r--   0        0        0      692 2022-12-15 20:10:31.054509 xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_client.py
--rw-r--r--   0        0        0      315 2021-07-28 20:35:08.800248 xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_json_rpc_client.py
--rw-r--r--   0        0        0     7099 2022-12-15 20:10:31.055584 xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_websocket_client.py
--rw-r--r--   0        0        0     1066 2022-12-15 20:10:31.056911 xrpl-py-2.0.0b0/xrpl/asyncio/clients/client.py
--rw-r--r--   0        0        0     1083 2021-07-28 20:35:08.801049 xrpl-py-2.0.0b0/xrpl/asyncio/clients/exceptions.py
--rw-r--r--   0        0        0     1612 2022-12-15 20:10:31.057676 xrpl-py-2.0.0b0/xrpl/asyncio/clients/json_rpc_base.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.923862 xrpl-py-2.0.0b0/xrpl/asyncio/clients/py.typed
--rw-r--r--   0        0        0     3341 2021-12-07 22:32:02.034730 xrpl-py-2.0.0b0/xrpl/asyncio/clients/utils.py
--rw-r--r--   0        0        0     7431 2022-12-15 20:10:31.058266 xrpl-py-2.0.0b0/xrpl/asyncio/clients/websocket_base.py
--rw-r--r--   0        0        0      328 2021-07-28 20:35:08.802964 xrpl-py-2.0.0b0/xrpl/asyncio/ledger/__init__.py
--rw-r--r--   0        0        0     3443 2022-12-15 20:10:31.059029 xrpl-py-2.0.0b0/xrpl/asyncio/ledger/main.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.923951 xrpl-py-2.0.0b0/xrpl/asyncio/ledger/py.typed
--rw-r--r--   0        0        0     2353 2022-04-26 22:13:55.274282 xrpl-py-2.0.0b0/xrpl/asyncio/ledger/utils.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924038 xrpl-py-2.0.0b0/xrpl/asyncio/py.typed
--rw-r--r--   0        0        0      956 2022-12-15 20:10:31.059741 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/__init__.py
--rw-r--r--   0        0        0     2077 2022-12-15 20:10:31.060567 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/ledger.py
--rw-r--r--   0        0        0    12247 2022-12-15 20:10:31.061290 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/main.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924123 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/py.typed
--rw-r--r--   0        0        0     3606 2022-12-15 20:10:31.062028 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/reliable_submission.py
--rw-r--r--   0        0        0      219 2021-07-28 20:35:08.805165 xrpl-py-2.0.0b0/xrpl/asyncio/wallet/__init__.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924197 xrpl-py-2.0.0b0/xrpl/asyncio/wallet/py.typed
--rw-r--r--   0        0        0     5657 2022-12-15 20:10:31.062888 xrpl-py-2.0.0b0/xrpl/asyncio/wallet/wallet_generation.py
--rw-r--r--   0        0        0      656 2021-07-28 20:35:08.805912 xrpl-py-2.0.0b0/xrpl/clients/__init__.py
--rw-r--r--   0        0        0      295 2021-07-28 20:35:08.806161 xrpl-py-2.0.0b0/xrpl/clients/json_rpc_client.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924276 xrpl-py-2.0.0b0/xrpl/clients/py.typed
--rw-r--r--   0        0        0      705 2022-12-15 20:10:31.064928 xrpl-py-2.0.0b0/xrpl/clients/sync_client.py
--rw-r--r--   0        0        0     8780 2022-12-15 20:10:31.065768 xrpl-py-2.0.0b0/xrpl/clients/websocket_client.py
--rw-r--r--   0        0        0     1414 2022-07-28 00:01:58.132202 xrpl-py-2.0.0b0/xrpl/constants.py
--rw-r--r--   0        0        0      171 2021-07-28 20:35:08.807482 xrpl-py-2.0.0b0/xrpl/core/__init__.py
--rw-r--r--   0        0        0     1131 2022-12-15 20:10:31.067161 xrpl-py-2.0.0b0/xrpl/core/addresscodec/__init__.py
--rw-r--r--   0        0        0     7175 2022-08-23 17:19:34.990879 xrpl-py-2.0.0b0/xrpl/core/addresscodec/codec.py
--rw-r--r--   0        0        0      194 2021-07-28 20:35:08.808480 xrpl-py-2.0.0b0/xrpl/core/addresscodec/exceptions.py
--rw-r--r--   0        0        0     5735 2022-12-15 20:10:31.067991 xrpl-py-2.0.0b0/xrpl/core/addresscodec/main.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924387 xrpl-py-2.0.0b0/xrpl/core/addresscodec/py.typed
--rw-r--r--   0        0        0      235 2021-07-28 20:35:08.808987 xrpl-py-2.0.0b0/xrpl/core/addresscodec/utils.py
--rw-r--r--   0        0        0      488 2021-07-28 20:35:08.809400 xrpl-py-2.0.0b0/xrpl/core/binarycodec/__init__.py
--rw-r--r--   0        0        0      296 2021-07-28 20:35:08.809791 xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/__init__.py
--rw-r--r--   0        0        0     9076 2021-07-28 20:35:08.810078 xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py
--rw-r--r--   0        0        0     4650 2021-12-07 22:32:02.051210 xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py
--rw-r--r--   0        0        0     1025 2021-07-28 20:35:08.810736 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/__init__.py
--rw-r--r--   0        0        0    44971 2022-08-23 17:19:34.991511 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/definitions.json
--rw-r--r--   0        0        0     8431 2021-07-28 20:35:08.811725 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/definitions.py
--rw-r--r--   0        0        0     1870 2021-07-28 20:35:08.812068 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_header.py
--rw-r--r--   0        0        0     1192 2021-07-28 20:35:08.812380 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_info.py
--rw-r--r--   0        0        0     1931 2022-07-05 22:56:20.051355 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_instance.py
--rw-r--r--   0        0        0      191 2021-07-28 20:35:08.813180 xrpl-py-2.0.0b0/xrpl/core/binarycodec/exceptions.py
--rw-r--r--   0        0        0     3942 2021-07-28 20:35:08.813524 xrpl-py-2.0.0b0/xrpl/core/binarycodec/field_id_codec.py
--rw-r--r--   0        0        0     3708 2022-07-05 22:56:20.052317 xrpl-py-2.0.0b0/xrpl/core/binarycodec/main.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924565 xrpl-py-2.0.0b0/xrpl/core/binarycodec/py.typed
--rw-r--r--   0        0        0     1255 2022-07-05 22:56:20.053538 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/__init__.py
--rw-r--r--   0        0        0     2956 2022-01-20 00:05:30.497701 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/account_id.py
--rw-r--r--   0        0        0    11234 2021-12-17 23:17:45.558659 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/amount.py
--rw-r--r--   0        0        0     1950 2021-07-28 20:35:08.815354 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/blob.py
--rw-r--r--   0        0        0     4347 2021-12-07 22:32:02.058589 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/currency.py
--rw-r--r--   0        0        0     2640 2021-12-07 22:32:02.059722 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash.py
--rw-r--r--   0        0        0      572 2021-07-28 20:35:08.816233 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash128.py
--rw-r--r--   0        0        0      571 2021-07-28 20:35:08.816481 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash160.py
--rw-r--r--   0        0        0      572 2021-07-28 20:35:08.816714 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash256.py
--rw-r--r--   0        0        0     9067 2021-07-28 20:35:08.817068 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/path_set.py
--rw-r--r--   0        0        0     2493 2022-07-05 22:56:20.055452 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/serialized_type.py
--rw-r--r--   0        0        0     3301 2022-07-05 22:56:20.055743 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/st_array.py
--rw-r--r--   0        0        0     8394 2022-07-05 22:56:20.056024 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/st_object.py
--rw-r--r--   0        0        0     3383 2021-07-28 20:35:08.818405 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint.py
--rw-r--r--   0        0        0     2063 2021-07-28 20:35:08.818693 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint16.py
--rw-r--r--   0        0        0     2283 2021-07-28 20:35:08.819029 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint32.py
--rw-r--r--   0        0        0     2854 2022-01-20 00:05:30.500382 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint64.py
--rw-r--r--   0        0        0     1994 2021-07-28 20:35:08.819489 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint8.py
--rw-r--r--   0        0        0     2905 2021-07-28 20:35:08.819794 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/vector256.py
--rw-r--r--   0        0        0      447 2022-12-15 20:10:31.069734 xrpl-py-2.0.0b0/xrpl/core/keypairs/__init__.py
--rw-r--r--   0        0        0     1275 2021-07-28 20:35:08.820427 xrpl-py-2.0.0b0/xrpl/core/keypairs/crypto_implementation.py
--rw-r--r--   0        0        0     3662 2022-12-15 20:10:31.070556 xrpl-py-2.0.0b0/xrpl/core/keypairs/ed25519.py
--rw-r--r--   0        0        0      182 2021-07-28 20:35:08.820941 xrpl-py-2.0.0b0/xrpl/core/keypairs/exceptions.py
--rw-r--r--   0        0        0      893 2022-12-15 20:10:31.071456 xrpl-py-2.0.0b0/xrpl/core/keypairs/helpers.py
--rw-r--r--   0        0        0     4788 2022-12-15 20:10:31.072827 xrpl-py-2.0.0b0/xrpl/core/keypairs/main.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924715 xrpl-py-2.0.0b0/xrpl/core/keypairs/py.typed
--rw-r--r--   0        0        0     7480 2022-07-28 00:01:58.132708 xrpl-py-2.0.0b0/xrpl/core/keypairs/secp256k1.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924787 xrpl-py-2.0.0b0/xrpl/core/py.typed
--rw-r--r--   0        0        0      314 2021-07-28 20:35:08.822692 xrpl-py-2.0.0b0/xrpl/ledger/__init__.py
--rw-r--r--   0        0        0     2283 2022-04-26 22:13:55.277744 xrpl-py-2.0.0b0/xrpl/ledger/main.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924863 xrpl-py-2.0.0b0/xrpl/ledger/py.typed
--rw-r--r--   0        0        0      858 2021-12-17 21:23:35.552124 xrpl-py-2.0.0b0/xrpl/models/__init__.py
--rw-r--r--   0        0        0      497 2021-12-17 23:17:45.561082 xrpl-py-2.0.0b0/xrpl/models/amounts/__init__.py
--rw-r--r--   0        0        0     1377 2021-12-17 23:17:45.561971 xrpl-py-2.0.0b0/xrpl/models/amounts/amount.py
--rw-r--r--   0        0        0     1349 2021-12-17 21:23:35.554848 xrpl-py-2.0.0b0/xrpl/models/amounts/issued_currency_amount.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924950 xrpl-py-2.0.0b0/xrpl/models/amounts/py.typed
--rw-r--r--   0        0        0    10663 2022-07-05 22:56:20.059672 xrpl-py-2.0.0b0/xrpl/models/base_model.py
--rw-r--r--   0        0        0      371 2021-07-28 20:35:08.825266 xrpl-py-2.0.0b0/xrpl/models/currencies/__init__.py
--rw-r--r--   0        0        0      319 2021-07-28 20:35:08.825634 xrpl-py-2.0.0b0/xrpl/models/currencies/currency.py
--rw-r--r--   0        0        0     2237 2021-12-17 21:23:35.557608 xrpl-py-2.0.0b0/xrpl/models/currencies/issued_currency.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925039 xrpl-py-2.0.0b0/xrpl/models/currencies/py.typed
--rw-r--r--   0        0        0     2500 2021-12-17 21:23:35.558615 xrpl-py-2.0.0b0/xrpl/models/currencies/xrp.py
--rw-r--r--   0        0        0      171 2021-07-28 20:35:08.826501 xrpl-py-2.0.0b0/xrpl/models/exceptions.py
--rw-r--r--   0        0        0     4300 2022-04-25 18:39:06.767427 xrpl-py-2.0.0b0/xrpl/models/flags.py
--rw-r--r--   0        0        0     2462 2022-12-15 20:10:31.074348 xrpl-py-2.0.0b0/xrpl/models/nested_model.py
--rw-r--r--   0        0        0     2088 2021-07-28 20:35:08.826856 xrpl-py-2.0.0b0/xrpl/models/path.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925126 xrpl-py-2.0.0b0/xrpl/models/py.typed
--rw-r--r--   0        0        0     3428 2022-06-02 20:58:35.644160 xrpl-py-2.0.0b0/xrpl/models/requests/__init__.py
--rw-r--r--   0        0        0     1599 2021-07-28 20:35:08.828304 xrpl-py-2.0.0b0/xrpl/models/requests/account_channels.py
--rw-r--r--   0        0        0     1213 2021-07-28 20:35:08.828881 xrpl-py-2.0.0b0/xrpl/models/requests/account_currencies.py
--rw-r--r--   0        0        0     1166 2021-07-28 20:35:08.829260 xrpl-py-2.0.0b0/xrpl/models/requests/account_info.py
--rw-r--r--   0        0        0     1373 2021-07-28 20:35:08.829871 xrpl-py-2.0.0b0/xrpl/models/requests/account_lines.py
--rw-r--r--   0        0        0     1170 2021-12-17 23:17:45.563593 xrpl-py-2.0.0b0/xrpl/models/requests/account_nfts.py
--rw-r--r--   0        0        0     1760 2021-07-28 20:35:08.830168 xrpl-py-2.0.0b0/xrpl/models/requests/account_objects.py
--rw-r--r--   0        0        0     1211 2021-07-28 20:35:08.830415 xrpl-py-2.0.0b0/xrpl/models/requests/account_offers.py
--rw-r--r--   0        0        0     1257 2021-07-28 20:35:08.830671 xrpl-py-2.0.0b0/xrpl/models/requests/account_tx.py
--rw-r--r--   0        0        0     1074 2021-07-28 20:35:08.830942 xrpl-py-2.0.0b0/xrpl/models/requests/book_offers.py
--rw-r--r--   0        0        0     3020 2021-07-28 20:35:08.831227 xrpl-py-2.0.0b0/xrpl/models/requests/channel_authorize.py
--rw-r--r--   0        0        0     1130 2021-07-28 20:35:08.831559 xrpl-py-2.0.0b0/xrpl/models/requests/channel_verify.py
--rw-r--r--   0        0        0     1204 2021-07-28 20:35:08.831844 xrpl-py-2.0.0b0/xrpl/models/requests/deposit_authorized.py
--rw-r--r--   0        0        0      625 2022-04-05 18:02:24.759920 xrpl-py-2.0.0b0/xrpl/models/requests/federator_info.py
--rw-r--r--   0        0        0      775 2021-07-28 20:35:08.832085 xrpl-py-2.0.0b0/xrpl/models/requests/fee.py
--rw-r--r--   0        0        0     1119 2021-07-28 20:35:08.832292 xrpl-py-2.0.0b0/xrpl/models/requests/gateway_balances.py
--rw-r--r--   0        0        0     3068 2022-06-02 20:58:35.644917 xrpl-py-2.0.0b0/xrpl/models/requests/generic_request.py
--rw-r--r--   0        0        0      832 2021-07-28 20:35:08.832476 xrpl-py-2.0.0b0/xrpl/models/requests/ledger.py
--rw-r--r--   0        0        0      944 2021-07-28 20:35:08.832645 xrpl-py-2.0.0b0/xrpl/models/requests/ledger_closed.py
--rw-r--r--   0        0        0      726 2021-07-28 20:35:08.832891 xrpl-py-2.0.0b0/xrpl/models/requests/ledger_current.py
--rw-r--r--   0        0        0     1135 2021-07-28 20:35:08.833259 xrpl-py-2.0.0b0/xrpl/models/requests/ledger_data.py
--rw-r--r--   0        0        0     4643 2021-07-28 20:35:08.833563 xrpl-py-2.0.0b0/xrpl/models/requests/ledger_entry.py
--rw-r--r--   0        0        0      853 2021-07-28 20:35:08.833795 xrpl-py-2.0.0b0/xrpl/models/requests/manifest.py
--rw-r--r--   0        0        0      763 2022-04-25 18:39:06.768162 xrpl-py-2.0.0b0/xrpl/models/requests/nft_buy_offers.py
--rw-r--r--   0        0        0      770 2022-04-25 18:39:06.768739 xrpl-py-2.0.0b0/xrpl/models/requests/nft_sell_offers.py
--rw-r--r--   0        0        0     1496 2021-07-28 20:35:08.834038 xrpl-py-2.0.0b0/xrpl/models/requests/no_ripple_check.py
--rw-r--r--   0        0        0     4347 2021-07-28 20:35:08.834320 xrpl-py-2.0.0b0/xrpl/models/requests/path_find.py
--rw-r--r--   0        0        0      547 2021-07-28 20:35:08.834534 xrpl-py-2.0.0b0/xrpl/models/requests/ping.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925225 xrpl-py-2.0.0b0/xrpl/models/requests/py.typed
--rw-r--r--   0        0        0      579 2021-07-28 20:35:08.834709 xrpl-py-2.0.0b0/xrpl/models/requests/random.py
--rw-r--r--   0        0        0     5646 2022-07-05 22:56:20.061515 xrpl-py-2.0.0b0/xrpl/models/requests/request.py
--rw-r--r--   0        0        0     2330 2021-07-28 20:35:08.835181 xrpl-py-2.0.0b0/xrpl/models/requests/ripple_path_find.py
--rw-r--r--   0        0        0      618 2021-07-28 20:35:08.835452 xrpl-py-2.0.0b0/xrpl/models/requests/server_info.py
--rw-r--r--   0        0        0     1194 2021-07-28 20:35:08.835707 xrpl-py-2.0.0b0/xrpl/models/requests/server_state.py
--rw-r--r--   0        0        0     4034 2022-07-05 22:56:20.063692 xrpl-py-2.0.0b0/xrpl/models/requests/sign.py
--rw-r--r--   0        0        0     5062 2022-07-05 22:56:20.065263 xrpl-py-2.0.0b0/xrpl/models/requests/sign_and_submit.py
--rw-r--r--   0        0        0     3274 2022-07-05 22:56:20.066563 xrpl-py-2.0.0b0/xrpl/models/requests/sign_for.py
--rw-r--r--   0        0        0     3758 2022-07-05 22:56:20.068102 xrpl-py-2.0.0b0/xrpl/models/requests/submit.py
--rw-r--r--   0        0        0     2478 2022-07-05 22:56:20.069204 xrpl-py-2.0.0b0/xrpl/models/requests/submit_multisigned.py
--rw-r--r--   0        0        0     2842 2021-07-28 20:35:08.836916 xrpl-py-2.0.0b0/xrpl/models/requests/submit_only.py
--rw-r--r--   0        0        0     2103 2021-07-28 20:35:08.837120 xrpl-py-2.0.0b0/xrpl/models/requests/subscribe.py
--rw-r--r--   0        0        0     1278 2021-07-28 20:35:08.837698 xrpl-py-2.0.0b0/xrpl/models/requests/transaction_entry.py
--rw-r--r--   0        0        0      817 2021-07-28 20:35:08.838021 xrpl-py-2.0.0b0/xrpl/models/requests/tx.py
--rw-r--r--   0        0        0     1595 2021-07-28 20:35:08.838365 xrpl-py-2.0.0b0/xrpl/models/requests/unsubscribe.py
--rw-r--r--   0        0        0      251 2021-07-28 20:35:08.838692 xrpl-py-2.0.0b0/xrpl/models/required.py
--rw-r--r--   0        0        0     3617 2021-12-07 22:32:02.066250 xrpl-py-2.0.0b0/xrpl/models/response.py
--rw-r--r--   0        0        0     3293 2022-06-02 20:58:35.645480 xrpl-py-2.0.0b0/xrpl/models/transactions/__init__.py
--rw-r--r--   0        0        0     1333 2021-07-28 20:35:08.839736 xrpl-py-2.0.0b0/xrpl/models/transactions/account_delete.py
--rw-r--r--   0        0        0     8629 2022-04-25 18:40:11.716081 xrpl-py-2.0.0b0/xrpl/models/transactions/account_set.py
--rw-r--r--   0        0        0     1101 2021-07-28 20:35:08.840429 xrpl-py-2.0.0b0/xrpl/models/transactions/check_cancel.py
--rw-r--r--   0        0        0     1993 2021-07-28 20:35:08.840706 xrpl-py-2.0.0b0/xrpl/models/transactions/check_cash.py
--rw-r--r--   0        0        0     1934 2021-07-28 20:35:08.841015 xrpl-py-2.0.0b0/xrpl/models/transactions/check_create.py
--rw-r--r--   0        0        0     1598 2021-07-28 20:35:08.841280 xrpl-py-2.0.0b0/xrpl/models/transactions/deposit_preauth.py
--rw-r--r--   0        0        0     1069 2021-07-28 20:35:08.841539 xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_cancel.py
--rw-r--r--   0        0        0     2617 2021-07-28 20:35:08.841747 xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_create.py
--rw-r--r--   0        0        0     2114 2021-07-28 20:35:08.841923 xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_finish.py
--rw-r--r--   0        0        0     1923 2022-12-15 20:10:31.075374 xrpl-py-2.0.0b0/xrpl/models/transactions/metadata.py
--rw-r--r--   0        0        0     4537 2022-04-25 18:39:06.770393 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_accept_offer.py
--rw-r--r--   0        0        0     1769 2022-04-25 18:39:06.771370 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_burn.py
--rw-r--r--   0        0        0     2015 2022-04-25 18:39:06.771874 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_cancel_offer.py
--rw-r--r--   0        0        0     4324 2022-04-25 18:40:20.537837 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_create_offer.py
--rw-r--r--   0        0        0     4762 2022-04-25 18:40:11.718521 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_mint.py
--rw-r--r--   0        0        0     1045 2021-07-28 20:35:08.842102 xrpl-py-2.0.0b0/xrpl/models/transactions/offer_cancel.py
--rw-r--r--   0        0        0     3866 2022-04-25 18:40:11.719936 xrpl-py-2.0.0b0/xrpl/models/transactions/offer_create.py
--rw-r--r--   0        0        0     5861 2022-04-25 18:40:11.721475 xrpl-py-2.0.0b0/xrpl/models/transactions/payment.py
--rw-r--r--   0        0        0     3917 2022-04-25 18:40:11.722725 xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_claim.py
--rw-r--r--   0        0        0     2367 2021-07-28 20:35:08.843065 xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_create.py
--rw-r--r--   0        0        0     1614 2021-07-28 20:35:08.843590 xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_fund.py
--rw-r--r--   0        0        0      575 2022-04-05 18:02:24.769631 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py
--rw-r--r--   0        0        0     3651 2022-04-05 18:02:24.770653 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py
--rw-r--r--   0        0        0     1366 2021-07-28 20:35:08.845018 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py
--rw-r--r--   0        0        0     1874 2021-07-28 20:35:08.845329 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py
--rw-r--r--   0        0        0     2262 2021-07-28 20:35:08.845606 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925358 xrpl-py-2.0.0b0/xrpl/models/transactions/py.typed
--rw-r--r--   0        0        0      959 2021-07-28 20:35:08.845886 xrpl-py-2.0.0b0/xrpl/models/transactions/set_regular_key.py
--rw-r--r--   0        0        0     4747 2022-09-15 21:17:23.562048 xrpl-py-2.0.0b0/xrpl/models/transactions/signer_list_set.py
--rw-r--r--   0        0        0      959 2021-12-07 22:32:02.070889 xrpl-py-2.0.0b0/xrpl/models/transactions/ticket_create.py
--rw-r--r--   0        0        0    14500 2022-09-15 21:17:23.562911 xrpl-py-2.0.0b0/xrpl/models/transactions/transaction.py
--rw-r--r--   0        0        0     2425 2022-04-25 18:40:11.724215 xrpl-py-2.0.0b0/xrpl/models/transactions/trust_set.py
--rw-r--r--   0        0        0      275 2021-07-28 20:35:08.847122 xrpl-py-2.0.0b0/xrpl/models/transactions/types/__init__.py
--rw-r--r--   0        0        0      287 2021-07-28 20:35:08.847388 xrpl-py-2.0.0b0/xrpl/models/transactions/types/pseudo_transaction_type.py
--rw-r--r--   0        0        0     1069 2021-12-17 23:17:45.570774 xrpl-py-2.0.0b0/xrpl/models/transactions/types/transaction_type.py
--rw-r--r--   0        0        0      749 2021-12-17 23:17:45.571050 xrpl-py-2.0.0b0/xrpl/models/types.py
--rw-r--r--   0        0        0     2174 2021-12-17 21:23:35.561520 xrpl-py-2.0.0b0/xrpl/models/utils.py
--rw-r--r--   0        0        0        0 2021-12-07 22:32:02.074339 xrpl-py-2.0.0b0/xrpl/py.typed
--rw-r--r--   0        0        0      958 2022-12-15 20:10:31.076208 xrpl-py-2.0.0b0/xrpl/transaction/__init__.py
--rw-r--r--   0        0        0     1951 2022-12-15 20:10:31.079134 xrpl-py-2.0.0b0/xrpl/transaction/ledger.py
--rw-r--r--   0        0        0     3896 2022-12-15 20:10:31.080226 xrpl-py-2.0.0b0/xrpl/transaction/main.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925547 xrpl-py-2.0.0b0/xrpl/transaction/py.typed
--rw-r--r--   0        0        0     1163 2021-12-07 22:32:02.077113 xrpl-py-2.0.0b0/xrpl/transaction/reliable_submission.py
--rw-r--r--   0        0        0      933 2022-08-23 17:19:34.993522 xrpl-py-2.0.0b0/xrpl/utils/__init__.py
--rw-r--r--   0        0        0     3412 2022-04-25 18:39:06.775209 xrpl-py-2.0.0b0/xrpl/utils/parse_nftoken_id.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925715 xrpl-py-2.0.0b0/xrpl/utils/py.typed
--rw-r--r--   0        0        0     1537 2022-07-05 22:56:20.074990 xrpl-py-2.0.0b0/xrpl/utils/sidechain.py
--rw-r--r--   0        0        0      788 2021-12-17 21:23:35.563169 xrpl-py-2.0.0b0/xrpl/utils/str_conversions.py
--rw-r--r--   0        0        0     4202 2022-07-28 00:01:58.134040 xrpl-py-2.0.0b0/xrpl/utils/time_conversions.py
--rw-r--r--   0        0        0      350 2022-08-23 17:19:34.994080 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/__init__.py
--rw-r--r--   0        0        0     1717 2022-07-05 22:56:20.082815 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_balance_changes.py
--rw-r--r--   0        0        0     1446 2022-07-05 22:56:20.083098 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_final_balances.py
--rw-r--r--   0        0        0      641 2022-08-23 17:19:34.994400 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_order_book_changes.py
--rw-r--r--   0        0        0      627 2022-08-23 17:19:34.995150 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/__init__.py
--rw-r--r--   0        0        0     5218 2022-08-23 17:19:34.995970 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/balance_parser.py
--rw-r--r--   0        0        0     2518 2022-12-15 20:10:31.082062 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/nodes.py
--rw-r--r--   0        0        0     6191 2022-08-23 17:19:34.996288 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py
--rw-r--r--   0        0        0     1192 2022-08-23 17:19:34.996460 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/parser.py
--rw-r--r--   0        0        0     1404 2022-12-15 20:10:31.082853 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/types.py
--rw-r--r--   0        0        0     3476 2022-07-28 00:01:58.134766 xrpl-py-2.0.0b0/xrpl/utils/xrp_conversions.py
--rw-r--r--   0        0        0      269 2021-07-28 20:35:08.852350 xrpl-py-2.0.0b0/xrpl/wallet/__init__.py
--rw-r--r--   0        0        0     8321 2022-12-15 20:10:31.083718 xrpl-py-2.0.0b0/xrpl/wallet/main.py
--rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925867 xrpl-py-2.0.0b0/xrpl/wallet/py.typed
--rw-r--r--   0        0        0     1370 2022-04-05 18:02:24.775775 xrpl-py-2.0.0b0/xrpl/wallet/wallet_generation.py
--rw-r--r--   0        0        0    18248 2022-12-15 20:19:48.363167 xrpl-py-2.0.0b0/setup.py
--rw-r--r--   0        0        0    17208 2022-12-15 20:19:48.364332 xrpl-py-2.0.0b0/PKG-INFO
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

### Comparing `xrpl-py-2.0.0b0/LICENSE` & `xrpl_py-2.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/README.md` & `xrpl_py-2.1.0b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 # create a wallet on the testnet
 from xrpl.wallet import generate_faucet_wallet
 test_wallet = generate_faucet_wallet(client)
 print(test_wallet)
 public_key: ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56
 private_key: -HIDDEN-
-classic_address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo
+address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo
 
 # look up account info
-from xrpl.models.requests.account_info import AccountInfo
+from xrpl.models import AccountInfo
 acct_info = AccountInfo(
     account="rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",
     ledger_index="current",
     queue=True,
     strict=True,
 )
 response = client.request(acct_info)
@@ -99,26 +99,26 @@
 #### `xrpl.wallet`
 
 Use the [`xrpl.wallet`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.wallet.html) module to create a wallet from a given seed or or via a [Testnet faucet](https://xrpl.org/xrp-testnet-faucet.html).
 
 To create a wallet from a seed (in this case, the value generated using [`xrpl.keypairs`](#xrpl-keypairs)):
 
 ```py
-wallet_from_seed = xrpl.wallet.Wallet(seed, 0)
+wallet_from_seed = xrpl.wallet.Wallet.from_seed(seed)
 print(wallet_from_seed)
 # pub_key: ED46949E414A3D6D758D347BAEC9340DC78F7397FEE893132AAF5D56E4D7DE77B0
 # priv_key: -HIDDEN-
-# classic_address: rG5ZvYsK5BPi9f1Nb8mhFGDTNMJhEhufn6
+# address: rG5ZvYsK5BPi9f1Nb8mhFGDTNMJhEhufn6
 ```
 
 To create a wallet from a Testnet faucet:
 
 ```py
 test_wallet = generate_faucet_wallet(client)
-test_account = test_wallet.classic_address
+test_account = test_wallet.address
 print("Classic address:", test_account)
 # Classic address: rEQB2hhp3rg7sHj6L8YyR4GG47Cb7pfcuw
 ```
 
 #### `xrpl.core.keypairs`
 
 Use the [`xrpl.core.keypairs`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html#module-xrpl.core.keypairs) module to generate seeds and derive keypairs and addresses from those seed values.
@@ -153,41 +153,41 @@
 
 Use the [`xrpl.transaction`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html) module to sign and submit transactions. The module offers three ways to do this:
 
 * [`sign_and_submit`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign_and_submit) — Signs a transaction locally, then submits it to the XRP Ledger. This method does not implement [reliable transaction submission](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission) best practices, so only use it for development or testing purposes.
 
 * [`sign`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign) — Signs a transaction locally. This method **does  not** submit the transaction to the XRP Ledger.
 
-* [`send_reliable_submission`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.send_reliable_submission) — An implementation of the [reliable transaction submission guidelines](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission), this method submits a signed transaction to the XRP Ledger and then verifies that it has been included in a validated ledger (or has failed to do so). Use this method to submit transactions for production purposes.
+* [`submit_and_wait`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.submit_and_wait) — An implementation of the [reliable transaction submission guidelines](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission), this method submits a signed transaction to the XRP Ledger and then verifies that it has been included in a validated ledger (or has failed to do so). Use this method to submit transactions for production purposes.
 
 
 ```py
 from xrpl.models.transactions import Payment
-from xrpl.transaction import sign, send_reliable_submission
+from xrpl.transaction import sign, submit_and_wait
 from xrpl.ledger import get_latest_validated_ledger_sequence
 from xrpl.account import get_next_valid_seq_number
 
 current_validated_ledger = get_latest_validated_ledger_sequence(client)
 
 # prepare the transaction
 # the amount is expressed in drops, not XRP
 # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
 my_tx_payment = Payment(
-    account=test_wallet.classic_address,
+    account=test_wallet.address,
     amount="2200000",
     destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",
     last_ledger_sequence=current_validated_ledger + 20,
-    sequence=get_next_valid_seq_number(test_wallet.classic_address, client),
+    sequence=get_next_valid_seq_number(test_wallet.address, client),
     fee="10",
 )
 # sign the transaction
 my_tx_payment_signed = sign(my_tx_payment,test_wallet)
 
 # submit the transaction
-tx_response = send_reliable_submission(my_tx_payment_signed, client)
+tx_response = submit_and_wait(my_tx_payment_signed, client)
 ```
 
 #### Get fee from the XRP Ledger
 
 
 In most cases, you can specify the minimum [transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) of `"10"` for the `fee` field unless you have a strong reason not to. But if you want to get the [current load-balanced transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) from the network, you can use the `get_fee` function:
 
@@ -200,27 +200,27 @@
 
 #### Auto-filled fields
 
 The `xrpl-py` library automatically populates the `fee`, `sequence` and `last_ledger_sequence` fields when you create transactions. In the example above, you could omit those fields and let the library fill them in for you.
 
 ```py
 from xrpl.models.transactions import Payment
-from xrpl.transaction import send_reliable_submission, autofill_and_sign
+from xrpl.transaction import submit_and_wait, autofill_and_sign
 # prepare the transaction
 # the amount is expressed in drops, not XRP
 # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
 my_tx_payment = Payment(
-    account=test_wallet.classic_address,
+    account=test_wallet.address,
     amount="2200000",
     destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe"
 )
 
 # sign the transaction with the autofill method
 # (this will auto-populate the fee, sequence, and last_ledger_sequence)
-my_tx_payment_signed = autofill_and_sign(my_tx_payment, test_wallet, client)
+my_tx_payment_signed = autofill_and_sign(my_tx_payment, client, test_wallet)
 print(my_tx_payment_signed)
 # Payment(
 #     account='rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz',
 #     transaction_type=<TransactionType.PAYMENT: 'Payment'>,
 #     fee='10',
 #     sequence=16034065,
 #     account_txn_id=None,
@@ -237,26 +237,26 @@
 #     invoice_id=None,
 #     paths=None,
 #     send_max=None,
 #     deliver_min=None
 # )
 
 # submit the transaction
-tx_response = send_reliable_submission(my_tx_payment_signed, client)
+tx_response = submit_and_wait(my_tx_payment_signed, client)
 ```
 
 
 ### Subscribe to ledger updates
 
 You can send `subscribe` and `unsubscribe` requests only using the WebSocket network client. These request methods allow you to be alerted of certain situations as they occur, such as when a new ledger is declared.
 
 ```py
 from xrpl.clients import WebsocketClient
 url = "wss://s.altnet.rippletest.net/"
-from xrpl.models.requests import Subscribe, StreamParameter
+from xrpl.models import Subscribe, StreamParameter
 req = Subscribe(streams=[StreamParameter.LEDGER])
 # NOTE: this code will run forever without a timeout, until the process is killed
 with WebsocketClient(url) as client:
     client.send(req)
     for message in client:
         print(message)
 # {'result': {'fee_base': 10, 'fee_ref': 10, 'ledger_hash': '7CD50477F23FF158B430772D8E82A961376A7B40E13C695AA849811EDF66C5C0', 'ledger_index': 18183504, 'ledger_time': 676412962, 'reserve_base': 20000000, 'reserve_inc': 5000000, 'validated_ledgers': '17469391-18183504'}, 'status': 'success', 'type': 'response'}
@@ -271,40 +271,37 @@
 This library supports Python's [`asyncio`](https://docs.python.org/3/library/asyncio.html) package, which is used to run asynchronous code. All the async code is in [`xrpl.asyncio`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.asyncio.html) If you are writing asynchronous code, please note that you will not be able to use any synchronous sugar functions, due to how event loops are handled. However, every synchronous method has a corresponding asynchronous method that you can use.
 
 This sample code is the asynchronous equivalent of the above section on submitting a transaction.
 
 ```py
 import asyncio
 from xrpl.models.transactions import Payment
-from xrpl.asyncio.transaction import sign, send_reliable_submission
+from xrpl.asyncio.transaction import sign, submit_and_wait
 from xrpl.asyncio.ledger import get_latest_validated_ledger_sequence
 from xrpl.asyncio.account import get_next_valid_seq_number
 from xrpl.asyncio.clients import AsyncJsonRpcClient
 
 async_client = AsyncJsonRpcClient(JSON_RPC_URL)
 
 async def submit_sample_transaction():
     current_validated_ledger = await get_latest_validated_ledger_sequence(async_client)
 
     # prepare the transaction
     # the amount is expressed in drops, not XRP
     # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
     my_tx_payment = Payment(
-        account=test_wallet.classic_address,
+        account=test_wallet.address,
         amount="2200000",
         destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",
         last_ledger_sequence=current_validated_ledger + 20,
-        sequence=await get_next_valid_seq_number(test_wallet.classic_address, async_client),
+        sequence=await get_next_valid_seq_number(test_wallet.address, async_client),
         fee="10",
     )
-    # sign the transaction
-    my_tx_payment_signed = await sign(my_tx_payment,test_wallet)
-
-    # submit the transaction
-    tx_response = await send_reliable_submission(my_tx_payment_signed, async_client)
+    # sign and submit the transaction
+    tx_response = await submit_and_wait(my_tx_payment_signed, async_client, test_wallet)
 
 asyncio.run(submit_sample_transaction())
 ```
 
 ### Encode addresses
 
 Use [`xrpl.core.addresscodec`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.addresscodec.html) to encode and decode addresses into and from the ["classic" and X-address formats](https://xrpl.org/accounts.html#addresses).
@@ -326,22 +323,26 @@
 
 ## Contributing
 
 If you want to contribute to this project, see [CONTRIBUTING.md].
 
 ### Mailing Lists
 
-We have a low-traffic mailing list for announcements of new `xrpl.js` releases. (About 1 email per week)
+We have a low-traffic mailing list for announcements of new `xrpl-py` releases. (About 1 email per week)
 
 + [Subscribe to xrpl-announce](https://groups.google.com/g/xrpl-announce)
 
 If you're using the XRP Ledger in production, you should run a [rippled server](https://github.com/ripple/rippled) and subscribe to the ripple-server mailing list as well.
 
 + [Subscribe to ripple-server](https://groups.google.com/g/ripple-server)
 
+### Code Samples
+- For samples of common use cases, see the [XRPL.org Code Samples](https://xrpl.org/code-samples.html) page.
+- You can also browse those samples [directly on GitHub](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples).
+
 ### Report an issue
 
 Experienced an issue? Report it [here](https://github.com/XRPLF/xrpl-py/issues/new).
 
 ## License
 
 The `xrpl-py` library is licensed under the ISC License. See [LICENSE] for more information.
```

### Comparing `xrpl-py-2.0.0b0/pyproject.toml` & `xrpl_py-2.1.0b0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xrpl-py"
-version = "2.0.0-beta.0"
+version = "2.1.0b0"
 description = "A complete Python library for interacting with the XRP ledger"
 readme = "README.md"
 repository = "https://github.com/XRPLF/xrpl-py"
 authors = [
   "Mayukha Vadari <mvadari@ripple.com>",
   "Greg Weisbrod <gweisbrod@ripple.com>",
   "Amie Corso <acorso@ripple.com>",
@@ -30,41 +30,41 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 base58 = "^2.1.0"
 ECPy = "^1.2.5"
 typing-extensions = "^4.2.0"
-httpx = ">=0.18.1,<0.24.0"
+httpx = ">=0.18.1,<0.25.0"
 websockets = [
     {version = ">=9.0.1 <11.0", python = ">= 3.7, < 3.10"},
     {version = "^10.0", python = "^3.10"}
 ]
 Deprecated = "^1.2.13"
 types-Deprecated = "^1.2.9"
 pycryptodome = "^3.16.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^3.8.4"
-black = "22.10.0"
-flake8-black = "^0.3.3"
-flake8-docstrings = "^1.5.0"
-mypy = "^0"
-isort = "^5.7.0"
-flake8-isort = "^5.0.0"
+black = "23.3.0"
+flake8-black = "^0.3.6"
+flake8-docstrings = "^1.7.0"
+mypy = "^1"
+isort = "^5.11.5"
+flake8-isort = "^6.0.0"
 flake8-annotations = "2.7.0"
 flake8-absolute-import = "^1.0"
 darglint = "^1.5.8"
-sphinx-rtd-theme = "^0.5.1"
+sphinx-rtd-theme = "^1.2.2"
 aiounittest = "^1.4.0"
-coverage = "^6.5.0"
+coverage = "^7.2.7"
 Jinja2 = "^3.1.2"
-MarkupSafe = "2.1.1"
+MarkupSafe = "2.1.3"
 Sphinx = "^5.3.0"
-poethepoet = "^0.16.5"
+poethepoet = "^0.19.0"
 
 [tool.isort]
 # Make sure that isort's settings line up with black
 profile = "black"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `xrpl-py-2.0.0b0/xrpl/account/main.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/account/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """High-level methods to obtain information about accounts."""
 
-import asyncio
-from typing import Dict, Union
+from typing import Dict, Union, cast
 
-from deprecated.sphinx import deprecated
+from xrpl.asyncio.clients import Client, XRPLRequestFailureException
+from xrpl.core.addresscodec import is_valid_xaddress, xaddress_to_classic_address
+from xrpl.models.requests import AccountInfo
 
-from xrpl.asyncio.account import main
-from xrpl.clients.sync_client import SyncClient
-from xrpl.models.response import Response
 
-
-def does_account_exist(
-    address: str, client: SyncClient, ledger_index: Union[str, int] = "validated"
+async def does_account_exist(
+    address: str, client: Client, ledger_index: Union[str, int] = "validated"
 ) -> bool:
     """
     Query the ledger for whether the account exists.
 
     Args:
         address: the account to query.
         client: the network client used to make network calls.
@@ -26,19 +23,26 @@
 
     Returns:
         Whether the account exists on the ledger.
 
     Raises:
         XRPLRequestFailureException: if the transaction fails.
     """
-    return asyncio.run(main.does_account_exist(address, client, ledger_index))
+    try:
+        await get_account_root(address, client, ledger_index=ledger_index)
+        return True
+    except XRPLRequestFailureException as e:
+        if e.error == "actNotFound":
+            # error code for if the account is not found on the ledger
+            return False
+        raise
 
 
-def get_next_valid_seq_number(
-    address: str, client: SyncClient, ledger_index: Union[str, int] = "current"
+async def get_next_valid_seq_number(
+    address: str, client: Client, ledger_index: Union[str, int] = "current"
 ) -> int:
     """
     Query the ledger for the next available sequence number for an account.
 
     Args:
         address: the account to query.
         client: the network client used to make network calls.
@@ -46,19 +50,21 @@
             ledger value or "current" (the current working version), "closed" (for the
             closed-and-proposed version), or "validated" (the most recent version
             validated by consensus). The default is "current".
 
     Returns:
         The next valid sequence number for the address.
     """
-    return asyncio.run(main.get_next_valid_seq_number(address, client, ledger_index))
+    return cast(
+        int, (await get_account_root(address, client, ledger_index))["Sequence"]
+    )
 
 
-def get_balance(
-    address: str, client: SyncClient, ledger_index: Union[str, int] = "validated"
+async def get_balance(
+    address: str, client: Client, ledger_index: Union[str, int] = "validated"
 ) -> int:
     """
     Query the ledger for the balance of the given account.
 
     Args:
         address: the account to query.
         client: the network client used to make network calls.
@@ -66,55 +72,48 @@
             ledger value or "current" (the current working version), "closed" (for the
             closed-and-proposed version), or "validated" (the most recent version
             validated by consensus). The default is "validated".
 
     Returns:
         The balance of the address.
     """
-    return asyncio.run(main.get_balance(address, client, ledger_index))
+    return int(
+        (await get_account_root(address, client, ledger_index=ledger_index))["Balance"]
+    )
 
 
-def get_account_root(
-    address: str, client: SyncClient, ledger_index: Union[str, int] = "validated"
+async def get_account_root(
+    address: str, client: Client, ledger_index: Union[str, int] = "validated"
 ) -> Dict[str, Union[int, str]]:
     """
     Query the ledger for the AccountRoot object associated with a given address.
 
     Args:
         address: the account to query.
         client: the network client used to make network calls.
         ledger_index: The ledger index to use for the request. Must be an integer
             ledger value or "current" (the current working version), "closed" (for the
             closed-and-proposed version), or "validated" (the most recent version
             validated by consensus). The default is "validated".
 
     Returns:
         The AccountRoot dictionary for the address.
-    """
-    return asyncio.run(main.get_account_root(address, client, ledger_index))
-
 
-@deprecated(
-    reason="Sending an AccountInfo request directly is just as easy to use.",
-    version="1.8.0",
-)
-def get_account_info(
-    address: str, client: SyncClient, ledger_index: Union[str, int] = "validated"
-) -> Response:
+    Raises:
+        XRPLRequestFailureException: if the rippled API call fails.
     """
-    Query the ledger for account info of given address.
+    classic_address = address
 
-    Args:
-        address: the account to query.
-        client: the network client used to make network calls.
-        ledger_index: The ledger index to use for the request. Must be an integer
-            ledger value or "current" (the current working version), "closed" (for the
-            closed-and-proposed version), or "validated" (the most recent version
-            validated by consensus). The default is "validated".
+    if is_valid_xaddress(address):
+        classic_address, _, _ = xaddress_to_classic_address(address)
 
-    Returns:
-        The account info for the address.
+    account_info = await client._request_impl(
+        AccountInfo(
+            account=classic_address,
+            ledger_index=ledger_index,
+        )
+    )
 
-    Raises:
-        XRPLRequestFailureException: if the rippled API call fails.
-    """
-    return asyncio.run(main.get_account_info(address, client, ledger_index))
+    if not account_info.is_successful():
+        raise XRPLRequestFailureException(account_info.result)
+
+    return cast(Dict[str, Union[int, str]], account_info.result["account_data"])
```

### Comparing `xrpl-py-2.0.0b0/xrpl/asyncio/clients/__init__.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_client.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/async_client.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_websocket_client.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/async_websocket_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,23 +112,21 @@
             # remember to run your entire program within a
             # `asyncio.run` call.
             asyncio.run(main())
     """
 
     async def open(self: AsyncWebsocketClient) -> None:
         """Connects the client to the Web Socket API at the given URL."""
-        if self.is_open():
-            return
-        await self._do_open()
+        if not self.is_open():
+            await self._do_open()
 
     async def close(self: AsyncWebsocketClient) -> None:
         """Closes the connection."""
-        if not self.is_open():
-            return
-        await self._do_close()
+        if self.is_open():
+            await self._do_close()
 
     async def __aenter__(self: AsyncWebsocketClient) -> AsyncWebsocketClient:
         """
         Enters an async context after opening itself.
 
         Returns:
             The opened client.
@@ -142,15 +140,20 @@
         _exc_val: BaseException,
         _trace: TracebackType,
     ) -> None:
         """Exits an async context after closing itself."""
         await self.close()
 
     async def __aiter__(self: AsyncWebsocketClient) -> AsyncIterator[Dict[str, Any]]:
-        """Iterate on received messages."""
+        """
+        Iterate on received messages.
+
+        Yields:
+            Message at the top of the queue.
+        """
         while self.is_open():
             yield await self._do_pop_message()
 
     async def send(self: AsyncWebsocketClient, request: Request) -> None:
         """
         Submit the request represented by the request to the
         rippled node specified by this client's URL. Unlike ``request``,
```

### Comparing `xrpl-py-2.0.0b0/xrpl/asyncio/clients/client.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Interface for all network clients to follow."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from typing import Optional
 
 from xrpl.models.requests.request import Request
 from xrpl.models.response import Response
 
 
 class Client(ABC):
     """
@@ -18,14 +19,16 @@
         """
         Initializes a client.
 
         Arguments:
             url: The url to which this client will connect
         """
         self.url = url
+        self.network_id: Optional[int] = None
+        self.build_version: Optional[str] = None
 
     @abstractmethod
     async def _request_impl(self: Client, request: Request) -> Response:
         """
         This is the actual driver for a given Client's request. It must be
         async because all of the helper functions in this library are
         async-first. Implement this in a given Client.
```

### Comparing `xrpl-py-2.0.0b0/xrpl/asyncio/clients/exceptions.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/asyncio/clients/json_rpc_base.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/json_rpc_base.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/asyncio/clients/utils.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/asyncio/clients/websocket_base.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/clients/websocket_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A client for interacting with the rippled WebSocket API."""
 from __future__ import annotations
 
+import asyncio
 import json
-from asyncio import Future, Queue, Task, create_task, get_running_loop
 from random import randrange
 from typing import TYPE_CHECKING, Any, Dict, Optional, cast
 
 from typing_extensions import Final
 from websockets.legacy.client import WebSocketClientProtocol, connect
 
 from xrpl.asyncio.clients.client import Client
@@ -15,28 +15,34 @@
 from xrpl.models.requests.request import Request
 from xrpl.models.response import Response
 
 _REQ_ID_MAX: Final[int] = 1_000_000
 # the types from asyncio are not implemented as generics in python 3.8 and
 # lower, so we need to only subscript them when running typechecking.
 if TYPE_CHECKING:
-    _REQUESTS_TYPE = Dict[str, Future[Dict[str, Any]]]
-    _MESSAGES_TYPE = Queue[Dict[str, Any]]
-    _HANDLER_TYPE = Task[None]
+    _REQUESTS_TYPE = Dict[str, asyncio.Future[Dict[str, Any]]]
+    _MESSAGES_TYPE = asyncio.Queue[Dict[str, Any]]
+    _HANDLER_TYPE = asyncio.Task[None]
 else:
-    _REQUESTS_TYPE = Dict[str, Future]
-    _MESSAGES_TYPE = Queue
-    _HANDLER_TYPE = Task
+    _REQUESTS_TYPE = Dict[str, asyncio.Future]
+    _MESSAGES_TYPE = asyncio.Queue
+    _HANDLER_TYPE = asyncio.Task
 
 
 def _inject_request_id(request: Request) -> Request:
     """
     Given a Request with an ID, return the same Request.
 
     Given a Request without an ID, make a copy with a randomly generated ID.
+
+    Arguments:
+        request: The request to inject an ID into.
+
+    Returns:
+        The request with an ID injected into it.
     """
     if request.id is not None:
         return request
     request_dict = request.to_dict()
     request_dict["id"] = f"{request.method}_{randrange(_REQ_ID_MAX)}"
     return Request.from_dict(request_dict)
 
@@ -81,18 +87,18 @@
 
     async def _do_open(self: WebsocketBase) -> None:
         """Connects the client to the Web Socket API at its URL."""
         # open the connection
         self._websocket = await connect(self.url)
 
         # make a message queue
-        self._messages = Queue()
+        self._messages = asyncio.Queue()
 
         # start the handler
-        self._handler_task = create_task(self._handler())
+        self._handler_task = asyncio.create_task(self._handler())
 
     async def _do_close(self: WebsocketBase) -> None:
         """Closes the connection."""
         # cancel the handler
         cast(_HANDLER_TYPE, self._handler_task).cancel()
         self._handler_task = None
 
@@ -131,41 +137,65 @@
             cast(_MESSAGES_TYPE, self._messages).put_nowait(response_dict)
 
     def _set_up_future(self: WebsocketBase, request: Request) -> None:
         """
         Only to be called from the public send and _request_impl functions.
         Given a request with an ID, ensure that that ID is backed by an open
         Future in self._open_requests.
+
+        Arguments:
+            request: The request with which to set up a future.
+
+        Raises:
+            XRPLWebsocketException: if there is already a request with this ID
+                in progress.
         """
         if request.id is None:
             return
         request_str = str(request.id)
         if (
             request_str in self._open_requests
             and not self._open_requests[request_str].done()
         ):
             raise XRPLWebsocketException(
                 f"Request {request_str} is already in progress."
             )
-        self._open_requests[request_str] = get_running_loop().create_future()
+        self._open_requests[request_str] = asyncio.get_running_loop().create_future()
 
     async def _do_send_no_future(self: WebsocketBase, request: Request) -> None:
+        """
+        Base websocket send function
+
+        Arguments:
+            request: The request to send.
+        """
         await cast(WebSocketClientProtocol, self._websocket).send(
             json.dumps(
                 request_to_websocket(request),
             ),
         )
 
     async def _do_send(self: WebsocketBase, request: Request) -> None:
+        """
+        Websocket send function that should be used by
+        any inherited classes.
+
+        Arguments:
+            request: The request to send.
+        """
         # we need to set up a future here, even if no one cares about it, so
         # that if a user submits a few requests with the same ID they fail.
         self._set_up_future(request)
         await self._do_send_no_future(request)
 
     async def _do_pop_message(self: WebsocketBase) -> Dict[str, Any]:
+        """
+        Returns:
+            The top message from the queue
+        """
         msg = await cast(_MESSAGES_TYPE, self._messages).get()
         cast(_MESSAGES_TYPE, self._messages).task_done()
         return msg
 
     async def _do_request_impl(self: WebsocketBase, request: Request) -> Response:
         """
         Base ``_request_impl`` implementation for websockets.
@@ -183,13 +213,13 @@
         # if no ID on this request, generate and inject one, and ensure it
         # is backed by a future
         request_with_id = _inject_request_id(request)
         request_str = str(request_with_id.id)
         self._set_up_future(request_with_id)
 
         # fire-and-forget the send, and await the Future
-        create_task(self._do_send_no_future(request_with_id))
+        asyncio.create_task(self._do_send_no_future(request_with_id))
         raw_response = await self._open_requests[request_str]
 
         # remove the resolved Future, hopefully getting it garbage colleted
         del self._open_requests[request_str]
         return websocket_to_response(raw_response)
```

### Comparing `xrpl-py-2.0.0b0/xrpl/asyncio/ledger/main.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/ledger/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/asyncio/ledger/utils.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/ledger/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/asyncio/transaction/__init__.py` & `xrpl_py-2.1.0b0/xrpl/transaction/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,26 @@
-"""Async methods for working with transactions on the XRP Ledger."""
-from xrpl.asyncio.transaction.ledger import get_transaction_from_hash
-from xrpl.asyncio.transaction.main import (
+"""Methods for working with transactions on the XRP Ledger."""
+from xrpl.asyncio.transaction import (
+    XRPLReliableSubmissionException,
+    transaction_json_to_binary_codec_form,
+)
+from xrpl.transaction.main import (
     autofill,
     autofill_and_sign,
-    safe_sign_and_autofill_transaction,
-    safe_sign_and_submit_transaction,
-    safe_sign_transaction,
     sign,
     sign_and_submit,
     submit,
-    submit_transaction,
-    transaction_json_to_binary_codec_form,
-)
-from xrpl.asyncio.transaction.reliable_submission import (
-    XRPLReliableSubmissionException,
-    send_reliable_submission,
 )
+from xrpl.transaction.multisign import multisign
+from xrpl.transaction.reliable_submission import submit_and_wait
 
 __all__ = [
     "autofill",
     "autofill_and_sign",
-    "get_transaction_from_hash",
-    "safe_sign_transaction",
-    "safe_sign_and_autofill_transaction",
-    "safe_sign_and_submit_transaction",
     "sign",
     "sign_and_submit",
     "submit",
-    "submit_transaction",
+    "submit_and_wait",
     "transaction_json_to_binary_codec_form",
-    "send_reliable_submission",
+    "multisign",
     "XRPLReliableSubmissionException",
 ]
```

### Comparing `xrpl-py-2.0.0b0/xrpl/asyncio/wallet/wallet_generation.py` & `xrpl_py-2.1.0b0/xrpl/asyncio/wallet/wallet_generation.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 from xrpl.asyncio.clients import Client, XRPLRequestFailureException
 from xrpl.constants import XRPLException
 from xrpl.wallet.main import Wallet
 
 _TEST_FAUCET_URL: Final[str] = "https://faucet.altnet.rippletest.net/accounts"
 _DEV_FAUCET_URL: Final[str] = "https://faucet.devnet.rippletest.net/accounts"
 _AMM_DEV_FAUCET_URL: Final[str] = "https://ammfaucet.devnet.rippletest.net/accounts"
-_NFT_DEV_FAUCET_URL: Final[str] = "https://faucet-nft.ripple.com/accounts"
-_HOOKS_V2_TEST_FAUCET_URL: Final[
+_HOOKS_V3_TEST_FAUCET_URL: Final[
     str
-] = "https://hooks-testnet-v2.xrpl-labs.com/accounts"
+] = "https://hooks-testnet-v3.xrpl-labs.com/accounts"
+_SIDECHAIN_DEVNET_FAUCET_URL: Final[
+    str
+] = "https://sidechain-faucet.devnet.rippletest.net/accounts"
 
 _TIMEOUT_SECONDS: Final[int] = 40
 
 
 class XRPLFaucetException(XRPLException):
     """Faucet generation exception."""
 
@@ -28,24 +30,32 @@
 
 
 async def generate_faucet_wallet(
     client: Client,
     wallet: Optional[Wallet] = None,
     debug: bool = False,
     faucet_host: Optional[str] = None,
+    usage_context: Optional[str] = None,
+    user_agent: Optional[str] = "xrpl-py",
 ) -> Wallet:
     """
     Generates a random wallet and funds it using the XRPL Testnet Faucet.
 
     Args:
         client: the network client used to make network calls.
         wallet: the wallet to fund. If omitted or `None`, a new wallet is created.
         debug: Whether to print debug information as it creates the wallet.
         faucet_host: A custom host to use for funding a wallet. In environments other
             than devnet and testnet, this parameter is required.
+        usage_context: The intended use case for the funding request
+            (for example, testing). This information  will be included
+            in the json body of the HTTP request to the faucet.
+        user_agent: A string representing the user agent (software/ client used)
+            for the HTTP request. Default is "xrpl-py".
+
 
     Returns:
         A Wallet on the testnet that contains some amount of XRP.
 
     Raises:
         XRPLFaucetException: if an address could not be funded with the faucet.
         XRPLRequestFailureException: if a request to the ledger fails.
@@ -54,24 +64,24 @@
     .. # noqa: DAR402 exception raised in private method
     """
     faucet_url = get_faucet_url(client.url, faucet_host)
 
     if wallet is None:
         wallet = Wallet.create()
 
-    address = wallet.classic_address
+    address = wallet.address
     # The faucet *can* be flakey... by printing info about this it's easier to
     # understand if tests are actually failing, or if it was just a faucet failure.
     if debug:
         print("Attempting to fund address {}".format(address))
     # Balance prior to asking for more funds
     starting_balance = await _check_wallet_balance(address, client)
 
     # Ask the faucet to send funds to the given address
-    await _request_funding(faucet_url, address)
+    await _request_funding(faucet_url, address, usage_context, user_agent)
     # Wait for the faucet to fund our account or until timeout
     # Waits one second checks if balance has changed
     # If balance doesn't change it will attempt again until _TIMEOUT_SECONDS
     is_funded = False
     for _ in range(_TIMEOUT_SECONDS):
         await asyncio.sleep(1)
         if not is_funded:  # faucet transaction hasn't been validated yet
@@ -106,24 +116,29 @@
         The URL of the matching faucet.
 
     Raises:
         XRPLFaucetException: if the provided URL is not for the testnet or devnet.
     """
     if faucet_host is not None:
         return f"https://{faucet_host}/accounts"
-    if "hooks-testnet-v2" in url:  # hooks v2 testnet
-        return _HOOKS_V2_TEST_FAUCET_URL
+    if "hooks-testnet-v3" in url:  # hooks v3 testnet
+        return _HOOKS_V3_TEST_FAUCET_URL
     if "altnet" in url or "testnet" in url:  # testnet
         return _TEST_FAUCET_URL
     if "amm" in url:  # amm devnet
         return _AMM_DEV_FAUCET_URL
+    if "sidechain-net1" in url:  # sidechain devnet
+        return _SIDECHAIN_DEVNET_FAUCET_URL
+    elif "sidechain-net2" in url:  # sidechain issuing chain devnet
+        raise XRPLFaucetException(
+            "Cannot fund an account on an issuing chain. Accounts must be created via "
+            "the bridge."
+        )
     if "devnet" in url:  # devnet
         return _DEV_FAUCET_URL
-    if "xls20-sandbox" in url:  # nft devnet
-        return _NFT_DEV_FAUCET_URL
     raise XRPLFaucetException(
         "Cannot fund an account with a client that is not on the testnet or devnet."
     )
 
 
 async def _check_wallet_balance(address: str, client: Client) -> int:
     try:
@@ -131,17 +146,25 @@
     except XRPLRequestFailureException as e:
         if e.error == "actNotFound":  # transaction has not gone through
             return 0
         # some other error
         raise
 
 
-async def _request_funding(url: str, address: str) -> None:
+async def _request_funding(
+    url: str,
+    address: str,
+    usage_context: Optional[str] = None,
+    user_agent: Optional[str] = None,
+) -> None:
     async with httpx.AsyncClient() as http_client:
-        response = await http_client.post(url=url, json={"destination": address})
+        json_body = {"destination": address, "userAgent": user_agent}
+        if usage_context is not None:
+            json_body["usageContext"] = usage_context
+        response = await http_client.post(url=url, json=json_body)
     if not response.status_code == httpx.codes.OK:
         response.raise_for_status()
 
 
 async def _try_to_get_next_seq(address: str, client: Client) -> Optional[int]:
     try:
         return await get_next_valid_seq_number(address, client)
```

### Comparing `xrpl-py-2.0.0b0/xrpl/clients/__init__.py` & `xrpl_py-2.1.0b0/xrpl/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/clients/sync_client.py` & `xrpl_py-2.1.0b0/xrpl/clients/sync_client.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/clients/websocket_client.py` & `xrpl_py-2.1.0b0/xrpl/clients/websocket_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A sync client for interacting with the rippled WebSocket API."""
 from __future__ import annotations
 
-from asyncio import AbstractEventLoop, new_event_loop, run_coroutine_threadsafe
+import asyncio
 from concurrent.futures import CancelledError, TimeoutError
 from threading import Thread
 from types import TracebackType
 from typing import Any, Dict, Iterator, Optional, Type, Union, cast
 
 from xrpl.asyncio.clients.exceptions import XRPLWebsocketException
 from xrpl.asyncio.clients.websocket_base import WebsocketBase
@@ -73,15 +73,15 @@
         Arguments:
             url: The URL of the rippled node to submit requests to.
             timeout: Maximum seconds to wait for a new message when
                 iterating. A value of 0 or None will result in no limit.
                 If this limit is met, iteration will stop.
         """
         self.timeout = timeout
-        self._loop: Optional[AbstractEventLoop] = None
+        self._loop: Optional[asyncio.AbstractEventLoop] = None
         self._thread: Optional[Thread] = None
         super().__init__(url)
 
     def is_open(self: WebsocketClient) -> bool:
         """
         Returns whether the client is currently open.
 
@@ -92,47 +92,47 @@
 
     def open(self: WebsocketClient) -> None:
         """Connects the client to the Web Socket API at the given URL."""
         if self.is_open():
             return
 
         # make a new asyncio event loop
-        self._loop = new_event_loop()
+        self._loop = asyncio.new_event_loop()
 
         # create and start a thread to run that event loop
         self._thread = Thread(
             target=self._loop.run_forever,
             daemon=True,
         )
         self._thread.start()
 
         # run WebsocketBase._do_open on the event loop of the child thread and
         # wait for it to finish
-        run_coroutine_threadsafe(self._do_open(), self._loop).result()
+        asyncio.run_coroutine_threadsafe(self._do_open(), self._loop).result()
 
     def close(self: WebsocketClient) -> None:
         """Closes the connection."""
         if not self.is_open():
             return
 
         # run WebsocketBase._do_close on the event loop of the child thread and
         # wait for it to finish
-        run_coroutine_threadsafe(
-            self._do_close(), cast(AbstractEventLoop, self._loop)
+        asyncio.run_coroutine_threadsafe(
+            self._do_close(), cast(asyncio.AbstractEventLoop, self._loop)
         ).result()
 
         # request the child thread to stop the loop and wait for it to
         # terminate
-        cast(AbstractEventLoop, self._loop).call_soon_threadsafe(
-            cast(AbstractEventLoop, self._loop).stop
+        cast(asyncio.AbstractEventLoop, self._loop).call_soon_threadsafe(
+            cast(asyncio.AbstractEventLoop, self._loop).stop
         )
         cast(Thread, self._thread).join()
 
         # close the stopped loop
-        cast(AbstractEventLoop, self._loop).close()
+        cast(asyncio.AbstractEventLoop, self._loop).close()
 
         # clear state
         self._loop = None
         self._thread = None
 
     def __enter__(self: WebsocketClient) -> WebsocketClient:
         """
@@ -156,18 +156,21 @@
     def __iter__(self: WebsocketClient) -> Iterator[Dict[str, Any]]:
         """
         Iterate on received messages. This iterator will block until
         a message is received. If no message is received within
         `self.timeout` seconds then the iterator will exit. If
         `self.timeout` is `None` or `0` then the iterator will block
         indefinetly for the next messsage.
+
+        Yields:
+            The message at the top of the queue.
         """
         while self.is_open():
-            future = run_coroutine_threadsafe(
-                self._do_pop_message(), cast(AbstractEventLoop, self._loop)
+            future = asyncio.run_coroutine_threadsafe(
+                self._do_pop_message(), cast(asyncio.AbstractEventLoop, self._loop)
             )
             try:
                 yield future.result(self.timeout)
             except TimeoutError:
                 # in this case, the future reached its timeout. we can safely
                 # cancel and stop listening
                 future.cancel()
@@ -189,16 +192,16 @@
 
         Raises:
             XRPLWebsocketException: If there is already an open request by the
                 request's ID, or if this WebsocketClient is not open.
         """
         if not self.is_open():
             raise XRPLWebsocketException("Websocket is not open")
-        run_coroutine_threadsafe(
-            self._do_send(request), cast(AbstractEventLoop, self._loop)
+        asyncio.run_coroutine_threadsafe(
+            self._do_send(request), cast(asyncio.AbstractEventLoop, self._loop)
         ).result()
 
     async def _request_impl(self: WebsocketClient, request: Request) -> Response:
         """
         ``_request_impl`` implementation for sync websockets that ensures the
         ``WebsocketBase._do_request_impl`` implementation is run on the other thread.
 
@@ -224,11 +227,11 @@
         # is a sync client we want to completely block until the request is
         # complete. also, `asyncio.run_coroutine_threadsafe` returns a
         # concurrent.futures.Future which is not awaitable.
         #
         # when this is run via `await client._request_impl`, it will
         # completely block the main thread until completed,
         # just as if it were not async.
-        return run_coroutine_threadsafe(
+        return asyncio.run_coroutine_threadsafe(
             self._do_request_impl(request),
-            cast(AbstractEventLoop, self._loop),
+            cast(asyncio.AbstractEventLoop, self._loop),
         ).result()
```

### Comparing `xrpl-py-2.0.0b0/xrpl/constants.py` & `xrpl_py-2.1.0b0/xrpl/constants.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/addresscodec/__init__.py` & `xrpl_py-2.1.0b0/xrpl/core/addresscodec/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/addresscodec/codec.py` & `xrpl_py-2.1.0b0/xrpl/core/addresscodec/codec.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/addresscodec/main.py` & `xrpl_py-2.1.0b0/xrpl/core/addresscodec/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/__init__.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/definitions.json` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/definitions.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9085559395904224%*

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
@@ -267,14 +297,24 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 20,
                 "type": "UInt16"
             }
         ],
         [
+            "NetworkID",
+            {
+                "isSerialized": true,
+                "isSigningField": true,
+                "isVLEncoded": false,
+                "nth": 1,
+                "type": "UInt32"
+            }
+        ],
+        [
             "Flags",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 2,
                 "type": "UInt32"
@@ -707,14 +747,54 @@
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
@@ -877,14 +957,44 @@
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
@@ -1057,14 +1167,24 @@
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
@@ -1327,14 +1447,44 @@
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
@@ -1367,14 +1517,124 @@
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
@@ -1707,14 +1967,74 @@
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
@@ -1757,14 +2077,64 @@
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
@@ -1967,14 +2337,84 @@
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
@@ -2057,14 +2497,24 @@
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
@@ -2105,20 +2555,72 @@
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
@@ -2129,17 +2631,23 @@
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
@@ -2173,19 +2681,37 @@
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
@@ -2211,15 +2737,19 @@
         "telCAN_NOT_QUEUE_BLOCKED": -389,
         "telCAN_NOT_QUEUE_BLOCKS": -390,
         "telCAN_NOT_QUEUE_FEE": -388,
         "telCAN_NOT_QUEUE_FULL": -387,
         "telFAILED_PROCESSING": -395,
         "telINSUF_FEE_P": -394,
         "telLOCAL_ERROR": -399,
+        "telNETWORK_ID_MAKES_TX_NON_CANONICAL": -384,
         "telNO_DST_PARTIAL": -393,
+        "telREQUIRES_NETWORK_ID": -385,
+        "telWRONG_NETWORK": -386,
+        "temBAD_AMM_TOKENS": -261,
         "temBAD_AMOUNT": -298,
         "temBAD_CURRENCY": -297,
         "temBAD_EXPIRATION": -296,
         "temBAD_FEE": -295,
         "temBAD_ISSUER": -294,
         "temBAD_LIMIT": -293,
         "temBAD_NFTOKEN_TRANSFER_FEE": -262,
@@ -2236,43 +2766,56 @@
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
@@ -2296,24 +2839,33 @@
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
@@ -2323,10 +2875,11 @@
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

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/definitions.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/definitions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_header.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_header.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_info.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_info.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_instance.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_instance.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/field_id_codec.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/field_id_codec.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/main.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/main.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/__init__.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/__init__.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/account_id.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/account_id.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/amount.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/amount.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,16 @@
     Raises:
         XRPLBinaryCodecException: If issued_currency_value is invalid.
     """
     decimal_value = Decimal(issued_currency_value)
     if decimal_value.is_zero():
         return
     exponent = decimal_value.as_tuple().exponent
+    if not isinstance(exponent, int):  # NaN, sNaN, Infinity
+        raise XRPLBinaryCodecException(f"Expected exponent to be int, is {exponent}")
     if (
         (_calculate_precision(issued_currency_value) > MAX_IOU_PRECISION)
         or (exponent > MAX_IOU_EXPONENT)
         or (exponent < MIN_IOU_EXPONENT)
     ):
         raise XRPLBinaryCodecException(
             "Decimal precision out of range for issued currency value."
@@ -145,14 +147,16 @@
     decimal_value = Decimal(value)
     if decimal_value.is_zero():
         return _ZERO_CURRENCY_AMOUNT_HEX.to_bytes(8, byteorder="big")
 
     # Convert components to integers ---------------------------------------
     sign, digits, exp = decimal_value.as_tuple()
     mantissa = int("".join([str(d) for d in digits]))
+    if not isinstance(exp, int):  # NaN, sNaN, Infinity
+        raise XRPLBinaryCodecException(f"Expected exp to be int, is {exp}")
 
     # Canonicalize to expected range ---------------------------------------
     while mantissa < MIN_IOU_MANTISSA and exp > MIN_IOU_EXPONENT:
         mantissa *= 10
         exp -= 1
 
     while mantissa > MAX_IOU_MANTISSA:
```

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/blob.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/blob.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/currency.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/currency.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash128.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash256.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Codec for serializing and deserializing a hash field with a width
-of 128 bits (16 bytes).
+of 256 bits (32 bytes).
 `See Hash Fields <https://xrpl.org/serialization.html#hash-fields>`_
 """
 from __future__ import annotations
 
 from typing import Type
 
 from xrpl.core.binarycodec.types.hash import Hash
 
 
-class Hash128(Hash):
+class Hash256(Hash):
     """
     Codec for serializing and deserializing a hash field with a width
-    of 128 bits (16 bytes).
+    of 256 bits (32 bytes).
     `See Hash Fields <https://xrpl.org/serialization.html#hash-fields>`_
     """
 
     @classmethod
-    def _get_length(cls: Type[Hash128]) -> int:
-        return 16
+    def _get_length(cls: Type[Hash256]) -> int:
+        return 32
```

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash160.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash160.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/path_set.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/path_set.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/serialized_type.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/serialized_type.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/st_array.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/st_array.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/st_object.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/st_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         from xrpl.core.binarycodec.binary_wrappers.binary_serializer import (
             BinarySerializer,
         )
 
         serializer = BinarySerializer()
 
         xaddress_decoded = {}
-        for (k, v) in value.items():
+        for k, v in value.items():
             if isinstance(v, str) and is_valid_xaddress(v):
                 handled = _handle_xaddress(k, v)
                 if (
                     _SOURCE_TAG in handled
                     and handled[_SOURCE_TAG] is not None
                     and _SOURCE_TAG in value
                     and value[_SOURCE_TAG] is not None
```

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint16.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint16.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint32.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint32.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint64.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint64.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint8.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint8.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/vector256.py` & `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/vector256.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/keypairs/crypto_implementation.py` & `xrpl_py-2.1.0b0/xrpl/core/keypairs/crypto_implementation.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/keypairs/ed25519.py` & `xrpl_py-2.1.0b0/xrpl/core/keypairs/ed25519.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/keypairs/helpers.py` & `xrpl_py-2.1.0b0/xrpl/core/keypairs/helpers.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/core/keypairs/main.py` & `xrpl_py-2.1.0b0/xrpl/core/keypairs/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Interface for cryptographic key pairs for use with the XRP Ledger."""
 from secrets import token_bytes
-from typing import Dict, Optional, Tuple, Type
+from typing import Dict, Optional, Tuple, Type, Union
 
 from typing_extensions import Final
 
 from xrpl.constants import CryptoAlgorithm
 from xrpl.core import addresscodec
 from xrpl.core.keypairs.crypto_implementation import CryptoImplementation
 from xrpl.core.keypairs.ed25519 import ED25519
@@ -93,25 +93,27 @@
     Returns:
         The classic address corresponding to the given public key.
     """
     account_id = get_account_id(bytes.fromhex(public_key))
     return addresscodec.encode_classic_address(account_id)
 
 
-def sign(message: bytes, private_key: str) -> str:
+def sign(message: Union[str, bytes], private_key: str) -> str:
     """
     Sign a message using a given private key.
 
     Args:
         message: The message to sign, as bytes.
         private_key: The private key to use to sign the message.
 
     Returns:
         Signed message, as hexadecimal.
     """
+    if isinstance(message, str):
+        message = bytes.fromhex(message)
     return (
         _get_module_from_key(private_key)
         .sign(
             message,
             private_key,
         )
         .hex()
```

### Comparing `xrpl-py-2.0.0b0/xrpl/core/keypairs/secp256k1.py` & `xrpl_py-2.1.0b0/xrpl/core/keypairs/secp256k1.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/ledger/main.py` & `xrpl_py-2.1.0b0/xrpl/ledger/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/__init__.py` & `xrpl_py-2.1.0b0/xrpl/models/__init__.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/models/amounts/amount.py` & `xrpl_py-2.1.0b0/xrpl/models/amounts/amount.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/amounts/issued_currency_amount.py` & `xrpl_py-2.1.0b0/xrpl/models/amounts/issued_currency_amount.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/base_model.py` & `xrpl_py-2.1.0b0/xrpl/models/base_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """The base class for all model types."""
 
 from __future__ import annotations
 
 import json
 import re
 from abc import ABC
-from dataclasses import fields
+from dataclasses import dataclass, fields
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
 
@@ -59,14 +69,15 @@
     if isinstance(value, dict):
         return {_key_to_json(k): _value_to_json(v) for (k, v) in value.items()}
     if isinstance(value, list):
         return [_value_to_json(sub_value) for sub_value in value]
     return value
 
 
+@dataclass(frozen=True)
 class BaseModel(ABC):
     """The base class for all model types."""
 
     @classmethod
     def is_dict_of_model(cls: Type[BM], dictionary: Any) -> bool:
         """
         Checks whether the provided ``dictionary`` is a dictionary representation
@@ -163,14 +174,18 @@
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
@@ -268,15 +283,15 @@
 
         If not overridden, returns the object dict with all non-None values.
 
         Returns:
             The dictionary representation of a BaseModel.
         """
         # mypy doesn't realize that BaseModel has a field called __dataclass_fields__
-        dataclass_fields = self.__dataclass_fields__.keys()  # type: ignore
+        dataclass_fields = self.__dataclass_fields__.keys()
         return {
             key: self._to_dict_elem(getattr(self, key))
             for key in dataclass_fields
             if getattr(self, key) is not None
         }
 
     def _to_dict_elem(self: BaseModel, elem: Any) -> Any:
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/currencies/issued_currency.py` & `xrpl_py-2.1.0b0/xrpl/models/currencies/issued_currency.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/currencies/xrp.py` & `xrpl_py-2.1.0b0/xrpl/models/currencies/xrp.py`

 * *Files 13% similar despite different names*

```diff
@@ -57,18 +57,32 @@
         Returns the dictionary representation of an XRP currency object.
 
         Returns:
             The dictionary representation of an XRP currency object.
         """
         return {**super().to_dict(), "currency": "XRP"}
 
-    def to_amount(self: XRP, value: Union[str, int]) -> str:
+    def to_amount(self: XRP, value: Union[str, int, float]) -> str:
         """
         Converts value to XRP.
 
         Args:
             value: The amount of XRP.
 
         Returns:
             A string representation of XRP amount.
         """
-        return str(value)
+        # import needed here to avoid circular dependency
+        from xrpl.utils.xrp_conversions import xrp_to_drops
+
+        if isinstance(value, str):
+            return xrp_to_drops(float(value))
+        return xrp_to_drops(value)
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

### Comparing `xrpl-py-2.0.0b0/xrpl/models/flags.py` & `xrpl_py-2.1.0b0/xrpl/models/flags.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,41 @@
-"""All transacion flags and utils to build a list of ints from a FlagInterface"""
+"""All transaction flags and utils to build a list of ints from a FlagInterface"""
 
 from typing import Dict, List, Union
 
 from typing_extensions import TypedDict
 
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.transactions.types.pseudo_transaction_type import PseudoTransactionType
 from xrpl.models.transactions.types.transaction_type import TransactionType
 
 TX_FLAGS: Dict[str, Dict[str, int]] = {
     "AccountSet": {
-        "asf_account_tx_id": 0x00000005,
-        "asf_authorized_nftoken_minter": 0x0000000A,
-        "asf_default_ripple": 0x00000008,
-        "asf_deposit_auth": 0x00000009,
-        "asf_disable_master": 0x00000004,
-        "asf_disallow_xrp": 0x00000003,
-        "asf_global_freeze": 0x00000007,
-        "asf_no_freeze": 0x00000006,
-        "asf_require_auth": 0x00000002,
-        "asf_require_dest": 0x00000001,
+        "tf_require_dest_tag": 0x00010000,
+        "tf_optional_dest_tag": 0x00020000,
+        "tf_require_auth": 0x00040000,
+        "tf_optional_auth": 0x00080000,
+        "tf_disallow_xrp": 0x00100000,
+        "tf_allow_xrp": 0x00200000,
+    },
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
     },
     "NFTokenCreateOffer": {
         "tf_sell_token": 0x00000001,
     },
     "NFTokenMint": {
         "tf_burnable": 0x00000001,
         "tf_only_xrp": 0x00000002,
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/nested_model.py` & `xrpl_py-2.1.0b0/xrpl/models/nested_model.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/path.py` & `xrpl_py-2.1.0b0/xrpl/models/path.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/__init__.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,35 @@
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
 from xrpl.models.requests.ledger import Ledger
 from xrpl.models.requests.ledger_closed import LedgerClosed
 from xrpl.models.requests.ledger_current import LedgerCurrent
 from xrpl.models.requests.ledger_data import LedgerData
-from xrpl.models.requests.ledger_entry import LedgerEntry
+from xrpl.models.requests.ledger_entry import LedgerEntry, LedgerEntryType
 from xrpl.models.requests.manifest import Manifest
 from xrpl.models.requests.nft_buy_offers import NFTBuyOffers
+from xrpl.models.requests.nft_history import NFTHistory
+from xrpl.models.requests.nft_info import NFTInfo
 from xrpl.models.requests.nft_sell_offers import NFTSellOffers
 from xrpl.models.requests.no_ripple_check import NoRippleCheck, NoRippleCheckRole
 from xrpl.models.requests.path_find import PathFind, PathFindSubcommand
 from xrpl.models.requests.ping import Ping
 from xrpl.models.requests.random import Random
 from xrpl.models.requests.request import Request
 from xrpl.models.requests.ripple_path_find import RipplePathFind
@@ -48,29 +52,34 @@
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
     "Ledger",
     "LedgerClosed",
     "LedgerCurrent",
     "LedgerData",
     "LedgerEntry",
+    "LedgerEntryType",
     "Manifest",
     "NFTBuyOffers",
     "NFTSellOffers",
+    "NFTInfo",
+    "NFTHistory",
     "NoRippleCheck",
     "NoRippleCheckRole",
     "PathFind",
     "PathFindSubcommand",
     "PathStep",
     "Ping",
     "Random",
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/account_channels.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_channels.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 destination. (A channel's "source" and "owner" are the same.)
 
 All information retrieved is relative to a particular version of the ledger.
 
 `See account_channels <https://xrpl.org/account_channels.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Any, Optional, Union
+from typing import Any, Optional
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountChannels(Request):
+class AccountChannels(Request, LookupByLedgerRequest):
     """
     This request returns information about an account's Payment Channels. This includes
     only channels where the specified account is the channel's source, not the
     destination. (A channel's "source" and "owner" are the same.)
 
     All information retrieved is relative to a particular version of the ledger.
 
@@ -37,9 +37,7 @@
     """
 
     destination_account: Optional[str] = None
     limit: int = 200
     # marker data shape is actually undefined in the spec, up to the
     # implementation of an individual server
     marker: Optional[Any] = None
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/account_currencies.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_currencies.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 
 This is not a thoroughly confirmed list, but it can be used to populate user
 interfaces.
 
 `See account_currencies <https://xrpl.org/account_currencies.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Optional, Union
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountCurrencies(Request):
+class AccountCurrencies(Request, LookupByLedgerRequest):
     """
     This request retrieves a list of currencies that an account can send or receive,
     based on its trust lines.
 
     This is not a thoroughly confirmed list, but it can be used to populate user
     interfaces.
 
@@ -30,12 +29,9 @@
 
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
-
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_CURRENCIES, init=False)
     strict: bool = False
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/account_info.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 balance.
 
 All information retrieved is relative to a particular version of the ledger.
 
 `See account_info <https://xrpl.org/account_info.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Optional, Union
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountInfo(Request):
+class AccountInfo(Request, LookupByLedgerRequest):
     """
     This request retrieves information about an account, its activity, and its XRP
     balance.
 
     All information retrieved is relative to a particular version of the ledger.
 
     `See account_info <https://xrpl.org/account_info.html>`_
@@ -29,13 +28,11 @@
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_INFO, init=False)
     queue: bool = False
     signer_lists: bool = False
     strict: bool = False
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/account_lines.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_lines.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 This request returns information about an account's trust lines, including balances
 in all non-XRP currencies and assets. All information retrieved is relative to a
 particular version of the ledger.
 
 `See account_lines <https://xrpl.org/account_lines.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Any, Optional, Union
+from typing import Any, Optional
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountLines(Request):
+class AccountLines(Request, LookupByLedgerRequest):
     """
     This request returns information about an account's trust lines, including balances
     in all non-XRP currencies and assets. All information retrieved is relative to a
     particular version of the ledger.
 
     `See account_lines <https://xrpl.org/account_lines.html>`_
     """
@@ -27,15 +27,13 @@
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_LINES, init=False)
     peer: Optional[str] = None
     limit: Optional[int] = None
     # marker data shape is actually undefined in the spec, up to the
     # implementation of an individual server
     marker: Optional[Any] = None
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/account_nfts.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_nfts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """This method retrieves all of the NFTs currently owned by the specified account."""
 from dataclasses import dataclass, field
 from typing import Any, Optional
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountNFTs(Request):
+class AccountNFTs(Request, LookupByLedgerRequest):
     """
     This method retrieves all of the NFTs currently owned
     by the specified account.
     """
 
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_NFTS, init=False)
     account: str = REQUIRED  # type: ignore
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/account_objects.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_objects.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,37 +4,41 @@
 For a higher-level view of an account's trust lines and balances, see
 AccountLinesRequest instead.
 
 `See account_objects <https://xrpl.org/account_objects.html>`_
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Any, Optional, Union
+from typing import Any, Optional
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
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
+    XCHAIN_OWNED_CREATE_ACCOUNT_CLAIM_ID = "xchain_owned_create_account_claim_id"
+    XCHAIN_OWNED_CLAIM_ID = "xchain_owned_claim_id"
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountObjects(Request):
+class AccountObjects(Request, LookupByLedgerRequest):
     """
     This request returns the raw ledger format for all objects owned by an account.
 
     For a higher-level view of an account's trust lines and balances, see
     AccountLinesRequest instead.
 
     `See account_objects <https://xrpl.org/account_objects.html>`_
@@ -43,16 +47,14 @@
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_OBJECTS, init=False)
     type: Optional[AccountObjectType] = None
     deletion_blockers_only: bool = False
     limit: Optional[int] = None
     # marker data shape is actually undefined in the spec, up to the
     # implementation of an individual server
     marker: Optional[Any] = None
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/account_offers.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_offers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 """
 This request retrieves a list of offers made by a given account that are
 outstanding as of a particular ledger version.
 
 `See account_offers <https://xrpl.org/account_offers.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Any, Optional, Union
+from typing import Any, Optional
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountOffers(Request):
+class AccountOffers(Request, LookupByLedgerRequest):
     """
     This request retrieves a list of offers made by a given account that are
     outstanding as of a particular ledger version.
 
     `See account_offers <https://xrpl.org/account_offers.html>`_
     """
 
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_OFFERS, init=False)
     limit: Optional[int] = None
     # marker data shape is actually undefined in the spec, up to the
     # implementation of an individual server
     marker: Optional[Any] = None
     strict: bool = False
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/account_tx.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/account_tx.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 """
 This request retrieves from the ledger a list of transactions that involved the
 specified account.
 
 `See account_tx <https://xrpl.org/account_tx.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Any, Optional, Union
+from typing import Any, Optional
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountTx(Request):
+class AccountTx(Request, LookupByLedgerRequest):
     """
     This request retrieves from the ledger a list of transactions that involved the
     specified account.
 
     `See account_tx <https://xrpl.org/account_tx.html>`_
     """
 
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_TX, init=False)
     ledger_index_min: Optional[int] = None
     ledger_index_max: Optional[int] = None
     binary: bool = False
     forward: bool = False
     limit: Optional[int] = None
     # marker data shape is actually undefined in the spec, up to the
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/book_offers.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/nft_buy_offers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,27 @@
 """
-The book_offers method retrieves a list of offers, also known
-as the order book, between two currencies.
+The `nft_buy_offers` method retrieves all of buy offers
+for the specified NFToken.
 """
 from dataclasses import dataclass, field
-from typing import Optional, Union
 
-from xrpl.models.currencies import Currency
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class BookOffers(Request):
+class NFTBuyOffers(Request, LookupByLedgerRequest):
     """
-    The book_offers method retrieves a list of offers, also known
-    as the order book, between two currencies.
+    The `nft_buy_offers` method retrieves all of buy offers
+    for the specified NFToken.
     """
 
-    taker_gets: Currency = REQUIRED  # type: ignore
+    method: RequestMethod = field(default=RequestMethod.NFT_BUY_OFFERS, init=False)
+    nft_id: str = REQUIRED  # type: ignore
     """
-    This field is required.
+    The unique identifier of an NFToken.
+    The request returns buy offers for this NFToken. This value is required.
 
     :meta hide-value:
     """
-
-    taker_pays: Currency = REQUIRED  # type: ignore
-    """
-    This field is required.
-
-    :meta hide-value:
-    """
-
-    method: RequestMethod = field(default=RequestMethod.BOOK_OFFERS, init=False)
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
-    limit: Optional[int] = None
-    taker: Optional[str] = None
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/channel_authorize.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/channel_authorize.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/channel_verify.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/unsubscribe.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/deposit_authorized.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/deposit_authorized.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
 The deposit_authorized command indicates whether one account
 is authorized to send payments directly to another. See
 Deposit Authorization for information on how to require
 authorization to deliver money to your account.
 """
 from dataclasses import dataclass, field
-from typing import Optional
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class DepositAuthorized(Request):
+class DepositAuthorized(Request, LookupByLedgerRequest):
     """
     The deposit_authorized command indicates whether one account
     is authorized to send payments directly to another. See
     Deposit Authorization for information on how to require
     authorization to deliver money to your account.
     """
 
@@ -33,9 +32,7 @@
     """
     This field is required.
 
     :meta hide-value:
     """
 
     method: RequestMethod = field(default=RequestMethod.DEPOSIT_AUTHORIZED, init=False)
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[str] = None
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/fee.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/fee.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/gateway_balances.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/gateway_balances.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,34 +3,32 @@
 excluding amounts held by operational addresses.
 
 `See gateway_balances <https://xrpl.org/gateway_balances.html>`_
 """
 from dataclasses import dataclass, field
 from typing import List, Optional, Union
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class GatewayBalances(Request):
+class GatewayBalances(Request, LookupByLedgerRequest):
     """
     This request calculates the total balances issued by a given account, optionally
     excluding amounts held by operational addresses.
 
     `See gateway_balances <https://xrpl.org/gateway_balances.html>`_
     """
 
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.GATEWAY_BALANCES, init=False)
     strict: bool = False
     hotwallet: Optional[Union[str, List[str]]] = None
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/generic_request.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/generic_request.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/ledger.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ledger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 Retrieve information about the public ledger.
 `See ledger <https://xrpl.org/ledger.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Optional, Union
+from typing import Optional
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.ledger_entry import LedgerEntryType
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class Ledger(Request):
+class Ledger(Request, LookupByLedgerRequest):
     """
     Retrieve information about the public ledger.
     `See ledger <https://xrpl.org/ledger.html>`_
     """
 
     method: RequestMethod = field(default=RequestMethod.LEDGER, init=False)
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
     full: bool = False
     accounts: bool = False
     transactions: bool = False
     expand: bool = False
     owner_funds: bool = False
     binary: bool = False
     queue: bool = False
+    type: Optional[LedgerEntryType] = None
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/ledger_closed.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ledger_closed.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/ledger_current.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ledger_current.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/ledger_data.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ledger_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 The ledger_data method retrieves contents of
 the specified ledger. You can iterate through
 several calls to retrieve the entire contents
 of a single ledger version.
 `See ledger data <https://xrpl.org/ledger_data.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Any, Optional, Union
+from typing import Any, Optional
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.ledger_entry import LedgerEntryType
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class LedgerData(Request):
+class LedgerData(Request, LookupByLedgerRequest):
     """
     The ledger_data method retrieves contents of
     the specified ledger. You can iterate through
     several calls to retrieve the entire contents
     of a single ledger version.
     `See ledger data <https://xrpl.org/ledger_data.html>`_
     """
 
     method: RequestMethod = field(default=RequestMethod.LEDGER_DATA, init=False)
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
     binary: bool = False
     limit: Optional[int] = None
     # marker data shape is actually undefined in the spec, up to the
     # implementation of an individual server
     marker: Optional[Any] = None
+    type: Optional[LedgerEntryType] = None
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/manifest.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/manifest.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/nft_buy_offers.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/nft_sell_offers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
-The `nft_buy_offers` method retrieves all of buy offers
+The `nft_sell_offers` method retrieves all of sell offers
 for the specified NFToken.
 """
 from dataclasses import dataclass, field
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class NFTBuyOffers(Request):
+class NFTSellOffers(Request, LookupByLedgerRequest):
     """
-    The `nft_buy_offers` method retrieves all of buy offers
+    The `nft_sell_offers` method retrieves all of sell offers
     for the specified NFToken.
     """
 
-    method: RequestMethod = field(default=RequestMethod.NFT_BUY_OFFERS, init=False)
+    method: RequestMethod = field(default=RequestMethod.NFT_SELL_OFFERS, init=False)
     nft_id: str = REQUIRED  # type: ignore
     """
     The unique identifier of an NFToken.
-    The request returns buy offers for this NFToken. This value is required.
+    The request returns sell offers for this NFToken. This value is required.
 
     :meta hide-value:
     """
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/nft_sell_offers.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/tx.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 """
-The `nft_sell_offers` method retrieves all of sell offers
-for the specified NFToken.
+The tx method retrieves information on a single transaction.
+
+`See tx <https://xrpl.org/tx.html>`_
 """
+
 from dataclasses import dataclass, field
+from typing import Optional
 
 from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class NFTSellOffers(Request):
+class Tx(Request):
     """
-    The `nft_sell_offers` method retrieves all of sell offers
-    for the specified NFToken.
+    The tx method retrieves information on a single transaction.
+
+    `See tx <https://xrpl.org/tx.html>`_
     """
 
-    method: RequestMethod = field(default=RequestMethod.NFT_SELL_OFFERS, init=False)
-    nft_id: str = REQUIRED  # type: ignore
+    method: RequestMethod = field(default=RequestMethod.TX, init=False)
+    transaction: str = REQUIRED  # type: ignore
     """
-    The unique identifier of an NFToken.
-    The request returns sell offers for this NFToken. This value is required.
+    This field is required.
 
     :meta hide-value:
     """
+
+    binary: bool = False
+    min_ledger: Optional[int] = None
+    max_ledger: Optional[int] = None
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/no_ripple_check.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/no_ripple_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 for an account and the No Ripple flag of its trust lines, compared with the
 recommended settings.
 
 `See noripple_check <https://xrpl.org/noripple_check.html>`_
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Optional, Union
+from typing import Optional
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 class NoRippleCheckRole(str, Enum):
     """Represents the options for the address role in a NoRippleCheckRequest."""
 
     GATEWAY = "gateway"
     USER = "user"
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class NoRippleCheck(Request):
+class NoRippleCheck(Request, LookupByLedgerRequest):
     """
     This request provides a quick way to check the status of the Default Ripple field
     for an account and the No Ripple flag of its trust lines, compared with the
     recommended settings.
 
     `See noripple_check <https://xrpl.org/noripple_check.html>`_
     """
@@ -35,16 +35,14 @@
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.NO_RIPPLE_CHECK, init=False)
     role: NoRippleCheckRole = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/path_find.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/path_find.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/ping.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ping.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/random.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/random.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/request.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,16 @@
     LEDGER_CURRENT = "ledger_current"
     LEDGER_DATA = "ledger_data"
     LEDGER_ENTRY = "ledger_entry"
 
     # NFT methods
     NFT_BUY_OFFERS = "nft_buy_offers"
     NFT_SELL_OFFERS = "nft_sell_offers"
+    NFT_INFO = "nft_info"  # clio only
+    NFT_HISTORY = "nft_history"  # clio only
 
     # subscription methods
     SUBSCRIBE = "subscribe"
     UNSUBSCRIBE = "unsubscribe"
 
     # server info methods
     FEE = "fee"
@@ -69,26 +71,25 @@
     SERVER_INFO = "server_info"
     SERVER_STATE = "server_state"
 
     # utility methods
     PING = "ping"
     RANDOM = "random"
 
-    # sidechain methods
-    FEDERATOR_INFO = "federator_info"
+    # amm methods
+    AMM_INFO = "amm_info"
 
     # generic unknown/unsupported request
     # (there is no XRPL analog, this model is specific to xrpl-py)
     GENERIC_REQUEST = "zzgeneric_request"
 
 
 R = TypeVar("R", bound="Request")
 
 
-@require_kwargs_on_init
 @dataclass(frozen=True)
 class Request(BaseModel):
     """
     The base class for all network request types.
     Represents fields common to all request types.
     """
 
@@ -157,14 +158,18 @@
             return xrpl.models.requests.NoRippleCheck
         if method == RequestMethod.ACCOUNT_NFTS:
             return xrpl.models.requests.AccountNFTs
         if method == RequestMethod.NFT_BUY_OFFERS:
             return xrpl.models.requests.NFTBuyOffers
         if method == RequestMethod.NFT_SELL_OFFERS:
             return xrpl.models.requests.NFTSellOffers
+        if method == RequestMethod.NFT_INFO:
+            return xrpl.models.requests.NFTInfo
+        if method == RequestMethod.NFT_HISTORY:
+            return xrpl.models.requests.NFTHistory
 
         parsed_name = "".join([word.capitalize() for word in method.split("_")])
         if parsed_name in xrpl.models.requests.__all__:
             return cast(Type[Request], getattr(xrpl.models.requests, parsed_name))
         return xrpl.models.requests.GenericRequest
 
     def to_dict(self: Request) -> Dict[str, Any]:
@@ -173,7 +178,22 @@
 
         Returns:
             The dictionary representation of a Request.
         """
         # we need to override this because method is using ``field``
         # which will not include the value in the object's __dict__
         return {**super().to_dict(), "method": self.method.value}
+
+
+@require_kwargs_on_init
+@dataclass(frozen=True)
+class LookupByLedgerRequest:
+    """Represents requests that need specifying an instance of the ledger"""
+
+    ledger_hash: Optional[str] = None
+    """
+    A 20-byte hex string for the ledger version to use.
+    """
+    ledger_index: Optional[Union[str, int]] = None
+    """
+    The ledger index of the ledger to use, or a shortcut string.
+    """
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/ripple_path_find.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/ripple_path_find.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 updates where possible.
 
 Although the rippled server tries to find the cheapest path or
 combination of paths for making a payment, it is not guaranteed that
 the paths returned by this method are, in fact, the best paths.
 """
 from dataclasses import dataclass, field
-from typing import List, Optional, Union
+from typing import List, Optional
 
 from xrpl.models.amounts import Amount
 from xrpl.models.currencies import Currency
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class RipplePathFind(Request):
+class RipplePathFind(Request, LookupByLedgerRequest):
     """
     The ripple_path_find method is a simplified version of the
     path_find method that provides a single response with a payment
     path you can use right away. It is available in both the WebSocket
     and JSON-RPC APIs. However, the results tend to become outdated as
     time passes. Instead of making multiple calls to stay updated, you
     should instead use the path_find method to subscribe to continued
@@ -58,9 +58,7 @@
 
     :meta hide-value:
     """
 
     method: RequestMethod = field(default=RequestMethod.RIPPLE_PATH_FIND, init=False)
     send_max: Optional[Amount] = None
     source_currencies: Optional[List[Currency]] = None
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/server_info.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/server_info.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/server_state.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/server_state.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/sign.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/sign.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/sign_and_submit.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/sign_and_submit.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/sign_for.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/sign_for.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/submit.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/submit.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/submit_multisigned.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/submit_multisigned.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/submit_only.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/submit_only.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/subscribe.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/subscribe.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/transaction_entry.py` & `xrpl_py-2.1.0b0/xrpl/models/requests/transaction_entry.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,34 +5,31 @@
 
 `See transaction_entry <https://xrpl.org/transaction_entry.html>`_
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Optional, Union
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class TransactionEntry(Request):
+class TransactionEntry(Request, LookupByLedgerRequest):
     """
     The transaction_entry method retrieves information on a single transaction from a
     specific ledger version. (The tx method, by contrast, searches all ledgers for the
     specified transaction. We recommend using that method instead.)
 
     `See transaction_entry <https://xrpl.org/transaction_entry.html>`_
     """
 
     method: RequestMethod = field(default=RequestMethod.TRANSACTION_ENTRY, init=False)
-    ledger_hash: Optional[str] = None
-    ledger_index: Optional[Union[str, int]] = None
     tx_hash: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/requests/unsubscribe.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_fund.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/models/response.py` & `xrpl_py-2.1.0b0/xrpl/models/response.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/account_delete.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/account_delete.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/account_set.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/account_set.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,24 +19,26 @@
 _MIN_TICK_SIZE: Final[int] = 3
 _MAX_TICK_SIZE: Final[int] = 15
 _DISABLE_TICK_SIZE: Final[int] = 0
 
 _MAX_DOMAIN_LENGTH: Final[int] = 256
 
 
-class AccountSetFlag(int, Enum):
+class AccountSetAsfFlag(int, Enum):
     """
+    Enum for AccountSet Flags.
+
     There are several options which can be either enabled or disabled for an account.
     Account options are represented by different types of flags depending on the
     situation. The AccountSet transaction type has several "AccountSet Flags" (prefixed
     `asf`) that can enable an option when passed as the SetFlag parameter, or disable
     an option when passed as the ClearFlag parameter. This enum represents those
     options.
 
-    `See AccountSet Flags <https://xrpl.org/accountset.html#accountset-flags>`_
+    `See AccountSet asf Flags <https://xrpl.org/accountset.html#accountset-flags>`_
     """
 
     ASF_ACCOUNT_TXN_ID = 5
     """
     Track the ID of this account's most recent transaction. Required for
     `AccountTxnID <https://xrpl.org/transaction-common-fields.html#accounttxnid>`_
     """
@@ -85,48 +87,93 @@
 
     ASF_REQUIRE_DEST = 1
     """Require a destination tag to send transactions to this account."""
 
     ASF_AUTHORIZED_NFTOKEN_MINTER = 10
     """Allow another account to mint and burn tokens on behalf of this account."""
 
+    ASF_DISABLE_INCOMING_NFTOKEN_OFFER = 12
+    """Disallow other accounts from creating NFTokenOffers directed at this account."""
+
+    ASF_DISABLE_INCOMING_CHECK = 13
+    """Disallow other accounts from creating Checks directed at this account."""
+
+    ASF_DISABLE_INCOMING_PAYCHAN = 14
+    """Disallow other accounts from creating PayChannels directed at this account."""
+
+    ASF_DISABLE_INCOMING_TRUSTLINE = 15
+    """Disallow other accounts from creating Trustlines directed at this account."""
+
+
+class AccountSetFlag(int, Enum):
+    """
+    Enum for AccountSet Transaction Flags.
+
+    Transactions of the AccountSet type support additional values in the Flags field.
+    This enum represents those options.
+
+    `See AccountSet tf Flags <https://xrpl.org/accountset.html#accountset-flags>`_
+    """
+
+    TF_REQUIRE_DEST_TAG = 0x00010000
+    """
+    The same as SetFlag: asfRequireDest.
+    """
+
+    TF_OPTIONAL_DEST_TAG = 0x00020000
+    """
+    The same as ClearFlag: asfRequireDest.
+    """
+
+    TF_REQUIRE_AUTH = 0x00040000
+    """
+    The same as SetFlag: asfRequireAuth.
+    """
+
+    TF_OPTIONAL_AUTH = 0x00080000
+    """
+    The same as ClearFlag: asfRequireAuth.
+    """
+
+    TF_DISALLOW_XRP = 0x00100000
+    """
+    The same as SetFlag: asfDisallowXRP.
+    """
+
+    TF_ALLOW_XRP = 0x00200000
+    """
+    The same as ClearFlag: asfDisallowXRP.
+    """
+
 
 class AccountSetFlagInterface(FlagInterface):
     """
-    There are several options which can be either enabled or disabled for an account.
-    Account options are represented by different types of flags depending on the
-    situation. The AccountSet transaction type has several "AccountSet Flags" (prefixed
-    `asf`) that can enable an option when passed as the SetFlag parameter, or disable
-    an option when passed as the ClearFlag parameter. This TypedDict represents those
-    options.
+    Transactions of the AccountSet type support additional values in the Flags field.
+    This TypedDict represents those options.
 
-    `See AccountSet Flags <https://xrpl.org/accountset.html#accountset-flags>`_
+    `See AccountSet tf Flags <https://xrpl.org/accountset.html#accountset-flags>`_
     """
 
-    ASF_ACCOUNT_TXN_ID: bool
-    ASF_DEFAULT_RIPPLE: bool
-    ASF_DEPOSIT_AUTH: bool
-    ASF_DISABLE_MASTER: bool
-    ASF_DISALLOW_XRP: bool
-    ASF_GLOBAL_FREEZE: bool
-    ASF_NO_FREEZE: bool
-    ASF_REQUIRE_AUTH: bool
-    ASF_REQUIRE_DEST: bool
-    ASF_AUTHORIZED_NFTOKEN_MINTER: bool
+    TF_REQUIRE_DEST_TAG: bool
+    TF_OPTIONAL_DEST_TAG: bool
+    TF_REQUIRE_AUTH: bool
+    TF_OPTIONAL_AUTH: bool
+    TF_DISALLOW_XRP: bool
+    TF_ALLOW_XRP: bool
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class AccountSet(Transaction):
     """
     Represents an `AccountSet transaction <https://xrpl.org/accountset.html>`_,
     which modifies the properties of an account in the XRP Ledger.
     """
 
-    clear_flag: Optional[int] = None
+    clear_flag: Optional[AccountSetAsfFlag] = None
     """
     Disable a specific `AccountSet Flag
     <https://xrpl.org/accountset.html#accountset-flags>`_
     """
 
     domain: Optional[str] = None
     """
@@ -139,15 +186,15 @@
     Set the MD5 Hash to be used for generating an avatar image for this
     account.
     """
 
     message_key: Optional[str] = None
     """Set a public key for sending encrypted messages to this account."""
 
-    set_flag: Optional[int] = None
+    set_flag: Optional[AccountSetAsfFlag] = None
     """
     Enable a specific `AccountSet Flag
     <https://xrpl.org/accountset.html#accountset-flags>`_
     """
 
     transfer_rate: Optional[int] = None
     """
@@ -163,15 +210,15 @@
     <https://xrpl.org/ticksize.html>`_ for details.
     """
 
     nftoken_minter: Optional[str] = None
     """
     Sets an alternate account that is allowed to mint NFTokens on this
     account's behalf using NFTokenMint's `Issuer` field. If set, you must
-    also set the AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER flag.
+    also set the AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER flag.
     """
 
     transaction_type: TransactionType = field(
         default=TransactionType.ACCOUNT_SET,
         init=False,
     )
 
@@ -220,29 +267,32 @@
     def _get_clear_flag_error(self: AccountSet) -> Optional[str]:
         if self.clear_flag is not None and self.clear_flag == self.set_flag:
             return "Must not be equal to the set_flag"
         return None
 
     def _get_nftoken_minter_error(self: AccountSet) -> Optional[str]:
         if (
-            self.set_flag != AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER
+            self.set_flag != AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER
             and self.nftoken_minter is not None
         ):
             return (
                 "Will not set the minter unless "
-                "AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER is set"
+                "AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER is set"
             )
         if (
-            self.set_flag == AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER
+            self.set_flag == AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER
             and self.nftoken_minter is None
         ):
-            return "\
-                Must be present if AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER is set"
+            return (
+                "Must be present if AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER "
+                "is set"
+            )
         if (
-            self.clear_flag == AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER
+            self.clear_flag == AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER
             and self.nftoken_minter is not None
         ):
             return (
-                "Must not be present if AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER "
-                "is unset using clear_flag"
+                "Must not be present if "
+                "AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER is unset "
+                "using clear_flag"
             )
         return None
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/check_cancel.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/check_cancel.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/check_cash.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/check_cash.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/check_create.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/check_create.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/deposit_preauth.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/deposit_preauth.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_cancel.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_cancel.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_create.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_create_claim_id.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_finish.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_finish.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/metadata.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/metadata.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 """Models for a transaction's metadata."""
 
 from typing import Dict, List, Union
 
-from typing_extensions import Literal, NotRequired, TypedDict
+from typing_extensions import Literal, NotRequired, TypeAlias, TypedDict, TypeGuard
 
 from xrpl.models.amounts.amount import Amount
 
 
+class NFTokenMetadataFields(TypedDict):
+    """Model for NFToken data in metadata."""
+
+    NFTokenID: str
+    URI: str
+
+
+class NFTokenMetadata(TypedDict):
+    """Model what NFTokens look like in metadata."""
+
+    NFToken: NFTokenMetadataFields
+
+
 class Fields(TypedDict):
     """Model for possible fields."""
 
     Flags: int
     Sequence: int
     Account: NotRequired[str]
     LowLimit: NotRequired[Dict[str, str]]
     HighLimit: NotRequired[Dict[str, str]]
     Balance: NotRequired[Union[Dict[str, str], str]]
     TakerGets: NotRequired[Union[Dict[str, str], str]]
     TakerPays: NotRequired[Union[Dict[str, str], str]]
     BookDirectory: NotRequired[str]
     Expiration: NotRequired[int]
+    NFTokens: NotRequired[List[NFTokenMetadata]]
 
 
 class CreatedNodeFields(TypedDict):
     """Fields of a CreatedNode."""
 
     LedgerEntryType: str
     LedgerIndex: str
@@ -73,7 +87,49 @@
 
     AffectedNodes: List[Union[CreatedNode, ModifiedNode, DeletedNode]]
     TransactionIndex: int
     TransactionResult: str
     DeliveredAmount: NotRequired[Amount]
     # "unavailable" possible for transactions before 2014-01-20
     delivered_amount: NotRequired[Union[Amount, Literal["unavailable"]]]
+
+
+Node: TypeAlias = Union[CreatedNode, ModifiedNode, DeletedNode]
+
+
+def isCreatedNode(node: Node) -> TypeGuard[CreatedNode]:
+    """
+    Typeguard for CreatedNode
+
+    Args:
+        node: A node of any type (CreatedNode, ModifiedNode, or DeletedNode)
+
+    Returns:
+        Whether this node is a CreatedNode.
+    """
+    return "CreatedNode" in node
+
+
+def isModifiedNode(node: Node) -> TypeGuard[ModifiedNode]:
+    """
+    Typeguard for ModifiedNode
+
+    Args:
+        node: A node of any type (CreatedNode, ModifiedNode, or DeletedNode)
+
+    Returns:
+        Whether this node is a ModifiedNode.
+    """
+    return "ModifiedNode" in node
+
+
+def isDeletedNode(node: Node) -> TypeGuard[DeletedNode]:
+    """
+    Typeguard for DeletedNode
+
+    Args:
+        node: A node of any type (CreatedNode, ModifiedNode, or DeletedNode)
+
+    Returns:
+        Whether this node is a DeletedNode.
+    """
+    return "DeletedNode" in node
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_accept_offer.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_accept_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_burn.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_burn.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_cancel_offer.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_cancel_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_create_offer.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_create_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_mint.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_mint.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/offer_cancel.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/offer_cancel.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/offer_create.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/offer_create.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/payment.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/payment.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_claim.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_claim.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_create.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_create.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_fund.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_claim.py`

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

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/set_regular_key.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/set_regular_key.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/signer_list_set.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/signer_list_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,27 +93,36 @@
                 "Must have a value of zero for `signer_quorum` if the signer list is "
                 "being deleted."
             )
 
         if self.signer_entries is None:  # deletion of the SignerList object
             return errors
 
-        if self.signer_quorum <= 0:
+        if self.signer_quorum == REQUIRED:
+            errors["signer_quorum"] = "`signer_quorum` is not set."
+        elif self.signer_quorum <= 0:
+            errors["signer_quorum"] = (
+                "`signer_quorum` must be greater than or equal to 0 when not deleting "
+                "signer_list."
+            )
+
+        if not isinstance(self.signer_entries, list):
             errors[
-                "signer_quorum"
-            ] = "`signer_quorum` must be greater than or equal to 0."
+                "signer_entries"
+            ] = "`signer_entries` must be a list of `SignerEntry` objects."
+            return errors
 
         if (
             len(self.signer_entries) < 1
             or len(self.signer_entries) > MAX_SIGNER_ENTRIES
         ):
             errors["signer_entries"] = (
-                "`signer_entries` must have at least 1 member and no more than {} "
-                "members. If this transaction is deleting the SignerList, then "
-                "this parameter must be omitted.".format(MAX_SIGNER_ENTRIES)
+                "`signer_entries` must have at least 1 member and no more than "
+                f"{MAX_SIGNER_ENTRIES} members. If this transaction is deleting the "
+                "SignerList, then this parameter must be omitted."
             )
             return errors
 
         account_set = set()
         signer_weight_sum = 0
 
         for signer_entry in self.signer_entries:
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/ticket_create.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/ticket_create.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/transaction.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/transaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,35 +3,33 @@
 
 from dataclasses import dataclass
 from hashlib import sha512
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 from typing_extensions import Final
 
-from xrpl.core.binarycodec import encode
+from xrpl.core.binarycodec import decode, encode
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
@@ -251,14 +256,17 @@
 
     txn_signature: Optional[str] = None
     """
     The cryptographic signature from the sender that authorizes this
     transaction. Automatically added during signing.
     """
 
+    network_id: Optional[int] = None
+    """The network id of the transaction."""
+
     def _get_errors(self: Transaction) -> Dict[str, str]:
         errors = super()._get_errors()
         if self.ticket_sequence is not None and (
             (self.sequence is not None and self.sequence != 0)
             or self.account_txn_id is not None
         ):
             errors[
@@ -312,14 +320,23 @@
         based on the Transaction object.
 
         Returns:
             A JSON-like dictionary in the JSON format used by the binary codec.
         """
         return transaction_json_to_binary_codec_form(self.to_dict())
 
+    def blob(self: Transaction) -> str:
+        """
+        Creates the canonical binary format of the Transaction object.
+
+        Returns:
+            The binary-encoded object, as a hexadecimal string.
+        """
+        return encode(self.to_xrpl())
+
     @classmethod
     def from_dict(cls: Type[T], value: Dict[str, Any]) -> T:
         """
         Construct a new Transaction from a dictionary of parameters.
 
         Args:
             value: The value to construct the Transaction from.
@@ -367,26 +384,44 @@
             return flag in interface_to_flag_list(
                 tx_type=self.transaction_type,
                 tx_flags=self.flags,
             )
         else:  # is List[int]
             return flag in self.flags
 
+    def is_signed(self: Transaction) -> bool:
+        """
+        Checks if a transaction has been signed.
+
+        Returns:
+            Whether the transaction has been signed
+        """
+        if self.signers:
+            for signer in self.signers:
+                if (
+                    signer.signing_pub_key is None or len(signer.signing_pub_key) <= 0
+                ) or (signer.txn_signature is None or len(signer.txn_signature) <= 0):
+                    return False
+            return True
+        return (
+            self.signing_pub_key is not None and len(self.signing_pub_key) > 0
+        ) and (self.txn_signature is not None and len(self.txn_signature) > 0)
+
     def get_hash(self: Transaction) -> str:
         """
         Hashes the Transaction object as the ledger does. Only valid for signed
         Transaction objects.
 
         Returns:
             The hash of the Transaction object.
 
         Raises:
             XRPLModelException: if the Transaction is unsigned.
         """
-        if self.txn_signature is None:
+        if self.txn_signature is None and self.signers is None:
             raise XRPLModelException(
                 "Cannot get the hash from an unsigned Transaction."
             )
         prefix = hex(_TRANSACTION_HASH_PREFIX)[2:].upper()
         encoded_str = bytes.fromhex(prefix + encode(self.to_xrpl()))
         return sha512(encoded_str).digest().hex().upper()[:64]
 
@@ -420,7 +455,20 @@
             t.value: getattr(pseudo_transaction_models, t)
             for t in transaction_models.types.PseudoTransactionType
         }
         if transaction_type in pseudo_transaction_types:
             return pseudo_transaction_types[transaction_type]
 
         raise XRPLModelException(f"{transaction_type} is not a valid Transaction type")
+
+    @staticmethod
+    def from_blob(tx_blob: str) -> Transaction:
+        """
+        Decodes a transaction blob.
+
+        Args:
+            tx_blob: the tx blob to decode.
+
+        Returns:
+            The formatted transaction.
+        """
+        return Transaction.from_xrpl(decode(tx_blob))
```

### Comparing `xrpl-py-2.0.0b0/xrpl/models/transactions/trust_set.py` & `xrpl_py-2.1.0b0/xrpl/models/transactions/trust_set.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/types.py` & `xrpl_py-2.1.0b0/xrpl/models/types.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/models/utils.py` & `xrpl_py-2.1.0b0/xrpl/models/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Helper util functions for the models module."""
 
 from dataclasses import is_dataclass
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, cast
 
 from xrpl.models.exceptions import XRPLModelException
 
 # Code source for requiring kwargs:
 # https://gist.github.com/mikeholler/4be180627d3f8fceb55704b729464adb
 
 _T = TypeVar("_T")
@@ -58,8 +58,8 @@
                 f"Found the following positional arguments: {args}"
             )
         original_init(self, **kwargs)
 
     # noinspection PyTypeHints
     cls.__init__ = new_init  # type: ignore
 
-    return cls
+    return cast(Type[_T], cls)
```

### Comparing `xrpl-py-2.0.0b0/xrpl/transaction/main.py` & `xrpl_py-2.1.0b0/xrpl/transaction/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,155 +1,132 @@
 """High-level transaction methods with XRPL transactions."""
 import asyncio
+from typing import Optional
 
 from xrpl.asyncio.transaction import main
 from xrpl.clients.sync_client import SyncClient
 from xrpl.models.response import Response
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.wallet.main import Wallet
 
 
 def sign_and_submit(
     transaction: Transaction,
-    wallet: Wallet,
     client: SyncClient,
+    wallet: Wallet,
     autofill: bool = True,
     check_fee: bool = True,
 ) -> Response:
     """
     Signs a transaction (locally, without trusting external rippled nodes) and submits
     it to the XRPL.
 
     Args:
         transaction: the transaction to be signed and submitted.
-        wallet: the wallet with which to sign the transaction.
         client: the network client with which to submit the transaction.
+        wallet: the wallet with which to sign the transaction.
         autofill: whether to autofill the relevant fields. Defaults to True.
         check_fee: whether to check if the fee is higher than the expected transaction
             type fee. Defaults to True.
 
     Returns:
         The response from the ledger.
     """
     return asyncio.run(
         main.sign_and_submit(
             transaction,
-            wallet,
             client,
+            wallet,
             autofill,
             check_fee,
         )
     )
 
 
-safe_sign_and_submit_transaction = sign_and_submit
-
-
 def submit(
     transaction: Transaction,
     client: SyncClient,
+    *,
+    fail_hard: bool = False,
 ) -> Response:
     """
     Submits a transaction to the ledger.
 
     Args:
         transaction: the Transaction to be submitted.
         client: the network client with which to submit the transaction.
+        fail_hard: an optional boolean. If True, and the transaction fails for
+            the initial server, do not retry or relay the transaction to other
+            servers. Defaults to False.
 
     Returns:
         The response from the ledger.
 
     Raises:
         XRPLRequestFailureException: if the rippled API call fails.
     """
     return asyncio.run(
         main.submit(
             transaction,
             client,
+            fail_hard=fail_hard,
         )
     )
 
 
-submit_transaction = submit
-
-
-def sign(
-    transaction: Transaction,
-    wallet: Wallet,
-    check_fee: bool = True,
-) -> Transaction:
-    """
-    Signs a transaction locally, without trusting external rippled nodes.
-
-    Args:
-        transaction: the transaction to be signed.
-        wallet: the wallet with which to sign the transaction.
-        check_fee: whether to check if the fee is higher than the expected transaction
-            type fee. Defaults to True.
-
-    Returns:
-        The signed transaction.
-    """
-    return asyncio.run(
-        main.sign(
-            transaction,
-            wallet,
-            check_fee,
-        )
-    )
-
-
-safe_sign_transaction = sign
+sign = main.sign
 
 
 def autofill_and_sign(
     transaction: Transaction,
-    wallet: Wallet,
     client: SyncClient,
+    wallet: Wallet,
     check_fee: bool = True,
 ) -> Transaction:
     """
     Signs a transaction locally, without trusting external rippled nodes. Autofills
     relevant fields.
 
     Args:
         transaction: the transaction to be signed.
-        wallet: the wallet with which to sign the transaction.
         client: a network client.
+        wallet: the wallet with which to sign the transaction.
         check_fee: whether to check if the fee is higher than the expected transaction
             type fee. Defaults to True.
 
     Returns:
         The signed transaction.
     """
     return asyncio.run(
         main.autofill_and_sign(
             transaction,
-            wallet,
             client,
+            wallet,
             check_fee,
         )
     )
 
 
-safe_sign_and_autofill_transaction = autofill_and_sign
-
-
-def autofill(transaction: Transaction, client: SyncClient) -> Transaction:
+def autofill(
+    transaction: Transaction, client: SyncClient, signers_count: Optional[int] = None
+) -> Transaction:
     """
     Autofills fields in a transaction. This will set `sequence`, `fee`, and
     `last_ledger_sequence` according to the current state of the server this Client is
     connected to. It also converts all X-Addresses to classic addresses.
 
     Args:
         transaction: the transaction to be signed.
         client: a network client.
+        signers_count: the expected number of signers for this transaction.
+            Only used for multisigned transactions.
 
     Returns:
         The autofilled transaction.
     """
     return asyncio.run(
         main.autofill(
             transaction,
             client,
+            signers_count,
         )
     )
```

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/__init__.py` & `xrpl_py-2.1.0b0/xrpl/utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Convenience utilities for the XRP Ledger"""
 
-from xrpl.utils.sidechain import create_cross_chain_payment
 from xrpl.utils.str_conversions import hex_to_str, str_to_hex
 from xrpl.utils.time_conversions import (
     XRPLTimeRangeException,
     datetime_to_ripple_time,
     posix_to_ripple_time,
     ripple_time_to_datetime,
     ripple_time_to_posix,
@@ -23,12 +22,11 @@
     "drops_to_xrp",
     "ripple_time_to_datetime",
     "datetime_to_ripple_time",
     "ripple_time_to_posix",
     "posix_to_ripple_time",
     "XRPRangeException",
     "XRPLTimeRangeException",
-    "create_cross_chain_payment",
     "get_balance_changes",
     "get_final_balances",
     "get_order_book_changes",
 ]
```

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/parse_nftoken_id.py` & `xrpl_py-2.1.0b0/xrpl/utils/parse_nftoken_id.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/str_conversions.py` & `xrpl_py-2.1.0b0/xrpl/utils/str_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/time_conversions.py` & `xrpl_py-2.1.0b0/xrpl/utils/time_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_balance_changes.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_balance_changes.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_final_balances.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_final_balances.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_order_book_changes.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_order_book_changes.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/__init__.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/balance_parser.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/balance_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/nodes.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/nodes.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/parser.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/parser.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/types.py` & `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/types.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/utils/xrp_conversions.py` & `xrpl_py-2.1.0b0/xrpl/utils/xrp_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-2.0.0b0/xrpl/wallet/main.py` & `xrpl_py-2.1.0b0/xrpl/wallet/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,69 +13,92 @@
     """
     The cryptographic keys needed to control an XRP Ledger account. See
     `Cryptographic Keys <https://xrpl.org/cryptographic-keys.html>`_ for
     details.
     """
 
     @property
-    def classic_address(self: Wallet) -> str:
+    def address(self: Wallet) -> str:
         """
-        The address that publicly identifies this wallet,
-        as a base58 string.
+        The XRPL address that publicly identifies this wallet,
+        as a base58 string. This is the same value as the `classic_address`.
         """  # noqa: DAR201
-        return self._classic_address
+        return self._address
 
-    address = classic_address
-    """
-    The address that publicly identifies this wallet, as a base58 string.
-    """
+    # TODO: Just alias classic_address once mypy has resolved this issue:
+    #       https://github.com/python/mypy/issues/6700
+    @property
+    def classic_address(self: Wallet) -> str:
+        """
+        `classic_address` is the same as `address`. It is called `classic_address` to
+        differentiate it from the x-address standard, which encodes the network,
+        destination tag, and XRPL address into a single value.
+        It's also a base58 string.
+        """  # noqa: DAR201
+        return self._address
 
     def __init__(
         self: Wallet,
         public_key: str,
         private_key: str,
         *,
         master_address: Optional[str] = None,
         seed: Optional[str] = None,
+        algorithm: Optional[CryptoAlgorithm] = None,
     ) -> None:
         """
         Generate a new Wallet.
 
         Args:
             public_key: The public key for the account.
             private_key: The private key used for signing transactions for the account.
             master_address: Include if a Wallet uses a Regular Key Pair. This sets the
                 address that this wallet corresponds to. The default is `None`.
             seed: The seed used to derive the account keys. The default is `None`.
+            algorithm: The algorithm used to encode the keys. Inferred from the seed if
+                not included
+        """
+        self.seed = seed
+        """
+        The core value that is used to derive all other information about
+        this wallet. MUST be kept secret!
         """
+
+        if algorithm is None:
+            if seed is not None and seed.startswith("sEd"):
+                wallet_algorithm = CryptoAlgorithm.ED25519
+            else:
+                wallet_algorithm = CryptoAlgorithm.SECP256K1
+        else:
+            wallet_algorithm = algorithm
+
+        self.algorithm = wallet_algorithm
+        """
+        The algorithm that is used to convert the seed into its public/private keypair.
+        """
+
         self.public_key = public_key
         """
         The public key that is used to identify this wallet's signatures, as
         a hexadecimal string.
         """
 
         self.private_key = private_key
         """
         The private key that is used to create signatures, as a hexadecimal
         string. MUST be kept secret!
         """
 
-        self._classic_address = (
+        self._address = (
             ensure_classic_address(master_address)
             if master_address is not None
             else derive_classic_address(self.public_key)
         )
         """Internal variable for classic_address. Use classic_address instead."""
 
-        self.seed = seed
-        """
-        The core value that is used to derive all other information about
-        this wallet. MUST be kept secret!
-        """
-
     @classmethod
     def create(
         cls: Type[Wallet], algorithm: CryptoAlgorithm = CryptoAlgorithm.ED25519
     ) -> Wallet:
         """
         Generates a new seed and Wallet.
 
@@ -107,15 +130,21 @@
             algorithm: The key-generation algorithm to use when generating the seed.
                 The default is `ED25519`.
 
         Returns:
             The wallet that is generated from the given secret.
         """
         public_key, private_key = derive_keypair(seed, algorithm=algorithm)
-        return cls(public_key, private_key, master_address=master_address, seed=seed)
+        return cls(
+            public_key,
+            private_key,
+            master_address=master_address,
+            seed=seed,
+            algorithm=algorithm,
+        )
 
     from_secret = from_seed
 
     @classmethod
     def from_entropy(
         cls: Type[Wallet],
         entropy: str,
@@ -218,23 +247,23 @@
             tag: The destination tag of the address. Defaults to `None`.
             is_test: Whether the address corresponds to an address on the test network.
                 Defaults to `False`.
 
         Returns:
             The X-Address of the Wallet's account.
         """
-        return classic_address_to_xaddress(self.classic_address, tag, is_test)
+        return classic_address_to_xaddress(self.address, tag, is_test)
 
     def __str__(self: Wallet) -> str:
         """
         Returns a string representation of a Wallet.
 
         Returns:
             A string representation of a Wallet.
         """
         return "\n".join(
             [
                 f"public_key: {self.public_key}",
                 "private_key: -HIDDEN-",
-                f"classic_address: {self.classic_address}",
+                f"classic_address: {self.address}",
             ]
         )
```

### Comparing `xrpl-py-2.0.0b0/xrpl/wallet/wallet_generation.py` & `xrpl_py-2.1.0b0/xrpl/wallet/wallet_generation.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,29 +8,35 @@
 
 
 def generate_faucet_wallet(
     client: SyncClient,
     wallet: Optional[Wallet] = None,
     debug: bool = False,
     faucet_host: Optional[str] = None,
+    usage_context: Optional[str] = None,
 ) -> Wallet:
     """
     Generates a random wallet and funds it using the XRPL Testnet Faucet.
 
     Args:
         client: the network client used to make network calls.
         wallet: the wallet to fund. If omitted or `None`, a new wallet is created.
         debug: Whether to print debug information as it creates the wallet.
         faucet_host: A custom host to use for funding a wallet. In environments other
             than devnet and testnet, this parameter is required.
+        usage_context: The intended use case for the funding request
+            (for example, testing). This information will be included in json body
+            of the HTTP request to the faucet.
 
     Returns:
         A Wallet on the testnet that contains some amount of XRP.
 
     Raises:
         XRPLFaucetException: if an address could not be funded with the faucet.
         XRPLRequestFailureException: if a request to the ledger fails.
         requests.exceptions.HTTPError: if the request to the faucet fails.
 
     .. # noqa: DAR402 exception raised in private method
     """
-    return asyncio.run(async_generate_faucet_wallet(client, wallet, debug, faucet_host))
+    return asyncio.run(
+        async_generate_faucet_wallet(client, wallet, debug, faucet_host, usage_context)
+    )
```

### Comparing `xrpl-py-2.0.0b0/setup.py` & `xrpl_py-2.1.0b0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,384 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
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
- 'httpx>=0.18.1,<0.24.0',
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
-    'version': '2.0.0b0',
-    'description': 'A complete Python library for interacting with the XRP ledger',
-    'long_description': '[![Documentation Status](https://readthedocs.org/projects/xrpl-py/badge)](https://xrpl-py.readthedocs.io/)\n\n# xrpl-py\n\nA pure Python implementation for interacting with the XRP Ledger, the `xrpl-py` library simplifies the hardest parts of XRP Ledger interaction, like serialization and transaction signing, by providing native Python methods and models for [XRP Ledger transactions](https://xrpl.org/transaction-formats.html) and core server [API](https://xrpl.org/api-conventions.html) ([`rippled`](https://github.com/ripple/rippled)) objects.\n\n\n\n```py\n# create a network client\nfrom xrpl.clients import JsonRpcClient\nclient = JsonRpcClient("https://s.altnet.rippletest.net:51234")\n\n# create a wallet on the testnet\nfrom xrpl.wallet import generate_faucet_wallet\ntest_wallet = generate_faucet_wallet(client)\nprint(test_wallet)\npublic_key: ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56\nprivate_key: -HIDDEN-\nclassic_address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo\n\n# look up account info\nfrom xrpl.models.requests.account_info import AccountInfo\nacct_info = AccountInfo(\n    account="rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",\n    ledger_index="current",\n    queue=True,\n    strict=True,\n)\nresponse = client.request(acct_info)\nresult = response.result\nimport json\nprint(json.dumps(result["account_data"], indent=4, sort_keys=True))\n# {\n#     "Account": "rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",\n#     "Balance": "1000000000",\n#     "Flags": 0,\n#     "LedgerEntryType": "AccountRoot",\n#     "OwnerCount": 0,\n#     "PreviousTxnID": "73CD4A37537A992270AAC8472F6681F44E400CBDE04EC8983C34B519F56AB107",\n#     "PreviousTxnLgrSeq": 16233962,\n#     "Sequence": 16233962,\n#     "index": "FD66EC588B52712DCE74831DCB08B24157DC3198C29A0116AA64D310A58512D7"\n# }\n```\n\n[![Downloads](https://pepy.tech/badge/xrpl-py/month)](https://pepy.tech/project/xrpl-py/month)\n[![Contributors](https://img.shields.io/github/contributors/xpring-eng/xrpl-py.svg)](https://github.com/xpring-eng/xrpl-py/graphs/contributors)\n\n## Installation and supported versions\n\nThe `xrpl-py` library is available on [PyPI](https://pypi.org/). Install with `pip`:\n\n\n```\npip3 install xrpl-py\n```\n\nThe library supports [Python 3.7](https://www.python.org/downloads/) and later.\n\n[![Supported Versions](https://img.shields.io/pypi/pyversions/xrpl-py.svg)](https://pypi.org/project/xrpl-py)\n\n\n## Features\n\nUse `xrpl-py` to build Python applications that leverage the [XRP Ledger](https://xrpl.org/). The library helps with all aspects of interacting with the XRP Ledger, including:\n\n* Key and wallet management\n* Serialization\n* Transaction Signing\n\n`xrpl-py` also provides:\n\n* A network client — See [`xrpl.clients`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.clients.html) for more information.\n* Methods for inspecting accounts — See [XRPL Account Methods](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.account.html) for more information.\n* Codecs for encoding and decoding addresses and other objects — See [Core Codecs](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.html) for more information.\n\n## [➡️ Reference Documentation](https://xrpl-py.readthedocs.io/en/stable/)\n\nSee the complete [`xrpl-py` reference documentation on Read the Docs](https://xrpl-py.readthedocs.io/en/stable/index.html).\n\n\n## Usage\n\nThe following sections describe some of the most commonly used modules in the `xrpl-py` library and provide sample code.\n\n### Network client\n\nUse the `xrpl.clients` library to create a network client for connecting to the XRP Ledger.\n\n```py\nfrom xrpl.clients import JsonRpcClient\nJSON_RPC_URL = "https://s.altnet.rippletest.net:51234"\nclient = JsonRpcClient(JSON_RPC_URL)\n```\n\n### Manage keys and wallets\n\n#### `xrpl.wallet`\n\nUse the [`xrpl.wallet`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.wallet.html) module to create a wallet from a given seed or or via a [Testnet faucet](https://xrpl.org/xrp-testnet-faucet.html).\n\nTo create a wallet from a seed (in this case, the value generated using [`xrpl.keypairs`](#xrpl-keypairs)):\n\n```py\nwallet_from_seed = xrpl.wallet.Wallet(seed, 0)\nprint(wallet_from_seed)\n# pub_key: ED46949E414A3D6D758D347BAEC9340DC78F7397FEE893132AAF5D56E4D7DE77B0\n# priv_key: -HIDDEN-\n# classic_address: rG5ZvYsK5BPi9f1Nb8mhFGDTNMJhEhufn6\n```\n\nTo create a wallet from a Testnet faucet:\n\n```py\ntest_wallet = generate_faucet_wallet(client)\ntest_account = test_wallet.classic_address\nprint("Classic address:", test_account)\n# Classic address: rEQB2hhp3rg7sHj6L8YyR4GG47Cb7pfcuw\n```\n\n#### `xrpl.core.keypairs`\n\nUse the [`xrpl.core.keypairs`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html#module-xrpl.core.keypairs) module to generate seeds and derive keypairs and addresses from those seed values.\n\nHere\'s an example of how to generate a `seed` value and derive an [XRP Ledger "classic" address](https://xrpl.org/cryptographic-keys.html#account-id-and-address) from that seed.\n\n\n```py\nfrom xrpl.core import keypairs\nseed = keypairs.generate_seed()\npublic, private = keypairs.derive_keypair(seed)\ntest_account = keypairs.derive_classic_address(public)\nprint("Here\'s the public key:")\nprint(public)\nprint("Here\'s the private key:")\nprint(private)\nprint("Store this in a secure place!")\n# Here\'s the public key:\n# ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56\n# Here\'s the private key:\n# EDE65EE7882847EF5345A43BFB8E6F5EEC60F45461696C384639B99B26AAA7A5CD\n# Store this in a secure place!\n```\n\n**Note:** You can use `xrpl.core.keypairs.sign` to sign transactions but `xrpl-py` also provides explicit methods for safely signing and submitting transactions. See [Transaction Signing](#transaction-signing) and [XRPL Transaction Methods](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#module-xrpl.transaction) for more information.\n\n\n### Serialize and sign transactions\n\nTo securely submit transactions to the XRP Ledger, you need to first serialize data from JSON and other formats into the [XRP Ledger\'s canonical format](https://xrpl.org/serialization.html), then to [authorize the transaction](https://xrpl.org/transaction-basics.html#authorizing-transactions) by digitally [signing it](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html?highlight=sign#xrpl.core.keypairs.sign) with the account\'s private key. The `xrpl-py` library provides several methods to simplify this process.\n\n\nUse the [`xrpl.transaction`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html) module to sign and submit transactions. The module offers three ways to do this:\n\n* [`sign_and_submit`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign_and_submit) — Signs a transaction locally, then submits it to the XRP Ledger. This method does not implement [reliable transaction submission](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission) best practices, so only use it for development or testing purposes.\n\n* [`sign`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign) — Signs a transaction locally. This method **does  not** submit the transaction to the XRP Ledger.\n\n* [`send_reliable_submission`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.send_reliable_submission) — An implementation of the [reliable transaction submission guidelines](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission), this method submits a signed transaction to the XRP Ledger and then verifies that it has been included in a validated ledger (or has failed to do so). Use this method to submit transactions for production purposes.\n\n\n```py\nfrom xrpl.models.transactions import Payment\nfrom xrpl.transaction import sign, send_reliable_submission\nfrom xrpl.ledger import get_latest_validated_ledger_sequence\nfrom xrpl.account import get_next_valid_seq_number\n\ncurrent_validated_ledger = get_latest_validated_ledger_sequence(client)\n\n# prepare the transaction\n# the amount is expressed in drops, not XRP\n# see https://xrpl.org/basic-data-types.html#specifying-currency-amounts\nmy_tx_payment = Payment(\n    account=test_wallet.classic_address,\n    amount="2200000",\n    destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",\n    last_ledger_sequence=current_validated_ledger + 20,\n    sequence=get_next_valid_seq_number(test_wallet.classic_address, client),\n    fee="10",\n)\n# sign the transaction\nmy_tx_payment_signed = sign(my_tx_payment,test_wallet)\n\n# submit the transaction\ntx_response = send_reliable_submission(my_tx_payment_signed, client)\n```\n\n#### Get fee from the XRP Ledger\n\n\nIn most cases, you can specify the minimum [transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) of `"10"` for the `fee` field unless you have a strong reason not to. But if you want to get the [current load-balanced transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) from the network, you can use the `get_fee` function:\n\n```py\nfrom xrpl.ledger import get_fee\nfee = get_fee(client)\nprint(fee)\n# 10\n```\n\n#### Auto-filled fields\n\nThe `xrpl-py` library automatically populates the `fee`, `sequence` and `last_ledger_sequence` fields when you create transactions. In the example above, you could omit those fields and let the library fill them in for you.\n\n```py\nfrom xrpl.models.transactions import Payment\nfrom xrpl.transaction import send_reliable_submission, autofill_and_sign\n# prepare the transaction\n# the amount is expressed in drops, not XRP\n# see https://xrpl.org/basic-data-types.html#specifying-currency-amounts\nmy_tx_payment = Payment(\n    account=test_wallet.classic_address,\n    amount="2200000",\n    destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe"\n)\n\n# sign the transaction with the autofill method\n# (this will auto-populate the fee, sequence, and last_ledger_sequence)\nmy_tx_payment_signed = autofill_and_sign(my_tx_payment, test_wallet, client)\nprint(my_tx_payment_signed)\n# Payment(\n#     account=\'rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz\',\n#     transaction_type=<TransactionType.PAYMENT: \'Payment\'>,\n#     fee=\'10\',\n#     sequence=16034065,\n#     account_txn_id=None,\n#     flags=0,\n#     last_ledger_sequence=10268600,\n#     memos=None,\n#     signers=None,\n#     source_tag=None,\n#     signing_pub_key=\'EDD9540FA398915F0BCBD6E65579C03BE5424836CB68B7EB1D6573F2382156B444\',\n#     txn_signature=\'938FB22AE7FE76CF26FD11F8F97668E175DFAABD2977BCA397233117E7E1C4A1E39681091CC4D6DF21403682803AB54CC21DC4FA2F6848811DEE10FFEF74D809\',\n#     amount=\'2200000\',\n#     destination=\'rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe\',\n#     destination_tag=None,\n#     invoice_id=None,\n#     paths=None,\n#     send_max=None,\n#     deliver_min=None\n# )\n\n# submit the transaction\ntx_response = send_reliable_submission(my_tx_payment_signed, client)\n```\n\n\n### Subscribe to ledger updates\n\nYou can send `subscribe` and `unsubscribe` requests only using the WebSocket network client. These request methods allow you to be alerted of certain situations as they occur, such as when a new ledger is declared.\n\n```py\nfrom xrpl.clients import WebsocketClient\nurl = "wss://s.altnet.rippletest.net/"\nfrom xrpl.models.requests import Subscribe, StreamParameter\nreq = Subscribe(streams=[StreamParameter.LEDGER])\n# NOTE: this code will run forever without a timeout, until the process is killed\nwith WebsocketClient(url) as client:\n    client.send(req)\n    for message in client:\n        print(message)\n# {\'result\': {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'7CD50477F23FF158B430772D8E82A961376A7B40E13C695AA849811EDF66C5C0\', \'ledger_index\': 18183504, \'ledger_time\': 676412962, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'validated_ledgers\': \'17469391-18183504\'}, \'status\': \'success\', \'type\': \'response\'}\n# {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'BAA743DABD168BD434804416C8087B7BDEF7E6D7EAD412B9102281DD83B10D00\', \'ledger_index\': 18183505, \'ledger_time\': 676412970, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'txn_count\': 0, \'type\': \'ledgerClosed\', \'validated_ledgers\': \'17469391-18183505\'}\n# {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'D8227DAF8F745AE3F907B251D40B4081E019D013ABC23B68C0B1431DBADA1A46\', \'ledger_index\': 18183506, \'ledger_time\': 676412971, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'txn_count\': 0, \'type\': \'ledgerClosed\', \'validated_ledgers\': \'17469391-18183506\'}\n# {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'CFC412B6DDB9A402662832A781C23F0F2E842EAE6CFC539FEEB287318092C0DE\', \'ledger_index\': 18183507, \'ledger_time\': 676412972, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'txn_count\': 0, \'type\': \'ledgerClosed\', \'validated_ledgers\': \'17469391-18183507\'}\n```\n\n\n### Asynchronous Code\n\nThis library supports Python\'s [`asyncio`](https://docs.python.org/3/library/asyncio.html) package, which is used to run asynchronous code. All the async code is in [`xrpl.asyncio`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.asyncio.html) If you are writing asynchronous code, please note that you will not be able to use any synchronous sugar functions, due to how event loops are handled. However, every synchronous method has a corresponding asynchronous method that you can use.\n\nThis sample code is the asynchronous equivalent of the above section on submitting a transaction.\n\n```py\nimport asyncio\nfrom xrpl.models.transactions import Payment\nfrom xrpl.asyncio.transaction import sign, send_reliable_submission\nfrom xrpl.asyncio.ledger import get_latest_validated_ledger_sequence\nfrom xrpl.asyncio.account import get_next_valid_seq_number\nfrom xrpl.asyncio.clients import AsyncJsonRpcClient\n\nasync_client = AsyncJsonRpcClient(JSON_RPC_URL)\n\nasync def submit_sample_transaction():\n    current_validated_ledger = await get_latest_validated_ledger_sequence(async_client)\n\n    # prepare the transaction\n    # the amount is expressed in drops, not XRP\n    # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts\n    my_tx_payment = Payment(\n        account=test_wallet.classic_address,\n        amount="2200000",\n        destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",\n        last_ledger_sequence=current_validated_ledger + 20,\n        sequence=await get_next_valid_seq_number(test_wallet.classic_address, async_client),\n        fee="10",\n    )\n    # sign the transaction\n    my_tx_payment_signed = await sign(my_tx_payment,test_wallet)\n\n    # submit the transaction\n    tx_response = await send_reliable_submission(my_tx_payment_signed, async_client)\n\nasyncio.run(submit_sample_transaction())\n```\n\n### Encode addresses\n\nUse [`xrpl.core.addresscodec`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.addresscodec.html) to encode and decode addresses into and from the ["classic" and X-address formats](https://xrpl.org/accounts.html#addresses).\n\n```py\n# convert classic address to x-address\nfrom xrpl.core import addresscodec\ntestnet_xaddress = (\n    addresscodec.classic_address_to_xaddress(\n        "rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz",\n        tag=0,\n        is_test_network=True,\n    )\n)\nprint(testnet_xaddress)\n# T7QDemmxnuN7a52A62nx2fxGPWcRahLCf3qaswfrsNW9Lps\n```\n\n\n## Contributing\n\nIf you want to contribute to this project, see [CONTRIBUTING.md].\n\n### Mailing Lists\n\nWe have a low-traffic mailing list for announcements of new `xrpl.js` releases. (About 1 email per week)\n\n+ [Subscribe to xrpl-announce](https://groups.google.com/g/xrpl-announce)\n\nIf you\'re using the XRP Ledger in production, you should run a [rippled server](https://github.com/ripple/rippled) and subscribe to the ripple-server mailing list as well.\n\n+ [Subscribe to ripple-server](https://groups.google.com/g/ripple-server)\n\n### Report an issue\n\nExperienced an issue? Report it [here](https://github.com/XRPLF/xrpl-py/issues/new).\n\n## License\n\nThe `xrpl-py` library is licensed under the ISC License. See [LICENSE] for more information.\n\n\n\n[CONTRIBUTING.md]: CONTRIBUTING.md\n[LICENSE]: LICENSE\n',
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
+[![Documentation Status](https://readthedocs.org/projects/xrpl-py/badge)](https://xrpl-py.readthedocs.io/)
 
+# xrpl-py
+
+A pure Python implementation for interacting with the XRP Ledger, the `xrpl-py` library simplifies the hardest parts of XRP Ledger interaction, like serialization and transaction signing, by providing native Python methods and models for [XRP Ledger transactions](https://xrpl.org/transaction-formats.html) and core server [API](https://xrpl.org/api-conventions.html) ([`rippled`](https://github.com/ripple/rippled)) objects.
+
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
 
-setup(**setup_kwargs)
```

