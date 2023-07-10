# Comparing `tmp/modelaapi-0.6.210.tar.gz` & `tmp/modelaapi-0.6.220.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelaapi-0.6.210.tar", last modified: Thu Jul  6 17:47:30 2023, max compression
+gzip compressed data, was "modelaapi-0.6.220.tar", last modified: Mon Jul 10 18:39:24 2023, max compression
```

## Comparing `modelaapi-0.6.210.tar` & `modelaapi-0.6.220.tar`

### file list

```diff
@@ -1,481 +1,481 @@
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.444219 modelaapi-0.6.210/
--rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.210/AUTHORS.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.210/CONTRIBUTING.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.210/DESCRIPTION.md
--rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.210/HISTORY.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.210/LICENSE.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.210/MANIFEST.in
--rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.210/Makefile
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-06 17:47:30.444219 modelaapi-0.6.210/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.210/README.md
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.412218 modelaapi-0.6.210/github/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.412218 modelaapi-0.6.210/github/com/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.412218 modelaapi-0.6.210/github/com/gogo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/gogo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.412218 modelaapi-0.6.210/github/com/gogo/protobuf/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/gogo/protobuf/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.412218 modelaapi-0.6.210/github/com/gogo/protobuf/gogoproto/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/gogo/protobuf/gogoproto/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.412218 modelaapi-0.6.210/github/com/metaprov/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.412218 modelaapi-0.6.210/github/com/metaprov/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.412218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.412218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23368 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51010 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/inference/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23177 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/infra/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/team/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/training/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    56923 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/account/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/account/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/account/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/account/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/alert/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/alert/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/alert/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/attachment/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/attachment/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/attachment/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/batchpredictord/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.416218 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/batchpredictord/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7549 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/catalog/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/cloudproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/commit/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/commit/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/commit/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/common/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/common/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/common/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/common/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/connection/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/connection/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/connection/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/conversation/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/conversation/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/conversation/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/data/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/data/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    73562 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataapp/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataapp/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataapp/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipeline/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipeline/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipelinerun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproduct/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproduct/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.420219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproductversion/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproductversion/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataset/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataset/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataset/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datasource/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datasource/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datasource/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dbproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dbproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/entity/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/entity/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/entity/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featuregroup/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featuregroup/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featurehistogram/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featurehistogram/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/fileservices/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/fileservices/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/fileservices/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.424219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/grpcinferenceservice/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18564 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/k8score/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/k8score/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/k8score/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/lab/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/lab/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/lab/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/license/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/license/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/license/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/license/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/model/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/model/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/model/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/model/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelasystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelasystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modeldsystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modeldsystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/notifier/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/notifier/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/notifier/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/objectstored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/objectstored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/objectstored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/offlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.428219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/onlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/postmortem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/postmortem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/postmortem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/prediction/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/prediction/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/prediction/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictionstore/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictionstore/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictor/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictor/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictor/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/publisherd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/publisherd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/publisherd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/recipe/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/recipe/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/recipe/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/reciperun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/reciperun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/reciperun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/report/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/report/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/report/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/report/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/review/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/review/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/review/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/review/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/runbook/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/runbook/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/runbook/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/servingsite/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/servingsite/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.432219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/servingsite/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlquery/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlquery/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlqueryrun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/study/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/study/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/study/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/study/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/system/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/system/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/system/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/system/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/tenant/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/tenant/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/tenant/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/todo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/todo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/todo/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/trainerd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/trainerd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/trainerd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/userroleclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/userroleclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/virtualbucket/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/virtualbucket/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-07-06 17:34:17.000000 modelaapi-0.6.210/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/google/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/google/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/google/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/google/api/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-07-06 17:34:17.000000 modelaapi-0.6.210/google/api/annotations_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-06 17:34:17.000000 modelaapi-0.6.210/google/api/annotations_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-07-06 17:34:17.000000 modelaapi-0.6.210/google/api/http_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-06 17:34:17.000000 modelaapi-0.6.210/google/api/http_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/k8s/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/k8s/io/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/k8s/io/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.436219 modelaapi-0.6.210/k8s/io/api/apps/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/api/apps/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/api/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/api/apps/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-07-06 17:34:17.000000 modelaapi-0.6.210/k8s/io/api/apps/v1/generated_pb2.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/api/core/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/api/core/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/api/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/api/core/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-07-06 17:34:17.000000 modelaapi-0.6.210/k8s/io/api/core/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/api/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/api/rbac/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/api/rbac/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/api/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/api/rbac/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-07-06 17:34:17.000000 modelaapi-0.6.210/k8s/io/api/rbac/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/api/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/apimachinery/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/apimachinery/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/apimachinery/pkg/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/apimachinery/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/api/resource/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-07-06 17:34:17.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/apimachinery/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/apimachinery/pkg/apis/meta/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/apis/meta/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/apimachinery/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-07-06 17:34:17.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/apimachinery/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/runtime/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-07-06 17:34:17.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/apimachinery/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-07-06 17:34:17.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/apimachinery/pkg/util/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/util/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/k8s/io/apimachinery/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/util/intstr/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-07-06 17:34:17.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.210/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.210/modelaapi/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.210/modelaapi/consts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.210/modelaapi/custom_transformers.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.210/modelaapi/graykite_model.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.210/modelaapi/ts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-07-06 17:47:19.000000 modelaapi-0.6.210/modelaapi/version.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-06 17:47:30.440219 modelaapi-0.6.210/modelaapi.egg-info/
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-06 17:47:30.000000 modelaapi-0.6.210/modelaapi.egg-info/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-07-06 17:47:30.000000 modelaapi-0.6.210/modelaapi.egg-info/SOURCES.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-07-06 17:47:30.000000 modelaapi-0.6.210/modelaapi.egg-info/dependency_links.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-07-06 17:47:30.000000 modelaapi-0.6.210/modelaapi.egg-info/entry_points.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.210/modelaapi.egg-info/not-zip-safe
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-07-06 17:47:30.000000 modelaapi-0.6.210/modelaapi.egg-info/requires.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-07-06 17:47:30.000000 modelaapi-0.6.210/modelaapi.egg-info/top_level.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.210/requirements.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-07-06 17:47:30.444219 modelaapi-0.6.210/setup.cfg
--rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.210/setup.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.482425 modelaapi-0.6.220/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.220/AUTHORS.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.220/CONTRIBUTING.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.220/DESCRIPTION.md
+-rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.220/HISTORY.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.220/LICENSE.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.220/MANIFEST.in
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.220/Makefile
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-10 18:39:24.482425 modelaapi-0.6.220/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.220/README.md
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/gogo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/gogo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/gogo/protobuf/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/gogo/protobuf/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/gogo/protobuf/gogoproto/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/gogo/protobuf/gogoproto/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23368 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    50953 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.450424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23177 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    56923 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4692 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.454424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    73562 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.458424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18564 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.462424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.466424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.470425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.474424 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-07-10 18:38:20.000000 modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/google/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/google/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/google/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/google/api/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-07-10 18:38:20.000000 modelaapi-0.6.220/google/api/annotations_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/google/api/annotations_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-07-10 18:38:20.000000 modelaapi-0.6.220/google/api/http_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-10 18:38:20.000000 modelaapi-0.6.220/google/api/http_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/apps/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/apps/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/apps/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/api/apps/v1/generated_pb2.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/core/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/core/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/core/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/api/core/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/rbac/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/rbac/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/api/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/rbac/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/api/rbac/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/api/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/resource/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.478425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.482425 modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/intstr/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-07-10 18:38:20.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.482425 modelaapi-0.6.220/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.220/modelaapi/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.220/modelaapi/consts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.220/modelaapi/custom_transformers.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.220/modelaapi/graykite_model.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.220/modelaapi/ts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-07-10 18:38:58.000000 modelaapi-0.6.220/modelaapi/version.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-10 18:39:24.482425 modelaapi-0.6.220/modelaapi.egg-info/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-10 18:39:24.000000 modelaapi-0.6.220/modelaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-07-10 18:39:24.000000 modelaapi-0.6.220/modelaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-07-10 18:39:24.000000 modelaapi-0.6.220/modelaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-07-10 18:39:24.000000 modelaapi-0.6.220/modelaapi.egg-info/entry_points.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.220/modelaapi.egg-info/not-zip-safe
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-07-10 18:39:24.000000 modelaapi-0.6.220/modelaapi.egg-info/requires.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-07-10 18:39:24.000000 modelaapi-0.6.220/modelaapi.egg-info/top_level.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.220/requirements.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-07-10 18:39:24.482425 modelaapi-0.6.220/setup.cfg
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.220/setup.py
```

### Comparing `modelaapi-0.6.210/CONTRIBUTING.rst` & `modelaapi-0.6.220/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/LICENSE.txt` & `modelaapi-0.6.220/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/Makefile` & `modelaapi-0.6.220/Makefile`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/PKG-INFO` & `modelaapi-0.6.220/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.210
+Version: 0.6.220
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.210
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.220
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.210
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.220
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.210/README.md` & `modelaapi-0.6.220/README.md`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/gogo/protobuf/gogoproto/gogo_pb2.py` & `modelaapi-0.6.220/github/com/gogo/protobuf/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_catalog_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nDgithub.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x12\x34github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x87\x01\n\x14\x41pprovalReviewStatus\x12\x10\n\x08reviewer\x18\x01 \x01(\t\x12\x0e\n\x06result\x18\x02 \x01(\t\x12>\n\napprovedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05notes\x18\x04 \x01(\t\"F\n\x0c\x41pprovalSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x14\n\x0c\x64\x65\x63isionType\x18\x02 \x01(\t\x12\x0f\n\x07members\x18\x03 \x03(\t\"}\n\x0e\x41pprovalStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12[\n\x07reviews\x18\x02 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalReviewStatus\"W\n\x0c\x42\x61rChartSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\x12\x0e\n\x06legend\x18\x04 \x01(\x08\x12\x0c\n\x04sort\x18\x05 \x01(\x08\"\xa0\x07\n\x06\x43olumn\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x02 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x0e\n\x06ignore\x18\x06 \x01(\x08\x12\x0e\n\x06target\x18\x07 \x01(\x08\x12\x10\n\x08nullable\x18\x08 \x01(\x08\x12\n\n\x02pk\x18\t \x01(\x08\x12\n\n\x02\x66k\x18\n \x01(\x08\x12\x12\n\nmultipleOf\x18\x0b \x01(\x05\x12\x0f\n\x07maximum\x18\x0c \x01(\x01\x12\x18\n\x10\x65xclusiveMaximum\x18\r \x01(\x08\x12\x0f\n\x07minimum\x18\x0e \x01(\x01\x12\x18\n\x10\x65xclusiveMinimum\x18\x0f \x01(\x08\x12\x11\n\tmaxLength\x18\x10 \x01(\x05\x12\x11\n\tminLength\x18\x11 \x01(\x05\x12\x0f\n\x07pattern\x18\x12 \x01(\t\x12\x10\n\x08required\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xample\x18\x14 \x01(\t\x12\x14\n\x0c\x65xternalDocs\x18\x15 \x01(\t\x12\x0c\n\x04\x65num\x18\x16 \x03(\t\x12\x10\n\x08maxItems\x18\x18 \x01(\x05\x12\x10\n\x08minItems\x18\x19 \x01(\x05\x12\x13\n\x0buniqueItems\x18\x1a \x01(\x08\x12\x0b\n\x03pii\x18\x1c \x01(\x08\x12\x0b\n\x03phi\x18\x1d \x01(\x08\x12\x11\n\tprotected\x18\x1f \x01(\x08\x12\x17\n\x0f\x64\x65\x66\x61ultValueNum\x18  \x01(\x01\x12\x0b\n\x03log\x18! \x01(\x08\x12\n\n\x02mu\x18\" \x01(\x01\x12\r\n\x05sigma\x18# \x01(\x01\x12\x15\n\rskewThreshold\x18$ \x01(\x01\x12\x16\n\x0e\x64riftThreshold\x18% \x01(\x01\x12\x0b\n\x03key\x18& \x01(\x08\x12\x0c\n\x04\x66old\x18\' \x01(\x08\x12\x0e\n\x06weight\x18( \x01(\x08\x12\x10\n\x08reserved\x18) \x01(\x08\x12\x12\n\nimputation\x18* \x01(\t\x12\x0f\n\x07scaling\x18+ \x01(\t\x12\x11\n\tgenerated\x18, \x01(\x08\x12\x0f\n\x07\x66ormula\x18- \x01(\t\x12\n\n\x02id\x18. \x01(\x08\x12\x0c\n\x04step\x18/ \x01(\x01\x12\x0b\n\x03loc\x18\x30 \x01(\x05\x12\x16\n\x0e\x64\x61tetimeFormat\x18\x31 \x01(\t\x12\x12\n\ntimeseries\x18\x32 \x01(\x08\x12\x11\n\tregressor\x18\x33 \x01(\x08\x12\x17\n\x0flaggedRegressor\x18\x34 \x01(\x08\x12\x11\n\ttimeIndex\x18\x35 \x01(\x08\x12\x0c\n\x04\x61ggr\x18\x36 \x01(\t\x12\x0e\n\x06window\x18\x37 \x01(\x05\"\xe0\x01\n\x0f\x43olumnHistogram\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Y\n\thistogram\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.HistogramData\x12U\n\x07metrics\x18\x03 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05\x64rift\x18\x04 \x01(\x08\"\x81\x01\n\nColumnSpec\x12\x0e\n\x06spacer\x18\x01 \x01(\x08\x12\r\n\x05width\x18\x02 \x01(\x05\x12T\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ComponentSpec\"\x92\x07\n\x10\x43olumnStatistics\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x01\x12\x10\n\x08\x64istinct\x18\x04 \x01(\x05\x12\x0f\n\x07missing\x18\x05 \x01(\x05\x12\x16\n\x0epercentMissing\x18\x06 \x01(\x01\x12\x0c\n\x04mean\x18\x07 \x01(\x01\x12\x0e\n\x06stddev\x18\x08 \x01(\x01\x12\x10\n\x08variance\x18\t \x01(\x01\x12\x0b\n\x03min\x18\n \x01(\x01\x12\x0b\n\x03max\x18\x0b \x01(\x01\x12\x10\n\x08kurtosis\x18\x0c \x01(\x01\x12\x10\n\x08skewness\x18\r \x01(\x01\x12\x0b\n\x03sum\x18\x0e \x01(\x01\x12\x0b\n\x03mad\x18\x0f \x01(\x01\x12\x0b\n\x03p25\x18\x10 \x01(\x01\x12\x0b\n\x03p50\x18\x11 \x01(\x01\x12\x0b\n\x03p75\x18\x12 \x01(\x01\x12\x0b\n\x03iqr\x18\x13 \x01(\x01\x12\x0c\n\x04mode\x18\x14 \x01(\t\x12\r\n\x05zeros\x18\x15 \x01(\x01\x12\x0f\n\x07invalid\x18\x16 \x01(\x05\x12\x12\n\nimportance\x18\x17 \x01(\x01\x12\x0e\n\x06target\x18\x18 \x01(\x08\x12\x0e\n\x06ignore\x18\x19 \x01(\x08\x12\x10\n\x08nullable\x18\x1a \x01(\x08\x12\x17\n\x0fhighCardinality\x18\x1b \x01(\x08\x12!\n\x19highCorrWithOtherFeatures\x18\x1c \x01(\x08\x12\x19\n\x11lowCorrWithTarget\x18\x1d \x01(\x08\x12\x16\n\x0ehighMissingPct\x18\x1e \x01(\x08\x12\x0e\n\x06skewed\x18\x1f \x01(\x08\x12\n\n\x02id\x18  \x01(\x08\x12\x10\n\x08\x63onstant\x18! \x01(\x08\x12\x11\n\tduplicate\x18\" \x01(\x08\x12\x10\n\x08reserved\x18# \x01(\x08\x12\x14\n\x0c\x63ompleteness\x18% \x01(\x01\x12\x1a\n\x12\x64istinctValueCount\x18& \x01(\x01\x12\x1b\n\x13mostFreqValuesRatio\x18\' \x01(\x01\x12Y\n\thistogram\x18) \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.HistogramData\x12\x14\n\x0c\x63orrToTarget\x18* \x01(\x01\x12\r\n\x05index\x18+ \x01(\x05\x12S\n\x08outliers\x18, \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.OutlierStat\"\x96\x01\n\rComponentSpec\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x0e\n\x06\x66ooter\x18\x03 \x01(\t\x12T\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ComponentView\"\xe3\x04\n\rComponentView\x12P\n\x06metric\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.MetricSpec\x12N\n\x05gauge\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GaugeSpec\x12V\n\thistogram\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.HistogramSpec\x12N\n\x05table\x18\x04 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.TableSpec\x12V\n\tlineChart\x18\x05 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LineChartSpec\x12T\n\x08\x62\x61rChart\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.BarChartSpec\x12Z\n\x0bscatterPlot\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ScatterPlotSpec\"P\n\x0b\x43orrelation\x12\x10\n\x08\x66\x65\x61ture1\x18\x01 \x01(\t\x12\x10\n\x08\x66\x65\x61ture2\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\x12\x0e\n\x06method\x18\x04 \x01(\t\">\n\x0f\x43orrelationSpec\x12\x0e\n\x06\x63utoff\x18\x01 \x01(\x01\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0b\n\x03top\x18\x03 \x01(\x05\"\xef\x01\n\x0b\x43svFileSpec\x12\x11\n\tdelimiter\x18\x01 \x01(\t\x12\r\n\x05quote\x18\x03 \x01(\t\x12\x12\n\nescapeChar\x18\x04 \x01(\t\x12\x14\n\x0c\x63ommentChars\x18\x05 \x01(\t\x12\x0e\n\x06header\x18\x06 \x01(\x08\x12\x10\n\x08skipRows\x18\x07 \x01(\x05\x12\x12\n\nnullValues\x18\x08 \x01(\t\x12\x10\n\x08\x65ncoding\x18\t \x01(\t\x12\x0f\n\x07maxRows\x18\n \x01(\x05\x12\x0e\n\x06strict\x18\x0b \x01(\x08\x12\x13\n\x0b\x63ompression\x18\x0c \x01(\t\x12\x16\n\x0ehasIndexColumn\x18\r \x01(\x08\"\xd2\x01\n\rDataInputSpec\x12\x0e\n\x06preSQL\x18\x01 \x03(\t\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12X\n\x06\x66ormat\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\"\x8c\x02\n\x0e\x44\x61taOutputSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\x12\x1d\n\x15\x63reateTableIfNotExist\x18\x05 \x01(\x08\x12\x17\n\x0fincludeFeatures\x18\x06 \x01(\x08\x12\x0b\n\x03xai\x18\x07 \x01(\x08\x12\x16\n\x0e\x64\x65tectOutliers\x18\x08 \x01(\x08\x12\x0f\n\x07postSQL\x18\t \x03(\t\"\x82\x02\n\x0c\x44\x61taPipeline\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineStatus\"\xa7\x01\n\x10\x44\x61taPipelineList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"\x8b\x02\n\x0f\x44\x61taPipelineRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunStatus\"\xa1\x01\n\x18\x44\x61taPipelineRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xad\x01\n\x13\x44\x61taPipelineRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRun\"\xc8\x02\n\x13\x44\x61taPipelineRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x18\n\x10\x64\x61tapipelineName\x18\x02 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0emodelClassName\x18\n \x01(\t\x12\x19\n\x11modelClassRunName\x18\x0b \x01(\t\"\x80\x04\n\x15\x44\x61taPipelineRunStatus\x12\x12\n\nrecipeRuns\x18\x01 \x03(\t\x12U\n\x06output\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\r\n\x05phase\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x06 \x01(\x03\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x10\n\x08progress\x18\t \x01(\x05\x12K\n\x04logs\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x0c \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x80\x06\n\x10\x44\x61taPipelineSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12t\n\x0f\x64\x61tasetSelector\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineSpec.DatasetSelectorEntry\x12U\n\x07recipes\x18\x05 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipePartSpec\x12T\n\x06output\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12_\n\x0cnotification\x18\x08 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\t \x01(\t\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x0b \x01(\t\x12\x0e\n\x06paused\x18\x0c \x01(\x08\x12\x0b\n\x03ttl\x18\r \x01(\x05\x1a\x36\n\x14\x44\x61tasetSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xba\x02\n\x12\x44\x61taPipelineStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\\\n\x08schedule\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x13\n\x0blastRunName\x18\x04 \x01(\t\x12\x11\n\trunsCount\x18\x05 \x01(\x05\x12\x43\n\nconditions\x18\x06 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xff\x01\n\x0b\x44\x61taProduct\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductStatus\"\xa5\x01\n\x0f\x44\x61taProductList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\"\xe8\x06\n\x0f\x44\x61taProductSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x0e\n\x06public\x18\x02 \x01(\x08\x12\x36\n\ttenantRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12V\n\x0bgitLocation\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GitLocation\x12\x17\n\x0f\x63\x61\x63heBucketName\x18\x06 \x01(\t\x12\x16\n\x0e\x64\x65\x66\x61ultLabName\x18\x07 \x01(\t\x12\x1e\n\x16\x64\x65\x66\x61ultServingSiteName\x18\x08 \x01(\t\x12\x19\n\x11\x64\x65\x66\x61ultBucketName\x18\t \x01(\t\x12\x0c\n\x04task\x18\n \x01(\t\x12\x0f\n\x07subtask\x18\x0b \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12_\n\x0cnotification\x18\r \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12`\n\x11trainingResources\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12_\n\x10servingResources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x10 \x01(\t\x12\r\n\x05\x63olor\x18\x11 \x01(\t\x12T\n\x08\x61pproval\x18\x12 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12]\n\x0bpermissions\x18\x13 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PermissionsSpec\x12\x0c\n\x04tags\x18\x14 \x03(\t\"\xa9\x04\n\x11\x44\x61taProductStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x18\n\x10\x64\x61tasourcesCount\x18\x03 \x01(\x05\x12\x15\n\rdatasetsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x64\x61taPipelineCount\x18\x05 \x01(\x05\x12\x1d\n\x15totalDataPipelineRuns\x18\x06 \x01(\x05\x12\x14\n\x0cstudiesCount\x18\x07 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x08 \x01(\x05\x12\x17\n\x0fpredictorsCount\x18\x0b \x01(\x05\x12\x15\n\rdataAppsCount\x18\r \x01(\x05\x12\x18\n\x10predictionsCount\x18\x0e \x01(\x05\x12\x17\n\x0finfoAlertsCount\x18\x0f \x01(\x05\x12\x18\n\x10\x65rrorAlertsCount\x18\x10 \x01(\x05\x12\x19\n\x11modelClassesCount\x18\x11 \x01(\x05\x12\x15\n\rfailureReason\x18\x12 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x13 \x01(\t\x12\x17\n\x0f\x62\x61selineVersion\x18\x14 \x01(\t\x12\x43\n\nconditions\x18\x15 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x94\x02\n\x12\x44\x61taProductVersion\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionSpec\x12^\n\x06status\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionStatus\"\xb3\x01\n\x16\x44\x61taProductVersionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\"\xa0\x01\n\x16\x44\x61taProductVersionSpec\x12\x37\n\nproductRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x17\n\x0fprevVersionName\x18\x03 \x01(\t\x12\x10\n\x08\x62\x61seline\x18\x04 \x01(\x08\x12\r\n\x05owner\x18\x05 \x01(\t\"\xe9\x01\n\x18\x44\x61taProductVersionStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xfc\x01\n\nDataSource\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceStatus\"\xa3\x01\n\x0e\x44\x61taSourceList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\"\x91\x06\n\x0e\x44\x61taSourceSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x61tasetType\x18\x04 \x01(\t\x12L\n\x06schema\x18\x05 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latfile\x18\x06 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x0f\n\x07labeled\x18\x07 \x01(\x08\x12P\n\x06sample\x18\t \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12\x0c\n\x04task\x18\n \x01(\t\x12\x0f\n\x07subtask\x18\x0b \x01(\t\x12]\n\rrelationships\x18\x0c \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RelationshipSpec\x12T\n\x08labeling\x18\r \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingSpec\x12[\n\x0cinferredFrom\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12]\n\x11unitTestsTemplate\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x14\n\x0cingestMethod\x18\x10 \x01(\t\"\xd2\x02\n\x10\x44\x61taSourceStatus\x12\x0c\n\x04\x63ols\x18\x01 \x01(\x05\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12H\n\x14lastDatasetCreatedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0flastDatasetName\x18\x04 \x01(\t\x12=\n\tupdatedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x06 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x43\n\nconditions\x18\x08 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf3\x01\n\x07\x44\x61taset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSpec\x12S\n\x06status\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetStatus\"\xe0\x01\n\x14\x44\x61tasetGroupByStatus\x12\x13\n\x0b\x64\x61tasetsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x12\n\nreportsURI\x18\x03 \x01(\t\x12\x14\n\x0cunitTestsURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66\x65\x61turesURI\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\x0b\x44\x61tasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12L\n\x05items\x18\x02 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x99\x0c\n\x0b\x44\x61tasetSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0e\x64\x61taSourceName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x08 \x01(\t\x12\x0c\n\x04role\x18\t \x01(\t\x12\x0c\n\x04tags\x18\n \x03(\t\x12\x0e\n\x06report\x18\x0b \x01(\x08\x12\x10\n\x08unitTest\x18\x0c \x01(\x08\x12U\n\x06origin\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12W\n\x08location\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12\x61rtifactBucketName\x18\x0f \x01(\t\x12X\n\tresources\x18\x10 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x11 \x01(\x03\x12\x0c\n\x04type\x18\x12 \x01(\t\x12P\n\x06sample\x18\x13 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12V\n\tsynthetic\x18\x14 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SyntheticSpec\x12\x0c\n\x04task\x18\x15 \x01(\t\x12\x0f\n\x07subtask\x18\x16 \x01(\t\x12Z\n\x0b\x63orrelation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.CorrelationSpec\x12\x0c\n\x04\x66\x61st\x18\x18 \x01(\x08\x12\x11\n\tfeaturize\x18\x19 \x01(\x08\x12\x33\n\x06labRef\x18\x1a \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\x11servingDatasetRef\x18\x1b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cpredictorRef\x18\x1c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12 \n\x18generateFeatureHistogram\x18\x1d \x01(\x08\x12U\n\tunitTests\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12R\n\x07groupBy\x18\x1f \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GroupBySpec\x12g\n\x0egroupLocations\x18  \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GroupDatasetLocationsSpec\x12\x0b\n\x03key\x18! \x03(\t\x12\x16\n\x0emodelClassName\x18\" \x01(\t\x12\x19\n\x11modelClassRunName\x18# \x01(\t\x12:\n\rfeatureGroups\x18$ \x03(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x18\n\x10\x66\x65\x61tureGroupName\x18% \x01(\t\x12_\n\x0cnotification\x18& \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\"\xd9\x02\n\x11\x44\x61tasetStatistics\x12W\n\x07\x63olumns\x18\x01 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnStatistics\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0c\n\x04\x63ols\x18\x04 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\x05 \x01(\x05\x12\x61\n\x16\x63orrelationsWithTarget\x18\x06 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18\x07 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\"\xbe\t\n\rDatasetStatus\x12[\n\nstatistics\x18\x01 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetStatistics\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x12\n\nreportName\x18\x03 \x01(\t\x12]\n\x0ereportLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fprofileLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12`\n\x11\x61nomaliesLocation\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x12\n\nimbalanced\x18\x07 \x01(\x08\x12\x1a\n\x12observedGeneration\x18\x08 \x01(\x03\x12\x61\n\x0funitTestResults\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12?\n\x0blastStudyAt\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\r \x01(\t\x12\x10\n\x08progress\x18\x0e \x01(\x05\x12\x0c\n\x04hash\x18\x0f \x01(\t\x12K\n\x04logs\x18\x10 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x12 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12O\n\x06images\x18\x13 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12?\n\x0b\x63ompletedAt\x18\x15 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12@\n\x13\x66\x65\x61tureHistogramRef\x18\x16 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12[\n\x07groupby\x18\x17 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetGroupByStatus\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xa6\x01\n\x0f\x44\x61tasetTemplate\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSpec\"/\n\x0e\x44riftThreshold\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"\xf0\x01\n\x06\x45ntity\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntitySpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntityStatus\"\x9b\x01\n\nEntityList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\"\x87\x01\n\nEntitySpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07joinKey\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x0c\n\x04tags\x18\x06 \x03(\t\"\xae\x01\n\x0c\x45ntityStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x03 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xc1\x01\n\x11\x45xcelNotebookSpec\x12\x1a\n\x12\x66irstSheetWithData\x18\x01 \x01(\x08\x12\x11\n\tsheetName\x18\x02 \x01(\t\x12\x12\n\nsheetIndex\x18\x03 \x01(\x05\x12\x15\n\rcolumnNameRow\x18\x04 \x01(\x05\x12R\n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ExcelSheetArea\"k\n\x0e\x45xcelSheetArea\x12\x13\n\x0b\x65ntireSheet\x18\x01 \x01(\x08\x12\x12\n\nfromColumn\x18\x02 \x01(\x05\x12\x10\n\x08toColumn\x18\x03 \x01(\x05\x12\x0f\n\x07\x66romRow\x18\x04 \x01(\x05\x12\r\n\x05toRow\x18\x05 \x01(\x05\"\x82\x02\n\x0c\x46\x65\x61tureGroup\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroupSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroupStatus\"\xa7\x01\n\x10\x46\x65\x61tureGroupList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\"\x84\x08\n\x10\x46\x65\x61tureGroupSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\r\n\x05owner\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x04 \x01(\t\x12\x12\n\ningestType\x18\x05 \x01(\t\x12\x12\n\nentityName\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x03(\t\x12\\\n\x0eingestSchedule\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12Z\n\x0csyncSchedule\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12Z\n\x08\x66latfile\x18\n \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12L\n\x06schema\x18\x0b \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Q\n\x05tests\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12W\n\x08location\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x12\n\ntimeColumn\x18\x0e \x01(\t\x12\x18\n\x10timeColumnFormat\x18\x0f \x01(\t\x12\x11\n\tkeyColumn\x18\x10 \x01(\t\x12\x62\n\x0fmaterialization\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.MaterializationSpec\x12X\n\tresources\x18\x12 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x33\n\x06labRef\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\x85\x05\n\x12\x46\x65\x61tureGroupStatus\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12=\n\tupdatedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x62\n\x0eingestSchedule\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12`\n\x0csyncSchedule\x18\x08 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12Z\n\x0bonlineTable\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x46\n\x12onlineTableCreated\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x19\n\x11ingestDatasetName\x18\x0b \x01(\t\x12\x15\n\rfailureReason\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\r \x01(\t\x12\x43\n\nconditions\x18\x0e \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x8e\x02\n\x10\x46\x65\x61tureHistogram\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramSpec\x12\\\n\x06status\x18\x03 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramStatus\"\xaf\x01\n\x14\x46\x65\x61tureHistogramList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\"\xf5\x04\n\x14\x46\x65\x61tureHistogramSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x05 \x03(\t\x12\x36\n\tsourceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08training\x18\x07 \x01(\x08\x12\x0c\n\x04live\x18\t \x01(\x08\x12\x39\n\x05start\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x37\n\x03\x65nd\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x34\n\x07\x62\x61seRef\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12]\n\x0f\x64riftThresholds\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12\x17\n\x0fsyncIntervalSec\x18\x0e \x01(\x05\x12U\n\tunitTests\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x14\n\x0cgenUnitTests\x18\x10 \x01(\x08\x12\x15\n\rfeatureFilter\x18\x11 \x01(\t\x12\x15\n\rreferenceType\x18\x12 \x01(\t\"\x9d\x04\n\x16\x46\x65\x61tureHistogramStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12V\n\x07\x63olumns\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnHistogram\x12=\n\tupdatedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05total\x18\n \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x0b \x01(\x05\x12\x43\n\nconditions\x18\x0c \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xa6\x02\n\x12\x46latFileFormatSpec\x12\x10\n\x08\x66ileType\x18\x01 \x01(\t\x12N\n\x03\x63sv\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.CsvFileSpec\x12V\n\x05\x65xcel\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ExcelNotebookSpec\x12V\n\x07parquet\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ParquetFileSpec\"M\n\tGaugeSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0b\n\x03row\x18\x03 \x01(\x05\x12\x0e\n\x06scalar\x18\x04 \x01(\t\"V\n\x0bGitLocation\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x0f\n\x07private\x18\x04 \x01(\x08\"]\n\x0bGroupBySpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07groupby\x18\x02 \x03(\t\x12\x0c\n\x04\x66req\x18\x03 \x01(\t\x12\x10\n\x08interval\x18\x04 \x01(\x05\x12\x0c\n\x04\x61ggr\x18\x05 \x01(\t\"\xc2\x01\n\x19GroupDatasetLocationsSpec\x12\x12\n\ngroupsRoot\x18\x01 \x01(\t\x12\x11\n\tgroupRoot\x18\x02 \x01(\t\x12\x17\n\x0fgroupDataFolder\x18\x03 \x01(\t\x12\x15\n\rgroupDataFile\x18\x04 \x01(\t\x12\x1a\n\x12groupProfileFolder\x18\x05 \x01(\t\x12\x17\n\x0fgroupReportFile\x18\x06 \x01(\t\x12\x19\n\x11groupFeaturesFile\x18\x07 \x01(\t\"=\n\rHistogramSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\x0c\n\x04\x62ins\x18\x03 \x01(\x05\"=\n\rImageLocation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\x16registryConnectionName\x18\x02 \x01(\t\"\"\n\x03KPI\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"?\n\x0cLabelingRule\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x10\n\x08operator\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xe1\x01\n\x0cLabelingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x14\n\x0cresultColumn\x18\x02 \x01(\t\x12T\n\x08positive\x18\x03 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingRule\x12T\n\x08negative\x18\x04 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingRule\"J\n\rLineChartSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\x12\x0e\n\x06legend\x18\x04 \x01(\x08\"\x86\x02\n\x13MaterializationSpec\x12\x0e\n\x06online\x18\x01 \x01(\x08\x12\x0f\n\x07offline\x18\x02 \x01(\x08\x12=\n\tstartDate\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x12\n\nofflineTTL\x18\x04 \x01(\x05\x12\x11\n\tonlineTTL\x18\x05 \x01(\x05\x12\x10\n\x08\x62\x61\x63kfill\x18\x06 \x01(\x05\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"N\n\nMetricSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0b\n\x03row\x18\x03 \x01(\x05\x12\x0e\n\x06scalar\x18\x04 \x01(\t\"<\n\x0bOutlierStat\x12\r\n\x05lower\x18\x01 \x01(\x05\x12\r\n\x05upper\x18\x02 \x01(\x05\x12\x0f\n\x07percent\x18\x03 \x01(\x02\"W\n\x08PageSpec\x12K\n\x04rows\x18\x01 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RowSpec\"!\n\x0fParquetFileSpec\x12\x0e\n\x06\x65ngine\x18\x01 \x01(\t\"\xf0\x01\n\x06Recipe\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeSpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStatus\"\x8f\x01\n\x0fRecipeInputSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\"\x9b\x01\n\nRecipeList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x97\x01\n\x10RecipeOutputSpec\x12\x15\n\rcreateDataset\x18\x01 \x01(\x08\x12\x13\n\x0b\x64\x61tasetName\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"8\n\x0eRecipePartSpec\x12\x12\n\nrecipeName\x18\x01 \x01(\t\x12\x12\n\ndependents\x18\x02 \x03(\t\"\xf9\x01\n\tRecipeRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRunSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRunStatus\"\xa1\x01\n\rRecipeRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\"\xe0\x02\n\rRecipeRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x12\n\nrecipeName\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03ttl\x18\x06 \x01(\x05\x12\x16\n\x0emodelClassName\x18\x07 \x01(\t\x12\x19\n\x11modelClassRunName\x18\x08 \x01(\t\"\x92\x03\n\x0fRecipeRunStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12\x15\n\rfailureReason\x18\x04 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x05 \x01(\t\x12\x13\n\x0btriggeredBy\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x0b \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xed\x04\n\nRecipeSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12T\n\x05input\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeInputSpec\x12O\n\x05steps\x18\x05 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStep\x12V\n\x06output\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeOutputSpec\x12P\n\x06sample\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\n \x01(\x03\x12\x0b\n\x03ttl\x18\x0b \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\x87\x02\n\x0cRecipeStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12W\n\x07lastRun\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12=\n\tupdatedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"s\n\nRecipeStep\x12\n\n\x02op\x18\x01 \x01(\t\x12Y\n\nparameters\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStepParam\".\n\x0fRecipeStepParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"X\n\x14RecommendationSchema\x12\x14\n\x0cuserIDColumn\x18\x01 \x01(\t\x12\x14\n\x0citemIDColumn\x18\x02 \x01(\t\x12\x14\n\x0cratingColumn\x18\x03 \x01(\t\"R\n\x10RelationshipSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\r\n\x05\x61rity\x18\x03 \x01(\t\x12\x11\n\trelatesTo\x18\x04 \x01(\t\"Y\n\x07RowSpec\x12N\n\x04\x63ols\x18\x01 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnSpec\"j\n\nSampleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0f\n\x07percent\x18\x04 \x01(\x05\x12\x0e\n\x06\x66ilter\x18\x05 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\"<\n\x0fScatterPlotSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\"\xb0\x02\n\x06Schema\x12`\n\x10timeSeriesSchema\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.TimeSeriesSchema\x12h\n\x14recommendationSchema\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecommendationSchema\x12M\n\x07\x63olumns\x18\x03 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Column\x12\x0b\n\x03key\x18\x04 \x03(\t\".\n\rSyntheticSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04rows\x18\x02 \x01(\x05\"\x84\x01\n\tTableSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\x12\x0f\n\x07\x66ilters\x18\x03 \x03(\t\x12\x0f\n\x07groupby\x18\x04 \x03(\t\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x11\n\tshowIndex\x18\x06 \x01(\x08\x12\x0e\n\x06\x62order\x18\x07 \x01(\x08\"@\n\x10TimeSeriesSchema\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x66req\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\x05\x42\x36Z4github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nDgithub.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x12\x34github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x87\x01\n\x14\x41pprovalReviewStatus\x12\x10\n\x08reviewer\x18\x01 \x01(\t\x12\x0e\n\x06result\x18\x02 \x01(\t\x12>\n\napprovedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05notes\x18\x04 \x01(\t\"F\n\x0c\x41pprovalSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x14\n\x0c\x64\x65\x63isionType\x18\x02 \x01(\t\x12\x0f\n\x07members\x18\x03 \x03(\t\"}\n\x0e\x41pprovalStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12[\n\x07reviews\x18\x02 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalReviewStatus\"W\n\x0c\x42\x61rChartSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\x12\x0e\n\x06legend\x18\x04 \x01(\x08\x12\x0c\n\x04sort\x18\x05 \x01(\x08\"\xa0\x07\n\x06\x43olumn\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x02 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x0e\n\x06ignore\x18\x06 \x01(\x08\x12\x0e\n\x06target\x18\x07 \x01(\x08\x12\x10\n\x08nullable\x18\x08 \x01(\x08\x12\n\n\x02pk\x18\t \x01(\x08\x12\n\n\x02\x66k\x18\n \x01(\x08\x12\x12\n\nmultipleOf\x18\x0b \x01(\x05\x12\x0f\n\x07maximum\x18\x0c \x01(\x01\x12\x18\n\x10\x65xclusiveMaximum\x18\r \x01(\x08\x12\x0f\n\x07minimum\x18\x0e \x01(\x01\x12\x18\n\x10\x65xclusiveMinimum\x18\x0f \x01(\x08\x12\x11\n\tmaxLength\x18\x10 \x01(\x05\x12\x11\n\tminLength\x18\x11 \x01(\x05\x12\x0f\n\x07pattern\x18\x12 \x01(\t\x12\x10\n\x08required\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xample\x18\x14 \x01(\t\x12\x14\n\x0c\x65xternalDocs\x18\x15 \x01(\t\x12\x0c\n\x04\x65num\x18\x16 \x03(\t\x12\x10\n\x08maxItems\x18\x18 \x01(\x05\x12\x10\n\x08minItems\x18\x19 \x01(\x05\x12\x13\n\x0buniqueItems\x18\x1a \x01(\x08\x12\x0b\n\x03pii\x18\x1c \x01(\x08\x12\x0b\n\x03phi\x18\x1d \x01(\x08\x12\x11\n\tprotected\x18\x1f \x01(\x08\x12\x17\n\x0f\x64\x65\x66\x61ultValueNum\x18  \x01(\x01\x12\x0b\n\x03log\x18! \x01(\x08\x12\n\n\x02mu\x18\" \x01(\x01\x12\r\n\x05sigma\x18# \x01(\x01\x12\x15\n\rskewThreshold\x18$ \x01(\x01\x12\x16\n\x0e\x64riftThreshold\x18% \x01(\x01\x12\x0b\n\x03key\x18& \x01(\x08\x12\x0c\n\x04\x66old\x18\' \x01(\x08\x12\x0e\n\x06weight\x18( \x01(\x08\x12\x10\n\x08reserved\x18) \x01(\x08\x12\x12\n\nimputation\x18* \x01(\t\x12\x0f\n\x07scaling\x18+ \x01(\t\x12\x11\n\tgenerated\x18, \x01(\x08\x12\x0f\n\x07\x66ormula\x18- \x01(\t\x12\n\n\x02id\x18. \x01(\x08\x12\x0c\n\x04step\x18/ \x01(\x01\x12\x0b\n\x03loc\x18\x30 \x01(\x05\x12\x16\n\x0e\x64\x61tetimeFormat\x18\x31 \x01(\t\x12\x12\n\ntimeseries\x18\x32 \x01(\x08\x12\x11\n\tregressor\x18\x33 \x01(\x08\x12\x17\n\x0flaggedRegressor\x18\x34 \x01(\x08\x12\x11\n\ttimeIndex\x18\x35 \x01(\x08\x12\x0c\n\x04\x61ggr\x18\x36 \x01(\t\x12\x0e\n\x06window\x18\x37 \x01(\x05\"\xe0\x01\n\x0f\x43olumnHistogram\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Y\n\thistogram\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.HistogramData\x12U\n\x07metrics\x18\x03 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05\x64rift\x18\x04 \x01(\x08\"\x81\x01\n\nColumnSpec\x12\x0e\n\x06spacer\x18\x01 \x01(\x08\x12\r\n\x05width\x18\x02 \x01(\x05\x12T\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ComponentSpec\"\x92\x07\n\x10\x43olumnStatistics\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x01\x12\x10\n\x08\x64istinct\x18\x04 \x01(\x05\x12\x0f\n\x07missing\x18\x05 \x01(\x05\x12\x16\n\x0epercentMissing\x18\x06 \x01(\x01\x12\x0c\n\x04mean\x18\x07 \x01(\x01\x12\x0e\n\x06stddev\x18\x08 \x01(\x01\x12\x10\n\x08variance\x18\t \x01(\x01\x12\x0b\n\x03min\x18\n \x01(\x01\x12\x0b\n\x03max\x18\x0b \x01(\x01\x12\x10\n\x08kurtosis\x18\x0c \x01(\x01\x12\x10\n\x08skewness\x18\r \x01(\x01\x12\x0b\n\x03sum\x18\x0e \x01(\x01\x12\x0b\n\x03mad\x18\x0f \x01(\x01\x12\x0b\n\x03p25\x18\x10 \x01(\x01\x12\x0b\n\x03p50\x18\x11 \x01(\x01\x12\x0b\n\x03p75\x18\x12 \x01(\x01\x12\x0b\n\x03iqr\x18\x13 \x01(\x01\x12\x0c\n\x04mode\x18\x14 \x01(\t\x12\r\n\x05zeros\x18\x15 \x01(\x01\x12\x0f\n\x07invalid\x18\x16 \x01(\x05\x12\x12\n\nimportance\x18\x17 \x01(\x01\x12\x0e\n\x06target\x18\x18 \x01(\x08\x12\x0e\n\x06ignore\x18\x19 \x01(\x08\x12\x10\n\x08nullable\x18\x1a \x01(\x08\x12\x17\n\x0fhighCardinality\x18\x1b \x01(\x08\x12!\n\x19highCorrWithOtherFeatures\x18\x1c \x01(\x08\x12\x19\n\x11lowCorrWithTarget\x18\x1d \x01(\x08\x12\x16\n\x0ehighMissingPct\x18\x1e \x01(\x08\x12\x0e\n\x06skewed\x18\x1f \x01(\x08\x12\n\n\x02id\x18  \x01(\x08\x12\x10\n\x08\x63onstant\x18! \x01(\x08\x12\x11\n\tduplicate\x18\" \x01(\x08\x12\x10\n\x08reserved\x18# \x01(\x08\x12\x14\n\x0c\x63ompleteness\x18% \x01(\x01\x12\x1a\n\x12\x64istinctValueCount\x18& \x01(\x01\x12\x1b\n\x13mostFreqValuesRatio\x18\' \x01(\x01\x12Y\n\thistogram\x18) \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.HistogramData\x12\x14\n\x0c\x63orrToTarget\x18* \x01(\x01\x12\r\n\x05index\x18+ \x01(\x05\x12S\n\x08outliers\x18, \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.OutlierStat\"\x96\x01\n\rComponentSpec\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x0e\n\x06\x66ooter\x18\x03 \x01(\t\x12T\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ComponentView\"\xe3\x04\n\rComponentView\x12P\n\x06metric\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.MetricSpec\x12N\n\x05gauge\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GaugeSpec\x12V\n\thistogram\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.HistogramSpec\x12N\n\x05table\x18\x04 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.TableSpec\x12V\n\tlineChart\x18\x05 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LineChartSpec\x12T\n\x08\x62\x61rChart\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.BarChartSpec\x12Z\n\x0bscatterPlot\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ScatterPlotSpec\"P\n\x0b\x43orrelation\x12\x10\n\x08\x66\x65\x61ture1\x18\x01 \x01(\t\x12\x10\n\x08\x66\x65\x61ture2\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\x12\x0e\n\x06method\x18\x04 \x01(\t\">\n\x0f\x43orrelationSpec\x12\x0e\n\x06\x63utoff\x18\x01 \x01(\x01\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0b\n\x03top\x18\x03 \x01(\x05\"\xef\x01\n\x0b\x43svFileSpec\x12\x11\n\tdelimiter\x18\x01 \x01(\t\x12\r\n\x05quote\x18\x03 \x01(\t\x12\x12\n\nescapeChar\x18\x04 \x01(\t\x12\x14\n\x0c\x63ommentChars\x18\x05 \x01(\t\x12\x0e\n\x06header\x18\x06 \x01(\x08\x12\x10\n\x08skipRows\x18\x07 \x01(\x05\x12\x12\n\nnullValues\x18\x08 \x01(\t\x12\x10\n\x08\x65ncoding\x18\t \x01(\t\x12\x0f\n\x07maxRows\x18\n \x01(\x05\x12\x0e\n\x06strict\x18\x0b \x01(\x08\x12\x13\n\x0b\x63ompression\x18\x0c \x01(\t\x12\x16\n\x0ehasIndexColumn\x18\r \x01(\x08\"\xc2\x01\n\rDataInputSpec\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12X\n\x06\x66ormat\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\"\x89\x02\n\x0e\x44\x61taOutputSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\x12\x1d\n\x15\x63reateTableIfNotExist\x18\x05 \x01(\x08\x12\x17\n\x0fincludeFeatures\x18\x06 \x01(\x08\x12\x19\n\x11includeShapValues\x18\x07 \x01(\x08\x12\x16\n\x0e\x64\x65tectOutliers\x18\x08 \x01(\x08\"\x82\x02\n\x0c\x44\x61taPipeline\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineStatus\"\xa7\x01\n\x10\x44\x61taPipelineList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"\x8b\x02\n\x0f\x44\x61taPipelineRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunStatus\"\xa1\x01\n\x18\x44\x61taPipelineRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xad\x01\n\x13\x44\x61taPipelineRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRun\"\xc8\x02\n\x13\x44\x61taPipelineRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x18\n\x10\x64\x61tapipelineName\x18\x02 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0emodelClassName\x18\n \x01(\t\x12\x19\n\x11modelClassRunName\x18\x0b \x01(\t\"\x80\x04\n\x15\x44\x61taPipelineRunStatus\x12\x12\n\nrecipeRuns\x18\x01 \x03(\t\x12U\n\x06output\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\r\n\x05phase\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x06 \x01(\x03\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x10\n\x08progress\x18\t \x01(\x05\x12K\n\x04logs\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x0c \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x80\x06\n\x10\x44\x61taPipelineSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12t\n\x0f\x64\x61tasetSelector\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineSpec.DatasetSelectorEntry\x12U\n\x07recipes\x18\x05 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipePartSpec\x12T\n\x06output\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12_\n\x0cnotification\x18\x08 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\t \x01(\t\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x0b \x01(\t\x12\x0e\n\x06paused\x18\x0c \x01(\x08\x12\x0b\n\x03ttl\x18\r \x01(\x05\x1a\x36\n\x14\x44\x61tasetSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xba\x02\n\x12\x44\x61taPipelineStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\\\n\x08schedule\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x13\n\x0blastRunName\x18\x04 \x01(\t\x12\x11\n\trunsCount\x18\x05 \x01(\x05\x12\x43\n\nconditions\x18\x06 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xff\x01\n\x0b\x44\x61taProduct\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductStatus\"\xa5\x01\n\x0f\x44\x61taProductList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\"\xe8\x06\n\x0f\x44\x61taProductSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x0e\n\x06public\x18\x02 \x01(\x08\x12\x36\n\ttenantRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12V\n\x0bgitLocation\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GitLocation\x12\x17\n\x0f\x63\x61\x63heBucketName\x18\x06 \x01(\t\x12\x16\n\x0e\x64\x65\x66\x61ultLabName\x18\x07 \x01(\t\x12\x1e\n\x16\x64\x65\x66\x61ultServingSiteName\x18\x08 \x01(\t\x12\x19\n\x11\x64\x65\x66\x61ultBucketName\x18\t \x01(\t\x12\x0c\n\x04task\x18\n \x01(\t\x12\x0f\n\x07subtask\x18\x0b \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12_\n\x0cnotification\x18\r \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12`\n\x11trainingResources\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12_\n\x10servingResources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x10 \x01(\t\x12\r\n\x05\x63olor\x18\x11 \x01(\t\x12T\n\x08\x61pproval\x18\x12 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12]\n\x0bpermissions\x18\x13 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PermissionsSpec\x12\x0c\n\x04tags\x18\x14 \x03(\t\"\xa9\x04\n\x11\x44\x61taProductStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x18\n\x10\x64\x61tasourcesCount\x18\x03 \x01(\x05\x12\x15\n\rdatasetsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x64\x61taPipelineCount\x18\x05 \x01(\x05\x12\x1d\n\x15totalDataPipelineRuns\x18\x06 \x01(\x05\x12\x14\n\x0cstudiesCount\x18\x07 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x08 \x01(\x05\x12\x17\n\x0fpredictorsCount\x18\x0b \x01(\x05\x12\x15\n\rdataAppsCount\x18\r \x01(\x05\x12\x18\n\x10predictionsCount\x18\x0e \x01(\x05\x12\x17\n\x0finfoAlertsCount\x18\x0f \x01(\x05\x12\x18\n\x10\x65rrorAlertsCount\x18\x10 \x01(\x05\x12\x19\n\x11modelClassesCount\x18\x11 \x01(\x05\x12\x15\n\rfailureReason\x18\x12 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x13 \x01(\t\x12\x17\n\x0f\x62\x61selineVersion\x18\x14 \x01(\t\x12\x43\n\nconditions\x18\x15 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x94\x02\n\x12\x44\x61taProductVersion\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionSpec\x12^\n\x06status\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionStatus\"\xb3\x01\n\x16\x44\x61taProductVersionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\"\xa0\x01\n\x16\x44\x61taProductVersionSpec\x12\x37\n\nproductRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x17\n\x0fprevVersionName\x18\x03 \x01(\t\x12\x10\n\x08\x62\x61seline\x18\x04 \x01(\x08\x12\r\n\x05owner\x18\x05 \x01(\t\"\xe9\x01\n\x18\x44\x61taProductVersionStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xfc\x01\n\nDataSource\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceStatus\"\xa3\x01\n\x0e\x44\x61taSourceList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\"\x91\x06\n\x0e\x44\x61taSourceSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x61tasetType\x18\x04 \x01(\t\x12L\n\x06schema\x18\x05 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latfile\x18\x06 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x0f\n\x07labeled\x18\x07 \x01(\x08\x12P\n\x06sample\x18\t \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12\x0c\n\x04task\x18\n \x01(\t\x12\x0f\n\x07subtask\x18\x0b \x01(\t\x12]\n\rrelationships\x18\x0c \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RelationshipSpec\x12T\n\x08labeling\x18\r \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingSpec\x12[\n\x0cinferredFrom\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12]\n\x11unitTestsTemplate\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x14\n\x0cingestMethod\x18\x10 \x01(\t\"\xd2\x02\n\x10\x44\x61taSourceStatus\x12\x0c\n\x04\x63ols\x18\x01 \x01(\x05\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12H\n\x14lastDatasetCreatedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0flastDatasetName\x18\x04 \x01(\t\x12=\n\tupdatedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x06 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x43\n\nconditions\x18\x08 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf3\x01\n\x07\x44\x61taset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSpec\x12S\n\x06status\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetStatus\"\xe0\x01\n\x14\x44\x61tasetGroupByStatus\x12\x13\n\x0b\x64\x61tasetsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x12\n\nreportsURI\x18\x03 \x01(\t\x12\x14\n\x0cunitTestsURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66\x65\x61turesURI\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\x0b\x44\x61tasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12L\n\x05items\x18\x02 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x99\x0c\n\x0b\x44\x61tasetSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0e\x64\x61taSourceName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x08 \x01(\t\x12\x0c\n\x04role\x18\t \x01(\t\x12\x0c\n\x04tags\x18\n \x03(\t\x12\x0e\n\x06report\x18\x0b \x01(\x08\x12\x10\n\x08unitTest\x18\x0c \x01(\x08\x12U\n\x06origin\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12W\n\x08location\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12\x61rtifactBucketName\x18\x0f \x01(\t\x12X\n\tresources\x18\x10 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x11 \x01(\x03\x12\x0c\n\x04type\x18\x12 \x01(\t\x12P\n\x06sample\x18\x13 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12V\n\tsynthetic\x18\x14 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SyntheticSpec\x12\x0c\n\x04task\x18\x15 \x01(\t\x12\x0f\n\x07subtask\x18\x16 \x01(\t\x12Z\n\x0b\x63orrelation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.CorrelationSpec\x12\x0c\n\x04\x66\x61st\x18\x18 \x01(\x08\x12\x11\n\tfeaturize\x18\x19 \x01(\x08\x12\x33\n\x06labRef\x18\x1a \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\x11servingDatasetRef\x18\x1b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cpredictorRef\x18\x1c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12 \n\x18generateFeatureHistogram\x18\x1d \x01(\x08\x12U\n\tunitTests\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12R\n\x07groupBy\x18\x1f \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GroupBySpec\x12g\n\x0egroupLocations\x18  \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GroupDatasetLocationsSpec\x12\x0b\n\x03key\x18! \x03(\t\x12\x16\n\x0emodelClassName\x18\" \x01(\t\x12\x19\n\x11modelClassRunName\x18# \x01(\t\x12:\n\rfeatureGroups\x18$ \x03(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x18\n\x10\x66\x65\x61tureGroupName\x18% \x01(\t\x12_\n\x0cnotification\x18& \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\"\xd9\x02\n\x11\x44\x61tasetStatistics\x12W\n\x07\x63olumns\x18\x01 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnStatistics\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0c\n\x04\x63ols\x18\x04 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\x05 \x01(\x05\x12\x61\n\x16\x63orrelationsWithTarget\x18\x06 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18\x07 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\"\xbe\t\n\rDatasetStatus\x12[\n\nstatistics\x18\x01 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetStatistics\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x12\n\nreportName\x18\x03 \x01(\t\x12]\n\x0ereportLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fprofileLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12`\n\x11\x61nomaliesLocation\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x12\n\nimbalanced\x18\x07 \x01(\x08\x12\x1a\n\x12observedGeneration\x18\x08 \x01(\x03\x12\x61\n\x0funitTestResults\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12?\n\x0blastStudyAt\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\r \x01(\t\x12\x10\n\x08progress\x18\x0e \x01(\x05\x12\x0c\n\x04hash\x18\x0f \x01(\t\x12K\n\x04logs\x18\x10 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x12 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12O\n\x06images\x18\x13 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12?\n\x0b\x63ompletedAt\x18\x15 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12@\n\x13\x66\x65\x61tureHistogramRef\x18\x16 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12[\n\x07groupby\x18\x17 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetGroupByStatus\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xa6\x01\n\x0f\x44\x61tasetTemplate\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSpec\"/\n\x0e\x44riftThreshold\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"\xf0\x01\n\x06\x45ntity\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntitySpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntityStatus\"\x9b\x01\n\nEntityList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\"\x87\x01\n\nEntitySpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07joinKey\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x0c\n\x04tags\x18\x06 \x03(\t\"\xae\x01\n\x0c\x45ntityStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x03 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xc1\x01\n\x11\x45xcelNotebookSpec\x12\x1a\n\x12\x66irstSheetWithData\x18\x01 \x01(\x08\x12\x11\n\tsheetName\x18\x02 \x01(\t\x12\x12\n\nsheetIndex\x18\x03 \x01(\x05\x12\x15\n\rcolumnNameRow\x18\x04 \x01(\x05\x12R\n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ExcelSheetArea\"k\n\x0e\x45xcelSheetArea\x12\x13\n\x0b\x65ntireSheet\x18\x01 \x01(\x08\x12\x12\n\nfromColumn\x18\x02 \x01(\x05\x12\x10\n\x08toColumn\x18\x03 \x01(\x05\x12\x0f\n\x07\x66romRow\x18\x04 \x01(\x05\x12\r\n\x05toRow\x18\x05 \x01(\x05\"\x82\x02\n\x0c\x46\x65\x61tureGroup\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroupSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroupStatus\"\xa7\x01\n\x10\x46\x65\x61tureGroupList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\"\x84\x08\n\x10\x46\x65\x61tureGroupSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\r\n\x05owner\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x04 \x01(\t\x12\x12\n\ningestType\x18\x05 \x01(\t\x12\x12\n\nentityName\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x03(\t\x12\\\n\x0eingestSchedule\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12Z\n\x0csyncSchedule\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12Z\n\x08\x66latfile\x18\n \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12L\n\x06schema\x18\x0b \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Q\n\x05tests\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12W\n\x08location\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x12\n\ntimeColumn\x18\x0e \x01(\t\x12\x18\n\x10timeColumnFormat\x18\x0f \x01(\t\x12\x11\n\tkeyColumn\x18\x10 \x01(\t\x12\x62\n\x0fmaterialization\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.MaterializationSpec\x12X\n\tresources\x18\x12 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x33\n\x06labRef\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\x85\x05\n\x12\x46\x65\x61tureGroupStatus\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12=\n\tupdatedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x62\n\x0eingestSchedule\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12`\n\x0csyncSchedule\x18\x08 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12Z\n\x0bonlineTable\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x46\n\x12onlineTableCreated\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x19\n\x11ingestDatasetName\x18\x0b \x01(\t\x12\x15\n\rfailureReason\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\r \x01(\t\x12\x43\n\nconditions\x18\x0e \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x8e\x02\n\x10\x46\x65\x61tureHistogram\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramSpec\x12\\\n\x06status\x18\x03 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramStatus\"\xaf\x01\n\x14\x46\x65\x61tureHistogramList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\"\xf5\x04\n\x14\x46\x65\x61tureHistogramSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x05 \x03(\t\x12\x36\n\tsourceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08training\x18\x07 \x01(\x08\x12\x0c\n\x04live\x18\t \x01(\x08\x12\x39\n\x05start\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x37\n\x03\x65nd\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x34\n\x07\x62\x61seRef\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12]\n\x0f\x64riftThresholds\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12\x17\n\x0fsyncIntervalSec\x18\x0e \x01(\x05\x12U\n\tunitTests\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x14\n\x0cgenUnitTests\x18\x10 \x01(\x08\x12\x15\n\rfeatureFilter\x18\x11 \x01(\t\x12\x15\n\rreferenceType\x18\x12 \x01(\t\"\x9d\x04\n\x16\x46\x65\x61tureHistogramStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12V\n\x07\x63olumns\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnHistogram\x12=\n\tupdatedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05total\x18\n \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x0b \x01(\x05\x12\x43\n\nconditions\x18\x0c \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xa6\x02\n\x12\x46latFileFormatSpec\x12\x10\n\x08\x66ileType\x18\x01 \x01(\t\x12N\n\x03\x63sv\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.CsvFileSpec\x12V\n\x05\x65xcel\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ExcelNotebookSpec\x12V\n\x07parquet\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ParquetFileSpec\"M\n\tGaugeSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0b\n\x03row\x18\x03 \x01(\x05\x12\x0e\n\x06scalar\x18\x04 \x01(\t\"V\n\x0bGitLocation\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x0f\n\x07private\x18\x04 \x01(\x08\"]\n\x0bGroupBySpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07groupby\x18\x02 \x03(\t\x12\x0c\n\x04\x66req\x18\x03 \x01(\t\x12\x10\n\x08interval\x18\x04 \x01(\x05\x12\x0c\n\x04\x61ggr\x18\x05 \x01(\t\"\xc2\x01\n\x19GroupDatasetLocationsSpec\x12\x12\n\ngroupsRoot\x18\x01 \x01(\t\x12\x11\n\tgroupRoot\x18\x02 \x01(\t\x12\x17\n\x0fgroupDataFolder\x18\x03 \x01(\t\x12\x15\n\rgroupDataFile\x18\x04 \x01(\t\x12\x1a\n\x12groupProfileFolder\x18\x05 \x01(\t\x12\x17\n\x0fgroupReportFile\x18\x06 \x01(\t\x12\x19\n\x11groupFeaturesFile\x18\x07 \x01(\t\"=\n\rHistogramSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\x0c\n\x04\x62ins\x18\x03 \x01(\x05\"=\n\rImageLocation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\x16registryConnectionName\x18\x02 \x01(\t\"\"\n\x03KPI\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"?\n\x0cLabelingRule\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x10\n\x08operator\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xe1\x01\n\x0cLabelingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x14\n\x0cresultColumn\x18\x02 \x01(\t\x12T\n\x08positive\x18\x03 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingRule\x12T\n\x08negative\x18\x04 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingRule\"J\n\rLineChartSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\x12\x0e\n\x06legend\x18\x04 \x01(\x08\"\x86\x02\n\x13MaterializationSpec\x12\x0e\n\x06online\x18\x01 \x01(\x08\x12\x0f\n\x07offline\x18\x02 \x01(\x08\x12=\n\tstartDate\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x12\n\nofflineTTL\x18\x04 \x01(\x05\x12\x11\n\tonlineTTL\x18\x05 \x01(\x05\x12\x10\n\x08\x62\x61\x63kfill\x18\x06 \x01(\x05\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"N\n\nMetricSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0b\n\x03row\x18\x03 \x01(\x05\x12\x0e\n\x06scalar\x18\x04 \x01(\t\"<\n\x0bOutlierStat\x12\r\n\x05lower\x18\x01 \x01(\x05\x12\r\n\x05upper\x18\x02 \x01(\x05\x12\x0f\n\x07percent\x18\x03 \x01(\x02\"W\n\x08PageSpec\x12K\n\x04rows\x18\x01 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RowSpec\"!\n\x0fParquetFileSpec\x12\x0e\n\x06\x65ngine\x18\x01 \x01(\t\"\xf0\x01\n\x06Recipe\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeSpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStatus\"\x8f\x01\n\x0fRecipeInputSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\"\x9b\x01\n\nRecipeList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x97\x01\n\x10RecipeOutputSpec\x12\x15\n\rcreateDataset\x18\x01 \x01(\x08\x12\x13\n\x0b\x64\x61tasetName\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"8\n\x0eRecipePartSpec\x12\x12\n\nrecipeName\x18\x01 \x01(\t\x12\x12\n\ndependents\x18\x02 \x03(\t\"\xf9\x01\n\tRecipeRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRunSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRunStatus\"\xa1\x01\n\rRecipeRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\"\xe0\x02\n\rRecipeRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x12\n\nrecipeName\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03ttl\x18\x06 \x01(\x05\x12\x16\n\x0emodelClassName\x18\x07 \x01(\t\x12\x19\n\x11modelClassRunName\x18\x08 \x01(\t\"\x92\x03\n\x0fRecipeRunStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12\x15\n\rfailureReason\x18\x04 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x05 \x01(\t\x12\x13\n\x0btriggeredBy\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x0b \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xed\x04\n\nRecipeSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12T\n\x05input\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeInputSpec\x12O\n\x05steps\x18\x05 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStep\x12V\n\x06output\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeOutputSpec\x12P\n\x06sample\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\n \x01(\x03\x12\x0b\n\x03ttl\x18\x0b \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\x87\x02\n\x0cRecipeStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12W\n\x07lastRun\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12=\n\tupdatedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"s\n\nRecipeStep\x12\n\n\x02op\x18\x01 \x01(\t\x12Y\n\nparameters\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStepParam\".\n\x0fRecipeStepParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"X\n\x14RecommendationSchema\x12\x14\n\x0cuserIDColumn\x18\x01 \x01(\t\x12\x14\n\x0citemIDColumn\x18\x02 \x01(\t\x12\x14\n\x0cratingColumn\x18\x03 \x01(\t\"R\n\x10RelationshipSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\r\n\x05\x61rity\x18\x03 \x01(\t\x12\x11\n\trelatesTo\x18\x04 \x01(\t\"Y\n\x07RowSpec\x12N\n\x04\x63ols\x18\x01 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnSpec\"j\n\nSampleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0f\n\x07percent\x18\x04 \x01(\x05\x12\x0e\n\x06\x66ilter\x18\x05 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\"<\n\x0fScatterPlotSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\"\xb0\x02\n\x06Schema\x12`\n\x10timeSeriesSchema\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.TimeSeriesSchema\x12h\n\x14recommendationSchema\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecommendationSchema\x12M\n\x07\x63olumns\x18\x03 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Column\x12\x0b\n\x03key\x18\x04 \x03(\t\".\n\rSyntheticSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04rows\x18\x02 \x01(\x05\"\x84\x01\n\tTableSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\x12\x0f\n\x07\x66ilters\x18\x03 \x03(\t\x12\x0f\n\x07groupby\x18\x04 \x03(\t\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x11\n\tshowIndex\x18\x06 \x01(\x08\x12\x0e\n\x06\x62order\x18\x07 \x01(\x08\"@\n\x10TimeSeriesSchema\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x66req\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\x05\x42\x36Z4github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z4github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1'
@@ -51,175 +51,175 @@
   _CORRELATION._serialized_start=3794
   _CORRELATION._serialized_end=3874
   _CORRELATIONSPEC._serialized_start=3876
   _CORRELATIONSPEC._serialized_end=3938
   _CSVFILESPEC._serialized_start=3941
   _CSVFILESPEC._serialized_end=4180
   _DATAINPUTSPEC._serialized_start=4183
-  _DATAINPUTSPEC._serialized_end=4393
-  _DATAOUTPUTSPEC._serialized_start=4396
-  _DATAOUTPUTSPEC._serialized_end=4664
-  _DATAPIPELINE._serialized_start=4667
-  _DATAPIPELINE._serialized_end=4925
-  _DATAPIPELINELIST._serialized_start=4928
-  _DATAPIPELINELIST._serialized_end=5095
-  _DATAPIPELINERUN._serialized_start=5098
-  _DATAPIPELINERUN._serialized_end=5365
-  _DATAPIPELINERUNCONDITION._serialized_start=5368
-  _DATAPIPELINERUNCONDITION._serialized_end=5529
-  _DATAPIPELINERUNLIST._serialized_start=5532
-  _DATAPIPELINERUNLIST._serialized_end=5705
-  _DATAPIPELINERUNSPEC._serialized_start=5708
-  _DATAPIPELINERUNSPEC._serialized_end=6036
-  _DATAPIPELINERUNSTATUS._serialized_start=6039
-  _DATAPIPELINERUNSTATUS._serialized_end=6551
-  _DATAPIPELINESPEC._serialized_start=6554
-  _DATAPIPELINESPEC._serialized_end=7322
-  _DATAPIPELINESPEC_DATASETSELECTORENTRY._serialized_start=7268
-  _DATAPIPELINESPEC_DATASETSELECTORENTRY._serialized_end=7322
-  _DATAPIPELINESTATUS._serialized_start=7325
-  _DATAPIPELINESTATUS._serialized_end=7639
-  _DATAPRODUCT._serialized_start=7642
-  _DATAPRODUCT._serialized_end=7897
-  _DATAPRODUCTLIST._serialized_start=7900
-  _DATAPRODUCTLIST._serialized_end=8065
-  _DATAPRODUCTSPEC._serialized_start=8068
-  _DATAPRODUCTSPEC._serialized_end=8940
-  _DATAPRODUCTSTATUS._serialized_start=8943
-  _DATAPRODUCTSTATUS._serialized_end=9496
-  _DATAPRODUCTVERSION._serialized_start=9499
-  _DATAPRODUCTVERSION._serialized_end=9775
-  _DATAPRODUCTVERSIONLIST._serialized_start=9778
-  _DATAPRODUCTVERSIONLIST._serialized_end=9957
-  _DATAPRODUCTVERSIONSPEC._serialized_start=9960
-  _DATAPRODUCTVERSIONSPEC._serialized_end=10120
-  _DATAPRODUCTVERSIONSTATUS._serialized_start=10123
-  _DATAPRODUCTVERSIONSTATUS._serialized_end=10356
-  _DATASOURCE._serialized_start=10359
-  _DATASOURCE._serialized_end=10611
-  _DATASOURCELIST._serialized_start=10614
-  _DATASOURCELIST._serialized_end=10777
-  _DATASOURCESPEC._serialized_start=10780
-  _DATASOURCESPEC._serialized_end=11565
-  _DATASOURCESTATUS._serialized_start=11568
-  _DATASOURCESTATUS._serialized_end=11906
-  _DATASET._serialized_start=11909
-  _DATASET._serialized_end=12152
-  _DATASETGROUPBYSTATUS._serialized_start=12155
-  _DATASETGROUPBYSTATUS._serialized_end=12379
-  _DATASETLIST._serialized_start=12382
-  _DATASETLIST._serialized_end=12539
-  _DATASETSPEC._serialized_start=12542
-  _DATASETSPEC._serialized_end=14103
-  _DATASETSTATISTICS._serialized_start=14106
-  _DATASETSTATISTICS._serialized_end=14451
-  _DATASETSTATUS._serialized_start=14454
-  _DATASETSTATUS._serialized_end=15668
-  _DATASETTEMPLATE._serialized_start=15671
-  _DATASETTEMPLATE._serialized_end=15837
-  _DRIFTTHRESHOLD._serialized_start=15839
-  _DRIFTTHRESHOLD._serialized_end=15886
-  _ENTITY._serialized_start=15889
-  _ENTITY._serialized_end=16129
-  _ENTITYLIST._serialized_start=16132
-  _ENTITYLIST._serialized_end=16287
-  _ENTITYSPEC._serialized_start=16290
-  _ENTITYSPEC._serialized_end=16425
-  _ENTITYSTATUS._serialized_start=16428
-  _ENTITYSTATUS._serialized_end=16602
-  _EXCELNOTEBOOKSPEC._serialized_start=16605
-  _EXCELNOTEBOOKSPEC._serialized_end=16798
-  _EXCELSHEETAREA._serialized_start=16800
-  _EXCELSHEETAREA._serialized_end=16907
-  _FEATUREGROUP._serialized_start=16910
-  _FEATUREGROUP._serialized_end=17168
-  _FEATUREGROUPLIST._serialized_start=17171
-  _FEATUREGROUPLIST._serialized_end=17338
-  _FEATUREGROUPSPEC._serialized_start=17341
-  _FEATUREGROUPSPEC._serialized_end=18369
-  _FEATUREGROUPSTATUS._serialized_start=18372
-  _FEATUREGROUPSTATUS._serialized_end=19017
-  _FEATUREHISTOGRAM._serialized_start=19020
-  _FEATUREHISTOGRAM._serialized_end=19290
-  _FEATUREHISTOGRAMLIST._serialized_start=19293
-  _FEATUREHISTOGRAMLIST._serialized_end=19468
-  _FEATUREHISTOGRAMSPEC._serialized_start=19471
-  _FEATUREHISTOGRAMSPEC._serialized_end=20100
-  _FEATUREHISTOGRAMSTATUS._serialized_start=20103
-  _FEATUREHISTOGRAMSTATUS._serialized_end=20644
-  _FLATFILEFORMATSPEC._serialized_start=20647
-  _FLATFILEFORMATSPEC._serialized_end=20941
-  _GAUGESPEC._serialized_start=20943
-  _GAUGESPEC._serialized_end=21020
-  _GITLOCATION._serialized_start=21022
-  _GITLOCATION._serialized_end=21108
-  _GROUPBYSPEC._serialized_start=21110
-  _GROUPBYSPEC._serialized_end=21203
-  _GROUPDATASETLOCATIONSSPEC._serialized_start=21206
-  _GROUPDATASETLOCATIONSSPEC._serialized_end=21400
-  _HISTOGRAMSPEC._serialized_start=21402
-  _HISTOGRAMSPEC._serialized_end=21463
-  _IMAGELOCATION._serialized_start=21465
-  _IMAGELOCATION._serialized_end=21526
-  _KPI._serialized_start=21528
-  _KPI._serialized_end=21562
-  _LABELINGRULE._serialized_start=21564
-  _LABELINGRULE._serialized_end=21627
-  _LABELINGSPEC._serialized_start=21630
-  _LABELINGSPEC._serialized_end=21855
-  _LINECHARTSPEC._serialized_start=21857
-  _LINECHARTSPEC._serialized_end=21931
-  _MATERIALIZATIONSPEC._serialized_start=21934
-  _MATERIALIZATIONSPEC._serialized_end=22196
-  _METRICSPEC._serialized_start=22198
-  _METRICSPEC._serialized_end=22276
-  _OUTLIERSTAT._serialized_start=22278
-  _OUTLIERSTAT._serialized_end=22338
-  _PAGESPEC._serialized_start=22340
-  _PAGESPEC._serialized_end=22427
-  _PARQUETFILESPEC._serialized_start=22429
-  _PARQUETFILESPEC._serialized_end=22462
-  _RECIPE._serialized_start=22465
-  _RECIPE._serialized_end=22705
-  _RECIPEINPUTSPEC._serialized_start=22708
-  _RECIPEINPUTSPEC._serialized_end=22851
-  _RECIPELIST._serialized_start=22854
-  _RECIPELIST._serialized_end=23009
-  _RECIPEOUTPUTSPEC._serialized_start=23012
-  _RECIPEOUTPUTSPEC._serialized_end=23163
-  _RECIPEPARTSPEC._serialized_start=23165
-  _RECIPEPARTSPEC._serialized_end=23221
-  _RECIPERUN._serialized_start=23224
-  _RECIPERUN._serialized_end=23473
-  _RECIPERUNLIST._serialized_start=23476
-  _RECIPERUNLIST._serialized_end=23637
-  _RECIPERUNSPEC._serialized_start=23640
-  _RECIPERUNSPEC._serialized_end=23992
-  _RECIPERUNSTATUS._serialized_start=23995
-  _RECIPERUNSTATUS._serialized_end=24397
-  _RECIPESPEC._serialized_start=24400
-  _RECIPESPEC._serialized_end=25021
-  _RECIPESTATUS._serialized_start=25024
-  _RECIPESTATUS._serialized_end=25287
-  _RECIPESTEP._serialized_start=25289
-  _RECIPESTEP._serialized_end=25404
-  _RECIPESTEPPARAM._serialized_start=25406
-  _RECIPESTEPPARAM._serialized_end=25452
-  _RECOMMENDATIONSCHEMA._serialized_start=25454
-  _RECOMMENDATIONSCHEMA._serialized_end=25542
-  _RELATIONSHIPSPEC._serialized_start=25544
-  _RELATIONSHIPSPEC._serialized_end=25626
-  _ROWSPEC._serialized_start=25628
-  _ROWSPEC._serialized_end=25717
-  _SAMPLESPEC._serialized_start=25719
-  _SAMPLESPEC._serialized_end=25825
-  _SCATTERPLOTSPEC._serialized_start=25827
-  _SCATTERPLOTSPEC._serialized_end=25887
-  _SCHEMA._serialized_start=25890
-  _SCHEMA._serialized_end=26194
-  _SYNTHETICSPEC._serialized_start=26196
-  _SYNTHETICSPEC._serialized_end=26242
-  _TABLESPEC._serialized_start=26245
-  _TABLESPEC._serialized_end=26377
-  _TIMESERIESSCHEMA._serialized_start=26379
-  _TIMESERIESSCHEMA._serialized_end=26443
+  _DATAINPUTSPEC._serialized_end=4377
+  _DATAOUTPUTSPEC._serialized_start=4380
+  _DATAOUTPUTSPEC._serialized_end=4645
+  _DATAPIPELINE._serialized_start=4648
+  _DATAPIPELINE._serialized_end=4906
+  _DATAPIPELINELIST._serialized_start=4909
+  _DATAPIPELINELIST._serialized_end=5076
+  _DATAPIPELINERUN._serialized_start=5079
+  _DATAPIPELINERUN._serialized_end=5346
+  _DATAPIPELINERUNCONDITION._serialized_start=5349
+  _DATAPIPELINERUNCONDITION._serialized_end=5510
+  _DATAPIPELINERUNLIST._serialized_start=5513
+  _DATAPIPELINERUNLIST._serialized_end=5686
+  _DATAPIPELINERUNSPEC._serialized_start=5689
+  _DATAPIPELINERUNSPEC._serialized_end=6017
+  _DATAPIPELINERUNSTATUS._serialized_start=6020
+  _DATAPIPELINERUNSTATUS._serialized_end=6532
+  _DATAPIPELINESPEC._serialized_start=6535
+  _DATAPIPELINESPEC._serialized_end=7303
+  _DATAPIPELINESPEC_DATASETSELECTORENTRY._serialized_start=7249
+  _DATAPIPELINESPEC_DATASETSELECTORENTRY._serialized_end=7303
+  _DATAPIPELINESTATUS._serialized_start=7306
+  _DATAPIPELINESTATUS._serialized_end=7620
+  _DATAPRODUCT._serialized_start=7623
+  _DATAPRODUCT._serialized_end=7878
+  _DATAPRODUCTLIST._serialized_start=7881
+  _DATAPRODUCTLIST._serialized_end=8046
+  _DATAPRODUCTSPEC._serialized_start=8049
+  _DATAPRODUCTSPEC._serialized_end=8921
+  _DATAPRODUCTSTATUS._serialized_start=8924
+  _DATAPRODUCTSTATUS._serialized_end=9477
+  _DATAPRODUCTVERSION._serialized_start=9480
+  _DATAPRODUCTVERSION._serialized_end=9756
+  _DATAPRODUCTVERSIONLIST._serialized_start=9759
+  _DATAPRODUCTVERSIONLIST._serialized_end=9938
+  _DATAPRODUCTVERSIONSPEC._serialized_start=9941
+  _DATAPRODUCTVERSIONSPEC._serialized_end=10101
+  _DATAPRODUCTVERSIONSTATUS._serialized_start=10104
+  _DATAPRODUCTVERSIONSTATUS._serialized_end=10337
+  _DATASOURCE._serialized_start=10340
+  _DATASOURCE._serialized_end=10592
+  _DATASOURCELIST._serialized_start=10595
+  _DATASOURCELIST._serialized_end=10758
+  _DATASOURCESPEC._serialized_start=10761
+  _DATASOURCESPEC._serialized_end=11546
+  _DATASOURCESTATUS._serialized_start=11549
+  _DATASOURCESTATUS._serialized_end=11887
+  _DATASET._serialized_start=11890
+  _DATASET._serialized_end=12133
+  _DATASETGROUPBYSTATUS._serialized_start=12136
+  _DATASETGROUPBYSTATUS._serialized_end=12360
+  _DATASETLIST._serialized_start=12363
+  _DATASETLIST._serialized_end=12520
+  _DATASETSPEC._serialized_start=12523
+  _DATASETSPEC._serialized_end=14084
+  _DATASETSTATISTICS._serialized_start=14087
+  _DATASETSTATISTICS._serialized_end=14432
+  _DATASETSTATUS._serialized_start=14435
+  _DATASETSTATUS._serialized_end=15649
+  _DATASETTEMPLATE._serialized_start=15652
+  _DATASETTEMPLATE._serialized_end=15818
+  _DRIFTTHRESHOLD._serialized_start=15820
+  _DRIFTTHRESHOLD._serialized_end=15867
+  _ENTITY._serialized_start=15870
+  _ENTITY._serialized_end=16110
+  _ENTITYLIST._serialized_start=16113
+  _ENTITYLIST._serialized_end=16268
+  _ENTITYSPEC._serialized_start=16271
+  _ENTITYSPEC._serialized_end=16406
+  _ENTITYSTATUS._serialized_start=16409
+  _ENTITYSTATUS._serialized_end=16583
+  _EXCELNOTEBOOKSPEC._serialized_start=16586
+  _EXCELNOTEBOOKSPEC._serialized_end=16779
+  _EXCELSHEETAREA._serialized_start=16781
+  _EXCELSHEETAREA._serialized_end=16888
+  _FEATUREGROUP._serialized_start=16891
+  _FEATUREGROUP._serialized_end=17149
+  _FEATUREGROUPLIST._serialized_start=17152
+  _FEATUREGROUPLIST._serialized_end=17319
+  _FEATUREGROUPSPEC._serialized_start=17322
+  _FEATUREGROUPSPEC._serialized_end=18350
+  _FEATUREGROUPSTATUS._serialized_start=18353
+  _FEATUREGROUPSTATUS._serialized_end=18998
+  _FEATUREHISTOGRAM._serialized_start=19001
+  _FEATUREHISTOGRAM._serialized_end=19271
+  _FEATUREHISTOGRAMLIST._serialized_start=19274
+  _FEATUREHISTOGRAMLIST._serialized_end=19449
+  _FEATUREHISTOGRAMSPEC._serialized_start=19452
+  _FEATUREHISTOGRAMSPEC._serialized_end=20081
+  _FEATUREHISTOGRAMSTATUS._serialized_start=20084
+  _FEATUREHISTOGRAMSTATUS._serialized_end=20625
+  _FLATFILEFORMATSPEC._serialized_start=20628
+  _FLATFILEFORMATSPEC._serialized_end=20922
+  _GAUGESPEC._serialized_start=20924
+  _GAUGESPEC._serialized_end=21001
+  _GITLOCATION._serialized_start=21003
+  _GITLOCATION._serialized_end=21089
+  _GROUPBYSPEC._serialized_start=21091
+  _GROUPBYSPEC._serialized_end=21184
+  _GROUPDATASETLOCATIONSSPEC._serialized_start=21187
+  _GROUPDATASETLOCATIONSSPEC._serialized_end=21381
+  _HISTOGRAMSPEC._serialized_start=21383
+  _HISTOGRAMSPEC._serialized_end=21444
+  _IMAGELOCATION._serialized_start=21446
+  _IMAGELOCATION._serialized_end=21507
+  _KPI._serialized_start=21509
+  _KPI._serialized_end=21543
+  _LABELINGRULE._serialized_start=21545
+  _LABELINGRULE._serialized_end=21608
+  _LABELINGSPEC._serialized_start=21611
+  _LABELINGSPEC._serialized_end=21836
+  _LINECHARTSPEC._serialized_start=21838
+  _LINECHARTSPEC._serialized_end=21912
+  _MATERIALIZATIONSPEC._serialized_start=21915
+  _MATERIALIZATIONSPEC._serialized_end=22177
+  _METRICSPEC._serialized_start=22179
+  _METRICSPEC._serialized_end=22257
+  _OUTLIERSTAT._serialized_start=22259
+  _OUTLIERSTAT._serialized_end=22319
+  _PAGESPEC._serialized_start=22321
+  _PAGESPEC._serialized_end=22408
+  _PARQUETFILESPEC._serialized_start=22410
+  _PARQUETFILESPEC._serialized_end=22443
+  _RECIPE._serialized_start=22446
+  _RECIPE._serialized_end=22686
+  _RECIPEINPUTSPEC._serialized_start=22689
+  _RECIPEINPUTSPEC._serialized_end=22832
+  _RECIPELIST._serialized_start=22835
+  _RECIPELIST._serialized_end=22990
+  _RECIPEOUTPUTSPEC._serialized_start=22993
+  _RECIPEOUTPUTSPEC._serialized_end=23144
+  _RECIPEPARTSPEC._serialized_start=23146
+  _RECIPEPARTSPEC._serialized_end=23202
+  _RECIPERUN._serialized_start=23205
+  _RECIPERUN._serialized_end=23454
+  _RECIPERUNLIST._serialized_start=23457
+  _RECIPERUNLIST._serialized_end=23618
+  _RECIPERUNSPEC._serialized_start=23621
+  _RECIPERUNSPEC._serialized_end=23973
+  _RECIPERUNSTATUS._serialized_start=23976
+  _RECIPERUNSTATUS._serialized_end=24378
+  _RECIPESPEC._serialized_start=24381
+  _RECIPESPEC._serialized_end=25002
+  _RECIPESTATUS._serialized_start=25005
+  _RECIPESTATUS._serialized_end=25268
+  _RECIPESTEP._serialized_start=25270
+  _RECIPESTEP._serialized_end=25385
+  _RECIPESTEPPARAM._serialized_start=25387
+  _RECIPESTEPPARAM._serialized_end=25433
+  _RECOMMENDATIONSCHEMA._serialized_start=25435
+  _RECOMMENDATIONSCHEMA._serialized_end=25523
+  _RELATIONSHIPSPEC._serialized_start=25525
+  _RELATIONSHIPSPEC._serialized_end=25607
+  _ROWSPEC._serialized_start=25609
+  _ROWSPEC._serialized_end=25698
+  _SAMPLESPEC._serialized_start=25700
+  _SAMPLESPEC._serialized_end=25806
+  _SCATTERPLOTSPEC._serialized_start=25808
+  _SCATTERPLOTSPEC._serialized_end=25868
+  _SCHEMA._serialized_start=25871
+  _SCHEMA._serialized_end=26175
+  _SYNTHETICSPEC._serialized_start=26177
+  _SYNTHETICSPEC._serialized_end=26223
+  _TABLESPEC._serialized_start=26226
+  _TABLESPEC._serialized_end=26358
+  _TIMESERIESSCHEMA._serialized_start=26360
+  _TIMESERIESSCHEMA._serialized_end=26424
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: github.com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord.proto
+# source: github.com/metaprov/modelaapi/services/notifier/v1/notifier.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
+from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_infra_dot_v1alpha1_dot_generated__pb2
-from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_data_dot_v1alpha1_dot_generated__pb2
-from github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_training_dot_v1alpha1_dot_generated__pb2
-from github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_inference_dot_v1alpha1_dot_generated__pb2
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from github.com.metaprov.modelaapi.services.common.v1 import common_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_common_dot_v1_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nOgithub.com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord.proto\x12\x39github.com.metaprov.modelaapi.services.batchpredictord.v1\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1aIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x1a\x1bgoogle/protobuf/empty.proto\"\x9e\x06\n\x13\x42\x61tchPredictRequest\x12Y\n\nprediction\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12X\n\nfromBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12Y\n\x0e\x66romConnection\x18\x03 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12r\n\nfromSecret\x18\x04 \x03(\x0b\x32^.github.com.metaprov.modelaapi.services.batchpredictord.v1.BatchPredictRequest.FromSecretEntry\x12V\n\x08toBucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12W\n\x0ctoConnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12n\n\x08toSecret\x18\x07 \x03(\x0b\x32\\.github.com.metaprov.modelaapi.services.batchpredictord.v1.BatchPredictRequest.ToSecretEntry\x1a\x31\n\x0f\x46romSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rToSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xe0\t\n\x1d\x42\x61tchPredictModelClassRequest\x12Y\n\nprediction\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05model\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12X\n\nmodelClass\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x08\x65ntities\x18\x05 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\x06 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12X\n\nfromBucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12Y\n\x0e\x66romConnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12|\n\nfromSecret\x18\t \x03(\x0b\x32h.github.com.metaprov.modelaapi.services.batchpredictord.v1.BatchPredictModelClassRequest.FromSecretEntry\x12V\n\x08toBucket\x18\n \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12W\n\x0ctoConnection\x18\x0b \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12x\n\x08toSecret\x18\x0c \x03(\x0b\x32\x66.github.com.metaprov.modelaapi.services.batchpredictord.v1.BatchPredictModelClassRequest.ToSecretEntry\x1a\x31\n\x0f\x46romSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rToSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"1\n\x14\x42\x61tchPredictResponse\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04rows\x18\x02 \x01(\x05\"\x11\n\x0fShutdownRequest\"\x12\n\x10ShutdownResponse2\xab\x04\n\x05\x42\x61tch\x12\xb1\x01\n\x0c\x42\x61tchPredict\x12N.github.com.metaprov.modelaapi.services.batchpredictord.v1.BatchPredictRequest\x1aO.github.com.metaprov.modelaapi.services.batchpredictord.v1.BatchPredictResponse\"\x00\x12\xc5\x01\n\x16\x42\x61tchPredictModelClass\x12X.github.com.metaprov.modelaapi.services.batchpredictord.v1.BatchPredictModelClassRequest\x1aO.github.com.metaprov.modelaapi.services.batchpredictord.v1.BatchPredictResponse\"\x00\x12\xa5\x01\n\x08Shutdown\x12J.github.com.metaprov.modelaapi.services.batchpredictord.v1.ShutdownRequest\x1aK.github.com.metaprov.modelaapi.services.batchpredictord.v1.ShutdownResponse\"\x00\x42;Z9github.com/metaprov/modelaapi/services/batchpredictord/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nAgithub.com/metaprov/modelaapi/services/notifier/v1/notifier.proto\x12\x32github.com.metaprov.modelaapi.services.notifier.v1\x1a google/protobuf/field_mask.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\"\xf7\x01\n\x14ListNotifiersRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x64\n\x06labels\x18\x02 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.notifier.v1.ListNotifiersRequest.LabelsEntry\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x10\n\x08order_by\x18\x05 \x01(\t\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x01\n\x15ListNotifiersResponse\x12V\n\tnotifiers\x18\x01 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotifierList\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x12\n\x10NotifierResponse\"j\n\x15\x43reateNotifierRequest\x12Q\n\x08notifier\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Notifier\"\x18\n\x16\x43reateNotifierResponse\"\x9a\x01\n\x15UpdateNotifierRequest\x12Q\n\x08notifier\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Notifier\x12.\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"\x18\n\x16UpdateNotifierResponse\"5\n\x12GetNotifierRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"v\n\x13GetNotifierResponse\x12Q\n\x08notifier\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Notifier\x12\x0c\n\x04yaml\x18\x02 \x01(\t\"8\n\x15\x44\x65leteNotifierRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x18\n\x16\x44\x65leteNotifierResponse2\xb9\x08\n\x0fNotifierService\x12\xc7\x01\n\rListNotifiers\x12H.github.com.metaprov.modelaapi.services.notifier.v1.ListNotifiersRequest\x1aI.github.com.metaprov.modelaapi.services.notifier.v1.ListNotifiersResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/v1/notifiers/{namespace}\x12\xc1\x01\n\x0e\x43reateNotifier\x12I.github.com.metaprov.modelaapi.services.notifier.v1.CreateNotifierRequest\x1aJ.github.com.metaprov.modelaapi.services.notifier.v1.CreateNotifierResponse\"\x18\x82\xd3\xe4\x93\x02\x12\"\r/v1/notifiers:\x01*\x12\xc8\x01\n\x0bGetNotifier\x12\x46.github.com.metaprov.modelaapi.services.notifier.v1.GetNotifierRequest\x1aG.github.com.metaprov.modelaapi.services.notifier.v1.GetNotifierResponse\"(\x82\xd3\xe4\x93\x02\"\x12 /v1/notifiers/{namespace}/{name}\x12\xf8\x01\n\x0eUpdateNotifier\x12I.github.com.metaprov.modelaapi.services.notifier.v1.UpdateNotifierRequest\x1aJ.github.com.metaprov.modelaapi.services.notifier.v1.UpdateNotifierResponse\"O\x82\xd3\xe4\x93\x02I\x1a\x44/v1/notifiers/{notifier.metadata.namespace}/{notifier.metadata.name}:\x01*\x12\xd1\x01\n\x0e\x44\x65leteNotifier\x12I.github.com.metaprov.modelaapi.services.notifier.v1.DeleteNotifierRequest\x1aJ.github.com.metaprov.modelaapi.services.notifier.v1.DeleteNotifierResponse\"(\x82\xd3\xe4\x93\x02\"* /v1/notifiers/{namespace}/{name}B4Z2github.com/metaprov/modelaapi/services/notifier/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.batchpredictord.v1.batchpredictord_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.notifier.v1.notifier_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z9github.com/metaprov/modelaapi/services/batchpredictord/v1'
-  _BATCHPREDICTREQUEST_FROMSECRETENTRY._options = None
-  _BATCHPREDICTREQUEST_FROMSECRETENTRY._serialized_options = b'8\001'
-  _BATCHPREDICTREQUEST_TOSECRETENTRY._options = None
-  _BATCHPREDICTREQUEST_TOSECRETENTRY._serialized_options = b'8\001'
-  _BATCHPREDICTMODELCLASSREQUEST_FROMSECRETENTRY._options = None
-  _BATCHPREDICTMODELCLASSREQUEST_FROMSECRETENTRY._serialized_options = b'8\001'
-  _BATCHPREDICTMODELCLASSREQUEST_TOSECRETENTRY._options = None
-  _BATCHPREDICTMODELCLASSREQUEST_TOSECRETENTRY._serialized_options = b'8\001'
-  _BATCHPREDICTREQUEST._serialized_start=462
-  _BATCHPREDICTREQUEST._serialized_end=1260
-  _BATCHPREDICTREQUEST_FROMSECRETENTRY._serialized_start=1162
-  _BATCHPREDICTREQUEST_FROMSECRETENTRY._serialized_end=1211
-  _BATCHPREDICTREQUEST_TOSECRETENTRY._serialized_start=1213
-  _BATCHPREDICTREQUEST_TOSECRETENTRY._serialized_end=1260
-  _BATCHPREDICTMODELCLASSREQUEST._serialized_start=1263
-  _BATCHPREDICTMODELCLASSREQUEST._serialized_end=2511
-  _BATCHPREDICTMODELCLASSREQUEST_FROMSECRETENTRY._serialized_start=1162
-  _BATCHPREDICTMODELCLASSREQUEST_FROMSECRETENTRY._serialized_end=1211
-  _BATCHPREDICTMODELCLASSREQUEST_TOSECRETENTRY._serialized_start=1213
-  _BATCHPREDICTMODELCLASSREQUEST_TOSECRETENTRY._serialized_end=1260
-  _BATCHPREDICTRESPONSE._serialized_start=2513
-  _BATCHPREDICTRESPONSE._serialized_end=2562
-  _SHUTDOWNREQUEST._serialized_start=2564
-  _SHUTDOWNREQUEST._serialized_end=2581
-  _SHUTDOWNRESPONSE._serialized_start=2583
-  _SHUTDOWNRESPONSE._serialized_end=2601
-  _BATCH._serialized_start=2604
-  _BATCH._serialized_end=3159
+  DESCRIPTOR._serialized_options = b'Z2github.com/metaprov/modelaapi/services/notifier/v1'
+  _LISTNOTIFIERSREQUEST_LABELSENTRY._options = None
+  _LISTNOTIFIERSREQUEST_LABELSENTRY._serialized_options = b'8\001'
+  _NOTIFIERSERVICE.methods_by_name['ListNotifiers']._options = None
+  _NOTIFIERSERVICE.methods_by_name['ListNotifiers']._serialized_options = b'\202\323\344\223\002\033\022\031/v1/notifiers/{namespace}'
+  _NOTIFIERSERVICE.methods_by_name['CreateNotifier']._options = None
+  _NOTIFIERSERVICE.methods_by_name['CreateNotifier']._serialized_options = b'\202\323\344\223\002\022\"\r/v1/notifiers:\001*'
+  _NOTIFIERSERVICE.methods_by_name['GetNotifier']._options = None
+  _NOTIFIERSERVICE.methods_by_name['GetNotifier']._serialized_options = b'\202\323\344\223\002\"\022 /v1/notifiers/{namespace}/{name}'
+  _NOTIFIERSERVICE.methods_by_name['UpdateNotifier']._options = None
+  _NOTIFIERSERVICE.methods_by_name['UpdateNotifier']._serialized_options = b'\202\323\344\223\002I\032D/v1/notifiers/{notifier.metadata.namespace}/{notifier.metadata.name}:\001*'
+  _NOTIFIERSERVICE.methods_by_name['DeleteNotifier']._options = None
+  _NOTIFIERSERVICE.methods_by_name['DeleteNotifier']._serialized_options = b'\202\323\344\223\002\"* /v1/notifiers/{namespace}/{name}'
+  _LISTNOTIFIERSREQUEST._serialized_start=320
+  _LISTNOTIFIERSREQUEST._serialized_end=567
+  _LISTNOTIFIERSREQUEST_LABELSENTRY._serialized_start=522
+  _LISTNOTIFIERSREQUEST_LABELSENTRY._serialized_end=567
+  _LISTNOTIFIERSRESPONSE._serialized_start=570
+  _LISTNOTIFIERSRESPONSE._serialized_end=706
+  _NOTIFIERRESPONSE._serialized_start=708
+  _NOTIFIERRESPONSE._serialized_end=726
+  _CREATENOTIFIERREQUEST._serialized_start=728
+  _CREATENOTIFIERREQUEST._serialized_end=834
+  _CREATENOTIFIERRESPONSE._serialized_start=836
+  _CREATENOTIFIERRESPONSE._serialized_end=860
+  _UPDATENOTIFIERREQUEST._serialized_start=863
+  _UPDATENOTIFIERREQUEST._serialized_end=1017
+  _UPDATENOTIFIERRESPONSE._serialized_start=1019
+  _UPDATENOTIFIERRESPONSE._serialized_end=1043
+  _GETNOTIFIERREQUEST._serialized_start=1045
+  _GETNOTIFIERREQUEST._serialized_end=1098
+  _GETNOTIFIERRESPONSE._serialized_start=1100
+  _GETNOTIFIERRESPONSE._serialized_end=1218
+  _DELETENOTIFIERREQUEST._serialized_start=1220
+  _DELETENOTIFIERREQUEST._serialized_end=1276
+  _DELETENOTIFIERRESPONSE._serialized_start=1278
+  _DELETENOTIFIERRESPONSE._serialized_end=1302
+  _NOTIFIERSERVICE._serialized_start=1305
+  _NOTIFIERSERVICE._serialized_end=2386
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: github.com/metaprov/modelaapi/services/notifier/v1/notifier.proto
+# source: github.com/metaprov/modelaapi/services/todo/v1/todo.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_infra_dot_v1alpha1_dot_generated__pb2
+from github.com.metaprov.modelaapi.pkg.apis.team.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_team_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.services.common.v1 import common_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_common_dot_v1_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nAgithub.com/metaprov/modelaapi/services/notifier/v1/notifier.proto\x12\x32github.com.metaprov.modelaapi.services.notifier.v1\x1a google/protobuf/field_mask.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\"\xf7\x01\n\x14ListNotifiersRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x64\n\x06labels\x18\x02 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.notifier.v1.ListNotifiersRequest.LabelsEntry\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x10\n\x08order_by\x18\x05 \x01(\t\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x01\n\x15ListNotifiersResponse\x12V\n\tnotifiers\x18\x01 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotifierList\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x12\n\x10NotifierResponse\"j\n\x15\x43reateNotifierRequest\x12Q\n\x08notifier\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Notifier\"\x18\n\x16\x43reateNotifierResponse\"\x9a\x01\n\x15UpdateNotifierRequest\x12Q\n\x08notifier\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Notifier\x12.\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"\x18\n\x16UpdateNotifierResponse\"5\n\x12GetNotifierRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"v\n\x13GetNotifierResponse\x12Q\n\x08notifier\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Notifier\x12\x0c\n\x04yaml\x18\x02 \x01(\t\"8\n\x15\x44\x65leteNotifierRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x18\n\x16\x44\x65leteNotifierResponse2\xb9\x08\n\x0fNotifierService\x12\xc7\x01\n\rListNotifiers\x12H.github.com.metaprov.modelaapi.services.notifier.v1.ListNotifiersRequest\x1aI.github.com.metaprov.modelaapi.services.notifier.v1.ListNotifiersResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/v1/notifiers/{namespace}\x12\xc1\x01\n\x0e\x43reateNotifier\x12I.github.com.metaprov.modelaapi.services.notifier.v1.CreateNotifierRequest\x1aJ.github.com.metaprov.modelaapi.services.notifier.v1.CreateNotifierResponse\"\x18\x82\xd3\xe4\x93\x02\x12\"\r/v1/notifiers:\x01*\x12\xc8\x01\n\x0bGetNotifier\x12\x46.github.com.metaprov.modelaapi.services.notifier.v1.GetNotifierRequest\x1aG.github.com.metaprov.modelaapi.services.notifier.v1.GetNotifierResponse\"(\x82\xd3\xe4\x93\x02\"\x12 /v1/notifiers/{namespace}/{name}\x12\xf8\x01\n\x0eUpdateNotifier\x12I.github.com.metaprov.modelaapi.services.notifier.v1.UpdateNotifierRequest\x1aJ.github.com.metaprov.modelaapi.services.notifier.v1.UpdateNotifierResponse\"O\x82\xd3\xe4\x93\x02I\x1a\x44/v1/notifiers/{notifier.metadata.namespace}/{notifier.metadata.name}:\x01*\x12\xd1\x01\n\x0e\x44\x65leteNotifier\x12I.github.com.metaprov.modelaapi.services.notifier.v1.DeleteNotifierRequest\x1aJ.github.com.metaprov.modelaapi.services.notifier.v1.DeleteNotifierResponse\"(\x82\xd3\xe4\x93\x02\"* /v1/notifiers/{namespace}/{name}B4Z2github.com/metaprov/modelaapi/services/notifier/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9github.com/metaprov/modelaapi/services/todo/v1/todo.proto\x12.github.com.metaprov.modelaapi.services.todo.v1\x1a google/protobuf/field_mask.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\"\xb2\x01\n\x10ListTodosRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\\\n\x06labels\x18\x02 \x03(\x0b\x32L.github.com.metaprov.modelaapi.services.todo.v1.ListTodosRequest.LabelsEntry\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"{\n\x11ListTodosResponse\x12M\n\x05todos\x18\x01 \x01(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.team.v1alpha1.TodoList\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"o\n\x11\x43reateTodoRequest\x12H\n\x04todo\x18\x01 \x01(\x0b\x32:.github.com.metaprov.modelaapi.pkg.apis.team.v1alpha1.Todo\x12\x10\n\x08password\x18\x02 \x01(\t\"\x14\n\x12\x43reateTodoResponse\"\x8d\x01\n\x11UpdateTodoRequest\x12H\n\x04todo\x18\x01 \x01(\x0b\x32:.github.com.metaprov.modelaapi.pkg.apis.team.v1alpha1.Todo\x12.\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"\x14\n\x12UpdateTodoResponse\"1\n\x0eGetTodoRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"i\n\x0fGetTodoResponse\x12H\n\x04todo\x18\x01 \x01(\x0b\x32:.github.com.metaprov.modelaapi.pkg.apis.team.v1alpha1.Todo\x12\x0c\n\x04yaml\x18\x02 \x01(\t\"4\n\x11\x44\x65leteTodoRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x14\n\x12\x44\x65leteTodoResponse2\xb5\x07\n\x0bTodoService\x12\xaf\x01\n\tListTodos\x12@.github.com.metaprov.modelaapi.services.todo.v1.ListTodosRequest\x1a\x41.github.com.metaprov.modelaapi.services.todo.v1.ListTodosResponse\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/v1/todos/{namespace}\x12\xa9\x01\n\nCreateTodo\x12\x41.github.com.metaprov.modelaapi.services.todo.v1.CreateTodoRequest\x1a\x42.github.com.metaprov.modelaapi.services.todo.v1.CreateTodoResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\"\t/v1/todos:\x01*\x12\xb0\x01\n\x07GetTodo\x12>.github.com.metaprov.modelaapi.services.todo.v1.GetTodoRequest\x1a?.github.com.metaprov.modelaapi.services.todo.v1.GetTodoResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/todos/{namespace}/{name}\x12\xd8\x01\n\nUpdateTodo\x12\x41.github.com.metaprov.modelaapi.services.todo.v1.UpdateTodoRequest\x1a\x42.github.com.metaprov.modelaapi.services.todo.v1.UpdateTodoResponse\"C\x82\xd3\xe4\x93\x02=\x1a\x38/v1/todos/{todo.metadata.namespace}/{todo.metadata.name}:\x01*\x12\xb9\x01\n\nDeleteTodo\x12\x41.github.com.metaprov.modelaapi.services.todo.v1.DeleteTodoRequest\x1a\x42.github.com.metaprov.modelaapi.services.todo.v1.DeleteTodoResponse\"$\x82\xd3\xe4\x93\x02\x1e*\x1c/v1/todos/{namespace}/{name}B0Z.github.com/metaprov/modelaapi/services/todo/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.notifier.v1.notifier_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.todo.v1.todo_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z2github.com/metaprov/modelaapi/services/notifier/v1'
-  _LISTNOTIFIERSREQUEST_LABELSENTRY._options = None
-  _LISTNOTIFIERSREQUEST_LABELSENTRY._serialized_options = b'8\001'
-  _NOTIFIERSERVICE.methods_by_name['ListNotifiers']._options = None
-  _NOTIFIERSERVICE.methods_by_name['ListNotifiers']._serialized_options = b'\202\323\344\223\002\033\022\031/v1/notifiers/{namespace}'
-  _NOTIFIERSERVICE.methods_by_name['CreateNotifier']._options = None
-  _NOTIFIERSERVICE.methods_by_name['CreateNotifier']._serialized_options = b'\202\323\344\223\002\022\"\r/v1/notifiers:\001*'
-  _NOTIFIERSERVICE.methods_by_name['GetNotifier']._options = None
-  _NOTIFIERSERVICE.methods_by_name['GetNotifier']._serialized_options = b'\202\323\344\223\002\"\022 /v1/notifiers/{namespace}/{name}'
-  _NOTIFIERSERVICE.methods_by_name['UpdateNotifier']._options = None
-  _NOTIFIERSERVICE.methods_by_name['UpdateNotifier']._serialized_options = b'\202\323\344\223\002I\032D/v1/notifiers/{notifier.metadata.namespace}/{notifier.metadata.name}:\001*'
-  _NOTIFIERSERVICE.methods_by_name['DeleteNotifier']._options = None
-  _NOTIFIERSERVICE.methods_by_name['DeleteNotifier']._serialized_options = b'\202\323\344\223\002\"* /v1/notifiers/{namespace}/{name}'
-  _LISTNOTIFIERSREQUEST._serialized_start=320
-  _LISTNOTIFIERSREQUEST._serialized_end=567
-  _LISTNOTIFIERSREQUEST_LABELSENTRY._serialized_start=522
-  _LISTNOTIFIERSREQUEST_LABELSENTRY._serialized_end=567
-  _LISTNOTIFIERSRESPONSE._serialized_start=570
-  _LISTNOTIFIERSRESPONSE._serialized_end=706
-  _NOTIFIERRESPONSE._serialized_start=708
-  _NOTIFIERRESPONSE._serialized_end=726
-  _CREATENOTIFIERREQUEST._serialized_start=728
-  _CREATENOTIFIERREQUEST._serialized_end=834
-  _CREATENOTIFIERRESPONSE._serialized_start=836
-  _CREATENOTIFIERRESPONSE._serialized_end=860
-  _UPDATENOTIFIERREQUEST._serialized_start=863
-  _UPDATENOTIFIERREQUEST._serialized_end=1017
-  _UPDATENOTIFIERRESPONSE._serialized_start=1019
-  _UPDATENOTIFIERRESPONSE._serialized_end=1043
-  _GETNOTIFIERREQUEST._serialized_start=1045
-  _GETNOTIFIERREQUEST._serialized_end=1098
-  _GETNOTIFIERRESPONSE._serialized_start=1100
-  _GETNOTIFIERRESPONSE._serialized_end=1218
-  _DELETENOTIFIERREQUEST._serialized_start=1220
-  _DELETENOTIFIERREQUEST._serialized_end=1276
-  _DELETENOTIFIERRESPONSE._serialized_start=1278
-  _DELETENOTIFIERRESPONSE._serialized_end=1302
-  _NOTIFIERSERVICE._serialized_start=1305
-  _NOTIFIERSERVICE._serialized_end=2386
+  DESCRIPTOR._serialized_options = b'Z.github.com/metaprov/modelaapi/services/todo/v1'
+  _LISTTODOSREQUEST_LABELSENTRY._options = None
+  _LISTTODOSREQUEST_LABELSENTRY._serialized_options = b'8\001'
+  _TODOSERVICE.methods_by_name['ListTodos']._options = None
+  _TODOSERVICE.methods_by_name['ListTodos']._serialized_options = b'\202\323\344\223\002\027\022\025/v1/todos/{namespace}'
+  _TODOSERVICE.methods_by_name['CreateTodo']._options = None
+  _TODOSERVICE.methods_by_name['CreateTodo']._serialized_options = b'\202\323\344\223\002\016\"\t/v1/todos:\001*'
+  _TODOSERVICE.methods_by_name['GetTodo']._options = None
+  _TODOSERVICE.methods_by_name['GetTodo']._serialized_options = b'\202\323\344\223\002\036\022\034/v1/todos/{namespace}/{name}'
+  _TODOSERVICE.methods_by_name['UpdateTodo']._options = None
+  _TODOSERVICE.methods_by_name['UpdateTodo']._serialized_options = b'\202\323\344\223\002=\0328/v1/todos/{todo.metadata.namespace}/{todo.metadata.name}:\001*'
+  _TODOSERVICE.methods_by_name['DeleteTodo']._options = None
+  _TODOSERVICE.methods_by_name['DeleteTodo']._serialized_options = b'\202\323\344\223\002\036*\034/v1/todos/{namespace}/{name}'
+  _LISTTODOSREQUEST._serialized_start=307
+  _LISTTODOSREQUEST._serialized_end=485
+  _LISTTODOSREQUEST_LABELSENTRY._serialized_start=440
+  _LISTTODOSREQUEST_LABELSENTRY._serialized_end=485
+  _LISTTODOSRESPONSE._serialized_start=487
+  _LISTTODOSRESPONSE._serialized_end=610
+  _CREATETODOREQUEST._serialized_start=612
+  _CREATETODOREQUEST._serialized_end=723
+  _CREATETODORESPONSE._serialized_start=725
+  _CREATETODORESPONSE._serialized_end=745
+  _UPDATETODOREQUEST._serialized_start=748
+  _UPDATETODOREQUEST._serialized_end=889
+  _UPDATETODORESPONSE._serialized_start=891
+  _UPDATETODORESPONSE._serialized_end=911
+  _GETTODOREQUEST._serialized_start=913
+  _GETTODOREQUEST._serialized_end=962
+  _GETTODORESPONSE._serialized_start=964
+  _GETTODORESPONSE._serialized_end=1069
+  _DELETETODOREQUEST._serialized_start=1071
+  _DELETETODOREQUEST._serialized_end=1123
+  _DELETETODORESPONSE._serialized_start=1125
+  _DELETETODORESPONSE._serialized_end=1145
+  _TODOSERVICE._serialized_start=1148
+  _TODOSERVICE._serialized_end=2097
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py` & `modelaapi-0.6.220/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/google/api/annotations_pb2.py` & `modelaapi-0.6.220/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/google/api/http_pb2.py` & `modelaapi-0.6.220/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/k8s/io/api/apps/v1/generated_pb2.py` & `modelaapi-0.6.220/k8s/io/api/apps/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/k8s/io/api/core/v1/generated_pb2.py` & `modelaapi-0.6.220/k8s/io/api/core/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/k8s/io/api/rbac/v1/generated_pb2.py` & `modelaapi-0.6.220/k8s/io/api/rbac/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py` & `modelaapi-0.6.220/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py` & `modelaapi-0.6.220/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/k8s/io/apimachinery/pkg/runtime/generated_pb2.py` & `modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py` & `modelaapi-0.6.220/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py` & `modelaapi-0.6.220/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/modelaapi/consts.py` & `modelaapi-0.6.220/modelaapi/consts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/modelaapi/custom_transformers.py` & `modelaapi-0.6.220/modelaapi/custom_transformers.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/modelaapi/graykite_model.py` & `modelaapi-0.6.220/modelaapi/graykite_model.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/modelaapi/ts.py` & `modelaapi-0.6.220/modelaapi/ts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/modelaapi/version.py` & `modelaapi-0.6.220/modelaapi/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
     "minor": 6,
-    "micro": 210,
+    "micro": 220,
     "releaselevel": "alpha",
     "post": 0,
     "serial": 1,
 }
 
 ##########################################################################
 ## Helper Functions
```

### Comparing `modelaapi-0.6.210/modelaapi.egg-info/PKG-INFO` & `modelaapi-0.6.220/modelaapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.210
+Version: 0.6.220
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.210
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.220
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.210
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.220
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.210/modelaapi.egg-info/SOURCES.txt` & `modelaapi-0.6.220/modelaapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/setup.cfg` & `modelaapi-0.6.220/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.210/setup.py` & `modelaapi-0.6.220/setup.py`

 * *Files identical despite different names*

