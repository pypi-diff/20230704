# Comparing `tmp/nibiru_proto-0.21.3b5.tar.gz` & `tmp/nibiru_proto-0.21.3b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nibiru_proto-0.21.3b5.tar", max compression
+gzip compressed data, was "nibiru_proto-0.21.3b7.tar", max compression
```

## Comparing `nibiru_proto-0.21.3b5.tar` & `nibiru_proto-0.21.3b7.tar`

### file list

```diff
@@ -1,544 +1,544 @@
--rw-r--r--   0        0        0     1069 2022-08-17 01:57:49.915436 nibiru_proto-0.21.3b5/LICENSE
--rw-r--r--   0        0        0       84 2023-07-03 23:42:13.832772 nibiru_proto-0.21.3b5/nibiru_proto/__init__.py
--rw-r--r--   0        0        0     2028 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/amino/amino_pb2.py
--rw-r--r--   0        0        0     3227 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/amino/amino_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/amino/amino_pb2_grpc.py
--rw-r--r--   0        0        0     2012 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.py
--rw-r--r--   0        0        0     4237 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1817 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/config_pb2.py
--rw-r--r--   0        0        0     5300 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/config_pb2_grpc.py
--rw-r--r--   0        0        0     1968 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/module_pb2.py
--rw-r--r--   0        0        0     6817 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1539 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/query_pb2.py
--rw-r--r--   0        0        0     1426 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/query_pb2.pyi
--rw-r--r--   0        0        0     2603 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1794 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/module/v1/module_pb2.py
--rw-r--r--   0        0        0     2675 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     4605 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.py
--rw-r--r--   0        0        0     5282 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/auth_pb2_grpc.py
--rw-r--r--   0        0        0     1899 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1555 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    12503 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    14414 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    19125 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2810 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1842 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2743 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1295 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/module/v1/module_pb2.py
--rw-r--r--   0        0        0      578 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     4039 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     4440 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0     2402 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/event_pb2.py
--rw-r--r--   0        0        0     2114 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/event_pb2_grpc.py
--rw-r--r--   0        0        0     1717 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1194 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     5558 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     7628 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6331 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     5129 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     4700 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     6246 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     4201 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/autocli/v1/options_pb2.py
--rw-r--r--   0        0        0    12271 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/autocli/v1/options_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/autocli/v1/options_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/autocli/v1/query_pb2.py
--rw-r--r--   0        0        0     2362 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/autocli/v1/query_pb2.pyi
--rw-r--r--   0        0        0     2886 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/autocli/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1439 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1637 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2480 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     1703 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0     6001 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.py
--rw-r--r--   0        0        0     8210 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/bank_pb2_grpc.py
--rw-r--r--   0        0        0     4070 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     3902 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    16803 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    23149 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    21828 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     6511 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     6731 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     8074 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     7125 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.py
--rw-r--r--   0        0        0    13374 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.py
--rw-r--r--   0        0        0     1570 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.py
--rw-r--r--   0        0        0     1558 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.py
--rw-r--r--   0        0        0     1868 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     1213 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     2762 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/node/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1598 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.py
--rw-r--r--   0        0        0     3440 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.py
--rw-r--r--   0        0        0     3071 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.py
--rw-r--r--   0        0        0     3055 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi
--rw-r--r--   0        0        0     5144 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0    10963 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py
--rw-r--r--   0        0        0    23085 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi
--rw-r--r--   0        0        0    13573 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0     4501 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py
--rw-r--r--   0        0        0     8467 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.py
--rw-r--r--   0        0        0     2626 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.py
--rw-r--r--   0        0        0     3087 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.py
--rw-r--r--   0        0        0     2508 2023-07-03 23:42:19.047520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.py
--rw-r--r--   0        0        0     5092 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2_grpc.py
--rw-r--r--   0        0        0    11465 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    18881 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    14492 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4471 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.py
--rw-r--r--   0        0        0     5547 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2_grpc.py
--rw-r--r--   0        0        0     3165 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/v1beta1/coin_pb2.py
--rw-r--r--   0        0        0     2703 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/v1beta1/coin_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/v1beta1/coin_pb2_grpc.py
--rw-r--r--   0        0        0     1383 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1020 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2171 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.py
--rw-r--r--   0        0        0     2304 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/v1beta1/capability_pb2_grpc.py
--rw-r--r--   0        0        0     2274 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2428 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1370 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/module/v1/module_pb2.py
--rw-r--r--   0        0        0      925 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2013 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/v1/query_pb2.py
--rw-r--r--   0        0        0     1699 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/v1/query_pb2.pyi
--rw-r--r--   0        0        0     2626 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2441 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/v1/tx_pb2.py
--rw-r--r--   0        0        0     2431 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     2734 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1447 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1178 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1727 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1192 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3940 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     3256 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4533 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2264 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.py
--rw-r--r--   0        0        0     1690 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/ed25519/keys_pb2_grpc.py
--rw-r--r--   0        0        0     1796 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.py
--rw-r--r--   0        0        0     1822 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2_grpc.py
--rw-r--r--   0        0        0     2566 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.py
--rw-r--r--   0        0        0     4311 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2_grpc.py
--rw-r--r--   0        0        0     2088 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/multisig/keys_pb2.py
--rw-r--r--   0        0        0     1351 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/multisig/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/multisig/keys_pb2_grpc.py
--rw-r--r--   0        0        0     1778 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py
--rw-r--r--   0        0        0     2062 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.py
--rw-r--r--   0        0        0     1893 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.py
--rw-r--r--   0        0        0     1519 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2_grpc.py
--rw-r--r--   0        0        0     1829 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.py
--rw-r--r--   0        0        0     1523 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2_grpc.py
--rw-r--r--   0        0        0     1481 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1108 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0    10924 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.py
--rw-r--r--   0        0        0    13195 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.py
--rw-r--r--   0        0        0    13143 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0    13975 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    19296 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    18475 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    20401 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0    10831 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     9210 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0    12766 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1316 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/module/v1/module_pb2.py
--rw-r--r--   0        0        0      581 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2529 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.py
--rw-r--r--   0        0        0     1725 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.py
--rw-r--r--   0        0        0     1336 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1155 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3644 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     4284 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     4459 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     3011 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2009 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2754 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1316 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.py
--rw-r--r--   0        0        0      581 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     6689 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.py
--rw-r--r--   0        0        0     6923 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.py
--rw-r--r--   0        0        0     1735 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1188 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     5469 2023-07-03 23:42:19.057520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     6877 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6420 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4183 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     3210 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4601 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1308 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/genutil/module/v1/module_pb2.py
--rw-r--r--   0        0        0      581 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/genutil/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/genutil/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1693 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1086 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1398 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1211 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2379 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/genesis_pb2.py
--rw-r--r--   0        0        0     3758 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    11245 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/gov_pb2.py
--rw-r--r--   0        0        0    20071 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/gov_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/gov_pb2_grpc.py
--rw-r--r--   0        0        0     9987 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/query_pb2.py
--rw-r--r--   0        0        0    16420 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/query_pb2.pyi
--rw-r--r--   0        0        0    14263 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     9114 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/tx_pb2.py
--rw-r--r--   0        0        0    10599 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/tx_pb2.pyi
--rw-r--r--   0        0        0    11056 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     3409 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     3284 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    15268 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.py
--rw-r--r--   0        0        0    16658 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/gov_pb2_grpc.py
--rw-r--r--   0        0        0    12442 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    15960 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    14598 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     7991 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     6779 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     7675 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1999 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1639 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     3952 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/events_pb2.py
--rw-r--r--   0        0        0     7707 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/events_pb2_grpc.py
--rw-r--r--   0        0        0     1830 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/genesis_pb2.py
--rw-r--r--   0        0        0     3456 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    16886 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/query_pb2.py
--rw-r--r--   0        0        0    28391 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/query_pb2.pyi
--rw-r--r--   0        0        0    25990 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0    20486 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/tx_pb2.py
--rw-r--r--   0        0        0    26007 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/tx_pb2.pyi
--rw-r--r--   0        0        0    25421 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0    12444 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/types_pb2.py
--rw-r--r--   0        0        0    26963 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/types_pb2_grpc.py
--rw-r--r--   0        0        0     1433 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1100 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1969 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1405 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3948 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.py
--rw-r--r--   0        0        0     2598 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/mint_pb2_grpc.py
--rw-r--r--   0        0        0     4507 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     3563 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6210 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2810 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1842 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2744 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1477 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/msg/v1/msg_pb2.py
--rw-r--r--   0        0        0     1385 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/msg/v1/msg_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/msg/v1/msg_pb2_grpc.py
--rw-r--r--   0        0        0     1285 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/module/v1/module_pb2.py
--rw-r--r--   0        0        0      576 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1734 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/event_pb2.py
--rw-r--r--   0        0        0     2997 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/event_pb2_grpc.py
--rw-r--r--   0        0        0     1600 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2311 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1901 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.py
--rw-r--r--   0        0        0     3664 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/nft_pb2_grpc.py
--rw-r--r--   0        0        0     6909 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    11302 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    12817 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2352 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1765 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2511 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1307 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.py
--rw-r--r--   0        0        0      712 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2_grpc.py
--rw-r--r--   0        0        0     4021 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.py
--rw-r--r--   0        0        0    10489 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.pyi
--rw-r--r--   0        0        0     4388 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2416 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/v1/orm_pb2.py
--rw-r--r--   0        0        0     7527 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/v1/orm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/v1/orm_pb2_grpc.py
--rw-r--r--   0        0        0     2205 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.py
--rw-r--r--   0        0        0     7358 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2_grpc.py
--rw-r--r--   0        0        0     1303 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/module/v1/module_pb2.py
--rw-r--r--   0        0        0      579 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2599 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/v1beta1/params_pb2.py
--rw-r--r--   0        0        0     2127 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/v1beta1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/v1beta1/params_pb2_grpc.py
--rw-r--r--   0        0        0     3388 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     3996 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     4478 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1337 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/query/v1/query_pb2.py
--rw-r--r--   0        0        0     1548 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/query/v1/query_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/query/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1947 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/reflection/v1/reflection_pb2.py
--rw-r--r--   0        0        0     1551 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/reflection/v1/reflection_pb2.pyi
--rw-r--r--   0        0        0     3070 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/reflection/v1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0     1365 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/module/v1/module_pb2.py
--rw-r--r--   0        0        0      924 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     4107 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     4850 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     5207 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     5194 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6284 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4640 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.py
--rw-r--r--   0        0        0     4327 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.py
--rw-r--r--   0        0        0     3903 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2693 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4596 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1411 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1516 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     3300 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     5176 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0     4470 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     4598 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    24823 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    29039 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    27948 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0    26092 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.py
--rw-r--r--   0        0        0    31868 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/staking_pb2_grpc.py
--rw-r--r--   0        0        0    15825 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0    13555 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0    13680 2023-07-03 23:42:19.067520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1429 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/config/v1/config_pb2.py
--rw-r--r--   0        0        0     1349 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/config/v1/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/config/v1/config_pb2_grpc.py
--rw-r--r--   0        0        0     3253 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.py
--rw-r--r--   0        0        0    10213 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.py
--rw-r--r--   0        0        0    10601 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/v1beta1/service_pb2.py
--rw-r--r--   0        0        0    20455 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/v1beta1/service_pb2.pyi
--rw-r--r--   0        0        0    16593 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/v1beta1/service_pb2_grpc.py
--rw-r--r--   0        0        0     7188 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0    21980 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1357 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.py
--rw-r--r--   0        0        0      923 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     5663 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     7077 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    10523 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     3740 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2804 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4582 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     4427 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.py
--rw-r--r--   0        0        0     5694 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.py
--rw-r--r--   0        0        0     1318 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/module/v1/module_pb2.py
--rw-r--r--   0        0        0      580 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     6897 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     5521 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     6844 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     7472 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.py
--rw-r--r--   0        0        0     7735 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.py
--rw-r--r--   0        0        0     2961 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/cosmos_proto/cosmos_pb2.py
--rw-r--r--   0        0        0     7141 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/cosmos_proto/cosmos_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/cosmos_proto/cosmos_pb2_grpc.py
--rw-r--r--   0        0        0    15929 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/gogoproto/gogo_pb2.py
--rw-r--r--   0        0        0    15691 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/gogoproto/gogo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/gogoproto/gogo_pb2_grpc.py
--rw-r--r--   0        0        0     1589 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/google/api/annotations_pb2.py
--rw-r--r--   0        0        0     1047 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     2335 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/google/api/http_pb2.py
--rw-r--r--   0        0        0    18274 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/__init__.py
--rw-r--r--   0        0        0     1882 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/event_pb2.py
--rw-r--r--   0        0        0     1813 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/event_pb2_grpc.py
--rw-r--r--   0        0        0     1813 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1108 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3219 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/query_pb2.py
--rw-r--r--   0        0        0     2319 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/query_pb2.pyi
--rw-r--r--   0        0        0     4378 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2925 2023-07-03 23:42:21.137519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/state_pb2.py
--rw-r--r--   0        0        0     2806 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/state_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/__init__.py
--rw-r--r--   0        0        0     2556 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/genesis_pb2.py
--rw-r--r--   0        0        0     3486 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3400 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/inflation_pb2.py
--rw-r--r--   0        0        0     2746 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/inflation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/inflation_pb2_grpc.py
--rw-r--r--   0        0        0     7143 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/query_pb2.py
--rw-r--r--   0        0        0     7309 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/query_pb2.pyi
--rw-r--r--   0        0        0    11682 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/__init__.py
--rw-r--r--   0        0        0     2959 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/event_pb2.py
--rw-r--r--   0        0        0     4208 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/event_pb2_grpc.py
--rw-r--r--   0        0        0     4399 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/genesis_pb2.py
--rw-r--r--   0        0        0     5191 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    10133 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/oracle_pb2.py
--rw-r--r--   0        0        0     8950 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/oracle_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/oracle_pb2_grpc.py
--rw-r--r--   0        0        0    14060 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/query_pb2.py
--rw-r--r--   0        0        0    15236 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/query_pb2.pyi
--rw-r--r--   0        0        0    21945 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2309 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/state_pb2.py
--rw-r--r--   0        0        0     1119 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/state_pb2_grpc.py
--rw-r--r--   0        0        0     6507 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/tx_pb2.py
--rw-r--r--   0        0        0     4671 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     6654 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/__init__.py
--rw-r--r--   0        0        0    11243 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/event_pb2.py
--rw-r--r--   0        0        0    13948 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/event_pb2_grpc.py
--rw-r--r--   0        0        0     2567 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/genesis_pb2.py
--rw-r--r--   0        0        0     2048 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     7749 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/query_pb2.py
--rw-r--r--   0        0        0     7284 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/query_pb2.pyi
--rw-r--r--   0        0        0     7818 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/query_pb2_grpc.py
--rw-r--r--   0        0        0    10001 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/state_pb2.py
--rw-r--r--   0        0        0    11123 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/state_pb2_grpc.py
--rw-r--r--   0        0        0    15189 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/tx_pb2.py
--rw-r--r--   0        0        0    15581 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/tx_pb2.pyi
--rw-r--r--   0        0        0    11019 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/tx_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/__init__.py
--rw-r--r--   0        0        0     6645 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/event_pb2.py
--rw-r--r--   0        0        0     8332 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/event_pb2_grpc.py
--rw-r--r--   0        0        0     1887 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1530 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     2113 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/params_pb2.py
--rw-r--r--   0        0        0     1850 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/params_pb2_grpc.py
--rw-r--r--   0        0        0     5491 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/pool_pb2.py
--rw-r--r--   0        0        0     5345 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/pool_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/pool_pb2_grpc.py
--rw-r--r--   0        0        0    19838 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/query_pb2.py
--rw-r--r--   0        0        0    21019 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/query_pb2.pyi
--rw-r--r--   0        0        0    29070 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     8791 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/tx_pb2.py
--rw-r--r--   0        0        0     7873 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     7328 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/__init__.py
--rw-r--r--   0        0        0     5369 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/events_pb2.py
--rw-r--r--   0        0        0     5131 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/events_pb2_grpc.py
--rw-r--r--   0        0        0     2123 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1434 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     2062 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/params_pb2.py
--rw-r--r--   0        0        0     3105 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/params_pb2_grpc.py
--rw-r--r--   0        0        0     8044 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/query_pb2.py
--rw-r--r--   0        0        0     7591 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/query_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     7329 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.py
--rw-r--r--   0        0        0     8386 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     8285 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 23:42:23.367519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/__init__.py
--rw-r--r--   0        0        0     1742 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/event_pb2.py
--rw-r--r--   0        0        0     1190 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/event_pb2_grpc.py
--rw-r--r--   0        0        0     2227 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/query_pb2.py
--rw-r--r--   0        0        0     1336 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/query_pb2.pyi
--rw-r--r--   0        0        0     2608 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1810 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/state_pb2.py
--rw-r--r--   0        0        0     1817 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/state_pb2_grpc.py
--rw-r--r--   0        0        0     1982 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/tx_pb2.py
--rw-r--r--   0        0        0     1975 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     3044 2023-07-03 23:42:21.147519 nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0    26856 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/abci/types_pb2.py
--rw-r--r--   0        0        0    56049 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/abci/types_pb2.pyi
--rw-r--r--   0        0        0    27809 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/abci/types_pb2_grpc.py
--rw-r--r--   0        0        0     1508 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/crypto/keys_pb2.py
--rw-r--r--   0        0        0     1280 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/crypto/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/crypto/keys_pb2_grpc.py
--rw-r--r--   0        0        0     2340 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/crypto/proof_pb2.py
--rw-r--r--   0        0        0     4101 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/crypto/proof_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/crypto/proof_pb2_grpc.py
--rw-r--r--   0        0        0     1238 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/libs/bits/types_pb2.py
--rw-r--r--   0        0        0     1049 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/libs/bits/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/libs/bits/types_pb2_grpc.py
--rw-r--r--   0        0        0     3673 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/p2p/types_pb2.py
--rw-r--r--   0        0        0     3901 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/p2p/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/p2p/types_pb2_grpc.py
--rw-r--r--   0        0        0     2226 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/block_pb2.py
--rw-r--r--   0        0        0     1707 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/block_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/block_pb2_grpc.py
--rw-r--r--   0        0        0     3741 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/evidence_pb2.py
--rw-r--r--   0        0        0     5767 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/evidence_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/evidence_pb2_grpc.py
--rw-r--r--   0        0        0     3323 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/params_pb2.py
--rw-r--r--   0        0        0     6262 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/params_pb2_grpc.py
--rw-r--r--   0        0        0    11770 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/types_pb2.py
--rw-r--r--   0        0        0    18408 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/types_pb2_grpc.py
--rw-r--r--   0        0        0     2351 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/validator_pb2.py
--rw-r--r--   0        0        0     3356 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/validator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/validator_pb2_grpc.py
--rw-r--r--   0        0        0     1597 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/version/types_pb2.py
--rw-r--r--   0        0        0     1793 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/version/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-03 23:42:19.077520 nibiru_proto-0.21.3b5/nibiru_proto/tendermint/version/types_pb2_grpc.py
--rw-r--r--   0        0        0      853 2023-07-03 23:44:28.570785 nibiru_proto-0.21.3b5/pyproject.toml
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 nibiru_proto-0.21.3b5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-08-17 01:57:49.915436 nibiru_proto-0.21.3b7/LICENSE
+-rw-r--r--   0        0        0       84 2023-07-04 00:17:01.407673 nibiru_proto-0.21.3b7/nibiru_proto/__init__.py
+-rw-r--r--   0        0        0     2028 2023-07-04 00:16:54.277673 nibiru_proto-0.21.3b7/nibiru_proto/amino/amino_pb2.py
+-rw-r--r--   0        0        0     3227 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/amino/amino_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.257673 nibiru_proto-0.21.3b7/nibiru_proto/amino/amino_pb2_grpc.py
+-rw-r--r--   0        0        0     2012 2023-07-04 00:16:57.867673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.py
+-rw-r--r--   0        0        0     4237 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.887673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1817 2023-07-04 00:16:57.967673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/config_pb2.py
+-rw-r--r--   0        0        0     5300 2023-07-04 00:15:50.431751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.037673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/config_pb2_grpc.py
+-rw-r--r--   0        0        0     1968 2023-07-04 00:16:57.917673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/module_pb2.py
+-rw-r--r--   0        0        0     6817 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.927673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1539 2023-07-04 00:16:57.987673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/query_pb2.py
+-rw-r--r--   0        0        0     1426 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/query_pb2.pyi
+-rw-r--r--   0        0        0     2603 2023-07-04 00:16:58.017673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1794 2023-07-04 00:16:55.807673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     2675 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.827673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     4605 2023-07-04 00:16:55.857674 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.py
+-rw-r--r--   0        0        0     5282 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.877673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/auth_pb2_grpc.py
+-rw-r--r--   0        0        0     1899 2023-07-04 00:16:55.897673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1555 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.927673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    12503 2023-07-04 00:16:55.967673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    14414 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    19125 2023-07-04 00:16:55.997673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2810 2023-07-04 00:16:55.947673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1842 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2743 2023-07-04 00:16:56.017673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1295 2023-07-04 00:16:58.797673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      578 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.827673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     4039 2023-07-04 00:16:58.887673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     4440 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.857673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0     2402 2023-07-04 00:16:58.947673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/event_pb2.py
+-rw-r--r--   0        0        0     2114 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:59.067673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     1717 2023-07-04 00:16:58.917673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1194 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.977673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     5558 2023-07-04 00:16:59.027673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     7628 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6331 2023-07-04 00:16:59.047673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     5129 2023-07-04 00:16:59.007673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     4700 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     6246 2023-07-04 00:16:59.097673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     4201 2023-07-04 00:16:56.977673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/options_pb2.py
+-rw-r--r--   0        0        0    12271 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/options_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.997673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/options_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-07-04 00:16:57.017673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/query_pb2.py
+-rw-r--r--   0        0        0     2362 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     2886 2023-07-04 00:16:57.037673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1439 2023-07-04 00:16:56.087673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1637 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.107673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2480 2023-07-04 00:16:56.147673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     1703 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.127673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0     6001 2023-07-04 00:16:56.327673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.py
+-rw-r--r--   0        0        0     8210 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.267673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/bank_pb2_grpc.py
+-rw-r--r--   0        0        0     4070 2023-07-04 00:16:56.177673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     3902 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.197673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    16803 2023-07-04 00:16:56.237673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    23149 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    21828 2023-07-04 00:16:56.287673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     6511 2023-07-04 00:16:56.217673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     6731 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     8074 2023-07-04 00:16:56.307673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     7125 2023-07-04 00:16:57.657673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.py
+-rw-r--r--   0        0        0    13374 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.637673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.py
+-rw-r--r--   0        0        0     1570 2023-07-04 00:16:57.237673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.py
+-rw-r--r--   0        0        0     1558 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.207673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.py
+-rw-r--r--   0        0        0     1868 2023-07-04 00:16:57.267673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     1213 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     2762 2023-07-04 00:16:57.297673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/node/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1598 2023-07-04 00:16:57.457673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.py
+-rw-r--r--   0        0        0     3440 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.437673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.py
+-rw-r--r--   0        0        0     3071 2023-07-04 00:16:57.407673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.py
+-rw-r--r--   0        0        0     3055 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi
+-rw-r--r--   0        0        0     5144 2023-07-04 00:16:57.387673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0    10963 2023-07-04 00:16:57.357673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py
+-rw-r--r--   0        0        0    23085 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi
+-rw-r--r--   0        0        0    13573 2023-07-04 00:16:57.327673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0     4501 2023-07-04 00:16:57.587673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py
+-rw-r--r--   0        0        0     8467 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.607673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.py
+-rw-r--r--   0        0        0     2626 2023-07-04 00:16:57.507673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.py
+-rw-r--r--   0        0        0     3087 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.477673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.py
+-rw-r--r--   0        0        0     2508 2023-07-04 00:16:57.537673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.py
+-rw-r--r--   0        0        0     5092 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.567673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2_grpc.py
+-rw-r--r--   0        0        0    11465 2023-07-04 00:16:57.707673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    18881 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    14492 2023-07-04 00:16:57.727673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4471 2023-07-04 00:16:57.747673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.py
+-rw-r--r--   0        0        0     5547 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.677673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2_grpc.py
+-rw-r--r--   0        0        0     3165 2023-07-04 00:16:57.777673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/v1beta1/coin_pb2.py
+-rw-r--r--   0        0        0     2703 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/v1beta1/coin_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.797673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/v1beta1/coin_pb2_grpc.py
+-rw-r--r--   0        0        0     1383 2023-07-04 00:17:00.947673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1020 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:00.967673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2171 2023-07-04 00:17:01.057673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.py
+-rw-r--r--   0        0        0     2304 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.007673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/capability_pb2_grpc.py
+-rw-r--r--   0        0        0     2274 2023-07-04 00:17:00.987673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2428 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.037673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1370 2023-07-04 00:16:59.437673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      925 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:59.447673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2013 2023-07-04 00:16:59.347673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/query_pb2.py
+-rw-r--r--   0        0        0     1699 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     2626 2023-07-04 00:16:59.387673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2441 2023-07-04 00:16:59.327673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/tx_pb2.py
+-rw-r--r--   0        0        0     2431 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2734 2023-07-04 00:16:59.417673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1447 2023-07-04 00:16:58.267673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1178 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.287673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1727 2023-07-04 00:16:58.317673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1192 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.337673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3940 2023-07-04 00:16:58.367673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     3256 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4533 2023-07-04 00:16:58.397673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2264 2023-07-04 00:16:55.617673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.py
+-rw-r--r--   0        0        0     1690 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.587673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/ed25519/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     1796 2023-07-04 00:16:55.637673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.py
+-rw-r--r--   0        0        0     1822 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.657673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2_grpc.py
+-rw-r--r--   0        0        0     2566 2023-07-04 00:16:55.697673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.py
+-rw-r--r--   0        0        0     4311 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.677673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2_grpc.py
+-rw-r--r--   0        0        0     2088 2023-07-04 00:16:55.787673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/keys_pb2.py
+-rw-r--r--   0        0        0     1351 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.717673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     1778 2023-07-04 00:16:55.767673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py
+-rw-r--r--   0        0        0     2062 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.737673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.py
+-rw-r--r--   0        0        0     1893 2023-07-04 00:16:55.567673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.py
+-rw-r--r--   0        0        0     1519 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.547673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     1829 2023-07-04 00:16:55.527673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.py
+-rw-r--r--   0        0        0     1523 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.497673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     1481 2023-07-04 00:16:59.467673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1108 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:59.487673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0    10924 2023-07-04 00:16:59.617673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.py
+-rw-r--r--   0        0        0    13195 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:59.507673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.py
+-rw-r--r--   0        0        0    13143 2023-07-04 00:16:59.527673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0    13975 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:59.557673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    19296 2023-07-04 00:16:59.627673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    18475 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    20401 2023-07-04 00:16:59.647673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0    10831 2023-07-04 00:16:59.587673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     9210 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0    12766 2023-07-04 00:16:59.667673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1316 2023-07-04 00:16:58.427673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      581 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.447673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2529 2023-07-04 00:16:58.587673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.py
+-rw-r--r--   0        0        0     1725 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.557673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.py
+-rw-r--r--   0        0        0     1336 2023-07-04 00:16:58.477673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1155 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.507673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3644 2023-07-04 00:16:58.617673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     4284 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     4459 2023-07-04 00:16:58.637673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3011 2023-07-04 00:16:58.527673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     2009 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2754 2023-07-04 00:16:58.667673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1316 2023-07-04 00:16:55.047673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      581 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.067673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     6689 2023-07-04 00:16:55.087674 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.py
+-rw-r--r--   0        0        0     6923 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.197673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.py
+-rw-r--r--   0        0        0     1735 2023-07-04 00:16:55.107674 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1188 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.127673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     5469 2023-07-04 00:16:55.177673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     6877 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6420 2023-07-04 00:16:55.217673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4183 2023-07-04 00:16:55.157673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     3210 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4601 2023-07-04 00:16:55.237673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1308 2023-07-04 00:16:58.687673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      581 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.717673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1693 2023-07-04 00:16:58.737673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1086 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.767673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1398 2023-07-04 00:16:56.527673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1211 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.547673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2379 2023-07-04 00:16:56.357673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     3758 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.377673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    11245 2023-07-04 00:16:56.407673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/gov_pb2.py
+-rw-r--r--   0        0        0    20071 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/gov_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.467673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/gov_pb2_grpc.py
+-rw-r--r--   0        0        0     9987 2023-07-04 00:16:56.447673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/query_pb2.py
+-rw-r--r--   0        0        0    16420 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    14263 2023-07-04 00:16:56.497673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     9114 2023-07-04 00:16:56.427673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/tx_pb2.py
+-rw-r--r--   0        0        0    10599 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0    11056 2023-07-04 00:16:56.507673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     3409 2023-07-04 00:16:56.567673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     3284 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.597673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    15268 2023-07-04 00:16:56.607673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.py
+-rw-r--r--   0        0        0    16658 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.687673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/gov_pb2_grpc.py
+-rw-r--r--   0        0        0    12442 2023-07-04 00:16:56.657673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    15960 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    14598 2023-07-04 00:16:56.707673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     7991 2023-07-04 00:16:56.637673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     6779 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     7675 2023-07-04 00:16:56.727673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1999 2023-07-04 00:16:59.987673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1639 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:00.037673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     3952 2023-07-04 00:16:59.777673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/events_pb2.py
+-rw-r--r--   0        0        0     7707 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:59.697673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/events_pb2_grpc.py
+-rw-r--r--   0        0        0     1830 2023-07-04 00:16:59.747673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     3456 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:59.817673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    16886 2023-07-04 00:16:59.867673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/query_pb2.py
+-rw-r--r--   0        0        0    28391 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    25990 2023-07-04 00:16:59.887673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0    20486 2023-07-04 00:16:59.837673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/tx_pb2.py
+-rw-r--r--   0        0        0    26007 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0    25421 2023-07-04 00:16:59.957673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0    12444 2023-07-04 00:16:59.917673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/types_pb2.py
+-rw-r--r--   0        0        0    26963 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:59.717673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/types_pb2_grpc.py
+-rw-r--r--   0        0        0     1433 2023-07-04 00:16:55.267673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1100 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.287673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1969 2023-07-04 00:16:55.337674 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1405 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.367673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3948 2023-07-04 00:16:55.307673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.py
+-rw-r--r--   0        0        0     2598 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:55.387673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/mint_pb2_grpc.py
+-rw-r--r--   0        0        0     4507 2023-07-04 00:16:55.427673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     3563 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6210 2023-07-04 00:16:55.457673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2810 2023-07-04 00:16:55.407673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1842 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2744 2023-07-04 00:16:55.477673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1477 2023-07-04 00:16:57.827673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/msg/v1/msg_pb2.py
+-rw-r--r--   0        0        0     1385 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/msg/v1/msg_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.847673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/msg/v1/msg_pb2_grpc.py
+-rw-r--r--   0        0        0     1285 2023-07-04 00:17:00.667673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      576 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:00.687673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1734 2023-07-04 00:17:00.737673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/event_pb2.py
+-rw-r--r--   0        0        0     2997 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:00.897673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     1600 2023-07-04 00:17:00.707673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2311 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:00.757673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1901 2023-07-04 00:17:00.787673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.py
+-rw-r--r--   0        0        0     3664 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:00.827673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/nft_pb2_grpc.py
+-rw-r--r--   0        0        0     6909 2023-07-04 00:17:00.847673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    11302 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    12817 2023-07-04 00:17:00.877673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2352 2023-07-04 00:17:00.807673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1765 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2511 2023-07-04 00:17:00.917673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1307 2023-07-04 00:16:56.797673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.py
+-rw-r--r--   0        0        0      712 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.817673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     4021 2023-07-04 00:16:56.847673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.py
+-rw-r--r--   0        0        0    10489 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.pyi
+-rw-r--r--   0        0        0     4388 2023-07-04 00:16:56.867673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2416 2023-07-04 00:16:56.767673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1/orm_pb2.py
+-rw-r--r--   0        0        0     7527 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1/orm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.747673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1/orm_pb2_grpc.py
+-rw-r--r--   0        0        0     2205 2023-07-04 00:16:56.917673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.py
+-rw-r--r--   0        0        0     7358 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.887673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     1303 2023-07-04 00:17:00.507673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      579 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:00.527673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2599 2023-07-04 00:17:00.587673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/params_pb2.py
+-rw-r--r--   0        0        0     2127 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:00.557673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/params_pb2_grpc.py
+-rw-r--r--   0        0        0     3388 2023-07-04 00:17:00.617673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     3996 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     4478 2023-07-04 00:17:00.637673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1337 2023-07-04 00:16:56.937673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/query/v1/query_pb2.py
+-rw-r--r--   0        0        0     1548 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/query/v1/query_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:56.957673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/query/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1947 2023-07-04 00:16:56.067673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/reflection/v1/reflection_pb2.py
+-rw-r--r--   0        0        0     1551 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/reflection/v1/reflection_pb2.pyi
+-rw-r--r--   0        0        0     3070 2023-07-04 00:16:56.037673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/reflection/v1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0     1365 2023-07-04 00:17:01.087673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      924 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.107673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     4107 2023-07-04 00:17:01.147673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     4850 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.177673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     5207 2023-07-04 00:17:01.217673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     5194 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6284 2023-07-04 00:17:01.237673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4640 2023-07-04 00:17:01.287673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.py
+-rw-r--r--   0        0        0     4327 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.127673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.py
+-rw-r--r--   0        0        0     3903 2023-07-04 00:17:01.197673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     2693 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4596 2023-07-04 00:17:01.267673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1411 2023-07-04 00:17:00.097673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1516 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:00.167673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     3300 2023-07-04 00:17:00.227673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     5176 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:00.197673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0     4470 2023-07-04 00:17:00.297673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     4598 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:00.357673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    24823 2023-07-04 00:17:00.427673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    29039 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    27948 2023-07-04 00:17:00.457673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0    26092 2023-07-04 00:17:00.327673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.py
+-rw-r--r--   0        0        0    31868 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:00.267673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/staking_pb2_grpc.py
+-rw-r--r--   0        0        0    15825 2023-07-04 00:17:00.397673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0    13555 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0    13680 2023-07-04 00:17:00.487673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1429 2023-07-04 00:16:58.067673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/config/v1/config_pb2.py
+-rw-r--r--   0        0        0     1349 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/config/v1/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.087673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/config/v1/config_pb2_grpc.py
+-rw-r--r--   0        0        0     3253 2023-07-04 00:16:58.137673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.py
+-rw-r--r--   0        0        0    10213 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.117673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.py
+-rw-r--r--   0        0        0    10601 2023-07-04 00:16:58.187673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/service_pb2.py
+-rw-r--r--   0        0        0    20455 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/service_pb2.pyi
+-rw-r--r--   0        0        0    16593 2023-07-04 00:16:58.217673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/service_pb2_grpc.py
+-rw-r--r--   0        0        0     7188 2023-07-04 00:16:58.167673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0    21980 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:58.237673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1357 2023-07-04 00:16:59.127673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      923 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:59.157673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     5663 2023-07-04 00:16:59.257673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     7077 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    10523 2023-07-04 00:16:59.287673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3740 2023-07-04 00:16:59.227673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     2804 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4582 2023-07-04 00:16:59.317673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     4427 2023-07-04 00:16:59.177673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.py
+-rw-r--r--   0        0        0     5694 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:59.207673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.py
+-rw-r--r--   0        0        0     1318 2023-07-04 00:16:57.067673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      580 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.087673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     6897 2023-07-04 00:16:57.157673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     5521 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     6844 2023-07-04 00:16:57.187673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     7472 2023-07-04 00:16:57.107673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.py
+-rw-r--r--   0        0        0     7735 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:57.137673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.py
+-rw-r--r--   0        0        0     2961 2023-07-04 00:16:54.307674 nibiru_proto-0.21.3b7/nibiru_proto/cosmos_proto/cosmos_pb2.py
+-rw-r--r--   0        0        0     7141 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/cosmos_proto/cosmos_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.327674 nibiru_proto-0.21.3b7/nibiru_proto/cosmos_proto/cosmos_pb2_grpc.py
+-rw-r--r--   0        0        0    15929 2023-07-04 00:16:54.217673 nibiru_proto-0.21.3b7/nibiru_proto/gogoproto/gogo_pb2.py
+-rw-r--r--   0        0        0    15691 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/gogoproto/gogo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.237673 nibiru_proto-0.21.3b7/nibiru_proto/gogoproto/gogo_pb2_grpc.py
+-rw-r--r--   0        0        0     1589 2023-07-04 00:17:01.387673 nibiru_proto-0.21.3b7/nibiru_proto/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0     1047 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.337673 nibiru_proto-0.21.3b7/nibiru_proto/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     2335 2023-07-04 00:17:01.317673 nibiru_proto-0.21.3b7/nibiru_proto/google/api/http_pb2.py
+-rw-r--r--   0        0        0    18274 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.367673 nibiru_proto-0.21.3b7/nibiru_proto/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0       83 2023-07-04 00:17:03.357673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:01.667673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:01.637673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/__init__.py
+-rw-r--r--   0        0        0     1882 2023-07-04 00:17:01.487673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/event_pb2.py
+-rw-r--r--   0        0        0     1813 2023-07-04 00:15:52.621750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.617673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     1826 2023-07-04 00:17:01.467673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     1108 2023-07-04 00:15:52.621750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.517673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3232 2023-07-04 00:17:01.567673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/query_pb2.py
+-rw-r--r--   0        0        0     2319 2023-07-04 00:15:52.621750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     4391 2023-07-04 00:17:01.587673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2925 2023-07-04 00:17:01.537673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/state_pb2.py
+-rw-r--r--   0        0        0     2806 2023-07-04 00:15:52.621750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.437673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/state_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:02.357673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:02.337673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/__init__.py
+-rw-r--r--   0        0        0     2569 2023-07-04 00:17:02.227673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     3486 2023-07-04 00:15:52.631750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:02.247673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3400 2023-07-04 00:17:02.197673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/inflation_pb2.py
+-rw-r--r--   0        0        0     2746 2023-07-04 00:15:52.621750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/inflation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:02.267673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/inflation_pb2_grpc.py
+-rw-r--r--   0        0        0     7156 2023-07-04 00:17:02.297673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/query_pb2.py
+-rw-r--r--   0        0        0     7309 2023-07-04 00:15:52.621750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    11695 2023-07-04 00:17:02.317673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:02.977673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:02.917673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/__init__.py
+-rw-r--r--   0        0        0     2972 2023-07-04 00:17:02.727673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/event_pb2.py
+-rw-r--r--   0        0        0     4208 2023-07-04 00:15:52.631750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:02.897673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     4412 2023-07-04 00:17:02.707673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     5191 2023-07-04 00:15:52.631750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:02.757673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    10133 2023-07-04 00:17:02.847673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/oracle_pb2.py
+-rw-r--r--   0        0        0     8950 2023-07-04 00:15:52.631750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/oracle_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:02.677673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/oracle_pb2_grpc.py
+-rw-r--r--   0        0        0    14073 2023-07-04 00:17:02.827673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/query_pb2.py
+-rw-r--r--   0        0        0    15236 2023-07-04 00:15:52.631750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    21958 2023-07-04 00:17:02.877673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2322 2023-07-04 00:17:02.777673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/state_pb2.py
+-rw-r--r--   0        0        0     1119 2023-07-04 00:15:52.631750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:02.657673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/state_pb2_grpc.py
+-rw-r--r--   0        0        0     6507 2023-07-04 00:17:02.807673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/tx_pb2.py
+-rw-r--r--   0        0        0     4671 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     6667 2023-07-04 00:17:02.947673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:02.627673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:02.587673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/__init__.py
+-rw-r--r--   0        0        0    11256 2023-07-04 00:17:02.427673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/event_pb2.py
+-rw-r--r--   0        0        0    13948 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:02.557673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/event_pb2_grpc.py
+-rw-r--r--   0        0        0     2580 2023-07-04 00:17:02.407673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/genesis_pb2.py
+-rw-r--r--   0        0        0     2048 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:02.457673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     7762 2023-07-04 00:17:02.517673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/query_pb2.py
+-rw-r--r--   0        0        0     7284 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/query_pb2.pyi
+-rw-r--r--   0        0        0     7831 2023-07-04 00:17:02.537673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/query_pb2_grpc.py
+-rw-r--r--   0        0        0    10001 2023-07-04 00:17:02.477673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/state_pb2.py
+-rw-r--r--   0        0        0    11123 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:02.377673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/state_pb2_grpc.py
+-rw-r--r--   0        0        0    15202 2023-07-04 00:17:02.497673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/tx_pb2.py
+-rw-r--r--   0        0        0    15581 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/tx_pb2.pyi
+-rw-r--r--   0        0        0    11032 2023-07-04 00:17:02.607673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/tx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:03.327673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:03.247673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/__init__.py
+-rw-r--r--   0        0        0     6658 2023-07-04 00:17:03.067673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/event_pb2.py
+-rw-r--r--   0        0        0     8332 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:03.227673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     1913 2023-07-04 00:17:03.047673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     1530 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:03.087673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     2113 2023-07-04 00:17:03.027673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/params_pb2.py
+-rw-r--r--   0        0        0     1850 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:03.007673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/params_pb2_grpc.py
+-rw-r--r--   0        0        0     5491 2023-07-04 00:17:03.197673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/pool_pb2.py
+-rw-r--r--   0        0        0     5345 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/pool_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:03.297673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/pool_pb2_grpc.py
+-rw-r--r--   0        0        0    19864 2023-07-04 00:17:03.137673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/query_pb2.py
+-rw-r--r--   0        0        0    21019 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    29083 2023-07-04 00:17:03.167673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     8804 2023-07-04 00:17:03.117673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/tx_pb2.py
+-rw-r--r--   0        0        0     7873 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     7341 2023-07-04 00:17:03.267673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:01.947673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:01.897673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/__init__.py
+-rw-r--r--   0        0        0     5369 2023-07-04 00:17:01.787673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/events_pb2.py
+-rw-r--r--   0        0        0     5131 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.717673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/events_pb2_grpc.py
+-rw-r--r--   0        0        0     2136 2023-07-04 00:17:01.757673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     1434 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.807673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     2062 2023-07-04 00:17:01.737673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/params_pb2.py
+-rw-r--r--   0        0        0     3105 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.687673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/params_pb2_grpc.py
+-rw-r--r--   0        0        0     8057 2023-07-04 00:17:01.857673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/query_pb2.py
+-rw-r--r--   0        0        0     7591 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     8241 2023-07-04 00:17:01.877673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     7329 2023-07-04 00:17:01.837673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.py
+-rw-r--r--   0        0        0     8386 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     8298 2023-07-04 00:17:01.927673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:02.177673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:17:02.127673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/__init__.py
+-rw-r--r--   0        0        0     1755 2023-07-04 00:17:01.997673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/event_pb2.py
+-rw-r--r--   0        0        0     1190 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:02.107673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     2240 2023-07-04 00:17:02.067673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/query_pb2.py
+-rw-r--r--   0        0        0     1336 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     2621 2023-07-04 00:17:02.087673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1810 2023-07-04 00:17:02.017673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/state_pb2.py
+-rw-r--r--   0        0        0     1817 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:17:01.967673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/state_pb2_grpc.py
+-rw-r--r--   0        0        0     1982 2023-07-04 00:17:02.037673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/tx_pb2.py
+-rw-r--r--   0        0        0     1975 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     3057 2023-07-04 00:17:02.157673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0    26856 2023-07-04 00:16:55.007673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/abci/types_pb2.py
+-rw-r--r--   0        0        0    56049 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/abci/types_pb2.pyi
+-rw-r--r--   0        0        0    27809 2023-07-04 00:16:54.977673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/abci/types_pb2_grpc.py
+-rw-r--r--   0        0        0     1508 2023-07-04 00:16:54.517673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/keys_pb2.py
+-rw-r--r--   0        0        0     1280 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.487673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     2340 2023-07-04 00:16:54.457673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/proof_pb2.py
+-rw-r--r--   0        0        0     4101 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/proof_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.427673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/proof_pb2_grpc.py
+-rw-r--r--   0        0        0     1238 2023-07-04 00:16:54.917673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/libs/bits/types_pb2.py
+-rw-r--r--   0        0        0     1049 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/libs/bits/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.877673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/libs/bits/types_pb2_grpc.py
+-rw-r--r--   0        0        0     3673 2023-07-04 00:16:54.397673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/p2p/types_pb2.py
+-rw-r--r--   0        0        0     3901 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/p2p/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.367673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/p2p/types_pb2_grpc.py
+-rw-r--r--   0        0        0     2226 2023-07-04 00:16:54.777673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/block_pb2.py
+-rw-r--r--   0        0        0     1707 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/block_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.637673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/block_pb2_grpc.py
+-rw-r--r--   0        0        0     3741 2023-07-04 00:16:54.747673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/evidence_pb2.py
+-rw-r--r--   0        0        0     5767 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/evidence_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.697673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/evidence_pb2_grpc.py
+-rw-r--r--   0        0        0     3323 2023-07-04 00:16:54.607674 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/params_pb2.py
+-rw-r--r--   0        0        0     6262 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.547673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/params_pb2_grpc.py
+-rw-r--r--   0        0        0    11770 2023-07-04 00:16:54.817674 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/types_pb2.py
+-rw-r--r--   0        0        0    18408 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.577674 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/types_pb2_grpc.py
+-rw-r--r--   0        0        0     2351 2023-07-04 00:16:54.667673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/validator_pb2.py
+-rw-r--r--   0        0        0     3356 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/validator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.717673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/validator_pb2_grpc.py
+-rw-r--r--   0        0        0     1597 2023-07-04 00:16:54.957673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/version/types_pb2.py
+-rw-r--r--   0        0        0     1793 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/version/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-04 00:16:54.937673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/version/types_pb2_grpc.py
+-rw-r--r--   0        0        0      853 2023-07-04 00:18:49.571961 nibiru_proto-0.21.3b7/pyproject.toml
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 nibiru_proto-0.21.3b7/PKG-INFO
```

### Comparing `nibiru_proto-0.21.3b5/LICENSE` & `nibiru_proto-0.21.3b7/LICENSE`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/amino/amino_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/amino/amino_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/amino/amino_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/amino/amino_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/config_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/config_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/app/v1alpha1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/auth/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/event_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/event_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/authz/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/autocli/v1/options_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/options_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/autocli/v1/options_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/autocli/v1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/autocli/v1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/autocli/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/bank/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/node/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/node/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/v1beta1/coin_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/v1beta1/coin_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/base/v1beta1/coin_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/v1beta1/coin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/v1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/v1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/v1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/v1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/consensus/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/multisig/keys_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/multisig/keys_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/genutil/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/genutil/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/gov_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/gov_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/gov_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/gov_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/gov/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/events_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/events_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/events_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/types_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/group/v1/types_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/mint/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/msg/v1/msg_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/msg/v1/msg_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/msg/v1/msg_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/msg/v1/msg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/event_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/event_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/nft/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/v1/orm_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1/orm_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/v1/orm_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1/orm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/v1beta1/params_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/v1beta1/params_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/params/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/query/v1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/query/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/query/v1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/query/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/reflection/v1/reflection_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/reflection/v1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/reflection/v1/reflection_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/reflection/v1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/reflection/v1/reflection_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/reflection/v1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/staking/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/config/v1/config_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/config/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/config/v1/config_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/config/v1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/v1beta1/service_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/v1beta1/service_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/v1beta1/service_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/module/v1/module_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos_proto/cosmos_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos_proto/cosmos_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/cosmos_proto/cosmos_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/cosmos_proto/cosmos_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/gogoproto/gogo_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/gogoproto/gogo_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/gogoproto/gogo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/google/api/annotations_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/google/api/annotations_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/google/api/http_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/google/api/http_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/event_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/event_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/genesis_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from nibiru.epochs.v1 import state_pb2 as nibiru_dot_epochs_dot_v1_dot_state__pb2
+from nibiru_proto.nibiru.epochs.v1 import state_pb2 as nibiru_dot_epochs_dot_v1_dot_state__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1enibiru/epochs/v1/genesis.proto\x12\x10nibiru.epochs.v1\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cnibiru/epochs/v1/state.proto\"I\n\x0cGenesisState\x12\x39\n\x06\x65pochs\x18\x01 \x03(\x0b\x32\x1b.nibiru.epochs.v1.EpochInfoB\x04\xc8\xde\x1f\x00R\x06\x65pochsB.Z,github.com/NibiruChain/nibiru/x/epochs/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.epochs.v1.genesis_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/query_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from cosmos.base.query.v1beta1 import pagination_pb2 as cosmos_dot_base_dot_query_dot_v1beta1_dot_pagination__pb2
-from nibiru.epochs.v1 import state_pb2 as nibiru_dot_epochs_dot_v1_dot_state__pb2
+from nibiru_proto.nibiru.epochs.v1 import state_pb2 as nibiru_dot_epochs_dot_v1_dot_state__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cnibiru/epochs/v1/query.proto\x12\x10nibiru.epochs.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a*cosmos/base/query/v1beta1/pagination.proto\x1a\x1cnibiru/epochs/v1/state.proto\"\x18\n\x16QueryEpochsInfoRequest\"T\n\x17QueryEpochsInfoResponse\x12\x39\n\x06\x65pochs\x18\x01 \x03(\x0b\x32\x1b.nibiru.epochs.v1.EpochInfoB\x04\xc8\xde\x1f\x00R\x06\x65pochs\":\n\x18QueryCurrentEpochRequest\x12\x1e\n\nidentifier\x18\x01 \x01(\tR\nidentifier\"@\n\x19QueryCurrentEpochResponse\x12#\n\rcurrent_epoch\x18\x01 \x01(\x04R\x0c\x63urrentEpoch2\xaa\x02\n\x05Query\x12\x88\x01\n\nEpochInfos\x12(.nibiru.epochs.v1.QueryEpochsInfoRequest\x1a).nibiru.epochs.v1.QueryEpochsInfoResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/nibiru/epochs/v1beta1/epochs\x12\x95\x01\n\x0c\x43urrentEpoch\x12*.nibiru.epochs.v1.QueryCurrentEpochRequest\x1a+.nibiru.epochs.v1.QueryCurrentEpochResponse\",\x82\xd3\xe4\x93\x02&\x12$/nibiru/epochs/v1beta1/current_epochB.Z,github.com/NibiruChain/nibiru/x/epochs/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.epochs.v1.query_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/query_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from nibiru.epochs.v1 import query_pb2 as nibiru_dot_epochs_dot_v1_dot_query__pb2
+from nibiru_proto.nibiru.epochs.v1 import query_pb2 as nibiru_dot_epochs_dot_v1_dot_query__pb2
 
 
 class QueryStub(object):
     """Query defines the gRPC querier service.
     """
 
     def __init__(self, channel):
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/state_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/state_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/epochs/v1/state_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/genesis_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from nibiru.inflation.v1 import inflation_pb2 as nibiru_dot_inflation_dot_v1_dot_inflation__pb2
+from nibiru_proto.nibiru.inflation.v1 import inflation_pb2 as nibiru_dot_inflation_dot_v1_dot_inflation__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!nibiru/inflation/v1/genesis.proto\x12\x13nibiru.inflation.v1\x1a\x14gogoproto/gogo.proto\x1a#nibiru/inflation/v1/inflation.proto\"\x88\x01\n\x0cGenesisState\x12\x39\n\x06params\x18\x01 \x01(\x0b\x32\x1b.nibiru.inflation.v1.ParamsB\x04\xc8\xde\x1f\x00R\x06params\x12\x16\n\x06period\x18\x02 \x01(\x04R\x06period\x12%\n\x0eskipped_epochs\x18\x03 \x01(\x04R\rskippedEpochs\"\xb6\x02\n\x06Params\x12+\n\x11inflation_enabled\x18\x01 \x01(\x08R\x10inflationEnabled\x12j\n\x17\x65xponential_calculation\x18\x02 \x01(\x0b\x32+.nibiru.inflation.v1.ExponentialCalculationB\x04\xc8\xde\x1f\x00R\x16\x65xponentialCalculation\x12g\n\x16inflation_distribution\x18\x03 \x01(\x0b\x32*.nibiru.inflation.v1.InflationDistributionB\x04\xc8\xde\x1f\x00R\x15inflationDistribution\x12*\n\x11\x65pochs_per_period\x18\x04 \x01(\x04R\x0f\x65pochsPerPeriodB1Z/github.com/NibiruChain/nibiru/x/inflation/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.inflation.v1.genesis_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/inflation_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/inflation_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/inflation_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/inflation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/query_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
-from nibiru.inflation.v1 import genesis_pb2 as nibiru_dot_inflation_dot_v1_dot_genesis__pb2
+from nibiru_proto.nibiru.inflation.v1 import genesis_pb2 as nibiru_dot_inflation_dot_v1_dot_genesis__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fnibiru/inflation/v1/query.proto\x12\x13nibiru.inflation.v1\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a!nibiru/inflation/v1/genesis.proto\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\"\x14\n\x12QueryPeriodRequest\"-\n\x13QueryPeriodResponse\x12\x16\n\x06period\x18\x01 \x01(\x04R\x06period\" \n\x1eQueryEpochMintProvisionRequest\"\xa7\x01\n\x1fQueryEpochMintProvisionResponse\x12\x83\x01\n\x14\x65poch_mint_provision\x18\x01 \x01(\x0b\x32\x1c.cosmos.base.v1beta1.DecCoinB3\xc8\xde\x1f\x00\xaa\xdf\x1f+github.com/cosmos/cosmos-sdk/types.DecCoinsR\x12\x65pochMintProvision\"\x1b\n\x19QuerySkippedEpochsRequest\"C\n\x1aQuerySkippedEpochsResponse\x12%\n\x0eskipped_epochs\x18\x01 \x01(\x04R\rskippedEpochs\"\x1f\n\x1dQueryCirculatingSupplyRequest\"\xa3\x01\n\x1eQueryCirculatingSupplyResponse\x12\x80\x01\n\x12\x63irculating_supply\x18\x01 \x01(\x0b\x32\x1c.cosmos.base.v1beta1.DecCoinB3\xc8\xde\x1f\x00\xaa\xdf\x1f+github.com/cosmos/cosmos-sdk/types.DecCoinsR\x11\x63irculatingSupply\"\x1b\n\x19QueryInflationRateRequest\"s\n\x1aQueryInflationRateResponse\x12U\n\x0einflation_rate\x18\x01 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\rinflationRate\"\x14\n\x12QueryParamsRequest\"P\n\x13QueryParamsResponse\x12\x39\n\x06params\x18\x01 \x01(\x0b\x32\x1b.nibiru.inflation.v1.ParamsB\x04\xc8\xde\x1f\x00R\x06params2\xb2\x07\n\x05Query\x12\x80\x01\n\x06Period\x12\'.nibiru.inflation.v1.QueryPeriodRequest\x1a(.nibiru.inflation.v1.QueryPeriodResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/nibiru/inflation/v1/period\x12\xb2\x01\n\x12\x45pochMintProvision\x12\x33.nibiru.inflation.v1.QueryEpochMintProvisionRequest\x1a\x34.nibiru.inflation.v1.QueryEpochMintProvisionResponse\"1\x82\xd3\xe4\x93\x02+\x12)/nibiru/inflation/v1/epoch_mint_provision\x12\x9d\x01\n\rSkippedEpochs\x12..nibiru.inflation.v1.QuerySkippedEpochsRequest\x1a/.nibiru.inflation.v1.QuerySkippedEpochsResponse\"+\x82\xd3\xe4\x93\x02%\x12#/nibiru/inflation/v1/skipped_epochs\x12\xad\x01\n\x11\x43irculatingSupply\x12\x32.nibiru.inflation.v1.QueryCirculatingSupplyRequest\x1a\x33.nibiru.inflation.v1.QueryCirculatingSupplyResponse\"/\x82\xd3\xe4\x93\x02)\x12\'/nibiru/inflation/v1/circulating_supply\x12\x9d\x01\n\rInflationRate\x12..nibiru.inflation.v1.QueryInflationRateRequest\x1a/.nibiru.inflation.v1.QueryInflationRateResponse\"+\x82\xd3\xe4\x93\x02%\x12#/nibiru/inflation/v1/inflation_rate\x12\x80\x01\n\x06Params\x12\'.nibiru.inflation.v1.QueryParamsRequest\x1a(.nibiru.inflation.v1.QueryParamsResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/nibiru/inflation/v1/paramsB1Z/github.com/NibiruChain/nibiru/x/inflation/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/inflation/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/query_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from nibiru.inflation.v1 import query_pb2 as nibiru_dot_inflation_dot_v1_dot_query__pb2
+from nibiru_proto.nibiru.inflation.v1 import query_pb2 as nibiru_dot_inflation_dot_v1_dot_query__pb2
 
 
 class QueryStub(object):
     """Query provides defines the gRPC querier service.
     """
 
     def __init__(self, channel):
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/event_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/event_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from nibiru.oracle.v1 import oracle_pb2 as nibiru_dot_oracle_dot_v1_dot_oracle__pb2
+from nibiru_proto.nibiru.oracle.v1 import oracle_pb2 as nibiru_dot_oracle_dot_v1_dot_oracle__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cnibiru/oracle/v1/event.proto\x12\x10nibiru.oracle.v1\x1a\x1dnibiru/oracle/v1/oracle.proto\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\"\x8f\x01\n\x10\x45ventPriceUpdate\x12\x12\n\x04pair\x18\x01 \x01(\tR\x04pair\x12\x44\n\x05price\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x05price\x12!\n\x0ctimestamp_ms\x18\x03 \x01(\x03R\x0btimestampMs\"R\n\x1a\x45ventDelegateFeederConsent\x12\x1c\n\tvalidator\x18\x01 \x01(\tR\tvalidator\x12\x16\n\x06\x66\x65\x65\x64\x65r\x18\x02 \x01(\tR\x06\x66\x65\x65\x64\x65r\"\xa3\x01\n\x12\x45ventAggregateVote\x12\x1c\n\tvalidator\x18\x01 \x01(\tR\tvalidator\x12\x16\n\x06\x66\x65\x65\x64\x65r\x18\x02 \x01(\tR\x06\x66\x65\x65\x64\x65r\x12W\n\x06prices\x18\x03 \x03(\x0b\x32#.nibiru.oracle.v1.ExchangeRateTupleB\x1a\xc8\xde\x1f\x00\xaa\xdf\x1f\x12\x45xchangeRateTuplesR\x06prices\"M\n\x15\x45ventAggregatePrevote\x12\x1c\n\tvalidator\x18\x01 \x01(\tR\tvalidator\x12\x16\n\x06\x66\x65\x65\x64\x65r\x18\x02 \x01(\tR\x06\x66\x65\x65\x64\x65rB.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/event_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/genesis_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from nibiru.oracle.v1 import oracle_pb2 as nibiru_dot_oracle_dot_v1_dot_oracle__pb2
+from nibiru_proto.nibiru.oracle.v1 import oracle_pb2 as nibiru_dot_oracle_dot_v1_dot_oracle__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1enibiru/oracle/v1/genesis.proto\x12\x10nibiru.oracle.v1\x1a\x14gogoproto/gogo.proto\x1a\x1dnibiru/oracle/v1/oracle.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"\xd2\x05\n\x0cGenesisState\x12\x36\n\x06params\x18\x01 \x01(\x0b\x32\x18.nibiru.oracle.v1.ParamsB\x04\xc8\xde\x1f\x00R\x06params\x12W\n\x12\x66\x65\x65\x64\x65r_delegations\x18\x02 \x03(\x0b\x32\".nibiru.oracle.v1.FeederDelegationB\x04\xc8\xde\x1f\x00R\x11\x66\x65\x65\x64\x65rDelegations\x12\x66\n\x0e\x65xchange_rates\x18\x03 \x03(\x0b\x32#.nibiru.oracle.v1.ExchangeRateTupleB\x1a\xc8\xde\x1f\x00\xaa\xdf\x1f\x12\x45xchangeRateTuplesR\rexchangeRates\x12H\n\rmiss_counters\x18\x04 \x03(\x0b\x32\x1d.nibiru.oracle.v1.MissCounterB\x04\xc8\xde\x1f\x00R\x0cmissCounters\x12}\n aggregate_exchange_rate_prevotes\x18\x05 \x03(\x0b\x32..nibiru.oracle.v1.AggregateExchangeRatePrevoteB\x04\xc8\xde\x1f\x00R\x1d\x61ggregateExchangeRatePrevotes\x12t\n\x1d\x61ggregate_exchange_rate_votes\x18\x06 \x03(\x0b\x32+.nibiru.oracle.v1.AggregateExchangeRateVoteB\x04\xc8\xde\x1f\x00R\x1a\x61ggregateExchangeRateVotes\x12O\n\x05pairs\x18\x07 \x03(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x05pairs\x12\x39\n\x07rewards\x18\x08 \x03(\x0b\x32\x19.nibiru.oracle.v1.RewardsB\x04\xc8\xde\x1f\x00R\x07rewards\"f\n\x10\x46\x65\x65\x64\x65rDelegation\x12%\n\x0e\x66\x65\x65\x64\x65r_address\x18\x01 \x01(\tR\rfeederAddress\x12+\n\x11validator_address\x18\x02 \x01(\tR\x10validatorAddress\"]\n\x0bMissCounter\x12+\n\x11validator_address\x18\x01 \x01(\tR\x10validatorAddress\x12!\n\x0cmiss_counter\x18\x02 \x01(\x04R\x0bmissCounterB.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.oracle.v1.genesis_pb2', globals())
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/oracle_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/oracle_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/oracle_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/oracle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/query_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from nibiru.oracle.v1 import oracle_pb2 as nibiru_dot_oracle_dot_v1_dot_oracle__pb2
+from nibiru_proto.nibiru.oracle.v1 import oracle_pb2 as nibiru_dot_oracle_dot_v1_dot_oracle__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cnibiru/oracle/v1/query.proto\x12\x10nibiru.oracle.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1dnibiru/oracle/v1/oracle.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"s\n\x18QueryExchangeRateRequest\x12M\n\x04pair\x18\x01 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair:\x08\x88\xa0\x1f\x00\xe8\xa0\x1f\x00\"p\n\x19QueryExchangeRateResponse\x12S\n\rexchange_rate\x18\x01 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0c\x65xchangeRate\"\x1b\n\x19QueryExchangeRatesRequest\"\x84\x01\n\x1aQueryExchangeRatesResponse\x12\x66\n\x0e\x65xchange_rates\x18\x01 \x03(\x0b\x32#.nibiru.oracle.v1.ExchangeRateTupleB\x1a\xc8\xde\x1f\x00\xaa\xdf\x1f\x12\x45xchangeRateTuplesR\rexchangeRates\"\x15\n\x13QueryActivesRequest\"k\n\x14QueryActivesResponse\x12S\n\x07\x61\x63tives\x18\x01 \x03(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x07\x61\x63tives\"\x19\n\x17QueryVoteTargetsRequest\"x\n\x18QueryVoteTargetsResponse\x12\\\n\x0cvote_targets\x18\x01 \x03(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x0bvoteTargets\"O\n\x1cQueryFeederDelegationRequest\x12%\n\x0evalidator_addr\x18\x01 \x01(\tR\rvalidatorAddr:\x08\x88\xa0\x1f\x00\xe8\xa0\x1f\x00\"@\n\x1dQueryFeederDelegationResponse\x12\x1f\n\x0b\x66\x65\x65\x64\x65r_addr\x18\x01 \x01(\tR\nfeederAddr\"J\n\x17QueryMissCounterRequest\x12%\n\x0evalidator_addr\x18\x01 \x01(\tR\rvalidatorAddr:\x08\x88\xa0\x1f\x00\xe8\xa0\x1f\x00\"=\n\x18QueryMissCounterResponse\x12!\n\x0cmiss_counter\x18\x01 \x01(\x04R\x0bmissCounter\"O\n\x1cQueryAggregatePrevoteRequest\x12%\n\x0evalidator_addr\x18\x01 \x01(\tR\rvalidatorAddr:\x08\x88\xa0\x1f\x00\xe8\xa0\x1f\x00\"\x82\x01\n\x1dQueryAggregatePrevoteResponse\x12\x61\n\x11\x61ggregate_prevote\x18\x01 \x01(\x0b\x32..nibiru.oracle.v1.AggregateExchangeRatePrevoteB\x04\xc8\xde\x1f\x00R\x10\x61ggregatePrevote\"\x1f\n\x1dQueryAggregatePrevotesRequest\"\x85\x01\n\x1eQueryAggregatePrevotesResponse\x12\x63\n\x12\x61ggregate_prevotes\x18\x01 \x03(\x0b\x32..nibiru.oracle.v1.AggregateExchangeRatePrevoteB\x04\xc8\xde\x1f\x00R\x11\x61ggregatePrevotes\"L\n\x19QueryAggregateVoteRequest\x12%\n\x0evalidator_addr\x18\x01 \x01(\tR\rvalidatorAddr:\x08\x88\xa0\x1f\x00\xe8\xa0\x1f\x00\"v\n\x1aQueryAggregateVoteResponse\x12X\n\x0e\x61ggregate_vote\x18\x01 \x01(\x0b\x32+.nibiru.oracle.v1.AggregateExchangeRateVoteB\x04\xc8\xde\x1f\x00R\raggregateVote\"\x1c\n\x1aQueryAggregateVotesRequest\"y\n\x1bQueryAggregateVotesResponse\x12Z\n\x0f\x61ggregate_votes\x18\x01 \x03(\x0b\x32+.nibiru.oracle.v1.AggregateExchangeRateVoteB\x04\xc8\xde\x1f\x00R\x0e\x61ggregateVotes\"\x14\n\x12QueryParamsRequest\"M\n\x13QueryParamsResponse\x12\x36\n\x06params\x18\x01 \x01(\x0b\x32\x18.nibiru.oracle.v1.ParamsB\x04\xc8\xde\x1f\x00R\x06params2\xc2\x0f\n\x05Query\x12\x95\x01\n\x0c\x45xchangeRate\x12*.nibiru.oracle.v1.QueryExchangeRateRequest\x1a+.nibiru.oracle.v1.QueryExchangeRateResponse\",\x82\xd3\xe4\x93\x02&\x12$/nibiru/oracle/v1beta1/exchange_rate\x12\x9e\x01\n\x10\x45xchangeRateTwap\x12*.nibiru.oracle.v1.QueryExchangeRateRequest\x1a+.nibiru.oracle.v1.QueryExchangeRateResponse\"1\x82\xd3\xe4\x93\x02+\x12)/nibiru/oracle/v1beta1/exchange_rate_twap\x12\x9f\x01\n\rExchangeRates\x12+.nibiru.oracle.v1.QueryExchangeRatesRequest\x1a,.nibiru.oracle.v1.QueryExchangeRatesResponse\"3\x82\xd3\xe4\x93\x02-\x12+/nibiru/oracle/v1beta1/pairs/exchange_rates\x12\x86\x01\n\x07\x41\x63tives\x12%.nibiru.oracle.v1.QueryActivesRequest\x1a&.nibiru.oracle.v1.QueryActivesResponse\",\x82\xd3\xe4\x93\x02&\x12$/nibiru/oracle/v1beta1/pairs/actives\x12\x97\x01\n\x0bVoteTargets\x12).nibiru.oracle.v1.QueryVoteTargetsRequest\x1a*.nibiru.oracle.v1.QueryVoteTargetsResponse\"1\x82\xd3\xe4\x93\x02+\x12)/nibiru/oracle/v1beta1/pairs/vote_targets\x12\xb6\x01\n\x10\x46\x65\x65\x64\x65rDelegation\x12..nibiru.oracle.v1.QueryFeederDelegationRequest\x1a/.nibiru.oracle.v1.QueryFeederDelegationResponse\"A\x82\xd3\xe4\x93\x02;\x12\x39/nibiru/oracle/v1beta1/validators/{validator_addr}/feeder\x12\xa5\x01\n\x0bMissCounter\x12).nibiru.oracle.v1.QueryMissCounterRequest\x1a*.nibiru.oracle.v1.QueryMissCounterResponse\"?\x82\xd3\xe4\x93\x02\x39\x12\x37/nibiru/oracle/v1beta1/validators/{validator_addr}/miss\x12\xc1\x01\n\x10\x41ggregatePrevote\x12..nibiru.oracle.v1.QueryAggregatePrevoteRequest\x1a/.nibiru.oracle.v1.QueryAggregatePrevoteResponse\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/nibiru/oracle/v1beta1/validators/{validator_addr}/aggregate_prevote\x12\xb4\x01\n\x11\x41ggregatePrevotes\x12/.nibiru.oracle.v1.QueryAggregatePrevotesRequest\x1a\x30.nibiru.oracle.v1.QueryAggregatePrevotesResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/nibiru/oracle/v1beta1/validators/aggregate_prevotes\x12\xb5\x01\n\rAggregateVote\x12+.nibiru.oracle.v1.QueryAggregateVoteRequest\x1a,.nibiru.oracle.v1.QueryAggregateVoteResponse\"I\x82\xd3\xe4\x93\x02\x43\x12\x41/nibiru/oracle/v1beta1/valdiators/{validator_addr}/aggregate_vote\x12\xa8\x01\n\x0e\x41ggregateVotes\x12,.nibiru.oracle.v1.QueryAggregateVotesRequest\x1a-.nibiru.oracle.v1.QueryAggregateVotesResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/nibiru/oracle/v1beta1/validators/aggregate_votes\x12|\n\x06Params\x12$.nibiru.oracle.v1.QueryParamsRequest\x1a%.nibiru.oracle.v1.QueryParamsResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/nibiru/oracle/v1beta1/paramsB.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.oracle.v1.query_pb2', globals())
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/query_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from nibiru.oracle.v1 import query_pb2 as nibiru_dot_oracle_dot_v1_dot_query__pb2
+from nibiru_proto.nibiru.oracle.v1 import query_pb2 as nibiru_dot_oracle_dot_v1_dot_query__pb2
 
 
 class QueryStub(object):
     """Query defines the gRPC querier service.
     """
 
     def __init__(self, channel):
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/state_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/state_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from nibiru.oracle.v1 import oracle_pb2 as nibiru_dot_oracle_dot_v1_dot_oracle__pb2
+from nibiru_proto.nibiru.oracle.v1 import oracle_pb2 as nibiru_dot_oracle_dot_v1_dot_oracle__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cnibiru/oracle/v1/state.proto\x12\x10nibiru.oracle.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1dnibiru/oracle/v1/oracle.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"\xd6\x01\n\rPriceSnapshot\x12\\\n\x04pair\x18\x01 \x01(\tBH\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xf2\xde\x1f\x0byaml:\"pair\"R\x04pair\x12\x44\n\x05price\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x05price\x12!\n\x0ctimestamp_ms\x18\x03 \x01(\x03R\x0btimestampMsB.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.oracle.v1.state_pb2', globals())
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/state_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/oracle/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/tx_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from nibiru.oracle.v1 import tx_pb2 as nibiru_dot_oracle_dot_v1_dot_tx__pb2
+from nibiru_proto.nibiru.oracle.v1 import tx_pb2 as nibiru_dot_oracle_dot_v1_dot_tx__pb2
 
 
 class MsgStub(object):
     """Msg defines the oracle Msg service.
     """
 
     def __init__(self, channel):
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/event_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/event_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
-from nibiru.perp.v2 import state_pb2 as nibiru_dot_perp_dot_v2_dot_state__pb2
+from nibiru_proto.nibiru.perp.v2 import state_pb2 as nibiru_dot_perp_dot_v2_dot_state__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1anibiru/perp/v2/event.proto\x12\x0enibiru.perp.v2\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x1anibiru/perp/v2/state.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xba\x05\n\x14PositionChangedEvent\x12\x45\n\x0e\x66inal_position\x18\x01 \x01(\x0b\x32\x18.nibiru.perp.v2.PositionB\x04\xc8\xde\x1f\x00R\rfinalPosition\x12[\n\x11position_notional\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x10positionNotional\x12\x62\n\x0ftransaction_fee\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x1e\xc8\xde\x1f\x00\xf2\xde\x1f\x16yaml:\"transaction_fee\"R\x0etransactionFee\x12Q\n\x0crealized_pnl\x18\x04 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0brealizedPnl\x12:\n\x08\x62\x61\x64_debt\x18\x05 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x07\x62\x61\x64\x44\x65\x62t\x12W\n\x0f\x66unding_payment\x18\x06 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12!\n\x0c\x62lock_height\x18\x07 \x01(\x03R\x0b\x62lockHeight\x12T\n\x0emargin_to_user\x18\x08 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.IntR\x0cmarginToUser\x12\x39\n\rchange_reason\x18\t \x01(\tB\x14\xc8\xde\x1f\x00\xda\xde\x1f\x0c\x43hangeReasonR\x0c\x63hangeReason\"\x87\x03\n\x17PositionLiquidatedEvent\x12`\n\x16position_changed_event\x18\x01 \x01(\x0b\x32$.nibiru.perp.v2.PositionChangedEventB\x04\xc8\xde\x1f\x00R\x14positionChangedEvent\x12-\n\x12liquidator_address\x18\x02 \x01(\tR\x11liquidatorAddress\x12g\n\x11\x66\x65\x65_to_liquidator\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB \xc8\xde\x1f\x00\xf2\xde\x1f\x18yaml:\"fee_to_liquidator\"R\x0f\x66\x65\x65ToLiquidator\x12r\n\x15\x66\x65\x65_to_ecosystem_fund\x18\x04 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB$\xc8\xde\x1f\x00\xf2\xde\x1f\x1cyaml:\"fee_to_ecosystem_fund\"R\x12\x66\x65\x65ToEcosystemFund\"\x97\x02\n\x14PositionSettledEvent\x12M\n\x04pair\x18\x01 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12%\n\x0etrader_address\x18\x02 \x01(\tR\rtraderAddress\x12\x88\x01\n\rsettled_coins\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinBH\xc8\xde\x1f\x00\xf2\xde\x1f\x14yaml:\"settled_coins\"\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.CoinsR\x0csettledCoins\"\xe5\x03\n\x17\x46undingRateChangedEvent\x12M\n\x04pair\x18\x01 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12V\n\x0fmark_price_twap\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\rmarkPriceTwap\x12X\n\x10index_price_twap\x18\x03 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0eindexPriceTwap\x12Y\n\x10premium_fraction\x18\x05 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0fpremiumFraction\x12n\n\x1b\x63umulative_premium_fraction\x18\x06 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x19\x63umulativePremiumFraction\"\xe9\x02\n\x16LiquidationFailedEvent\x12M\n\x04pair\x18\x01 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12\x16\n\x06trader\x18\x02 \x01(\tR\x06trader\x12\x1e\n\nliquidator\x18\x03 \x01(\tR\nliquidator\x12V\n\x06reason\x18\x04 \x01(\x0e\x32>.nibiru.perp.v2.LiquidationFailedEvent.LiquidationFailedReasonR\x06reason\"p\n\x17LiquidationFailedReason\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x14\n\x10POSITION_HEALTHY\x10\x01\x12\x14\n\x10NONEXISTENT_PAIR\x10\x02\x12\x18\n\x14NONEXISTENT_POSITION\x10\x03\"\xfb\x01\n\x0f\x41mmUpdatedEvent\x12\x36\n\tfinal_amm\x18\x01 \x01(\x0b\x32\x13.nibiru.perp.v2.AMMB\x04\xc8\xde\x1f\x00R\x08\x66inalAmm\x12V\n\x0fmark_price_twap\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\rmarkPriceTwap\x12X\n\x10index_price_twap\x18\x03 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0eindexPriceTwap\"U\n\x12MarketUpdatedEvent\x12?\n\x0c\x66inal_market\x18\x01 \x01(\x0b\x32\x16.nibiru.perp.v2.MarketB\x04\xc8\xde\x1f\x00R\x0b\x66inalMarketB/Z-github.com/NibiruChain/nibiru/x/perp/v2/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.perp.v2.event_pb2', globals())
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/event_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/genesis_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
-from nibiru.perp.v2 import state_pb2 as nibiru_dot_perp_dot_v2_dot_state__pb2
+from nibiru_proto.nibiru.perp.v2 import state_pb2 as nibiru_dot_perp_dot_v2_dot_state__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cnibiru/perp/v2/genesis.proto\x12\x0enibiru.perp.v2\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x1anibiru/perp/v2/state.proto\"\x87\x02\n\x0cGenesisState\x12\x36\n\x07markets\x18\x02 \x03(\x0b\x32\x16.nibiru.perp.v2.MarketB\x04\xc8\xde\x1f\x00R\x07markets\x12-\n\x04\x61mms\x18\x03 \x03(\x0b\x32\x13.nibiru.perp.v2.AMMB\x04\xc8\xde\x1f\x00R\x04\x61mms\x12<\n\tpositions\x18\x04 \x03(\x0b\x32\x18.nibiru.perp.v2.PositionB\x04\xc8\xde\x1f\x00R\tpositions\x12R\n\x11reserve_snapshots\x18\x05 \x03(\x0b\x32\x1f.nibiru.perp.v2.ReserveSnapshotB\x04\xc8\xde\x1f\x00R\x10reserveSnapshotsB/Z-github.com/NibiruChain/nibiru/x/perp/v2/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.perp.v2.genesis_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/query_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from nibiru.perp.v2 import state_pb2 as nibiru_dot_perp_dot_v2_dot_state__pb2
+from nibiru_proto.nibiru.perp.v2 import state_pb2 as nibiru_dot_perp_dot_v2_dot_state__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1anibiru/perp/v2/query.proto\x12\x0enibiru.perp.v2\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1anibiru/perp/v2/state.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"/\n\x15QueryPositionsRequest\x12\x16\n\x06trader\x18\x01 \x01(\tR\x06trader\"c\n\x16QueryPositionsResponse\x12I\n\tpositions\x18\x01 \x03(\x0b\x32%.nibiru.perp.v2.QueryPositionResponseB\x04\xc8\xde\x1f\x00R\tpositions\"}\n\x14QueryPositionRequest\x12M\n\x04pair\x18\x01 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12\x16\n\x06trader\x18\x02 \x01(\tR\x06trader\"\xda\x02\n\x15QueryPositionResponse\x12:\n\x08position\x18\x01 \x01(\x0b\x32\x18.nibiru.perp.v2.PositionB\x04\xc8\xde\x1f\x00R\x08position\x12[\n\x11position_notional\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x10positionNotional\x12U\n\x0eunrealized_pnl\x18\x03 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\runrealizedPnl\x12Q\n\x0cmargin_ratio\x18\x04 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0bmarginRatio\"\x1c\n\x1aQueryModuleAccountsRequest\"c\n\x1bQueryModuleAccountsResponse\x12\x44\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\".nibiru.perp.v2.AccountWithBalanceB\x04\xc8\xde\x1f\x00R\x08\x61\x63\x63ounts\"\xa9\x01\n\x12\x41\x63\x63ountWithBalance\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07\x61\x64\x64ress\x18\x02 \x01(\tR\x07\x61\x64\x64ress\x12\x65\n\x07\x62\x61lance\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.CoinsR\x07\x62\x61lance\"n\n\tAmmMarket\x12\x34\n\x06market\x18\x01 \x01(\x0b\x32\x16.nibiru.perp.v2.MarketB\x04\xc8\xde\x1f\x00R\x06market\x12+\n\x03\x61mm\x18\x02 \x01(\x0b\x32\x13.nibiru.perp.v2.AMMB\x04\xc8\xde\x1f\x00R\x03\x61mm\"\x15\n\x13QueryMarketsRequest\"X\n\x14QueryMarketsResponse\x12@\n\x0b\x61mm_markets\x18\x01 \x03(\x0b\x32\x19.nibiru.perp.v2.AmmMarketB\x04\xc8\xde\x1f\x00R\nammMarkets2\x9d\x04\n\x05Query\x12~\n\rQueryPosition\x12$.nibiru.perp.v2.QueryPositionRequest\x1a%.nibiru.perp.v2.QueryPositionResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/nibiru/perp/v2/position\x12\x82\x01\n\x0eQueryPositions\x12%.nibiru.perp.v2.QueryPositionsRequest\x1a&.nibiru.perp.v2.QueryPositionsResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/nibiru/perp/v2/positions\x12\x92\x01\n\x0eModuleAccounts\x12*.nibiru.perp.v2.QueryModuleAccountsRequest\x1a+.nibiru.perp.v2.QueryModuleAccountsResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/nibiru/perp/v2/module_accounts\x12z\n\x0cQueryMarkets\x12#.nibiru.perp.v2.QueryMarketsRequest\x1a$.nibiru.perp.v2.QueryMarketsResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/nibiru/perp/v2/marketsB/Z-github.com/NibiruChain/nibiru/x/perp/v2/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.perp.v2.query_pb2', globals())
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/query_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from nibiru.perp.v2 import query_pb2 as nibiru_dot_perp_dot_v2_dot_query__pb2
+from nibiru_proto.nibiru.perp.v2 import query_pb2 as nibiru_dot_perp_dot_v2_dot_query__pb2
 
 
 class QueryStub(object):
     """Query defines the gRPC querier service.
     """
 
     def __init__(self, channel):
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/state_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/state_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/state_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/tx_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from nibiru.perp.v2 import state_pb2 as nibiru_dot_perp_dot_v2_dot_state__pb2
+from nibiru_proto.nibiru.perp.v2 import state_pb2 as nibiru_dot_perp_dot_v2_dot_state__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17nibiru/perp/v2/tx.proto\x12\x0enibiru.perp.v2\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x1anibiru/perp/v2/state.proto\"\xb1\x01\n\x0fMsgRemoveMargin\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12\x37\n\x06margin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x06margin\"\xe8\x01\n\x17MsgRemoveMarginResponse\x12>\n\nmargin_out\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\tmarginOut\x12W\n\x0f\x66unding_payment\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12\x34\n\x08position\x18\x03 \x01(\x0b\x32\x18.nibiru.perp.v2.PositionR\x08position\"\xae\x01\n\x0cMsgAddMargin\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12\x37\n\x06margin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x06margin\"\xa5\x01\n\x14MsgAddMarginResponse\x12W\n\x0f\x66unding_payment\x18\x01 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12\x34\n\x08position\x18\x02 \x01(\x0b\x32\x18.nibiru.perp.v2.PositionR\x08position\"\xf4\x01\n\x11MsgMultiLiquidate\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12Q\n\x0cliquidations\x18\x02 \x03(\x0b\x32-.nibiru.perp.v2.MsgMultiLiquidate.LiquidationR\x0cliquidations\x1at\n\x0bLiquidation\x12M\n\x04pair\x18\x01 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12\x16\n\x06trader\x18\x02 \x01(\tR\x06trader\"\xb6\x03\n\x19MsgMultiLiquidateResponse\x12\x61\n\x0cliquidations\x18\x01 \x03(\x0b\x32=.nibiru.perp.v2.MsgMultiLiquidateResponse.LiquidationResponseR\x0cliquidations\x1a\xb5\x02\n\x13LiquidationResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x02 \x01(\tR\x05\x65rror\x12\x46\n\x0eliquidator_fee\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x01R\rliquidatorFee\x12?\n\x0bperp_ef_fee\x18\x04 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x01R\tperpEfFee\x12\x16\n\x06trader\x18\x05 \x01(\tR\x06trader\x12M\n\x04pair\x18\x06 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\"\xb7\x03\n\x0eMsgMarketOrder\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12-\n\x04side\x18\x03 \x01(\x0e\x32\x19.nibiru.perp.v2.DirectionR\x04side\x12\\\n\x12quote_asset_amount\x18\x04 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.IntR\x10quoteAssetAmount\x12J\n\x08leverage\x18\x05 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x08leverage\x12\x65\n\x17\x62\x61se_asset_amount_limit\x18\x06 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.IntR\x14\x62\x61seAssetAmountLimit\"\xe3\x05\n\x16MsgMarketOrderResponse\x12\x34\n\x08position\x18\x01 \x01(\x0b\x32\x18.nibiru.perp.v2.PositionR\x08position\x12h\n\x18\x65xchanged_notional_value\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x16\x65xchangedNotionalValue\x12\x66\n\x17\x65xchanged_position_size\x18\x03 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x15\x65xchangedPositionSize\x12W\n\x0f\x66unding_payment\x18\x04 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12Q\n\x0crealized_pnl\x18\x05 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0brealizedPnl\x12`\n\x14unrealized_pnl_after\x18\x06 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x12unrealizedPnlAfter\x12V\n\x0fmargin_to_vault\x18\x07 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\rmarginToVault\x12[\n\x11position_notional\x18\x08 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x10positionNotional\"y\n\x10MsgClosePosition\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\"\xf2\x03\n\x18MsgClosePositionResponse\x12h\n\x18\x65xchanged_notional_value\x18\x01 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x16\x65xchangedNotionalValue\x12\x66\n\x17\x65xchanged_position_size\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x15\x65xchangedPositionSize\x12W\n\x0f\x66unding_payment\x18\x03 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12Q\n\x0crealized_pnl\x18\x04 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0brealizedPnl\x12X\n\x10margin_to_trader\x18\x07 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0emarginToTrader\"\x82\x01\n\x18MsgDonateToEcosystemFund\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12N\n\x08\x64onation\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x17\xc8\xde\x1f\x00\xf2\xde\x1f\x0fyaml:\"donation\"R\x08\x64onation\"\"\n MsgDonateToEcosystemFundResponse2\xc5\x04\n\x03Msg\x12Z\n\x0cRemoveMargin\x12\x1f.nibiru.perp.v2.MsgRemoveMargin\x1a\'.nibiru.perp.v2.MsgRemoveMarginResponse\"\x00\x12Q\n\tAddMargin\x12\x1c.nibiru.perp.v2.MsgAddMargin\x1a$.nibiru.perp.v2.MsgAddMarginResponse\"\x00\x12`\n\x0eMultiLiquidate\x12!.nibiru.perp.v2.MsgMultiLiquidate\x1a).nibiru.perp.v2.MsgMultiLiquidateResponse\"\x00\x12W\n\x0bMarketOrder\x12\x1e.nibiru.perp.v2.MsgMarketOrder\x1a&.nibiru.perp.v2.MsgMarketOrderResponse\"\x00\x12]\n\rClosePosition\x12 .nibiru.perp.v2.MsgClosePosition\x1a(.nibiru.perp.v2.MsgClosePositionResponse\"\x00\x12u\n\x15\x44onateToEcosystemFund\x12(.nibiru.perp.v2.MsgDonateToEcosystemFund\x1a\x30.nibiru.perp.v2.MsgDonateToEcosystemFundResponse\"\x00\x42/Z-github.com/NibiruChain/nibiru/x/perp/v2/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.perp.v2.tx_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/perp/v2/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/tx_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from nibiru.perp.v2 import tx_pb2 as nibiru_dot_perp_dot_v2_dot_tx__pb2
+from nibiru_proto.nibiru.perp.v2 import tx_pb2 as nibiru_dot_perp_dot_v2_dot_tx__pb2
 
 
 class MsgStub(object):
     """Msg defines the x/perp Msg service.
     """
 
     def __init__(self, channel):
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/event_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/event_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
-from nibiru.spot.v1 import pool_pb2 as nibiru_dot_spot_dot_v1_dot_pool__pb2
+from nibiru_proto.nibiru.spot.v1 import pool_pb2 as nibiru_dot_spot_dot_v1_dot_pool__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1anibiru/spot/v1/event.proto\x12\x0enibiru.spot.v1\x1a\x14gogoproto/gogo.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x19nibiru/spot/v1/pool.proto\"\xf2\x01\n\x10\x45ventPoolCreated\x12\x18\n\x07\x63reator\x18\x01 \x01(\tR\x07\x63reator\x12\x33\n\x04\x66\x65\x65s\x18\x02 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x04\x66\x65\x65s\x12\x39\n\nfinal_pool\x18\x04 \x01(\x0b\x32\x14.nibiru.spot.v1.PoolB\x04\xc8\xde\x1f\x00R\tfinalPool\x12T\n\x16\x66inal_user_pool_shares\x18\x05 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x13\x66inalUserPoolShares\"\x81\x03\n\x0f\x45ventPoolJoined\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\x12<\n\ttokens_in\x18\x02 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x08tokensIn\x12G\n\x0fpool_shares_out\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\rpoolSharesOut\x12<\n\trem_coins\x18\x04 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x08remCoins\x12\x39\n\nfinal_pool\x18\x05 \x01(\x0b\x32\x14.nibiru.spot.v1.PoolB\x04\xc8\xde\x1f\x00R\tfinalPool\x12T\n\x16\x66inal_user_pool_shares\x18\x06 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x13\x66inalUserPoolShares\"\xf8\x02\n\x0f\x45ventPoolExited\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\x12\x45\n\x0epool_shares_in\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x0cpoolSharesIn\x12>\n\ntokens_out\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\ttokensOut\x12\x33\n\x04\x66\x65\x65s\x18\x04 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x04\x66\x65\x65s\x12\x39\n\nfinal_pool\x18\x05 \x01(\x0b\x32\x14.nibiru.spot.v1.PoolB\x04\xc8\xde\x1f\x00R\tfinalPool\x12T\n\x16\x66inal_user_pool_shares\x18\x06 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x13\x66inalUserPoolShares\"\x96\x02\n\x12\x45ventAssetsSwapped\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\x12:\n\x08token_in\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x07tokenIn\x12<\n\ttoken_out\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x08tokenOut\x12\x31\n\x03\x66\x65\x65\x18\x04 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x03\x66\x65\x65\x12\x39\n\nfinal_pool\x18\x05 \x01(\x0b\x32\x14.nibiru.spot.v1.PoolB\x04\xc8\xde\x1f\x00R\tfinalPoolB,Z*github.com/NibiruChain/nibiru/x/spot/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.spot.v1.event_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/event_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/genesis_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from nibiru.spot.v1 import params_pb2 as nibiru_dot_spot_dot_v1_dot_params__pb2
-from nibiru.spot.v1 import pool_pb2 as nibiru_dot_spot_dot_v1_dot_pool__pb2
+from nibiru_proto.nibiru.spot.v1 import params_pb2 as nibiru_dot_spot_dot_v1_dot_params__pb2
+from nibiru_proto.nibiru.spot.v1 import pool_pb2 as nibiru_dot_spot_dot_v1_dot_pool__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cnibiru/spot/v1/genesis.proto\x12\x0enibiru.spot.v1\x1a\x1bnibiru/spot/v1/params.proto\x1a\x19nibiru/spot/v1/pool.proto\x1a\x14gogoproto/gogo.proto\"v\n\x0cGenesisState\x12\x34\n\x06params\x18\x01 \x01(\x0b\x32\x16.nibiru.spot.v1.ParamsB\x04\xc8\xde\x1f\x00R\x06params\x12\x30\n\x05pools\x18\x02 \x03(\x0b\x32\x14.nibiru.spot.v1.PoolB\x04\xc8\xde\x1f\x00R\x05poolsB,Z*github.com/NibiruChain/nibiru/x/spot/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.spot.v1.genesis_pb2', globals())
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/params_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/params_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/pool_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/pool_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/pool_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/pool_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/query_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from cosmos.base.query.v1beta1 import pagination_pb2 as cosmos_dot_base_dot_query_dot_v1beta1_dot_pagination__pb2
-from nibiru.spot.v1 import params_pb2 as nibiru_dot_spot_dot_v1_dot_params__pb2
-from nibiru.spot.v1 import pool_pb2 as nibiru_dot_spot_dot_v1_dot_pool__pb2
+from nibiru_proto.nibiru.spot.v1 import params_pb2 as nibiru_dot_spot_dot_v1_dot_params__pb2
+from nibiru_proto.nibiru.spot.v1 import pool_pb2 as nibiru_dot_spot_dot_v1_dot_pool__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1anibiru/spot/v1/query.proto\x12\x0enibiru.spot.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a*cosmos/base/query/v1beta1/pagination.proto\x1a\x1bnibiru/spot/v1/params.proto\x1a\x19nibiru/spot/v1/pool.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"\x14\n\x12QueryParamsRequest\"K\n\x13QueryParamsResponse\x12\x34\n\x06params\x18\x01 \x01(\x0b\x32\x16.nibiru.spot.v1.ParamsB\x04\xc8\xde\x1f\x00R\x06params\"\x18\n\x16QueryPoolNumberRequest\"2\n\x17QueryPoolNumberResponse\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\"+\n\x10QueryPoolRequest\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\"=\n\x11QueryPoolResponse\x12(\n\x04pool\x18\x01 \x01(\x0b\x32\x14.nibiru.spot.v1.PoolR\x04pool\"[\n\x11QueryPoolsRequest\x12\x46\n\npagination\x18\x01 \x01(\x0b\x32&.cosmos.base.query.v1beta1.PageRequestR\npagination\"\x89\x01\n\x12QueryPoolsResponse\x12*\n\x05pools\x18\x01 \x03(\x0b\x32\x14.nibiru.spot.v1.PoolR\x05pools\x12G\n\npagination\x18\x02 \x01(\x0b\x32\'.cosmos.base.query.v1beta1.PageResponseR\npagination\"1\n\x16QueryPoolParamsRequest\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\"V\n\x17QueryPoolParamsResponse\x12;\n\x0bpool_params\x18\x01 \x01(\x0b\x32\x1a.nibiru.spot.v1.PoolParamsR\npoolParams\"\x16\n\x14QueryNumPoolsRequest\"4\n\x15QueryNumPoolsResponse\x12\x1b\n\tnum_pools\x18\x01 \x01(\x04R\x08numPools\"\x1c\n\x1aQueryTotalLiquidityRequest\"\x9c\x01\n\x1bQueryTotalLiquidityResponse\x12}\n\tliquidity\x18\x01 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinBD\xc8\xde\x1f\x00\xf2\xde\x1f\x10yaml:\"liquidity\"\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.CoinsR\tliquidity\"9\n\x1eQueryTotalPoolLiquidityRequest\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\"\xa0\x01\n\x1fQueryTotalPoolLiquidityResponse\x12}\n\tliquidity\x18\x01 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinBD\xc8\xde\x1f\x00\xf2\xde\x1f\x10yaml:\"liquidity\"\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.CoinsR\tliquidity\"2\n\x17QueryTotalSharesRequest\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\"u\n\x18QueryTotalSharesResponse\x12Y\n\x0ctotal_shares\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x1b\xc8\xde\x1f\x00\xf2\xde\x1f\x13yaml:\"total_shares\"R\x0btotalShares\"~\n\x15QuerySpotPriceRequest\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\x12$\n\x0etoken_in_denom\x18\x02 \x01(\tR\x0ctokenInDenom\x12&\n\x0ftoken_out_denom\x18\x03 \x01(\tR\rtokenOutDenom\"7\n\x16QuerySpotPriceResponse\x12\x1d\n\nspot_price\x18\x01 \x01(\tR\tspotPrice\"\xaf\x01\n\x1dQuerySwapExactAmountInRequest\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\x12M\n\x08token_in\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x17\xc8\xde\x1f\x00\xf2\xde\x1f\x0fyaml:\"token_in\"R\x07tokenIn\x12&\n\x0ftoken_out_denom\x18\x03 \x01(\tR\rtokenOutDenom\"\xb3\x01\n\x1eQuerySwapExactAmountInResponse\x12P\n\ttoken_out\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x18\xc8\xde\x1f\x00\xf2\xde\x1f\x10yaml:\"token_out\"R\x08tokenOut\x12?\n\x03\x66\x65\x65\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x12\xc8\xde\x1f\x00\xf2\xde\x1f\nyaml:\"fee\"R\x03\x66\x65\x65\"\xb1\x01\n\x1eQuerySwapExactAmountOutRequest\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\x12P\n\ttoken_out\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x18\xc8\xde\x1f\x00\xf2\xde\x1f\x10yaml:\"token_out\"R\x08tokenOut\x12$\n\x0etoken_in_denom\x18\x03 \x01(\tR\x0ctokenInDenom\"p\n\x1fQuerySwapExactAmountOutResponse\x12M\n\x08token_in\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x17\xc8\xde\x1f\x00\xf2\xde\x1f\x0fyaml:\"token_in\"R\x07tokenIn\"\xb6\x01\n\x1dQueryJoinExactAmountInRequest\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\x12|\n\ttokens_in\x18\x02 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinBD\xc8\xde\x1f\x00\xf2\xde\x1f\x10yaml:\"tokens_in\"\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.CoinsR\x08tokensIn\"\x90\x02\n\x1eQueryJoinExactAmountInResponse\x12p\n\x0fpool_shares_out\x18\x01 \x01(\tBH\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xf2\xde\x1f\x16yaml:\"pool_shares_out\"R\rpoolSharesOut\x12|\n\trem_coins\x18\x02 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinBD\xc8\xde\x1f\x00\xf2\xde\x1f\x10yaml:\"rem_coins\"\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.CoinsR\x08remCoins\"9\n\x1eQueryJoinExactAmountOutRequest\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\"!\n\x1fQueryJoinExactAmountOutResponse\"\xa7\x01\n\x1dQueryExitExactAmountInRequest\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\x12m\n\x0epool_shares_in\x18\x02 \x01(\tBG\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xf2\xde\x1f\x15yaml:\"pool_shares_in\"R\x0cpoolSharesIn\"\x91\x02\n\x1eQueryExitExactAmountInResponse\x12\x7f\n\ntokens_out\x18\x01 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinBE\xc8\xde\x1f\x00\xf2\xde\x1f\x11yaml:\"tokens_out\"\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.CoinsR\ttokensOut\x12n\n\x04\x66\x65\x65s\x18\x02 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB?\xc8\xde\x1f\x00\xf2\xde\x1f\x0byaml:\"fees\"\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.CoinsR\x04\x66\x65\x65s\"9\n\x1eQueryExitExactAmountOutRequest\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\"!\n\x1fQueryExitExactAmountOutResponse2\xa5\x13\n\x05Query\x12n\n\x06Params\x12\".nibiru.spot.v1.QueryParamsRequest\x1a#.nibiru.spot.v1.QueryParamsResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/nibiru/spot/params\x12\x7f\n\nPoolNumber\x12&.nibiru.spot.v1.QueryPoolNumberRequest\x1a\'.nibiru.spot.v1.QueryPoolNumberResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/nibiru/spot/pool_number\x12\x66\n\x04Pool\x12 .nibiru.spot.v1.QueryPoolRequest\x1a!.nibiru.spot.v1.QueryPoolResponse\"\x19\x82\xd3\xe4\x93\x02\x13\x12\x11/nibiru/spot/pool\x12j\n\x05Pools\x12!.nibiru.spot.v1.QueryPoolsRequest\x1a\".nibiru.spot.v1.QueryPoolsResponse\"\x1a\x82\xd3\xe4\x93\x02\x14\x12\x12/nibiru/spot/pools\x12\x8a\x01\n\nPoolParams\x12&.nibiru.spot.v1.QueryPoolParamsRequest\x1a\'.nibiru.spot.v1.QueryPoolParamsResponse\"+\x82\xd3\xe4\x93\x02%\x12#/nibiru/spot/pools/{pool_id}/params\x12w\n\x08NumPools\x12$.nibiru.spot.v1.QueryNumPoolsRequest\x1a%.nibiru.spot.v1.QueryNumPoolsResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/nibiru/spot/num_pools\x12\x8f\x01\n\x0eTotalLiquidity\x12*.nibiru.spot.v1.QueryTotalLiquidityRequest\x1a+.nibiru.spot.v1.QueryTotalLiquidityResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/nibiru/spot/total_liquidity\x12\xb0\x01\n\x12TotalPoolLiquidity\x12..nibiru.spot.v1.QueryTotalPoolLiquidityRequest\x1a/.nibiru.spot.v1.QueryTotalPoolLiquidityResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/nibiru/spot/pools/{pool_id}/total_pool_liquidity\x12\x93\x01\n\x0bTotalShares\x12\'.nibiru.spot.v1.QueryTotalSharesRequest\x1a(.nibiru.spot.v1.QueryTotalSharesResponse\"1\x82\xd3\xe4\x93\x02+\x12)/nibiru/spot/pools/{pool_id}/total_shares\x12\x87\x01\n\tSpotPrice\x12%.nibiru.spot.v1.QuerySpotPriceRequest\x1a&.nibiru.spot.v1.QuerySpotPriceResponse\"+\x82\xd3\xe4\x93\x02%\x12#/nibiru/spot/pools/{pool_id}/prices\x12\xb8\x01\n\x19\x45stimateSwapExactAmountIn\x12-.nibiru.spot.v1.QuerySwapExactAmountInRequest\x1a..nibiru.spot.v1.QuerySwapExactAmountInResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/nibiru/spot/{pool_id}/estimate/swap_exact_amount_in\x12\xbc\x01\n\x1a\x45stimateSwapExactAmountOut\x12..nibiru.spot.v1.QuerySwapExactAmountOutRequest\x1a/.nibiru.spot.v1.QuerySwapExactAmountOutResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/nibiru/spot/{pool_id}/estimate/swap_exact_amount_out\x12\xb8\x01\n\x19\x45stimateJoinExactAmountIn\x12-.nibiru.spot.v1.QueryJoinExactAmountInRequest\x1a..nibiru.spot.v1.QueryJoinExactAmountInResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/nibiru/spot/{pool_id}/estimate/join_exact_amount_in\x12\xbc\x01\n\x1a\x45stimateJoinExactAmountOut\x12..nibiru.spot.v1.QueryJoinExactAmountOutRequest\x1a/.nibiru.spot.v1.QueryJoinExactAmountOutResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/nibiru/spot/{pool_id}/estimate/join_exact_amount_out\x12\xb8\x01\n\x19\x45stimateExitExactAmountIn\x12-.nibiru.spot.v1.QueryExitExactAmountInRequest\x1a..nibiru.spot.v1.QueryExitExactAmountInResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/nibiru/spot/{pool_id}/estimate/exit_exact_amount_in\x12\xbc\x01\n\x1a\x45stimateExitExactAmountOut\x12..nibiru.spot.v1.QueryExitExactAmountOutRequest\x1a/.nibiru.spot.v1.QueryExitExactAmountOutResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/nibiru/spot/{pool_id}/estimate/exit_exact_amount_outB,Z*github.com/NibiruChain/nibiru/x/spot/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.spot.v1.query_pb2', globals())
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/query_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from nibiru.spot.v1 import query_pb2 as nibiru_dot_spot_dot_v1_dot_query__pb2
+from nibiru_proto.nibiru.spot.v1 import query_pb2 as nibiru_dot_spot_dot_v1_dot_query__pb2
 
 
 class QueryStub(object):
     """Query defines the gRPC querier service.
     """
 
     def __init__(self, channel):
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/tx_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from nibiru.spot.v1 import pool_pb2 as nibiru_dot_spot_dot_v1_dot_pool__pb2
+from nibiru_proto.nibiru.spot.v1 import pool_pb2 as nibiru_dot_spot_dot_v1_dot_pool__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17nibiru/spot/v1/tx.proto\x12\x0enibiru.spot.v1\x1a\x19nibiru/spot/v1/pool.proto\x1a\x14gogoproto/gogo.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x1cgoogle/api/annotations.proto\"\xc0\x01\n\rMsgCreatePool\x12\x18\n\x07\x63reator\x18\x01 \x01(\tR\x07\x63reator\x12S\n\x0bpool_params\x18\x02 \x01(\x0b\x32\x1a.nibiru.spot.v1.PoolParamsB\x16\xf2\xde\x1f\x12yaml:\"pool_params\"R\npoolParams\x12@\n\x0bpool_assets\x18\x03 \x03(\x0b\x32\x19.nibiru.spot.v1.PoolAssetB\x04\xc8\xde\x1f\x00R\npoolAssets\"0\n\x15MsgCreatePoolResponse\x12\x17\n\x07pool_id\x18\x01 \x01(\x04R\x06poolId\"\xf5\x01\n\x0bMsgJoinPool\x12)\n\x06sender\x18\x01 \x01(\tB\x11\xf2\xde\x1f\ryaml:\"sender\"R\x06sender\x12+\n\x07pool_id\x18\x02 \x01(\x04\x42\x12\xf2\xde\x1f\x0eyaml:\"pool_id\"R\x06poolId\x12P\n\ttokens_in\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x18\xc8\xde\x1f\x00\xf2\xde\x1f\x10yaml:\"tokens_in\"R\x08tokensIn\x12<\n\ruse_all_coins\x18\x04 \x01(\x08\x42\x18\xf2\xde\x1f\x14yaml:\"use_all_coins\"R\x0buseAllCoins\"\x8b\x02\n\x13MsgJoinPoolResponse\x12(\n\x04pool\x18\x01 \x01(\x0b\x32\x14.nibiru.spot.v1.PoolR\x04pool\x12l\n\x13num_pool_shares_out\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\"\xc8\xde\x1f\x00\xf2\xde\x1f\x1ayaml:\"num_pool_shares_out\"R\x10numPoolSharesOut\x12\\\n\x0fremaining_coins\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x18\xc8\xde\x1f\x00\xf2\xde\x1f\x10yaml:\"tokens_in\"R\x0eremainingCoins\"\xbd\x01\n\x0bMsgExitPool\x12)\n\x06sender\x18\x01 \x01(\tB\x11\xf2\xde\x1f\ryaml:\"sender\"R\x06sender\x12+\n\x07pool_id\x18\x02 \x01(\x04\x42\x12\xf2\xde\x1f\x0eyaml:\"pool_id\"R\x06poolId\x12V\n\x0bpool_shares\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x1a\xc8\xde\x1f\x00\xf2\xde\x1f\x12yaml:\"pool_shares\"R\npoolShares\"j\n\x13MsgExitPoolResponse\x12S\n\ntokens_out\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x19\xc8\xde\x1f\x00\xf2\xde\x1f\x11yaml:\"tokens_out\"R\ttokensOut\"\xfa\x01\n\rMsgSwapAssets\x12)\n\x06sender\x18\x01 \x01(\tB\x11\xf2\xde\x1f\ryaml:\"sender\"R\x06sender\x12+\n\x07pool_id\x18\x02 \x01(\x04\x42\x12\xf2\xde\x1f\x0eyaml:\"pool_id\"R\x06poolId\x12M\n\x08token_in\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x17\xc8\xde\x1f\x00\xf2\xde\x1f\x0fyaml:\"token_in\"R\x07tokenIn\x12\x42\n\x0ftoken_out_denom\x18\x04 \x01(\tB\x1a\xf2\xde\x1f\x16yaml:\"token_out_denom\"R\rtokenOutDenom\"i\n\x15MsgSwapAssetsResponse\x12P\n\ttoken_out\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x18\xc8\xde\x1f\x00\xf2\xde\x1f\x10yaml:\"token_out\"R\x08tokenOut2\xd3\x03\n\x03Msg\x12m\n\nCreatePool\x12\x1d.nibiru.spot.v1.MsgCreatePool\x1a%.nibiru.spot.v1.MsgCreatePoolResponse\"\x19\x82\xd3\xe4\x93\x02\x13\"\x11/nibiru/spot/pool\x12q\n\x08JoinPool\x12\x1b.nibiru.spot.v1.MsgJoinPool\x1a#.nibiru.spot.v1.MsgJoinPoolResponse\"#\x82\xd3\xe4\x93\x02\x1d\"\x1b/nibiru/spot/{pool_id}/join\x12q\n\x08\x45xitPool\x12\x1b.nibiru.spot.v1.MsgExitPool\x1a#.nibiru.spot.v1.MsgExitPoolResponse\"#\x82\xd3\xe4\x93\x02\x1d\"\x1b/nibiru/spot/{pool_id}/exit\x12w\n\nSwapAssets\x12\x1d.nibiru.spot.v1.MsgSwapAssets\x1a%.nibiru.spot.v1.MsgSwapAssetsResponse\"#\x82\xd3\xe4\x93\x02\x1d\"\x1b/nibiru/spot/{pool_id}/swapB,Z*github.com/NibiruChain/nibiru/x/spot/typesb\x06proto3')
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/spot/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/tx_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from nibiru.spot.v1 import tx_pb2 as nibiru_dot_spot_dot_v1_dot_tx__pb2
+from nibiru_proto.nibiru.spot.v1 import tx_pb2 as nibiru_dot_spot_dot_v1_dot_tx__pb2
 
 
 class MsgStub(object):
     """Msg defines the Msg service.
     """
 
     def __init__(self, channel):
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/events_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/events_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/events_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from nibiru.stablecoin.v1 import params_pb2 as nibiru_dot_stablecoin_dot_v1_dot_params__pb2
+from nibiru_proto.nibiru.stablecoin.v1 import params_pb2 as nibiru_dot_stablecoin_dot_v1_dot_params__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"nibiru/stablecoin/v1/genesis.proto\x12\x14nibiru.stablecoin.v1\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a!nibiru/stablecoin/v1/params.proto\"\xc2\x01\n\x0cGenesisState\x12:\n\x06params\x18\x01 \x01(\x0b\x32\x1c.nibiru.stablecoin.v1.ParamsB\x04\xc8\xde\x1f\x00R\x06params\x12v\n\x16module_account_balance\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB%\xc8\xde\x1f\x00\xf2\xde\x1f\x1dyaml:\"module_account_balance\"R\x14moduleAccountBalanceB2Z0github.com/NibiruChain/nibiru/x/stablecoin/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.stablecoin.v1.genesis_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/params_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/params_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/query_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from cosmos.base.query.v1beta1 import pagination_pb2 as cosmos_dot_base_dot_query_dot_v1beta1_dot_pagination__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
-from nibiru.stablecoin.v1 import params_pb2 as nibiru_dot_stablecoin_dot_v1_dot_params__pb2
+from nibiru_proto.nibiru.stablecoin.v1 import params_pb2 as nibiru_dot_stablecoin_dot_v1_dot_params__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n nibiru/stablecoin/v1/query.proto\x12\x14nibiru.stablecoin.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a*cosmos/base/query/v1beta1/pagination.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a!nibiru/stablecoin/v1/params.proto\"\x14\n\x12QueryParamsRequest\"Q\n\x13QueryParamsResponse\x12:\n\x06params\x18\x01 \x01(\x0b\x32\x1c.nibiru.stablecoin.v1.ParamsB\x04\xc8\xde\x1f\x00R\x06params\"\x1c\n\x1aQueryModuleAccountBalances\"\xba\x01\n\"QueryModuleAccountBalancesResponse\x12\x93\x01\n\x17module_account_balances\x18\x01 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB@\xc8\xde\x1f\x00\xf2\xde\x1f\x0cyaml:\"coins\"\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.CoinsR\x15moduleAccountBalances\"\x1a\n\x18QueryCirculatingSupplies\"\x8c\x01\n QueryCirculatingSuppliesResponse\x12\x33\n\x04nibi\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x04nibi\x12\x33\n\x04nusd\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x04nusd\"W\n\x14QueryGovToMintStable\x12?\n\ncollateral\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\ncollateral\"Q\n\x1cQueryGovToMintStableResponse\x12\x31\n\x03gov\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x03gov\"\x8b\x02\n\x12LiquidityRatioInfo\x12W\n\x0fliquidity_ratio\x18\x01 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0eliquidityRatio\x12M\n\nupper_band\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\tupperBand\x12M\n\nlower_band\x18\x03 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\tlowerBand\" \n\x1eQueryLiquidityRatioInfoRequest\"e\n\x1fQueryLiquidityRatioInfoResponse\x12\x42\n\x04info\x18\x01 \x01(\x0b\x32(.nibiru.stablecoin.v1.LiquidityRatioInfoB\x04\xc8\xde\x1f\x00R\x04info2\xac\x05\n\x05Query\x12\x83\x01\n\x06Params\x12(.nibiru.stablecoin.v1.QueryParamsRequest\x1a).nibiru.stablecoin.v1.QueryParamsResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/nibiru/stablecoin/v1/params\x12\xb6\x01\n\x15ModuleAccountBalances\x12\x30.nibiru.stablecoin.v1.QueryModuleAccountBalances\x1a\x38.nibiru.stablecoin.v1.QueryModuleAccountBalancesResponse\"1\x82\xd3\xe4\x93\x02+\x12)/nibiru/stablecoin/module_account_balance\x12\xae\x01\n\x13\x43irculatingSupplies\x12..nibiru.stablecoin.v1.QueryCirculatingSupplies\x1a\x36.nibiru.stablecoin.v1.QueryCirculatingSuppliesResponse\"/\x82\xd3\xe4\x93\x02)\x12\'/nibiru/stablecoin/circulating_supplies\x12\xb2\x01\n\x12LiquidityRatioInfo\x12\x34.nibiru.stablecoin.v1.QueryLiquidityRatioInfoRequest\x1a\x35.nibiru.stablecoin.v1.QueryLiquidityRatioInfoResponse\"/\x82\xd3\xe4\x93\x02)\x12\'/nibiru/stablecoin/liquidity_ratio_infoB2Z0github.com/NibiruChain/nibiru/x/stablecoin/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.stablecoin.v1.query_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/query_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from nibiru.stablecoin.v1 import query_pb2 as nibiru_dot_stablecoin_dot_v1_dot_query__pb2
+from nibiru_proto.nibiru.stablecoin.v1 import query_pb2 as nibiru_dot_stablecoin_dot_v1_dot_query__pb2
 
 
 class QueryStub(object):
     """Query defines the gRPC querier service.
     """
 
     def __init__(self, channel):
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/stablecoin/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/tx_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from nibiru.stablecoin.v1 import tx_pb2 as nibiru_dot_stablecoin_dot_v1_dot_tx__pb2
+from nibiru_proto.nibiru.stablecoin.v1 import tx_pb2 as nibiru_dot_stablecoin_dot_v1_dot_tx__pb2
 
 
 class MsgStub(object):
     """Msg defines the x/stablecoin Msg service.
     """
 
     def __init__(self, channel):
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/event_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/event_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from nibiru.sudo.v1 import state_pb2 as nibiru_dot_sudo_dot_v1_dot_state__pb2
+from nibiru_proto.nibiru.sudo.v1 import state_pb2 as nibiru_dot_sudo_dot_v1_dot_state__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1anibiru/sudo/v1/event.proto\x12\x0enibiru.sudo.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1anibiru/sudo/v1/state.proto\"e\n\x12\x45ventUpdateSudoers\x12\x37\n\x07sudoers\x18\x01 \x01(\x0b\x32\x17.nibiru.sudo.v1.SudoersB\x04\xc8\xde\x1f\x00R\x07sudoers\x12\x16\n\x06\x61\x63tion\x18\x02 \x01(\tR\x06\x61\x63tionB)Z\'github.com/NibiruChain/nibiru/x/sudo/pbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.sudo.v1.event_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/event_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/query_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/query_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from nibiru.sudo.v1 import state_pb2 as nibiru_dot_sudo_dot_v1_dot_state__pb2
+from nibiru_proto.nibiru.sudo.v1 import state_pb2 as nibiru_dot_sudo_dot_v1_dot_state__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1anibiru/sudo/v1/query.proto\x12\x0enibiru.sudo.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1anibiru/sudo/v1/state.proto\"\x15\n\x13QuerySudoersRequest\"O\n\x14QuerySudoersResponse\x12\x37\n\x07sudoers\x18\x01 \x01(\x0b\x32\x17.nibiru.sudo.v1.SudoersB\x04\xc8\xde\x1f\x00R\x07sudoers2\x80\x01\n\x05Query\x12w\n\x0cQuerySudoers\x12#.nibiru.sudo.v1.QuerySudoersRequest\x1a$.nibiru.sudo.v1.QuerySudoersResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/nibiru/sudo/sudoersB)Z\'github.com/NibiruChain/nibiru/x/sudo/pbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.sudo.v1.query_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/query_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/query_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from nibiru.sudo.v1 import query_pb2 as nibiru_dot_sudo_dot_v1_dot_query__pb2
+from nibiru_proto.nibiru.sudo.v1 import query_pb2 as nibiru_dot_sudo_dot_v1_dot_query__pb2
 
 
 class QueryStub(object):
     """Query defines the gRPC querier service.
     """
 
     def __init__(self, channel):
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/state_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/state_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/state_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/tx_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/tx_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/nibiru/sudo/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/tx_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from nibiru.sudo.v1 import tx_pb2 as nibiru_dot_sudo_dot_v1_dot_tx__pb2
+from nibiru_proto.nibiru.sudo.v1 import tx_pb2 as nibiru_dot_sudo_dot_v1_dot_tx__pb2
 
 
 class MsgStub(object):
     """Msg defines the x/sudo module's Msg service. Protobuf `Msg` services are
     called from `BaseApp` instances during `DeliverTx`. The `Msg` service will be
     responsible for processing `sdk.Msg` requests.
     """
```

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/abci/types_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/abci/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/abci/types_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/abci/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/abci/types_pb2_grpc.py` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/abci/types_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/crypto/keys_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/crypto/keys_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/crypto/proof_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/proof_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/crypto/proof_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/proof_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/libs/bits/types_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/libs/bits/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/libs/bits/types_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/libs/bits/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/p2p/types_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/p2p/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/p2p/types_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/p2p/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/block_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/block_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/block_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/evidence_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/evidence_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/evidence_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/evidence_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/params_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/params_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/params_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/types_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/types_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/validator_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/types/validator_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/validator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/version/types_pb2.py` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/version/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/nibiru_proto/tendermint/version/types_pb2.pyi` & `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/version/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b5/pyproject.toml` & `nibiru_proto-0.21.3b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nibiru-proto"
-version = "0.21.3b5"
+version = "0.21.3b7"
 description = "Nibiru Chain Python SDK"
 authors = ["Nibiru Chain <dev@nibiru.fi>"]
 packages = [{ include = "nibiru_proto" }]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nibiru_proto-0.21.3b5/PKG-INFO` & `nibiru_proto-0.21.3b7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibiru-proto
-Version: 0.21.3b5
+Version: 0.21.3b7
 Summary: Nibiru Chain Python SDK
 License: MIT
 Author: Nibiru Chain
 Author-email: dev@nibiru.fi
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

