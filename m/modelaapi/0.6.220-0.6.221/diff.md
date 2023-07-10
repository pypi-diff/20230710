# Comparing `tmp/modelaapi-0.6.220.tar.gz` & `tmp/modelaapi-0.6.221.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelaapi-0.6.220.tar", last modified: Mon Jul 10 18:39:24 2023, max compression
+gzip compressed data, was "modelaapi-0.6.221.tar", last modified: Mon Jul 10 19:36:06 2023, max compression
```

## Comparing `modelaapi-0.6.220.tar` & `modelaapi-0.6.221.tar`

### file list

```diff
@@ -1,481 +1,481 @@
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.482425 modelaapi-0.6.220/
--rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.220/AUTHORS.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.220/CONTRIBUTING.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.220/DESCRIPTION.md
--rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.220/HISTORY.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.220/LICENSE.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.220/MANIFEST.in
--rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.220/Makefile
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-10 18:39:24.482425 modelaapi-0.6.220/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.220/README.md
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/gogo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/gogo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/gogo/protobuf/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/gogo/protobuf/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/gogo/protobuf/gogoproto/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/gogo/protobuf/gogoproto/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23368 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    50953 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23177 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    56923 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4692 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    73562 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18564 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/google/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/google/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/google/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/google/api/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-07-10 18:38:20.000000 modelaapi-0.6.220/google/api/annotations_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/google/api/annotations_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-07-10 18:38:20.000000 modelaapi-0.6.220/google/api/http_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/google/api/http_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/apps/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/apps/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/apps/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/api/apps/v1/generated_pb2.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/core/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/core/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/core/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/api/core/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/rbac/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/rbac/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/rbac/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/api/rbac/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/resource/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.482425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/intstr/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.482425 modelaapi-0.6.220/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.220/modelaapi/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.220/modelaapi/consts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.220/modelaapi/custom_transformers.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.220/modelaapi/graykite_model.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.220/modelaapi/ts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-07-10 18:38:58.000000 modelaapi-0.6.220/modelaapi/version.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.482425 modelaapi-0.6.220/modelaapi.egg-info/
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-10 18:39:24.000000 modelaapi-0.6.220/modelaapi.egg-info/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-07-10 18:39:24.000000 modelaapi-0.6.220/modelaapi.egg-info/SOURCES.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-07-10 18:39:24.000000 modelaapi-0.6.220/modelaapi.egg-info/dependency_links.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-07-10 18:39:24.000000 modelaapi-0.6.220/modelaapi.egg-info/entry_points.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.220/modelaapi.egg-info/not-zip-safe
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-07-10 18:39:24.000000 modelaapi-0.6.220/modelaapi.egg-info/requires.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-07-10 18:39:24.000000 modelaapi-0.6.220/modelaapi.egg-info/top_level.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.220/requirements.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-07-10 18:39:24.482425 modelaapi-0.6.220/setup.cfg
--rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.220/setup.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.221/AUTHORS.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.221/CONTRIBUTING.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.221/DESCRIPTION.md
+-rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.221/HISTORY.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.221/LICENSE.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.221/MANIFEST.in
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.221/Makefile
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-10 19:36:06.135758 modelaapi-0.6.221/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.221/README.md
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/gogo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/gogo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/gogo/protobuf/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/gogo/protobuf/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/gogo/protobuf/gogoproto/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/gogo/protobuf/gogoproto/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23368 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    50953 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    22695 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    56885 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.107757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4692 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.111757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    73562 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.115757 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18564 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.119758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.123758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.127758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-07-10 19:34:42.000000 modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/google/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/google/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/google/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/google/api/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-07-10 19:34:42.000000 modelaapi-0.6.221/google/api/annotations_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/google/api/annotations_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-07-10 19:34:42.000000 modelaapi-0.6.221/google/api/http_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 19:34:42.000000 modelaapi-0.6.221/google/api/http_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/k8s/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/k8s/io/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/k8s/io/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/k8s/io/api/apps/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/apps/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/k8s/io/api/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/apps/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/api/apps/v1/generated_pb2.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.131758 modelaapi-0.6.221/k8s/io/api/core/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/core/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/api/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/core/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/api/core/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/api/rbac/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/rbac/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/api/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/rbac/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/api/rbac/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/api/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/resource/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/intstr/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-07-10 19:34:42.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.221/modelaapi/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.221/modelaapi/consts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.221/modelaapi/custom_transformers.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.221/modelaapi/graykite_model.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.221/modelaapi/ts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-07-10 19:35:45.000000 modelaapi-0.6.221/modelaapi/version.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 19:36:06.135758 modelaapi-0.6.221/modelaapi.egg-info/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-10 19:36:06.000000 modelaapi-0.6.221/modelaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-07-10 19:36:06.000000 modelaapi-0.6.221/modelaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-07-10 19:36:06.000000 modelaapi-0.6.221/modelaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-07-10 19:36:06.000000 modelaapi-0.6.221/modelaapi.egg-info/entry_points.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.221/modelaapi.egg-info/not-zip-safe
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-07-10 19:36:06.000000 modelaapi-0.6.221/modelaapi.egg-info/requires.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-07-10 19:36:06.000000 modelaapi-0.6.221/modelaapi.egg-info/top_level.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.221/requirements.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-07-10 19:36:06.139758 modelaapi-0.6.221/setup.cfg
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.221/setup.py
```

### Comparing `modelaapi-0.6.220/CONTRIBUTING.rst` & `modelaapi-0.6.221/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/LICENSE.txt` & `modelaapi-0.6.221/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/Makefile` & `modelaapi-0.6.221/Makefile`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/PKG-INFO` & `modelaapi-0.6.221/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.220
+Version: 0.6.221
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.220
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.221
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.220
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.221
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.220/README.md` & `modelaapi-0.6.221/README.md`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/gogo/protobuf/gogoproto/gogo_pb2.py` & `modelaapi-0.6.221/github/com/gogo/protobuf/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_training_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x12\x39github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x82\x01\n\x0f\x41utoScalingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x13\n\x0bminReplicas\x18\x02 \x01(\x05\x12\x13\n\x0bmaxReplicas\x18\x03 \x01(\x05\x12\x19\n\x11\x63puAvgUtilization\x18\x04 \x01(\x05\x12\x19\n\x11memAvgUtilization\x18\x05 \x01(\x05\"\x8e\x01\n\x13\x42\x61\x63kwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rconfidenceLow\x18\x04 \x01(\x01\x12\x16\n\x0e\x63onfidenceHigh\x18\x05 \x01(\x01\"|\n\rCustomAppSpec\x12\r\n\x05owner\x18\x01 \x01(\x08\x12\r\n\x05title\x18\x02 \x01(\t\x12M\n\x05pages\x18\x03 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"\xfd\x01\n\x07\x44\x61taApp\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppStatus\"\xa2\x01\n\x0b\x44\x61taAppList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataApp\"\xc9\x03\n\x0b\x44\x61taAppSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0emodelClassName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x11\n\tmodelName\x18\x05 \x01(\t\x12S\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x07 \x01(\x05\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingsiteRef\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06\x63ustom\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.CustomAppSpec\"\xd8\x02\n\rDataAppStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\x10\x64\x65ploymentStatus\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0eservicetStatus\x18\x04 \x01(\x0b\x32!.k8s.io.api.core.v1.ServiceStatus\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf0\x03\n\x12\x44riftDetectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rgenDriftTests\x18\x02 \x01(\x08\x12\x16\n\x0eminPredictions\x18\x03 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12]\n\x0f\x64riftThresholds\x18\x05 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12]\n\x11unitTestsTemplate\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x45\n\x18outlierDetectionModelRef\x18\x08 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rmaxHistograms\x18\t \x01(\x05\x12\x15\n\rperiodSeconds\x18\n \x01(\x05\"\xc5\x01\n\x11\x46\x61stSlowModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x39\n\x0c\x66\x61stModelRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cslowModelRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bprobaLowPct\x18\x04 \x01(\x05\x12\x14\n\x0cprobaHighPct\x18\x05 \x01(\x05\"\xce\x01\n\x10\x46\x65\x65\x64\x62\x61\x63kTestSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"\xa8\x02\n\x16\x46orecastPredictionSpec\x12\x7f\n\x0fhierarchyValues\x18\x01 \x03(\x0b\x32\x66.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec.HierarchyValuesEntry\x12U\n\x07horizon\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x1a\x36\n\x14HierarchyValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x01\n\x0b\x46orecastRun\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x15\n\rmodelLocation\x18\x02 \x01(\t\x12U\n\x07horizon\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\"\xe4\x01\n\x0c\x46orecastSpec\x12_\n\x04runs\x18\t \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastSpec.RunsEntry\x1as\n\tRunsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12U\n\x05value\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastRun:\x02\x38\x01\"\xd1\x01\n\x0e\x46orecastStatus\x12\x12\n\nprofileURI\x18\x01 \x01(\t\x12\x11\n\treportURI\x18\x02 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x03 \x01(\t\x12\x0e\n\x06\x66\x61iled\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"o\n\x12\x46orwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07percent\x18\x03 \x01(\x05\"0\n\rMetricHistory\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0f\n\x07history\x18\x02 \x03(\x01\"\xad\x02\n\x15ModelDeploymentRecord\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12>\n\ndeployedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\tretiredAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x1a\n\x12\x61vgDailyPrediction\x18\x08 \x01(\x05\x12\x12\n\navgLatency\x18\t \x01(\x01\"\x9d\x07\n\x15ModelDeploymentStatus\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12:\n\rdeploymentRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x33\n\x06hpaRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12>\n\ndeployedAt\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x16lastFeedbackDatasetRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x46\n\x12lastFeedbackTestAt\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x65\n\x17lastFeedbackTestResults\x18\x0c \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12|\n\x0emetricsHistory\x18\r \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus.MetricsHistoryEntry\x12\x1a\n\x12\x61vgDailyPrediction\x18\x0e \x01(\x05\x12\x12\n\navgLatency\x18\x0f \x01(\x01\x12\x10\n\x08\x65ndpoint\x18\x10 \x01(\t\x1a\x7f\n\x13MetricsHistoryEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12W\n\x05value\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.MetricHistory:\x02\x38\x01\"\x80\x01\n\x10ModelServingSpec\x12\x12\n\nserverless\x18\x02 \x01(\x08\x12X\n\x0cservingTests\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\";\n\x16OnlineFeatureStoreSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08hostname\x18\x02 \x01(\t\"U\n\x11OnlineStoreStatus\x12@\n\x0clastAccessed\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"=\n PartitionPredictionLocationsSpec\x12\x19\n\x11groupForecastFile\x18\x02 \x01(\t\"\x86\x02\n\nPrediction\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionStatus\"\x83\x01\n\x13PredictionCacheSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08inMemory\x18\x02 \x01(\x08\x12\r\n\x05redis\x18\x03 \x01(\x08\x12:\n\rconnectionRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xa8\x01\n\x0ePredictionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\"\x83\x02\n\x15PredictionLoggingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rsamplePercent\x18\x02 \x01(\x05\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x19\n\x11\x62\x61\x63kupFreqSeconds\x18\x04 \x01(\x05\x12@\n\x13\x62\x61\x63kupConnectionRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xdc\x07\n\x0ePredictionSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x39\n\x0cpredictorRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07labeled\x18\x04 \x01(\x08\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12:\n\rdataSourceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12R\n\x05input\x18\x07 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataInputSpec\x12T\n\x06output\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12\x15\n\rcreateDataset\x18\t \x01(\x08\x12[\n\tunitTests\x18\n \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelTestSuite\x12\r\n\x05owner\x18\x0b \x01(\t\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\r \x01(\x03\x12\x10\n\x08priority\x18\x0e \x01(\t\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x0b\n\x03ttl\x18\x10 \x01(\x05\x12g\n\x0c\x66orecastSpec\x18\x11 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec\x12;\n\x0eservingsiteRef\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12v\n\x11partitionLocation\x18\x14 \x01(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PartitionPredictionLocationsSpec\x12\x0f\n\x07workers\x18\x15 \x01(\x05\"\xe0\x06\n\x10PredictionStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x61\n\x0funitTestsResult\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x13\n\x0btriggeredBy\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12\x37\n\ndatasetRef\x18\x0b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12V\n\x07\x63olumns\x18\x0c \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnHistogram\x12\x0f\n\x07\x64rifted\x18\r \x01(\x08\x12[\n\x08\x66orecast\x18\x0e \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastStatus\x12[\n\x05usage\x18\x0f \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x10 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x83\x02\n\tPredictor\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorStatus\"\xa6\x01\n\rPredictorList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\"\xb1\r\n\rPredictorSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x37\n\nproductRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08template\x18\x05 \x01(\x08\x12;\n\x0eservingSiteRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\\\n\x06models\x18\x08 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ModelDeploymentSpec\x12_\n\x0bprogressive\x18\t \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ProgressiveSpec\x12S\n\x06\x61\x63\x63\x65ss\x18\x0b \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x0c \x01(\x05\x12_\n\x0b\x61utoScaling\x18\r \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.AutoScalingSpec\x12\r\n\x05owner\x18\x0e \x01(\t\x12X\n\tresources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12]\n\x05\x63\x61\x63he\x18\x10 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionCacheSpec\x12`\n\x05store\x18\x11 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineFeatureStoreSpec\x12\\\n\x07serving\x18\x12 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelServingSpec\x12\x0c\n\x04task\x18\x13 \x01(\t\x12\\\n\x05\x64rift\x18\x15 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DriftDetectionSpec\x12]\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x16 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FeedbackTestSpec\x12_\n\x0cnotification\x18\x17 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12k\n\x11predictionLogging\x18\x18 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionLoggingSpec\x12\x65\n\x0e\x66orwardCurtain\x18\x19 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForwardCurtainSpec\x12g\n\x0f\x62\x61\x63kwardCurtain\x18\x1a \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.BackwardCurtainSpec\x12^\n\x08\x66\x61stSlow\x18\x1b \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FastSlowModelSpec\"\xd6\x06\n\x0fPredictorStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12\x61\n\x07history\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentRecord\x12\x65\n\x0bmodelStatus\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus\x12i\n\x12predictorletStatus\x18\x05 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorletStatus\x12g\n\x11onlineStoreStatus\x18\x07 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineStoreStatus\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0b \x01(\t\x12\x42\n\x12loadBalancerStatus\x18\x0c \x01(\x0b\x32&.k8s.io.api.core.v1.LoadBalancerStatus\x12\x42\n\x15lastPredictionDataset\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x65\n\x13servingTestsResults\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x43\n\nconditions\x18\x11 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x86\x03\n\x12PredictorletStatus\x12:\n\rdeploymentRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\ndeployedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0b\n\x03p50\x18\x04 \x01(\x01\x12\x0b\n\x03p95\x18\x05 \x01(\x01\x12\x0b\n\x03p99\x18\x06 \x01(\x01\x12\x1a\n\x12\x61vgDailyPrediction\x18\x07 \x01(\x05\x12\x18\n\x10totalPredictions\x18\x08 \x01(\x05\x12\x46\n\x12lastPredictionTime\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\"R\n\x0fProgressiveSpec\x12\x0e\n\x06warmup\x18\x01 \x01(\x05\x12\x18\n\x10trafficIncrement\x18\x02 \x01(\x05\x12\x15\n\rcanaryMetrics\x18\x03 \x03(\t\"[\n\x0fValidationError\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x0e\n\x06metric\x18\x02 \x01(\t\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\x0b\n\x03max\x18\x04 \x01(\x01\x12\x0e\n\x06\x61\x63tual\x18\x05 \x01(\x01\x42;Z9github.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x12\x39github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x82\x01\n\x0f\x41utoScalingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x13\n\x0bminReplicas\x18\x02 \x01(\x05\x12\x13\n\x0bmaxReplicas\x18\x03 \x01(\x05\x12\x19\n\x11\x63puAvgUtilization\x18\x04 \x01(\x05\x12\x19\n\x11memAvgUtilization\x18\x05 \x01(\x05\"\x8e\x01\n\x13\x42\x61\x63kwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rconfidenceLow\x18\x04 \x01(\x01\x12\x16\n\x0e\x63onfidenceHigh\x18\x05 \x01(\x01\"|\n\rCustomAppSpec\x12\r\n\x05owner\x18\x01 \x01(\x08\x12\r\n\x05title\x18\x02 \x01(\t\x12M\n\x05pages\x18\x03 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"\xfd\x01\n\x07\x44\x61taApp\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppStatus\"\xa2\x01\n\x0b\x44\x61taAppList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataApp\"\xc9\x03\n\x0b\x44\x61taAppSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0emodelClassName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x11\n\tmodelName\x18\x05 \x01(\t\x12S\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x07 \x01(\x05\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingsiteRef\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06\x63ustom\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.CustomAppSpec\"\xd8\x02\n\rDataAppStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\x10\x64\x65ploymentStatus\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0eservicetStatus\x18\x04 \x01(\x0b\x32!.k8s.io.api.core.v1.ServiceStatus\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf0\x03\n\x12\x44riftDetectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rgenDriftTests\x18\x02 \x01(\x08\x12\x16\n\x0eminPredictions\x18\x03 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12]\n\x0f\x64riftThresholds\x18\x05 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12]\n\x11unitTestsTemplate\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x45\n\x18outlierDetectionModelRef\x18\x08 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rmaxHistograms\x18\t \x01(\x05\x12\x15\n\rperiodSeconds\x18\n \x01(\x05\"\xc5\x01\n\x11\x46\x61stSlowModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x39\n\x0c\x66\x61stModelRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cslowModelRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bprobaLowPct\x18\x04 \x01(\x05\x12\x14\n\x0cprobaHighPct\x18\x05 \x01(\x05\"\xce\x01\n\x10\x46\x65\x65\x64\x62\x61\x63kTestSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"\xa8\x02\n\x16\x46orecastPredictionSpec\x12\x7f\n\x0fhierarchyValues\x18\x01 \x03(\x0b\x32\x66.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec.HierarchyValuesEntry\x12U\n\x07horizon\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x1a\x36\n\x14HierarchyValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x01\n\x0b\x46orecastRun\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x15\n\rmodelLocation\x18\x02 \x01(\t\x12U\n\x07horizon\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\"\xe4\x01\n\x0c\x46orecastSpec\x12_\n\x04runs\x18\t \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastSpec.RunsEntry\x1as\n\tRunsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12U\n\x05value\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastRun:\x02\x38\x01\"\xd1\x01\n\x0e\x46orecastStatus\x12\x12\n\nprofileURI\x18\x01 \x01(\t\x12\x11\n\treportURI\x18\x02 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x03 \x01(\t\x12\x0e\n\x06\x66\x61iled\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"o\n\x12\x46orwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07percent\x18\x03 \x01(\x05\"0\n\rMetricHistory\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0f\n\x07history\x18\x02 \x03(\x01\"\xad\x02\n\x15ModelDeploymentRecord\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12>\n\ndeployedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\tretiredAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x1a\n\x12\x61vgDailyPrediction\x18\x08 \x01(\x05\x12\x12\n\navgLatency\x18\t \x01(\x01\"\x9d\x07\n\x15ModelDeploymentStatus\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12:\n\rdeploymentRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x33\n\x06hpaRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12>\n\ndeployedAt\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x16lastFeedbackDatasetRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x46\n\x12lastFeedbackTestAt\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x65\n\x17lastFeedbackTestResults\x18\x0c \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12|\n\x0emetricsHistory\x18\r \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus.MetricsHistoryEntry\x12\x1a\n\x12\x61vgDailyPrediction\x18\x0e \x01(\x05\x12\x12\n\navgLatency\x18\x0f \x01(\x01\x12\x10\n\x08\x65ndpoint\x18\x10 \x01(\t\x1a\x7f\n\x13MetricsHistoryEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12W\n\x05value\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.MetricHistory:\x02\x38\x01\"\x80\x01\n\x10ModelServingSpec\x12\x12\n\nserverless\x18\x02 \x01(\x08\x12X\n\x0cservingTests\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\";\n\x16OnlineFeatureStoreSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08hostname\x18\x02 \x01(\t\"U\n\x11OnlineStoreStatus\x12@\n\x0clastAccessed\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"=\n PartitionPredictionLocationsSpec\x12\x19\n\x11groupForecastFile\x18\x02 \x01(\t\"\x86\x02\n\nPrediction\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionStatus\"\x83\x01\n\x13PredictionCacheSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08inMemory\x18\x02 \x01(\x08\x12\r\n\x05redis\x18\x03 \x01(\x08\x12:\n\rconnectionRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xa8\x01\n\x0ePredictionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\"\x83\x02\n\x15PredictionLoggingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rsamplePercent\x18\x02 \x01(\x05\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x19\n\x11\x62\x61\x63kupFreqSeconds\x18\x04 \x01(\x05\x12@\n\x13\x62\x61\x63kupConnectionRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xd2\x06\n\x0ePredictionSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12R\n\x05input\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataInputSpec\x12T\n\x06output\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12;\n\x0eservingSiteRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x35\n\x08modelRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rcreateDataset\x18\x07 \x01(\x08\x12\x0f\n\x07labeled\x18\x08 \x01(\x08\x12U\n\tunitTests\x18\t \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x0b \x01(\x03\x12\r\n\x05\x61\x62ort\x18\x0c \x01(\x08\x12g\n\x0c\x66orecastSpec\x18\r \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec\x12v\n\x11partitionLocation\x18\x0e \x01(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PartitionPredictionLocationsSpec\x12\x16\n\x0emodelClassName\x18\x0f \x01(\t\"\xcb\x05\n\x10PredictionStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x61\n\x0funitTestsResult\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12\x37\n\ndatasetRef\x18\x0b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12[\n\x08\x66orecast\x18\x0e \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastStatus\x12[\n\x05usage\x18\x0f \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x10 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x83\x02\n\tPredictor\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorStatus\"\xa6\x01\n\rPredictorList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\"\xb1\r\n\rPredictorSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x37\n\nproductRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08template\x18\x05 \x01(\x08\x12;\n\x0eservingSiteRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\\\n\x06models\x18\x08 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ModelDeploymentSpec\x12_\n\x0bprogressive\x18\t \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ProgressiveSpec\x12S\n\x06\x61\x63\x63\x65ss\x18\x0b \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x0c \x01(\x05\x12_\n\x0b\x61utoScaling\x18\r \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.AutoScalingSpec\x12\r\n\x05owner\x18\x0e \x01(\t\x12X\n\tresources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12]\n\x05\x63\x61\x63he\x18\x10 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionCacheSpec\x12`\n\x05store\x18\x11 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineFeatureStoreSpec\x12\\\n\x07serving\x18\x12 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelServingSpec\x12\x0c\n\x04task\x18\x13 \x01(\t\x12\\\n\x05\x64rift\x18\x15 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DriftDetectionSpec\x12]\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x16 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FeedbackTestSpec\x12_\n\x0cnotification\x18\x17 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12k\n\x11predictionLogging\x18\x18 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionLoggingSpec\x12\x65\n\x0e\x66orwardCurtain\x18\x19 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForwardCurtainSpec\x12g\n\x0f\x62\x61\x63kwardCurtain\x18\x1a \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.BackwardCurtainSpec\x12^\n\x08\x66\x61stSlow\x18\x1b \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FastSlowModelSpec\"\xd6\x06\n\x0fPredictorStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12\x61\n\x07history\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentRecord\x12\x65\n\x0bmodelStatus\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus\x12i\n\x12predictorletStatus\x18\x05 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorletStatus\x12g\n\x11onlineStoreStatus\x18\x07 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineStoreStatus\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0b \x01(\t\x12\x42\n\x12loadBalancerStatus\x18\x0c \x01(\x0b\x32&.k8s.io.api.core.v1.LoadBalancerStatus\x12\x42\n\x15lastPredictionDataset\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x65\n\x13servingTestsResults\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x43\n\nconditions\x18\x11 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x86\x03\n\x12PredictorletStatus\x12:\n\rdeploymentRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\ndeployedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0b\n\x03p50\x18\x04 \x01(\x01\x12\x0b\n\x03p95\x18\x05 \x01(\x01\x12\x0b\n\x03p99\x18\x06 \x01(\x01\x12\x1a\n\x12\x61vgDailyPrediction\x18\x07 \x01(\x05\x12\x18\n\x10totalPredictions\x18\x08 \x01(\x05\x12\x46\n\x12lastPredictionTime\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\"R\n\x0fProgressiveSpec\x12\x0e\n\x06warmup\x18\x01 \x01(\x05\x12\x18\n\x10trafficIncrement\x18\x02 \x01(\x05\x12\x15\n\rcanaryMetrics\x18\x03 \x03(\t\"[\n\x0fValidationError\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x0e\n\x06metric\x18\x02 \x01(\t\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\x0b\n\x03max\x18\x04 \x01(\x01\x12\x0e\n\x06\x61\x63tual\x18\x05 \x01(\x01\x42;Z9github.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z9github.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1'
@@ -89,25 +89,25 @@
   _PREDICTIONCACHESPEC._serialized_start=5972
   _PREDICTIONCACHESPEC._serialized_end=6103
   _PREDICTIONLIST._serialized_start=6106
   _PREDICTIONLIST._serialized_end=6274
   _PREDICTIONLOGGINGSPEC._serialized_start=6277
   _PREDICTIONLOGGINGSPEC._serialized_end=6536
   _PREDICTIONSPEC._serialized_start=6539
-  _PREDICTIONSPEC._serialized_end=7527
-  _PREDICTIONSTATUS._serialized_start=7530
-  _PREDICTIONSTATUS._serialized_end=8394
-  _PREDICTOR._serialized_start=8397
-  _PREDICTOR._serialized_end=8656
-  _PREDICTORLIST._serialized_start=8659
-  _PREDICTORLIST._serialized_end=8825
-  _PREDICTORSPEC._serialized_start=8828
-  _PREDICTORSPEC._serialized_end=10541
-  _PREDICTORSTATUS._serialized_start=10544
-  _PREDICTORSTATUS._serialized_end=11398
-  _PREDICTORLETSTATUS._serialized_start=11401
-  _PREDICTORLETSTATUS._serialized_end=11791
-  _PROGRESSIVESPEC._serialized_start=11793
-  _PROGRESSIVESPEC._serialized_end=11875
-  _VALIDATIONERROR._serialized_start=11877
-  _VALIDATIONERROR._serialized_end=11968
+  _PREDICTIONSPEC._serialized_end=7389
+  _PREDICTIONSTATUS._serialized_start=7392
+  _PREDICTIONSTATUS._serialized_end=8107
+  _PREDICTOR._serialized_start=8110
+  _PREDICTOR._serialized_end=8369
+  _PREDICTORLIST._serialized_start=8372
+  _PREDICTORLIST._serialized_end=8538
+  _PREDICTORSPEC._serialized_start=8541
+  _PREDICTORSPEC._serialized_end=10254
+  _PREDICTORSTATUS._serialized_start=10257
+  _PREDICTORSTATUS._serialized_end=11111
+  _PREDICTORLETSTATUS._serialized_start=11114
+  _PREDICTORLETSTATUS._serialized_end=11504
+  _PROGRESSIVESPEC._serialized_start=11506
+  _PROGRESSIVESPEC._serialized_end=11588
+  _VALIDATIONERROR._serialized_start=11590
+  _VALIDATIONERROR._serialized_end=11681
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_data_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x12\x38github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x80\x01\n\x17\x41lgorithmParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12W\n\x06ranges\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\x9f\x01\n\x18\x41lgorithmSearchSpaceSpec\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\x12\x61\n\x06\x63ustom\x18\x03 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmParameterRange\"`\n\x07\x41nomaly\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x64jDeltaColumn\x18\x03 \x01(\t\x12\r\n\x05start\x18\x04 \x01(\t\x12\x0b\n\x03\x65nd\x18\x05 \x01(\t\"\'\n\x11\x41udioPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"M\n\x0c\x42\x61\x63ktestSpec\x12\x0f\n\x07sliding\x18\x01 \x01(\x08\x12\x0e\n\x06splits\x18\x02 \x01(\x05\x12\x0f\n\x07Initial\x18\x03 \x01(\x05\x12\x0b\n\x03gap\x18\x05 \x01(\x05\"?\n\x0c\x42\x61selineSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbaselines\x18\x02 \x03(\t\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"\r\n\x0b\x43hangePoint\"\x96\x01\n\x0e\x43heckpointSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12\x63heckpointInterval\x18\x02 \x01(\x05\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x92\x01\n\x16\x43lassicalEstimatorSpec\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x61\n\nparameters\x18\x02 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperParameterValue\"a\n\x10\x43ustomReportSpec\x12M\n\x05pages\x18\x08 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"L\n\nDataHashes\x12\x11\n\ttrainHash\x18\x01 \x01(\t\x12\x13\n\x0btestingHash\x18\x02 \x01(\t\x12\x16\n\x0evalidationHash\x18\x03 \x01(\t\"\xab\x01\n\rDataSplitSpec\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\r\n\x05train\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x0c\n\x04test\x18\x04 \x01(\x05\x12\x13\n\x0bsplitColumn\x18\x05 \x01(\t\x12\x14\n\x0ctrainDataset\x18\x07 \x01(\t\x12\x13\n\x0btestDataset\x18\x08 \x01(\t\x12\x19\n\x11validationDataset\x18\t \x01(\t\"\xa5\x01\n\x12\x44\x65\x65pEstimatorLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12^\n\nparameters\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NNLayerParameter\x12\x13\n\x0binputLayers\x18\x04 \x03(\t\"\xe6\x01\n\x11\x44\x65\x65pEstimatorSpec\x12\\\n\x06layers\x18\x01 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorLayer\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x11\n\tbatchSize\x18\x03 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x04 \x01(\x05\x12\x17\n\x0fvalidationSplit\x18\x05 \x01(\x05\x12\r\n\x05isSeq\x18\x06 \x01(\x08\x12\x0c\n\x04gpus\x18\x07 \x01(\x05\x12\x0c\n\x04loss\x18\x08 \x01(\t\".\n\x13\x44riftDetectorStatus\x12\x17\n\x0foutlierModelURI\x18\x01 \x01(\t\"O\n\rEarlyStopSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07initial\x18\x02 \x01(\x05\x12\x1c\n\x14modelsWithNoProgress\x18\x03 \x01(\x05\"\xfb\x01\n\x0c\x45nsembleSpec\x12\x0e\n\x06models\x18\x01 \x03(\t\x12\x64\n\nestimators\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12g\n\rbaseEstimator\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x0c\n\x04type\x18\x04 \x01(\t\"_\n\rEnsemblesSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0evotingEnsemble\x18\x02 \x01(\x08\x12\x18\n\x10stackingEnsemble\x18\x03 \x01(\x08\x12\x0b\n\x03top\x18\x04 \x01(\x05\"*\n\tEntityRef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"\x89\x01\n\x0b\x45valMetrics\x12\x11\n\tselection\x18\x01 \x01(\t\x12\x11\n\treporting\x18\x02 \x03(\t\x12\x0f\n\x07\x61ggFunc\x18\x03 \x01(\t\x12\x11\n\taggPeriod\x18\x04 \x01(\x05\x12\x17\n\x0fnullModelParams\x18\x05 \x01(\t\x12\x17\n\x0frelErrTolerance\x18\x06 \x01(\x01\"\xe0\x01\n\nEvalPeriod\x12\x13\n\x0btestHorizon\x18\x01 \x01(\x05\x12\x1f\n\x17periodsBetweenTrainTest\x18\x02 \x01(\x05\x12\x1e\n\x16\x63vPeriodsBetweenSplits\x18\x03 \x01(\x05\x12\x1a\n\x12\x63vExpandingWindows\x18\x04 \x01(\x08\x12\x11\n\tcvHorizon\x18\x05 \x01(\x05\x12\x19\n\x11\x63vMinTrainPeriods\x18\x06 \x01(\x05\x12\x13\n\x0b\x63vMaxSplits\x18\x07 \x01(\x05\x12\x1d\n\x15\x63vUseMostRecentSplits\x18\x08 \x01(\x08\"\xf2\x02\n\x1a\x46\x65\x61tureEngineeringPipeline\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\x12\x12\n\nimputation\x18\x04 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x05 \x01(\t\x12\x0f\n\x07scaling\x18\x06 \x01(\t\x12\x16\n\x0e\x64iscretisation\x18\x07 \x01(\t\x12\x1e\n\x16variableTransformation\x18\x08 \x01(\t\x12\x17\n\x0foutlierHandling\x18\t \x01(\t\x12\x1e\n\x16\x64\x61tetimeTransformation\x18\n \x01(\t\x12X\n\x04text\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TextPipelineSpec\x12\x0c\n\x04\x64rop\x18\x0c \x01(\x08\x12\x13\n\x0bpassthrough\x18\r \x01(\x08\"\xcd\x02\n\x1c\x46\x65\x61tureEngineeringSearchSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\testimator\x18\x03 \x01(\t\x12\x11\n\tmaxModels\x18\x04 \x01(\x05\x12\x0f\n\x07maxTime\x18\x05 \x01(\x05\x12\x10\n\x08trainers\x18\x06 \x01(\x05\x12\r\n\x05reuse\x18\t \x01(\x08\x12h\n\x10\x66\x65\x61tureSelection\x18\n \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\"\x80\x01\n\x1e\x46\x65\x61tureEngineeringSearchStatus\x12^\n\x04\x62\x65st\x18\x01 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\"\xf7\x01\n\x16\x46\x65\x61tureEngineeringSpec\x12g\n\tpipelines\x18\x01 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringPipeline\x12\x11\n\timbalance\x18\x02 \x01(\t\x12\x61\n\tselection\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\"8\n\x11\x46\x65\x61tureImportance\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x01\":\n\x0b\x46\x65\x61tureInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"#\n\x0b\x46\x65\x61turePair\x12\t\n\x01x\x18\x01 \x01(\t\x12\t\n\x01y\x18\x02 \x01(\t\"\xd5\x01\n\x14\x46\x65\x61tureSelectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tembedding\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\x08\x12\x0f\n\x07wrapper\x18\x05 \x01(\x08\x12\x10\n\x08pipeline\x18\x06 \x03(\t\x12\x14\n\x0cvarThreshold\x18\x07 \x01(\x05\x12\x15\n\rcorrThreshold\x18\x08 \x01(\x05\x12\x13\n\x0bmaxFeatures\x18\t \x01(\x05\x12\x12\n\npercentile\x18\n \x01(\x05\x12\x10\n\x08reserved\x18\x0c \x03(\t\"\xf8\x07\n\x0e\x46orecasterSpec\x12Y\n\x06\x65vents\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TimeSeriesEvent\x12R\n\x04past\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12T\n\x06\x66uture\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12\x10\n\x08\x63overage\x18\x06 \x01(\x01\x12]\n\x0eoutputLocation\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x10\n\x08\x66\x65\x61tures\x18\x08 \x03(\t\x12\x0e\n\x06groups\x18\t \x03(\t\x12\x1a\n\x12predefinedTemplate\x18\n \x01(\t\x12T\n\tanomalies\x18\x0b \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Anomaly\x12\x14\n\x0ctrainEndData\x18\x0c \x01(\t\x12\x13\n\x0bvalueColumn\x18\r \x01(\t\x12\x11\n\thpoBudget\x18\x0e \x01(\x05\x12`\n\x11\x65valuationMetrics\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalMetrics\x12^\n\x10\x65valuationPeriod\x18\x10 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalPeriod\x12^\n\x0bseasonality\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalitySpec\x12\x12\n\nregressors\x18\x12 \x03(\t\x12\x18\n\x10laggedRegressors\x18\x13 \x03(\t\x12\x0e\n\x06growth\x18\x14 \x01(\t\x12\x0b\n\x03key\x18\x15 \x03(\t\x12\x12\n\nestimators\x18\x16 \x03(\t\x12\x0b\n\x03hts\x18\x17 \x01(\t\"e\n\x15GarbageCollectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12!\n\x19keepBestModelPerAlgorithm\x18\x02 \x01(\x08\x12\x18\n\x10keepPrunedModels\x18\x03 \x01(\x08\"\x8e\x01\n\x17GarbageCollectionStatus\x12\x1c\n\x14\x63ollectedModelsCount\x18\x01 \x01(\x05\x12U\n\x06models\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelResult\"f\n\x13GeneratedColumnSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x66irst\x18\x03 \x01(\t\x12\x0e\n\x06second\x18\x04 \x01(\t\x12\x10\n\x08original\x18\x05 \x01(\t\"V\n\x17GroupSplitLocationsSpec\x12\x1d\n\x15groupTrainingDataFile\x18\x01 \x01(\t\x12\x1c\n\x14groupTestingDataFile\x18\x02 \x01(\t\"2\n\x13HyperParameterValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"o\n\x10HyperbandOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x14\n\x0cmaxResources\x18\x02 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"\'\n\x11ImagePipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\";\n\x15ImbalanceHandlingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\timbalance\x18\x02 \x01(\t\"\x9a\x02\n\x14InterpretabilitySpec\x12\x0b\n\x03ice\x18\x01 \x01(\x08\x12W\n\x08icepairs\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x0c\n\x04lime\x18\x03 \x01(\x08\x12\x0c\n\x04shap\x18\x04 \x01(\t\x12X\n\tshappairs\x18\x05 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x16\n\x0e\x63ounterfactual\x18\x06 \x01(\x08\x12\x0e\n\x06\x61nchor\x18\x07 \x01(\x08\"\xaa\x04\n\x16InterpretabilityStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x11\x65xplainerLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x66\n\x17trainShapValuesLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x65\n\x16testShapValuesLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\nimportance\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\"k\n\x13MedianPrunerOptions\x12\x15\n\rstartupTrials\x18\x01 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x02 \x01(\x05\x12\x15\n\rintervalSteps\x18\x03 \x01(\x05\x12\x11\n\tminTrials\x18\x04 \x01(\x05\"\xf5\x01\n\x05Model\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStatus\"\x84\x02\n\nModelClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassStatus\"\xcd\x04\n\x12ModelClassDataSpec\x12[\n\x0cobservations\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12Z\n\x0bpredictions\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12L\n\x06schema\x18\x03 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latFile\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x12\n\nprimaryKey\x18\x05 \x03(\t\x12\x1c\n\x14predictionTimeColumn\x18\x06 \x01(\t\x12\x0e\n\x06target\x18\x07 \x01(\t\x12Q\n\x05tests\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x1e\n\x16onlineFeatureStoreName\x18\t \x01(\t\x12\x1f\n\x17offlineFeatureStoreName\x18\n \x01(\t\"\xa7\x01\n\x0eModelClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\"\x8d\x02\n\rModelClassRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Y\n\x04spec\x18\x02 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunSpec\x12]\n\x06status\x18\x03 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunStatus\"\xad\x01\n\x11ModelClassRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12V\n\x05items\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\"\xce\x01\n\x11ModelClassRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x16\n\x0emodelClassName\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x0b\n\x03ttl\x18\t \x01(\x05\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\"\xed\x04\n\x13ModelClassRunStatus\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x11\n\tstudyName\x18\x02 \x01(\t\x12\x11\n\tmodelName\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x07 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x08 \x01(\t\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12=\n\tupdatedAt\x18\x0c \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\r \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12>\n\npromotedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04\x61uto\x18\x0f \x01(\x08\x12\x37\n\napprovedBy\x18\x10 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bmodelsCount\x18\x11 \x01(\x05\x12\x43\n\nconditions\x18\x12 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xd5\x02\n\x15ModelClassServingSpec\x12W\n\x08template\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12`\n\x12monitoringSchedule\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12`\n\x12predictionSchedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0e\n\x06preSQL\x18\x04 \x03(\t\x12\x0f\n\x07postSQL\x18\x05 \x03(\t\"\xc9\x06\n\x0eModelClassSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\x12\x0f\n\x07subtask\x18\x05 \x01(\t\x12Y\n\tobjective\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12U\n\x08\x65ntities\x18\x07 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EntityRef\x12Z\n\x04\x64\x61ta\x18\x08 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassDataSpec\x12\x62\n\x08training\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassTrainingSpec\x12`\n\x07serving\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassServingSpec\x12_\n\x0cnotification\x18\x0b \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\x0ereportSchedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0c\n\x04\x66\x61st\x18\r \x01(\x08\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12\x12\n\nregistered\x18\x0f \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x10 \x01(\t\"\xe7\x08\n\x10ModelClassStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12j\n\x16trainingScheduleStatus\x18\x04 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18predictionScheduleStatus\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18monitoringScheduleStatus\x18\x06 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12h\n\x14reportScheduleStatus\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x16\n\x0e\x62\x65stModelScore\x18\x08 \x01(\x01\x12\x0f\n\x07retired\x18\t \x03(\t\x12\x15\n\rpredictorName\x18\n \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x0b \x01(\t\x12\x13\n\x0btriggeredBy\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0e \x01(\t\x12=\n\tlastRunAt\x18\x0f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0blastRunName\x18\x10 \x01(\t\x12\x44\n\x10lastPredictionAt\x18\x11 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12lastPredictionName\x18\x12 \x01(\t\x12\x18\n\x10predictionsCount\x18\x13 \x01(\x05\x12\x11\n\trunsCount\x18\x14 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x15 \x01(\x05\x12\x0c\n\x04live\x18\x16 \x01(\x08\x12\x17\n\x0fpredictorsCount\x18\x17 \x01(\x05\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x87\x05\n\x16ModelClassTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x19\n\x11studyTemplateName\x18\x02 \x01(\t\x12Z\n\x0emodelUnitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12^\n\x10trainingSchedule\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12g\n\x0bsearchSpace\x18\x08 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\x12\x0e\n\x06paused\x18\x0b \x01(\x08\x12\x0f\n\x07maxTime\x18\x0c \x01(\x05\x12\x11\n\tmaxModels\x18\r \x01(\x05\x12\x10\n\x08trainers\x18\x0e \x01(\x05\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x11\n\texplained\x18\x10 \x01(\x08\x12\x0e\n\x06preSQL\x18\x11 \x03(\t\x12\x0f\n\x07postSQL\x18\x12 \x03(\t\"\xb3\x01\n\x12ModelGroupByStatus\x12\x11\n\tmodelsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x14\n\x0c\x66orecastsURI\x18\x03 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\tModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"]\n\x0bModelResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\talgorithm\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x01\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x0f\n\x07trialID\x18\x05 \x01(\x05\"\x95\x0c\n\tModelSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x03 \x01(\t\x12\x11\n\tstudyName\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x05 \x01(\t\x12\x0c\n\x04task\x18\x06 \x01(\t\x12\x0f\n\x07subtask\x18\x07 \x01(\t\x12Y\n\tobjective\x18\x08 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12l\n\x12\x66\x65\x61tureEngineering\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12\x63\n\testimator\x18\n \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12X\n\x08\x65nsemble\x18\x0b \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsembleSpec\x12X\n\x08training\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x0c\n\x04test\x18\r \x01(\x08\x12\r\n\x05\x61\x62ort\x18\x0e \x01(\x08\x12\x0f\n\x07package\x18\x0f \x01(\x08\x12\x0e\n\x06report\x18\x10 \x01(\x08\x12\r\n\x05pause\x18\x11 \x01(\x08\x12\x0f\n\x07profile\x18\x12 \x01(\x08\x12\x10\n\x08\x66orecast\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x14 \x01(\x08\x12\x10\n\x08unitTest\x18\x15 \x01(\x08\x12\x10\n\x08\x62\x61seline\x18\x16 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x17 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x18 \x01(\t\x12]\n\x0b\x66orecasting\x18\x19 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x1a \x01(\x03\x12\x15\n\restimatorType\x18\x1b \x01(\t\x12\x12\n\nmodelClass\x18\x1c \x01(\t\x12\x0f\n\x07trialID\x18\x1d \x01(\x05\x12T\n\x08\x61pproval\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12h\n\x10interpretability\x18\x1f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12U\n\tunitTests\x18  \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12q\n\x12partitionLocations\x18! \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PartitionModelLocationsSpec\x12\x16\n\x0emodelClassName\x18\" \x01(\t\x12\x19\n\x11modelClassRunName\x18# \x01(\t\x12_\n\x0cnotification\x18$ \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\"\x93\x02\n\x10ModelStageStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05\x65rror\x18\n \x01(\t\"\xeb\"\n\x0bModelStatus\x12\x45\n\x11trainingStartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12G\n\x13trainingCompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x44\n\x10testingStartedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x46\n\x12testingCompletedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0fvalidationScore\x18\x08 \x01(\x01\x12\x15\n\rtrainingScore\x18\t \x01(\x01\x12\x11\n\ttestScore\x18\n \x01(\x01\x12X\n\nvalidation\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12S\n\x05train\x18\x0e \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04test\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04tune\x18\x10 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12V\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x11 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05phase\x18\x12 \x01(\t\x12\x12\n\nreportName\x18\x13 \x01(\t\x12]\n\x0ereportLocation\x18\x14 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x63\n\x14trainWeightsLocation\x18\x15 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testWeightsLocation\x18\x16 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13\x66ullWeightsLocation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19trainLabelEncoderLocation\x18\x18 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fprofileLocation\x18\x1b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19misclassificationLocation\x18\x1c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\x10\x66orecastLocation\x18\x1d \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fpackageLocation\x18\x1e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12g\n\x12impurityImportance\x18\x1f \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12j\n\x15permutationImportance\x18  \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12X\n\x07runtime\x18! \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus\x12\x63\n\x14trainDatasetLocation\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18# \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18$ \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18% \x01(\x03\x12\x14\n\x0ctrainingRows\x18& \x01(\x05\x12\x13\n\x0btestingRows\x18\' \x01(\x05\x12\x16\n\x0evalidationRows\x18( \x01(\x05\x12\x16\n\x0e\x66\x61ilureMessage\x18* \x01(\t\x12\x10\n\x08progress\x18+ \x01(\x05\x12\x13\n\x0bsizeInBytes\x18, \x01(\x05\x12\x0f\n\x07latency\x18- \x01(\x01\x12X\n\x07serving\x18/ \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingStatus\x12\x13\n\x0btarFileHash\x18\x30 \x01(\t\x12^\n\x10trainingDataHash\x18\x31 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12g\n\x11trainingResources\x18\x32 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x66\n\x10testingResources\x18\x33 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x11\n\ttrainedBy\x18\x34 \x01(\t\x12K\n\x04logs\x18\x35 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12V\n\x08rocCurve\x18\x36 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RocAucCurve\x12Q\n\x07prCurve\x18\x37 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PRCurve\x12\x66\n\x14trainConfusionMatrix\x18\x38 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18\x39 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x61\n\x16\x63orrelationsWithTarget\x18: \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18; \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12=\n\tupdatedAt\x18< \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12V\n\x08\x61pproval\x18= \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalStatus\x12j\n\x10interpretability\x18> \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilityStatus\x12O\n\x06images\x18? \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12\x61\n\x0funitTestResults\x18@ \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x65\n\x13\x66\x65\x65\x64\x62\x61\x63kTestResults\x18\x41 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12]\n\x07groupby\x18\x42 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus\x12[\n\x05usage\x18\x44 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x45 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdf\x01\n\x0eModelTestSuite\x12=\n\x10\x62\x61selineModelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\ndatasetRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"/\n\x10NNLayerParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"=\n\x10OutlierModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10outlierAlgorithm\x18\x02 \x01(\t\"\xcc\x01\n\x1bPartitionModelLocationsSpec\x12\x17\n\x0fpartitionFolder\x18\x01 \x01(\t\x12\x1e\n\x16partitionProfileFolder\x18\x02 \x01(\t\x12\x1b\n\x13partitionReportFile\x18\x03 \x01(\t\x12\x1c\n\x14partitionModelFolder\x18\x04 \x01(\t\x12\x1a\n\x12partitionModelFile\x18\x05 \x01(\t\x12\x1d\n\x15partitionForecastFile\x18\x06 \x01(\t\"\x84\x01\n\x17PercentilePrunerOptions\x12\x12\n\npercentile\x18\x01 \x01(\x05\x12\x15\n\rstartupTrials\x18\x02 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x16\n\x0eintervalTrials\x18\x04 \x01(\x05\x12\x11\n\tminTrials\x18\x05 \x01(\x05\"\x93\x04\n\nPrunerSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12]\n\x06median\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.MedianPrunerOptions\x12\x65\n\npercentile\x18\x03 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PercentilePrunerOptions\x12m\n\x11successiveHalving\x18\x04 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingOptions\x12]\n\thyperband\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperbandOptions\x12\x63\n\tthreshold\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ThresholdPrunerOptions\"\xd0\x01\n\x18RegressionForecasterSpec\x12\x10\n\x08\x65nsemble\x18\x01 \x01(\x08\x12\x12\n\nimputation\x18\x02 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x0f\n\x07scaling\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\x08\x12\x0f\n\x07windows\x18\x06 \x03(\x05\x12\x0c\n\x04lags\x18\x07 \x03(\x05\x12\x11\n\tfunctions\x18\x08 \x03(\t\x12\x0b\n\x03\x65ma\x18\t \x01(\x08\x12\x0b\n\x03log\x18\n \x01(\x08\x12\x11\n\treduction\x18\x0b \x01(\t\"\xf8\x01\n\x06Report\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportStatus\"\x8a\x01\n\x13ReportGroupByStatus\x12\x12\n\nreportsURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9f\x01\n\nReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe9\x03\n\nReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x36\n\tentityRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nreportType\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12_\n\x0cnotification\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\x06 \x01(\t\x12X\n\tresources\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x08 \x01(\x03\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03key\x18\n \x03(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x0b \x01(\t\x12\x16\n\x0emodelClassName\x18\x0c \x01(\t\x12\x19\n\x11modelClassRunName\x18\r \x01(\t\"\xb3\x04\n\x0cReportStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12^\n\x07groupby\x18\t \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportGroupByStatus\x12\x43\n\nconditions\x18\n \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xde\x01\n\rRuntimeStatus\x12\x15\n\rpythonVersion\x18\x01 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12s\n\x0epythonPackages\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus.PythonPackagesEntry\x1a\x35\n\x13PythonPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x05\n\nSearchSpec\x12\x0f\n\x07sampler\x18\x01 \x01(\t\x12T\n\x06pruner\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PrunerSpec\x12\x0f\n\x07maxTime\x18\x04 \x01(\x05\x12\x11\n\tmaxModels\x18\x05 \x01(\x05\x12\x10\n\x08maxScore\x18\x06 \x01(\x01\x12\x10\n\x08trainers\x18\x07 \x01(\x05\x12\x0c\n\x04test\x18\x08 \x01(\x05\x12\x11\n\tretainTop\x18\t \x01(\x05\x12\x13\n\x0bretainedFor\x18\n \x01(\x05\x12g\n\x0bsearchSpace\x18\x0b \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\x12Y\n\tobjective\x18\r \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x62\n\x12secondaryObjective\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x0c\n\x04goal\x18\x0f \x01(\t\"L\n\x15SeasonalityPeriodSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x61uto\x18\x02 \x01(\x08\x12\x14\n\x0c\x66ourierOrder\x18\x03 \x01(\x05\"\x87\x04\n\x0fSeasonalitySpec\x12\x0c\n\x04\x61uto\x18\x01 \x01(\x08\x12_\n\x06yearly\x18\x02 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12\x62\n\tquarterly\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12`\n\x07monthly\x18\x04 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12_\n\x06weekly\x18\x05 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12^\n\x05\x64\x61ily\x18\x06 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\"\xb7\x03\n\x12ServingEnvironment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12;\n\x0eservingSiteRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12S\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x05 \x01(\x05\x12\x0e\n\x06online\x18\x06 \x01(\x08\x12\x11\n\tdashboard\x18\x07 \x01(\x08\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0e\n\x06preSQL\x18\t \x03(\t\x12\x0f\n\x07postSQL\x18\n \x03(\t\"\xe2\x03\n\x0bServingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12X\n\tresources\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingSiteRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06online\x18\x07 \x01(\x08\x12\x11\n\tdashboard\x18\x08 \x01(\x08\x12S\n\x06\x61\x63\x63\x65ss\x18\t \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\n \x01(\x05\x12\x11\n\tpromotion\x18\x0c \x01(\t\x12\x37\n\napprovedBy\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\x7f\n\rServingStatus\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x03 \x01(\t\x12\x19\n\x11predictorEndpoint\x18\x04 \x01(\t\x12\x19\n\x11\x64\x61shboardEndpoint\x18\x05 \x01(\t\x12\x0c\n\x04role\x18\x06 \x01(\t\"\xf5\x01\n\x05Study\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudySpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyStatus\"\x9d\x01\n\tStudyList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\xb4\x02\n\x10StudyPhaseStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12waitingModelsCount\x18\x03 \x01(\x05\x12\x1a\n\x12runningModelsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x66\x61iledModelsCount\x18\x05 \x01(\x05\x12\x1c\n\x14\x63ompletedModelsCount\x18\x06 \x01(\x05\x12\x11\n\tbestScore\x18\x07 \x01(\x01\x12\x1c\n\x14modelsWithNoProgress\x18\x08 \x01(\x05\"a\n\x11StudyScheduleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12;\n\x07startAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xc5\x0e\n\tStudySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetName\x18\x04 \x01(\t\x12\x0c\n\x04task\x18\x05 \x01(\t\x12\x0f\n\x07subtask\x18\x06 \x01(\t\x12h\n\x08\x66\x65Search\x18\x07 \x01(\x0b\x32V.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSearchSpec\x12i\n\x10imbalanceHandler\x18\x08 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImbalanceHandlingSpec\x12X\n\x08\x62\x61seline\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.BaselineSpec\x12T\n\x06search\x18\n \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SearchSpec\x12Z\n\tensembles\x18\x0b \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsemblesSpec\x12`\n\x10trainingTemplate\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x62\n\x10\x66orecastTemplate\x18\r \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12]\n\x08schedule\x18\x0e \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyScheduleSpec\x12h\n\x10interpretability\x18\x0f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12`\n\x0coutlierModel\x18\x10 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.OutlierModelSpec\x12\r\n\x05\x61\x62ort\x18\x11 \x01(\x08\x12\x0e\n\x06report\x18\x12 \x01(\x08\x12\r\n\x05pause\x18\x13 \x01(\x08\x12\x0f\n\x07profile\x18\x14 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x15 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x16 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x17 \x01(\t\x12\r\n\x05owner\x18\x18 \x01(\t\x12\x10\n\x08template\x18\x19 \x01(\x08\x12_\n\x0cnotification\x18\x1a \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12[\n\x02gc\x18\x1b \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionSpec\x12\x14\n\x0cmodelVersion\x18\x1c \x01(\t\x12\x0f\n\x07timeout\x18\x1d \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12i\n\x0egroupLocations\x18\x1f \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GroupSplitLocationsSpec\x12\x16\n\x0emodelClassName\x18  \x01(\t\x12\x19\n\x11modelClassRunName\x18! \x01(\t\x12V\n\x07serving\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\"\xfe\x10\n\x0bStudyStatus\x12\x13\n\x0bmodelsCount\x18\x01 \x01(\x05\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tbestModel\x18\x03 \x01(\t\x12\x16\n\x0e\x62\x65stModelScore\x18\x04 \x01(\x01\x12^\n\x0fprofileLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12]\n\x0ereportLocation\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x12\n\nreportName\x18\x07 \x01(\t\x12\r\n\x05phase\x18\x08 \x01(\t\x12\x1a\n\x12observedGeneration\x18\t \x01(\x03\x12\x63\n\x14trainDatasetLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18\x0b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12`\n\x11optimizerLocation\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x13\n\x0blastModelID\x18\x0e \x01(\x03\x12\x15\n\rfailureReason\x18\x0f \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x10 \x01(\t\x12\x19\n\x11trainingRowsCount\x18\x11 \x01(\x05\x12\x18\n\x10testingRowsCount\x18\x12 \x01(\x05\x12\x1b\n\x13validationRowsCount\x18\x13 \x01(\x05\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12^\n\x10trainingDataHash\x18\x15 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12\x13\n\x0btriggeredBy\x18\x16 \x01(\t\x12K\n\x04logs\x18\x17 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x66\n\x12\x66\x65\x61tureEngineering\x18\x18 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x62\x61seline\x18\x19 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12Z\n\x06search\x18\x1a \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x65nsemble\x18\x1b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12X\n\x04test\x18\x1c \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12[\n\x07\x65xplain\x18\x1d \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\x65\n\x0e\x64riftDetection\x18\x1e \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftDetectorStatus\x12=\n\tupdatedAt\x18\x1f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12p\n\x16\x62\x65stFeatureEngineering\x18  \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12]\n\x02gc\x18! \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionStatus\x12\x43\n\nconditions\x18% \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x7f\n\x18SuccessiveHalvingOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x02 \x01(\x05\x12\x1c\n\x14minEarlyStoppingRate\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"h\n\x15SuccessiveHalvingSpec\x12\x0e\n\x06\x62udget\x18\x01 \x01(\x05\x12\x0f\n\x07\x62racket\x18\x02 \x01(\x05\x12\x0c\n\x04rung\x18\x03 \x01(\x05\x12\x0e\n\x06\x63onfID\x18\x04 \x01(\x05\x12\x10\n\x08modality\x18\x1a \x01(\t\"\xad\x01\n\x10TextPipelineSpec\x12\x0f\n\x07\x65ncoder\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x02 \x01(\t\x12\x11\n\tstopwords\x18\x03 \x01(\x08\x12\x0b\n\x03pos\x18\x04 \x01(\x08\x12\r\n\x05lemma\x18\x05 \x01(\x08\x12\x0c\n\x04stem\x18\x06 \x01(\x08\x12\x11\n\tembedding\x18\x07 \x01(\t\x12\x0b\n\x03svd\x18\x08 \x01(\x08\x12\x18\n\x10maxSvdComponents\x18\t \x01(\x05\"b\n\x16ThresholdPrunerOptions\x12\r\n\x05lower\x18\x01 \x01(\x01\x12\r\n\x05upper\x18\x02 \x01(\x01\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x15\n\rintervalSteps\x18\x04 \x01(\x05\"\x8a\x01\n\x0fTimeSeriesEvent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0f\n\x07holiday\x18\x03 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x10\n\x08preEvent\x18\x05 \x01(\x05\x12\x11\n\tpostEvent\x18\x06 \x01(\x05\x12\x12\n\ntimePoints\x18\x07 \x03(\t\"\xe2\x04\n\x0cTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08priority\x18\x02 \x01(\t\x12\x0e\n\x06\x63vtype\x18\x03 \x01(\t\x12\r\n\x05\x66olds\x18\x05 \x01(\x05\x12V\n\x05split\x18\x06 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataSplitSpec\x12\x13\n\x0b\x65valMetrics\x18\x07 \x03(\t\x12[\n\x02sh\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingSpec\x12\x0c\n\x04seed\x18\x0b \x01(\x01\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03gpu\x18\r \x01(\x08\x12\x19\n\x11\x66\x65\x61tureImportance\x18\x0f \x01(\x08\x12\x11\n\tsamplePct\x18\x11 \x01(\x05\x12\\\n\ncheckpoint\x18\x12 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CheckpointSpec\x12\x10\n\x08logLevel\x18\x13 \x01(\t\x12\x0f\n\x07timeout\x18\x14 \x01(\x05\"\xdc\x01\n\x18UnivariateForecastStatus\x12\x1b\n\x13gridSearchResultURI\x18\x01 \x01(\t\x12g\n\rbaseEstimator\x18\x02 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x10\n\x08modelURI\x18\x03 \x01(\t\x12\x13\n\x0b\x63vResultURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x05 \x01(\t\"\'\n\x11VideoPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"=\n\nWindowSpec\x12\x10\n\x08interval\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x0e\n\x06length\x18\x03 \x01(\x05\x42:Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x12\x38github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x80\x01\n\x17\x41lgorithmParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12W\n\x06ranges\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\x9f\x01\n\x18\x41lgorithmSearchSpaceSpec\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\x12\x61\n\x06\x63ustom\x18\x03 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmParameterRange\"`\n\x07\x41nomaly\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x64jDeltaColumn\x18\x03 \x01(\t\x12\r\n\x05start\x18\x04 \x01(\t\x12\x0b\n\x03\x65nd\x18\x05 \x01(\t\"\'\n\x11\x41udioPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"M\n\x0c\x42\x61\x63ktestSpec\x12\x0f\n\x07sliding\x18\x01 \x01(\x08\x12\x0e\n\x06splits\x18\x02 \x01(\x05\x12\x0f\n\x07Initial\x18\x03 \x01(\x05\x12\x0b\n\x03gap\x18\x05 \x01(\x05\"?\n\x0c\x42\x61selineSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbaselines\x18\x02 \x03(\t\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"\r\n\x0b\x43hangePoint\"\x96\x01\n\x0e\x43heckpointSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12\x63heckpointInterval\x18\x02 \x01(\x05\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x92\x01\n\x16\x43lassicalEstimatorSpec\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x61\n\nparameters\x18\x02 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperParameterValue\"a\n\x10\x43ustomReportSpec\x12M\n\x05pages\x18\x08 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"L\n\nDataHashes\x12\x11\n\ttrainHash\x18\x01 \x01(\t\x12\x13\n\x0btestingHash\x18\x02 \x01(\t\x12\x16\n\x0evalidationHash\x18\x03 \x01(\t\"\xab\x01\n\rDataSplitSpec\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\r\n\x05train\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x0c\n\x04test\x18\x04 \x01(\x05\x12\x13\n\x0bsplitColumn\x18\x05 \x01(\t\x12\x14\n\x0ctrainDataset\x18\x07 \x01(\t\x12\x13\n\x0btestDataset\x18\x08 \x01(\t\x12\x19\n\x11validationDataset\x18\t \x01(\t\"\xa5\x01\n\x12\x44\x65\x65pEstimatorLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12^\n\nparameters\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NNLayerParameter\x12\x13\n\x0binputLayers\x18\x04 \x03(\t\"\xe6\x01\n\x11\x44\x65\x65pEstimatorSpec\x12\\\n\x06layers\x18\x01 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorLayer\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x11\n\tbatchSize\x18\x03 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x04 \x01(\x05\x12\x17\n\x0fvalidationSplit\x18\x05 \x01(\x05\x12\r\n\x05isSeq\x18\x06 \x01(\x08\x12\x0c\n\x04gpus\x18\x07 \x01(\x05\x12\x0c\n\x04loss\x18\x08 \x01(\t\".\n\x13\x44riftDetectorStatus\x12\x17\n\x0foutlierModelURI\x18\x01 \x01(\t\"O\n\rEarlyStopSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07initial\x18\x02 \x01(\x05\x12\x1c\n\x14modelsWithNoProgress\x18\x03 \x01(\x05\"\xfb\x01\n\x0c\x45nsembleSpec\x12\x0e\n\x06models\x18\x01 \x03(\t\x12\x64\n\nestimators\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12g\n\rbaseEstimator\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x0c\n\x04type\x18\x04 \x01(\t\"_\n\rEnsemblesSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0evotingEnsemble\x18\x02 \x01(\x08\x12\x18\n\x10stackingEnsemble\x18\x03 \x01(\x08\x12\x0b\n\x03top\x18\x04 \x01(\x05\"*\n\tEntityRef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"\x89\x01\n\x0b\x45valMetrics\x12\x11\n\tselection\x18\x01 \x01(\t\x12\x11\n\treporting\x18\x02 \x03(\t\x12\x0f\n\x07\x61ggFunc\x18\x03 \x01(\t\x12\x11\n\taggPeriod\x18\x04 \x01(\x05\x12\x17\n\x0fnullModelParams\x18\x05 \x01(\t\x12\x17\n\x0frelErrTolerance\x18\x06 \x01(\x01\"\xe0\x01\n\nEvalPeriod\x12\x13\n\x0btestHorizon\x18\x01 \x01(\x05\x12\x1f\n\x17periodsBetweenTrainTest\x18\x02 \x01(\x05\x12\x1e\n\x16\x63vPeriodsBetweenSplits\x18\x03 \x01(\x05\x12\x1a\n\x12\x63vExpandingWindows\x18\x04 \x01(\x08\x12\x11\n\tcvHorizon\x18\x05 \x01(\x05\x12\x19\n\x11\x63vMinTrainPeriods\x18\x06 \x01(\x05\x12\x13\n\x0b\x63vMaxSplits\x18\x07 \x01(\x05\x12\x1d\n\x15\x63vUseMostRecentSplits\x18\x08 \x01(\x08\"\xf2\x02\n\x1a\x46\x65\x61tureEngineeringPipeline\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\x12\x12\n\nimputation\x18\x04 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x05 \x01(\t\x12\x0f\n\x07scaling\x18\x06 \x01(\t\x12\x16\n\x0e\x64iscretisation\x18\x07 \x01(\t\x12\x1e\n\x16variableTransformation\x18\x08 \x01(\t\x12\x17\n\x0foutlierHandling\x18\t \x01(\t\x12\x1e\n\x16\x64\x61tetimeTransformation\x18\n \x01(\t\x12X\n\x04text\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TextPipelineSpec\x12\x0c\n\x04\x64rop\x18\x0c \x01(\x08\x12\x13\n\x0bpassthrough\x18\r \x01(\x08\"\xcd\x02\n\x1c\x46\x65\x61tureEngineeringSearchSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\testimator\x18\x03 \x01(\t\x12\x11\n\tmaxModels\x18\x04 \x01(\x05\x12\x0f\n\x07maxTime\x18\x05 \x01(\x05\x12\x10\n\x08trainers\x18\x06 \x01(\x05\x12\r\n\x05reuse\x18\t \x01(\x08\x12h\n\x10\x66\x65\x61tureSelection\x18\n \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\"\x80\x01\n\x1e\x46\x65\x61tureEngineeringSearchStatus\x12^\n\x04\x62\x65st\x18\x01 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\"\xf7\x01\n\x16\x46\x65\x61tureEngineeringSpec\x12g\n\tpipelines\x18\x01 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringPipeline\x12\x11\n\timbalance\x18\x02 \x01(\t\x12\x61\n\tselection\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\"8\n\x11\x46\x65\x61tureImportance\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x01\":\n\x0b\x46\x65\x61tureInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"#\n\x0b\x46\x65\x61turePair\x12\t\n\x01x\x18\x01 \x01(\t\x12\t\n\x01y\x18\x02 \x01(\t\"\xd5\x01\n\x14\x46\x65\x61tureSelectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tembedding\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\x08\x12\x0f\n\x07wrapper\x18\x05 \x01(\x08\x12\x10\n\x08pipeline\x18\x06 \x03(\t\x12\x14\n\x0cvarThreshold\x18\x07 \x01(\x05\x12\x15\n\rcorrThreshold\x18\x08 \x01(\x05\x12\x13\n\x0bmaxFeatures\x18\t \x01(\x05\x12\x12\n\npercentile\x18\n \x01(\x05\x12\x10\n\x08reserved\x18\x0c \x03(\t\"\xf8\x07\n\x0e\x46orecasterSpec\x12Y\n\x06\x65vents\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TimeSeriesEvent\x12R\n\x04past\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12T\n\x06\x66uture\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12\x10\n\x08\x63overage\x18\x06 \x01(\x01\x12]\n\x0eoutputLocation\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x10\n\x08\x66\x65\x61tures\x18\x08 \x03(\t\x12\x0e\n\x06groups\x18\t \x03(\t\x12\x1a\n\x12predefinedTemplate\x18\n \x01(\t\x12T\n\tanomalies\x18\x0b \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Anomaly\x12\x14\n\x0ctrainEndData\x18\x0c \x01(\t\x12\x13\n\x0bvalueColumn\x18\r \x01(\t\x12\x11\n\thpoBudget\x18\x0e \x01(\x05\x12`\n\x11\x65valuationMetrics\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalMetrics\x12^\n\x10\x65valuationPeriod\x18\x10 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalPeriod\x12^\n\x0bseasonality\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalitySpec\x12\x12\n\nregressors\x18\x12 \x03(\t\x12\x18\n\x10laggedRegressors\x18\x13 \x03(\t\x12\x0e\n\x06growth\x18\x14 \x01(\t\x12\x0b\n\x03key\x18\x15 \x03(\t\x12\x12\n\nestimators\x18\x16 \x03(\t\x12\x0b\n\x03hts\x18\x17 \x01(\t\"e\n\x15GarbageCollectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12!\n\x19keepBestModelPerAlgorithm\x18\x02 \x01(\x08\x12\x18\n\x10keepPrunedModels\x18\x03 \x01(\x08\"\x8e\x01\n\x17GarbageCollectionStatus\x12\x1c\n\x14\x63ollectedModelsCount\x18\x01 \x01(\x05\x12U\n\x06models\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelResult\"f\n\x13GeneratedColumnSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x66irst\x18\x03 \x01(\t\x12\x0e\n\x06second\x18\x04 \x01(\t\x12\x10\n\x08original\x18\x05 \x01(\t\"V\n\x17GroupSplitLocationsSpec\x12\x1d\n\x15groupTrainingDataFile\x18\x01 \x01(\t\x12\x1c\n\x14groupTestingDataFile\x18\x02 \x01(\t\"2\n\x13HyperParameterValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"o\n\x10HyperbandOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x14\n\x0cmaxResources\x18\x02 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"\'\n\x11ImagePipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\";\n\x15ImbalanceHandlingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\timbalance\x18\x02 \x01(\t\"\x9a\x02\n\x14InterpretabilitySpec\x12\x0b\n\x03ice\x18\x01 \x01(\x08\x12W\n\x08icepairs\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x0c\n\x04lime\x18\x03 \x01(\x08\x12\x0c\n\x04shap\x18\x04 \x01(\t\x12X\n\tshappairs\x18\x05 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x16\n\x0e\x63ounterfactual\x18\x06 \x01(\x08\x12\x0e\n\x06\x61nchor\x18\x07 \x01(\x08\"\xaa\x04\n\x16InterpretabilityStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x11\x65xplainerLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x66\n\x17trainShapValuesLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x65\n\x16testShapValuesLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\nimportance\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\"k\n\x13MedianPrunerOptions\x12\x15\n\rstartupTrials\x18\x01 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x02 \x01(\x05\x12\x15\n\rintervalSteps\x18\x03 \x01(\x05\x12\x11\n\tminTrials\x18\x04 \x01(\x05\"\xf5\x01\n\x05Model\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStatus\"\x84\x02\n\nModelClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassStatus\"\xcd\x04\n\x12ModelClassDataSpec\x12[\n\x0cobservations\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12Z\n\x0bpredictions\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12L\n\x06schema\x18\x03 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latFile\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x12\n\nprimaryKey\x18\x05 \x03(\t\x12\x1c\n\x14predictionTimeColumn\x18\x06 \x01(\t\x12\x0e\n\x06target\x18\x07 \x01(\t\x12Q\n\x05tests\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x1e\n\x16onlineFeatureStoreName\x18\t \x01(\t\x12\x1f\n\x17offlineFeatureStoreName\x18\n \x01(\t\"\xa7\x01\n\x0eModelClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\"\x8d\x02\n\rModelClassRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Y\n\x04spec\x18\x02 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunSpec\x12]\n\x06status\x18\x03 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunStatus\"\xad\x01\n\x11ModelClassRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12V\n\x05items\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\"\xce\x01\n\x11ModelClassRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x16\n\x0emodelClassName\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x0b\n\x03ttl\x18\t \x01(\x05\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\"\xed\x04\n\x13ModelClassRunStatus\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x11\n\tstudyName\x18\x02 \x01(\t\x12\x11\n\tmodelName\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x07 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x08 \x01(\t\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12=\n\tupdatedAt\x18\x0c \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\r \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12>\n\npromotedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04\x61uto\x18\x0f \x01(\x08\x12\x37\n\napprovedBy\x18\x10 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bmodelsCount\x18\x11 \x01(\x05\x12\x43\n\nconditions\x18\x12 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xd5\x02\n\x15ModelClassServingSpec\x12W\n\x08template\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12`\n\x12monitoringSchedule\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12`\n\x12predictionSchedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0e\n\x06preSQL\x18\x04 \x03(\t\x12\x0f\n\x07postSQL\x18\x05 \x03(\t\"\xc9\x06\n\x0eModelClassSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\x12\x0f\n\x07subtask\x18\x05 \x01(\t\x12Y\n\tobjective\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12U\n\x08\x65ntities\x18\x07 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EntityRef\x12Z\n\x04\x64\x61ta\x18\x08 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassDataSpec\x12\x62\n\x08training\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassTrainingSpec\x12`\n\x07serving\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassServingSpec\x12_\n\x0cnotification\x18\x0b \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\x0ereportSchedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0c\n\x04\x66\x61st\x18\r \x01(\x08\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12\x12\n\nregistered\x18\x0f \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x10 \x01(\t\"\xe7\x08\n\x10ModelClassStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12j\n\x16trainingScheduleStatus\x18\x04 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18predictionScheduleStatus\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18monitoringScheduleStatus\x18\x06 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12h\n\x14reportScheduleStatus\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x16\n\x0e\x62\x65stModelScore\x18\x08 \x01(\x01\x12\x0f\n\x07retired\x18\t \x03(\t\x12\x15\n\rpredictorName\x18\n \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x0b \x01(\t\x12\x13\n\x0btriggeredBy\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0e \x01(\t\x12=\n\tlastRunAt\x18\x0f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0blastRunName\x18\x10 \x01(\t\x12\x44\n\x10lastPredictionAt\x18\x11 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12lastPredictionName\x18\x12 \x01(\t\x12\x18\n\x10predictionsCount\x18\x13 \x01(\x05\x12\x11\n\trunsCount\x18\x14 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x15 \x01(\x05\x12\x0c\n\x04live\x18\x16 \x01(\x08\x12\x17\n\x0fpredictorsCount\x18\x17 \x01(\x05\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x87\x05\n\x16ModelClassTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x19\n\x11studyTemplateName\x18\x02 \x01(\t\x12Z\n\x0emodelUnitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12^\n\x10trainingSchedule\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12g\n\x0bsearchSpace\x18\x08 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\x12\x0e\n\x06paused\x18\x0b \x01(\x08\x12\x0f\n\x07maxTime\x18\x0c \x01(\x05\x12\x11\n\tmaxModels\x18\r \x01(\x05\x12\x10\n\x08trainers\x18\x0e \x01(\x05\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x11\n\texplained\x18\x10 \x01(\x08\x12\x0e\n\x06preSQL\x18\x11 \x03(\t\x12\x0f\n\x07postSQL\x18\x12 \x03(\t\"\xb3\x01\n\x12ModelGroupByStatus\x12\x11\n\tmodelsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x14\n\x0c\x66orecastsURI\x18\x03 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\tModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"]\n\x0bModelResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\talgorithm\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x01\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x0f\n\x07trialID\x18\x05 \x01(\x05\"\x95\x0c\n\tModelSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x03 \x01(\t\x12\x11\n\tstudyName\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x05 \x01(\t\x12\x0c\n\x04task\x18\x06 \x01(\t\x12\x0f\n\x07subtask\x18\x07 \x01(\t\x12Y\n\tobjective\x18\x08 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12l\n\x12\x66\x65\x61tureEngineering\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12\x63\n\testimator\x18\n \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12X\n\x08\x65nsemble\x18\x0b \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsembleSpec\x12X\n\x08training\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x0c\n\x04test\x18\r \x01(\x08\x12\r\n\x05\x61\x62ort\x18\x0e \x01(\x08\x12\x0f\n\x07package\x18\x0f \x01(\x08\x12\x0e\n\x06report\x18\x10 \x01(\x08\x12\r\n\x05pause\x18\x11 \x01(\x08\x12\x0f\n\x07profile\x18\x12 \x01(\x08\x12\x10\n\x08\x66orecast\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x14 \x01(\x08\x12\x10\n\x08unitTest\x18\x15 \x01(\x08\x12\x10\n\x08\x62\x61seline\x18\x16 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x17 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x18 \x01(\t\x12]\n\x0b\x66orecasting\x18\x19 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x1a \x01(\x03\x12\x15\n\restimatorType\x18\x1b \x01(\t\x12\x12\n\nmodelClass\x18\x1c \x01(\t\x12\x0f\n\x07trialID\x18\x1d \x01(\x05\x12T\n\x08\x61pproval\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12h\n\x10interpretability\x18\x1f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12U\n\tunitTests\x18  \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12q\n\x12partitionLocations\x18! \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PartitionModelLocationsSpec\x12\x16\n\x0emodelClassName\x18\" \x01(\t\x12\x19\n\x11modelClassRunName\x18# \x01(\t\x12_\n\x0cnotification\x18$ \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\"\x93\x02\n\x10ModelStageStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05\x65rror\x18\n \x01(\t\"\xeb\"\n\x0bModelStatus\x12\x45\n\x11trainingStartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12G\n\x13trainingCompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x44\n\x10testingStartedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x46\n\x12testingCompletedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0fvalidationScore\x18\x08 \x01(\x01\x12\x15\n\rtrainingScore\x18\t \x01(\x01\x12\x11\n\ttestScore\x18\n \x01(\x01\x12X\n\nvalidation\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12S\n\x05train\x18\x0e \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04test\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04tune\x18\x10 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12V\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x11 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05phase\x18\x12 \x01(\t\x12\x12\n\nreportName\x18\x13 \x01(\t\x12]\n\x0ereportLocation\x18\x14 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x63\n\x14trainWeightsLocation\x18\x15 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testWeightsLocation\x18\x16 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13\x66ullWeightsLocation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19trainLabelEncoderLocation\x18\x18 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fprofileLocation\x18\x1b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19misclassificationLocation\x18\x1c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\x10\x66orecastLocation\x18\x1d \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fpackageLocation\x18\x1e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12g\n\x12impurityImportance\x18\x1f \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12j\n\x15permutationImportance\x18  \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12X\n\x07runtime\x18! \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus\x12\x63\n\x14trainDatasetLocation\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18# \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18$ \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18% \x01(\x03\x12\x14\n\x0ctrainingRows\x18& \x01(\x05\x12\x13\n\x0btestingRows\x18\' \x01(\x05\x12\x16\n\x0evalidationRows\x18( \x01(\x05\x12\x16\n\x0e\x66\x61ilureMessage\x18* \x01(\t\x12\x10\n\x08progress\x18+ \x01(\x05\x12\x13\n\x0bsizeInBytes\x18, \x01(\x05\x12\x0f\n\x07latency\x18- \x01(\x01\x12X\n\x07serving\x18/ \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingStatus\x12\x13\n\x0btarFileHash\x18\x30 \x01(\t\x12^\n\x10trainingDataHash\x18\x31 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12g\n\x11trainingResources\x18\x32 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x66\n\x10testingResources\x18\x33 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x11\n\ttrainedBy\x18\x34 \x01(\t\x12K\n\x04logs\x18\x35 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12V\n\x08rocCurve\x18\x36 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RocAucCurve\x12Q\n\x07prCurve\x18\x37 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PRCurve\x12\x66\n\x14trainConfusionMatrix\x18\x38 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18\x39 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x61\n\x16\x63orrelationsWithTarget\x18: \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18; \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12=\n\tupdatedAt\x18< \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12V\n\x08\x61pproval\x18= \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalStatus\x12j\n\x10interpretability\x18> \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilityStatus\x12O\n\x06images\x18? \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12\x61\n\x0funitTestResults\x18@ \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x65\n\x13\x66\x65\x65\x64\x62\x61\x63kTestResults\x18\x41 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12]\n\x07groupby\x18\x42 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus\x12[\n\x05usage\x18\x44 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x45 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdf\x01\n\x0eModelTestSuite\x12=\n\x10\x62\x61selineModelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\ndatasetRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"/\n\x10NNLayerParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"=\n\x10OutlierModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10outlierAlgorithm\x18\x02 \x01(\t\"\xcc\x01\n\x1bPartitionModelLocationsSpec\x12\x17\n\x0fpartitionFolder\x18\x01 \x01(\t\x12\x1e\n\x16partitionProfileFolder\x18\x02 \x01(\t\x12\x1b\n\x13partitionReportFile\x18\x03 \x01(\t\x12\x1c\n\x14partitionModelFolder\x18\x04 \x01(\t\x12\x1a\n\x12partitionModelFile\x18\x05 \x01(\t\x12\x1d\n\x15partitionForecastFile\x18\x06 \x01(\t\"\x84\x01\n\x17PercentilePrunerOptions\x12\x12\n\npercentile\x18\x01 \x01(\x05\x12\x15\n\rstartupTrials\x18\x02 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x16\n\x0eintervalTrials\x18\x04 \x01(\x05\x12\x11\n\tminTrials\x18\x05 \x01(\x05\"\x93\x04\n\nPrunerSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12]\n\x06median\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.MedianPrunerOptions\x12\x65\n\npercentile\x18\x03 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PercentilePrunerOptions\x12m\n\x11successiveHalving\x18\x04 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingOptions\x12]\n\thyperband\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperbandOptions\x12\x63\n\tthreshold\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ThresholdPrunerOptions\"\xd0\x01\n\x18RegressionForecasterSpec\x12\x10\n\x08\x65nsemble\x18\x01 \x01(\x08\x12\x12\n\nimputation\x18\x02 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x0f\n\x07scaling\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\x08\x12\x0f\n\x07windows\x18\x06 \x03(\x05\x12\x0c\n\x04lags\x18\x07 \x03(\x05\x12\x11\n\tfunctions\x18\x08 \x03(\t\x12\x0b\n\x03\x65ma\x18\t \x01(\x08\x12\x0b\n\x03log\x18\n \x01(\x08\x12\x11\n\treduction\x18\x0b \x01(\t\"\xf8\x01\n\x06Report\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportStatus\"\x8a\x01\n\x13ReportGroupByStatus\x12\x12\n\nreportsURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9f\x01\n\nReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe9\x03\n\nReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x36\n\tentityRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nreportType\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12_\n\x0cnotification\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\x06 \x01(\t\x12X\n\tresources\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x08 \x01(\x03\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03key\x18\n \x03(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x0b \x01(\t\x12\x16\n\x0emodelClassName\x18\x0c \x01(\t\x12\x19\n\x11modelClassRunName\x18\r \x01(\t\"\xb3\x04\n\x0cReportStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12^\n\x07groupby\x18\t \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportGroupByStatus\x12\x43\n\nconditions\x18\n \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xde\x01\n\rRuntimeStatus\x12\x15\n\rpythonVersion\x18\x01 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12s\n\x0epythonPackages\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus.PythonPackagesEntry\x1a\x35\n\x13PythonPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x05\n\nSearchSpec\x12\x0f\n\x07sampler\x18\x01 \x01(\t\x12T\n\x06pruner\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PrunerSpec\x12\x0f\n\x07maxTime\x18\x04 \x01(\x05\x12\x11\n\tmaxModels\x18\x05 \x01(\x05\x12\x10\n\x08maxScore\x18\x06 \x01(\x01\x12\x10\n\x08trainers\x18\x07 \x01(\x05\x12\x0c\n\x04test\x18\x08 \x01(\x05\x12\x11\n\tretainTop\x18\t \x01(\x05\x12\x13\n\x0bretainedFor\x18\n \x01(\x05\x12g\n\x0bsearchSpace\x18\x0b \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\x12Y\n\tobjective\x18\r \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x62\n\x12secondaryObjective\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x0c\n\x04goal\x18\x0f \x01(\t\"L\n\x15SeasonalityPeriodSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x61uto\x18\x02 \x01(\x08\x12\x14\n\x0c\x66ourierOrder\x18\x03 \x01(\x05\"\x87\x04\n\x0fSeasonalitySpec\x12\x0c\n\x04\x61uto\x18\x01 \x01(\x08\x12_\n\x06yearly\x18\x02 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12\x62\n\tquarterly\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12`\n\x07monthly\x18\x04 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12_\n\x06weekly\x18\x05 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12^\n\x05\x64\x61ily\x18\x06 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\"\xb7\x03\n\x12ServingEnvironment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12;\n\x0eservingSiteRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12S\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x05 \x01(\x05\x12\x0e\n\x06online\x18\x06 \x01(\x08\x12\x11\n\tdashboard\x18\x07 \x01(\x08\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0e\n\x06preSQL\x18\t \x03(\t\x12\x0f\n\x07postSQL\x18\n \x03(\t\"\xd2\x03\n\x0bServingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12X\n\tresources\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingSiteRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x11\n\tdashboard\x18\x08 \x01(\x08\x12S\n\x06\x61\x63\x63\x65ss\x18\t \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\n \x01(\x05\x12\x11\n\tpromotion\x18\x0c \x01(\t\x12\x37\n\napprovedBy\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\x7f\n\rServingStatus\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x03 \x01(\t\x12\x19\n\x11predictorEndpoint\x18\x04 \x01(\t\x12\x19\n\x11\x64\x61shboardEndpoint\x18\x05 \x01(\t\x12\x0c\n\x04role\x18\x06 \x01(\t\"\xf5\x01\n\x05Study\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudySpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyStatus\"\x9d\x01\n\tStudyList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\xb4\x02\n\x10StudyPhaseStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12waitingModelsCount\x18\x03 \x01(\x05\x12\x1a\n\x12runningModelsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x66\x61iledModelsCount\x18\x05 \x01(\x05\x12\x1c\n\x14\x63ompletedModelsCount\x18\x06 \x01(\x05\x12\x11\n\tbestScore\x18\x07 \x01(\x01\x12\x1c\n\x14modelsWithNoProgress\x18\x08 \x01(\x05\"a\n\x11StudyScheduleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12;\n\x07startAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xc5\x0e\n\tStudySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetName\x18\x04 \x01(\t\x12\x0c\n\x04task\x18\x05 \x01(\t\x12\x0f\n\x07subtask\x18\x06 \x01(\t\x12h\n\x08\x66\x65Search\x18\x07 \x01(\x0b\x32V.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSearchSpec\x12i\n\x10imbalanceHandler\x18\x08 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImbalanceHandlingSpec\x12X\n\x08\x62\x61seline\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.BaselineSpec\x12T\n\x06search\x18\n \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SearchSpec\x12Z\n\tensembles\x18\x0b \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsemblesSpec\x12`\n\x10trainingTemplate\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x62\n\x10\x66orecastTemplate\x18\r \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12]\n\x08schedule\x18\x0e \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyScheduleSpec\x12h\n\x10interpretability\x18\x0f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12`\n\x0coutlierModel\x18\x10 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.OutlierModelSpec\x12\r\n\x05\x61\x62ort\x18\x11 \x01(\x08\x12\x0e\n\x06report\x18\x12 \x01(\x08\x12\r\n\x05pause\x18\x13 \x01(\x08\x12\x0f\n\x07profile\x18\x14 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x15 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x16 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x17 \x01(\t\x12\r\n\x05owner\x18\x18 \x01(\t\x12\x10\n\x08template\x18\x19 \x01(\x08\x12_\n\x0cnotification\x18\x1a \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12[\n\x02gc\x18\x1b \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionSpec\x12\x14\n\x0cmodelVersion\x18\x1c \x01(\t\x12\x0f\n\x07timeout\x18\x1d \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12i\n\x0egroupLocations\x18\x1f \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GroupSplitLocationsSpec\x12\x16\n\x0emodelClassName\x18  \x01(\t\x12\x19\n\x11modelClassRunName\x18! \x01(\t\x12V\n\x07serving\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\"\xfe\x10\n\x0bStudyStatus\x12\x13\n\x0bmodelsCount\x18\x01 \x01(\x05\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tbestModel\x18\x03 \x01(\t\x12\x16\n\x0e\x62\x65stModelScore\x18\x04 \x01(\x01\x12^\n\x0fprofileLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12]\n\x0ereportLocation\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x12\n\nreportName\x18\x07 \x01(\t\x12\r\n\x05phase\x18\x08 \x01(\t\x12\x1a\n\x12observedGeneration\x18\t \x01(\x03\x12\x63\n\x14trainDatasetLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18\x0b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12`\n\x11optimizerLocation\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x13\n\x0blastModelID\x18\x0e \x01(\x03\x12\x15\n\rfailureReason\x18\x0f \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x10 \x01(\t\x12\x19\n\x11trainingRowsCount\x18\x11 \x01(\x05\x12\x18\n\x10testingRowsCount\x18\x12 \x01(\x05\x12\x1b\n\x13validationRowsCount\x18\x13 \x01(\x05\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12^\n\x10trainingDataHash\x18\x15 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12\x13\n\x0btriggeredBy\x18\x16 \x01(\t\x12K\n\x04logs\x18\x17 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x66\n\x12\x66\x65\x61tureEngineering\x18\x18 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x62\x61seline\x18\x19 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12Z\n\x06search\x18\x1a \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x65nsemble\x18\x1b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12X\n\x04test\x18\x1c \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12[\n\x07\x65xplain\x18\x1d \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\x65\n\x0e\x64riftDetection\x18\x1e \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftDetectorStatus\x12=\n\tupdatedAt\x18\x1f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12p\n\x16\x62\x65stFeatureEngineering\x18  \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12]\n\x02gc\x18! \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionStatus\x12\x43\n\nconditions\x18% \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x7f\n\x18SuccessiveHalvingOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x02 \x01(\x05\x12\x1c\n\x14minEarlyStoppingRate\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"h\n\x15SuccessiveHalvingSpec\x12\x0e\n\x06\x62udget\x18\x01 \x01(\x05\x12\x0f\n\x07\x62racket\x18\x02 \x01(\x05\x12\x0c\n\x04rung\x18\x03 \x01(\x05\x12\x0e\n\x06\x63onfID\x18\x04 \x01(\x05\x12\x10\n\x08modality\x18\x1a \x01(\t\"\xad\x01\n\x10TextPipelineSpec\x12\x0f\n\x07\x65ncoder\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x02 \x01(\t\x12\x11\n\tstopwords\x18\x03 \x01(\x08\x12\x0b\n\x03pos\x18\x04 \x01(\x08\x12\r\n\x05lemma\x18\x05 \x01(\x08\x12\x0c\n\x04stem\x18\x06 \x01(\x08\x12\x11\n\tembedding\x18\x07 \x01(\t\x12\x0b\n\x03svd\x18\x08 \x01(\x08\x12\x18\n\x10maxSvdComponents\x18\t \x01(\x05\"b\n\x16ThresholdPrunerOptions\x12\r\n\x05lower\x18\x01 \x01(\x01\x12\r\n\x05upper\x18\x02 \x01(\x01\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x15\n\rintervalSteps\x18\x04 \x01(\x05\"\x8a\x01\n\x0fTimeSeriesEvent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0f\n\x07holiday\x18\x03 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x10\n\x08preEvent\x18\x05 \x01(\x05\x12\x11\n\tpostEvent\x18\x06 \x01(\x05\x12\x12\n\ntimePoints\x18\x07 \x03(\t\"\xe2\x04\n\x0cTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08priority\x18\x02 \x01(\t\x12\x0e\n\x06\x63vtype\x18\x03 \x01(\t\x12\r\n\x05\x66olds\x18\x05 \x01(\x05\x12V\n\x05split\x18\x06 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataSplitSpec\x12\x13\n\x0b\x65valMetrics\x18\x07 \x03(\t\x12[\n\x02sh\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingSpec\x12\x0c\n\x04seed\x18\x0b \x01(\x01\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03gpu\x18\r \x01(\x08\x12\x19\n\x11\x66\x65\x61tureImportance\x18\x0f \x01(\x08\x12\x11\n\tsamplePct\x18\x11 \x01(\x05\x12\\\n\ncheckpoint\x18\x12 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CheckpointSpec\x12\x10\n\x08logLevel\x18\x13 \x01(\t\x12\x0f\n\x07timeout\x18\x14 \x01(\x05\"\xdc\x01\n\x18UnivariateForecastStatus\x12\x1b\n\x13gridSearchResultURI\x18\x01 \x01(\t\x12g\n\rbaseEstimator\x18\x02 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x10\n\x08modelURI\x18\x03 \x01(\t\x12\x13\n\x0b\x63vResultURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x05 \x01(\t\"\'\n\x11VideoPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"=\n\nWindowSpec\x12\x10\n\x08interval\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x0e\n\x06length\x18\x03 \x01(\x05\x42:Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1'
@@ -180,41 +180,41 @@
   _SEASONALITYPERIODSPEC._serialized_start=23313
   _SEASONALITYPERIODSPEC._serialized_end=23389
   _SEASONALITYSPEC._serialized_start=23392
   _SEASONALITYSPEC._serialized_end=23911
   _SERVINGENVIRONMENT._serialized_start=23914
   _SERVINGENVIRONMENT._serialized_end=24353
   _SERVINGSPEC._serialized_start=24356
-  _SERVINGSPEC._serialized_end=24838
-  _SERVINGSTATUS._serialized_start=24840
-  _SERVINGSTATUS._serialized_end=24967
-  _STUDY._serialized_start=24970
-  _STUDY._serialized_end=25215
-  _STUDYLIST._serialized_start=25218
-  _STUDYLIST._serialized_end=25375
-  _STUDYPHASESTATUS._serialized_start=25378
-  _STUDYPHASESTATUS._serialized_end=25686
-  _STUDYSCHEDULESPEC._serialized_start=25688
-  _STUDYSCHEDULESPEC._serialized_end=25785
-  _STUDYSPEC._serialized_start=25788
-  _STUDYSPEC._serialized_end=27649
-  _STUDYSTATUS._serialized_start=27652
-  _STUDYSTATUS._serialized_end=29826
-  _SUCCESSIVEHALVINGOPTIONS._serialized_start=29828
-  _SUCCESSIVEHALVINGOPTIONS._serialized_end=29955
-  _SUCCESSIVEHALVINGSPEC._serialized_start=29957
-  _SUCCESSIVEHALVINGSPEC._serialized_end=30061
-  _TEXTPIPELINESPEC._serialized_start=30064
-  _TEXTPIPELINESPEC._serialized_end=30237
-  _THRESHOLDPRUNEROPTIONS._serialized_start=30239
-  _THRESHOLDPRUNEROPTIONS._serialized_end=30337
-  _TIMESERIESEVENT._serialized_start=30340
-  _TIMESERIESEVENT._serialized_end=30478
-  _TRAININGSPEC._serialized_start=30481
-  _TRAININGSPEC._serialized_end=31091
-  _UNIVARIATEFORECASTSTATUS._serialized_start=31094
-  _UNIVARIATEFORECASTSTATUS._serialized_end=31314
-  _VIDEOPIPELINESPEC._serialized_start=31316
-  _VIDEOPIPELINESPEC._serialized_end=31355
-  _WINDOWSPEC._serialized_start=31357
-  _WINDOWSPEC._serialized_end=31418
+  _SERVINGSPEC._serialized_end=24822
+  _SERVINGSTATUS._serialized_start=24824
+  _SERVINGSTATUS._serialized_end=24951
+  _STUDY._serialized_start=24954
+  _STUDY._serialized_end=25199
+  _STUDYLIST._serialized_start=25202
+  _STUDYLIST._serialized_end=25359
+  _STUDYPHASESTATUS._serialized_start=25362
+  _STUDYPHASESTATUS._serialized_end=25670
+  _STUDYSCHEDULESPEC._serialized_start=25672
+  _STUDYSCHEDULESPEC._serialized_end=25769
+  _STUDYSPEC._serialized_start=25772
+  _STUDYSPEC._serialized_end=27633
+  _STUDYSTATUS._serialized_start=27636
+  _STUDYSTATUS._serialized_end=29810
+  _SUCCESSIVEHALVINGOPTIONS._serialized_start=29812
+  _SUCCESSIVEHALVINGOPTIONS._serialized_end=29939
+  _SUCCESSIVEHALVINGSPEC._serialized_start=29941
+  _SUCCESSIVEHALVINGSPEC._serialized_end=30045
+  _TEXTPIPELINESPEC._serialized_start=30048
+  _TEXTPIPELINESPEC._serialized_end=30221
+  _THRESHOLDPRUNEROPTIONS._serialized_start=30223
+  _THRESHOLDPRUNEROPTIONS._serialized_end=30321
+  _TIMESERIESEVENT._serialized_start=30324
+  _TIMESERIESEVENT._serialized_end=30462
+  _TRAININGSPEC._serialized_start=30465
+  _TRAININGSPEC._serialized_end=31075
+  _UNIVARIATEFORECASTSTATUS._serialized_start=31078
+  _UNIVARIATEFORECASTSTATUS._serialized_end=31298
+  _VIDEOPIPELINESPEC._serialized_start=31300
+  _VIDEOPIPELINESPEC._serialized_end=31339
+  _WINDOWSPEC._serialized_start=31341
+  _WINDOWSPEC._serialized_end=31402
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py` & `modelaapi-0.6.221/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/google/api/annotations_pb2.py` & `modelaapi-0.6.221/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/google/api/http_pb2.py` & `modelaapi-0.6.221/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/k8s/io/api/apps/v1/generated_pb2.py` & `modelaapi-0.6.221/k8s/io/api/apps/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/k8s/io/api/core/v1/generated_pb2.py` & `modelaapi-0.6.221/k8s/io/api/core/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/k8s/io/api/rbac/v1/generated_pb2.py` & `modelaapi-0.6.221/k8s/io/api/rbac/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py` & `modelaapi-0.6.221/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py` & `modelaapi-0.6.221/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/generated_pb2.py` & `modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py` & `modelaapi-0.6.221/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py` & `modelaapi-0.6.221/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/modelaapi/consts.py` & `modelaapi-0.6.221/modelaapi/consts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/modelaapi/custom_transformers.py` & `modelaapi-0.6.221/modelaapi/custom_transformers.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/modelaapi/graykite_model.py` & `modelaapi-0.6.221/modelaapi/graykite_model.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/modelaapi/ts.py` & `modelaapi-0.6.221/modelaapi/ts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/modelaapi/version.py` & `modelaapi-0.6.221/modelaapi/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
     "minor": 6,
-    "micro": 220,
+    "micro": 221,
     "releaselevel": "alpha",
     "post": 0,
     "serial": 1,
 }
 
 ##########################################################################
 ## Helper Functions
```

### Comparing `modelaapi-0.6.220/modelaapi.egg-info/PKG-INFO` & `modelaapi-0.6.221/modelaapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.220
+Version: 0.6.221
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.220
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.221
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.220
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.221
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.220/modelaapi.egg-info/SOURCES.txt` & `modelaapi-0.6.221/modelaapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/setup.cfg` & `modelaapi-0.6.221/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.220/setup.py` & `modelaapi-0.6.221/setup.py`

 * *Files identical despite different names*

