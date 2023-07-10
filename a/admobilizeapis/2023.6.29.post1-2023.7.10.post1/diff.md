# Comparing `tmp/admobilizeapis-2023.6.29.post1.tar.gz` & `tmp/admobilizeapis-2023.7.10.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/admobilizeapis-2023.6.29.post1.tar", last modified: Thu Jun 29 17:16:05 2023, max compression
+gzip compressed data, was "dist/admobilizeapis-2023.7.10.post1.tar", last modified: Mon Jul 10 14:53:50 2023, max compression
```

## Comparing `admobilizeapis-2023.6.29.post1.tar` & `admobilizeapis-2023.7.10.post1.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/google/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/google/longrunning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/google/longrunning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8090 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/google/longrunning/operations_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10932 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/google/longrunning/operations_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/v1/wifi_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2457 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/v1/wifi_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8861 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8708 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    25837 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4250 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    35932 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6645 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10396 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14597 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/model_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4194 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/model_pb2.py
--rw-r--r--   0 root         (0) root         (0)    26810 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)     6478 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5542 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5528 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15461 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    39106 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    28693 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10609 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28083 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    18992 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    20392 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    99455 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    76701 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    13543 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    41623 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29786 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9576 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14877 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15271 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6954 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    22477 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8758 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/driver_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4590 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/driver_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6136 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/maloseye_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/maloseye_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    14646 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    31149 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    28346 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15801 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    21203 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3157 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18378 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    24106 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3240 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/job_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/admobilize_types_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4485 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/entity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/admobilize_types_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2897 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/entity_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/billing/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/billing/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/billing/v1alpha1/billing_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)    22301 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16652 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29481 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24348 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21841 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3174 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16356 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)     6814 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      849 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1201 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/README.md
--rw-r--r--   0 root         (0) root         (0)     1293 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/google/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/google/longrunning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/google/longrunning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8090 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/google/longrunning/operations_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10932 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/google/longrunning/operations_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/v1/wifi_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/v1/wifi_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8861 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    25837 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4250 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    35932 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10396 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14597 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/model_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/model_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    26810 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)     6478 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5542 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5528 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39106 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    28693 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10609 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28083 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    18992 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    20392 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    99455 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    76701 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13543 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    41623 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29786 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9576 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14877 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15271 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6954 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    22477 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/driver_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4590 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/driver_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6136 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/maloseye_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/maloseye_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15710 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32988 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29571 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15801 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    21203 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18378 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    24106 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/job_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/admobilize_types_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4485 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/entity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/admobilize_types_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/entity_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/billing/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/billing/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/billing/v1alpha1/billing_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)    22301 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16652 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24348 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21841 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3174 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16356 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)     6814 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      849 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/setup.cfg
```

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/google/longrunning/operations_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/google/longrunning/operations_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/v1/wifi_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/v1/wifi_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/model_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/driver_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/maloseye_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/maloseye_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/resources_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)admobilize/query/v1alpha1/resources.proto\x12\x19\x61\x64mobilize.query.v1alpha1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"B\n\x07Project\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x12\n\ncreated_at\x18\x02 \x01(\t\x12\x12\n\nupdated_at\x18\x03 \x01(\t\"\x80\x01\n\x06Metric\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x66ield\x18\x02 \x01(\t\x12\x11\n\toperation\x18\x03 \x01(\t\x12\x0e\n\x06\x66ilter\x18\x04 \x03(\t\x12\r\n\x05order\x18\x05 \x01(\t\x12\x19\n\x11\x63onversion_factor\x18\x06 \x01(\x01\x12\x0c\n\x04\x63\x61st\x18\x07 \x01(\t\"@\n\x0f\x41ggregateResult\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\x12\n\n\x02\x61s\x18\x03 \x01(\t\"\xbb\x01\n\x0fQueryFromResult\x12\x0e\n\x06select\x18\x01 \x03(\t\x12\x0b\n\x03sum\x18\x02 \x03(\t\x12\x0b\n\x03\x61vg\x18\x03 \x03(\t\x12\x0f\n\x07groupBy\x18\x04 \x03(\t\x12\x43\n\x07orderBy\x18\x05 \x03(\x0b\x32\x32.admobilize.query.v1alpha1.QueryFromResult.OrderBy\x1a(\n\x07OrderBy\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\t\"4\n\rEncoderParams\x12\x0f\n\x07metrics\x18\x01 \x03(\t\x12\x12\n\ndimensions\x18\x02 \x03(\t\"?\n\x07\x44\x61taset\x12\r\n\x05label\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value\")\n\x0bSchemaField\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x80\x01\n\nClassifier\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\x12\r\n\x05\x66ield\x18\x03 \x01(\t\x12\x42\n\nconditions\x18\x04 \x03(\x0b\x32..admobilize.query.v1alpha1.ClassifierCondition\"+\n\nOrderField\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\t\"M\n\x13\x43lassifierCondition\x12\x0c\n\x04when\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x02\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x02\x12\x0c\n\x04then\x18\x04 \x01(\t\"5\n\x06Status\x12\x13\n\x0bstatus_code\x18\x01 \x01(\t\x12\x16\n\x0estatus_message\x18\x02 \x01(\t\"3\n\tDeviceMap\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x02 \x01(\t\"\xc0\x01\n\x03Job\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x35\n\x06status\x18\x02 \x01(\x0e\x32%.admobilize.query.v1alpha1.Job.Status\x12\x0e\n\x06\x64\x65tail\x18\x03 \x01(\t\x12\x16\n\x0estatus_message\x18\x04 \x01(\t\x12\x11\n\tself_link\x18\x05 \x01(\t\"7\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\x08\n\x04\x44ONE\x10\x03\x12\t\n\x05\x45RROR\x10\x04\"\xc9\x04\n\x06Report\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x64vertisers\x18\x02 \x03(\t\x12.\n\ncreated_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x64\x61ys_to_send\x18\x04 \x03(\t\x12\x12\n\ndevice_ids\x18\x05 \x03(\t\x12\r\n\x05\x65mail\x18\x06 \x03(\t\x12\x0e\n\x06\x66ields\x18\x07 \x03(\t\x12\x0e\n\x06\x66ormat\x18\x08 \x01(\t\x12\x11\n\tfrequency\x18\t \x01(\t\x12\x10\n\x08interval\x18\n \x01(\t\x12-\n\tlast_sent\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0flast_report_url\x18\x0c \x01(\t\x12\r\n\x05media\x18\r \x03(\t\x12\x0c\n\x04name\x18\x0e \x01(\t\x12\x12\n\nproject_id\x18\x0f \x01(\t\x12.\n\nstart_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_date\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x19\n\x11\x66ilter_by_weekday\x18\x16 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x17 \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x0e\n\x06status\x18\x11 \x01(\t\x12\r\n\x05table\x18\x12 \x01(\t\x12\x10\n\x08timezone\x18\x13 \x01(\t\x12\x0c\n\x04type\x18\x14 \x01(\t\"*\n\x0c\x46ilterByTime\x12\r\n\x05start\x18\x01 \x01(\t\x12\x0b\n\x03\x65nd\x18\x02 \x01(\t\")\n\x08\x46ilterBy\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"(\n\x0c\x43MSDimension\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02\x61s\x18\x02 \x01(\t\"~\n\rCMSDescriptor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x15\n\rplaylog_table\x18\x03 \x01(\t\x12\x39\n\x07\x63olumns\x18\x04 \x01(\x0b\x32(.admobilize.query.v1alpha1.CMSColumnsMap\"V\n\rCMSColumnsMap\x12\x13\n\x0b\x61\x64vertisers\x18\x01 \x01(\t\x12\r\n\x05sites\x18\x02 \x01(\t\x12\x0e\n\x06medias\x18\x03 \x01(\t\x12\x11\n\ttimestamp\x18\x04 \x01(\tB\x93\x01\n\x1d\x63om.admobilize.query.v1alpha1B\nQueryProtoP\x01Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\xa2\x02\x05\x41\x44MQY\xaa\x02\x19\x41\x64Mobilize.Query.V1Alpha1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)admobilize/query/v1alpha1/resources.proto\x12\x19\x61\x64mobilize.query.v1alpha1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"B\n\x07Project\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x12\n\ncreated_at\x18\x02 \x01(\t\x12\x12\n\nupdated_at\x18\x03 \x01(\t\"2\n\x0bHeatmapData\x12\t\n\x01x\x18\x01 \x01(\r\x12\t\n\x01y\x18\x02 \x01(\r\x12\r\n\x05value\x18\x03 \x01(\x02\"?\n\x07Heatmap\x12\x34\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32&.admobilize.query.v1alpha1.HeatmapData\"\x80\x01\n\x06Metric\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x66ield\x18\x02 \x01(\t\x12\x11\n\toperation\x18\x03 \x01(\t\x12\x0e\n\x06\x66ilter\x18\x04 \x03(\t\x12\r\n\x05order\x18\x05 \x01(\t\x12\x19\n\x11\x63onversion_factor\x18\x06 \x01(\x01\x12\x0c\n\x04\x63\x61st\x18\x07 \x01(\t\"@\n\x0f\x41ggregateResult\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\x12\n\n\x02\x61s\x18\x03 \x01(\t\"\xbb\x01\n\x0fQueryFromResult\x12\x0e\n\x06select\x18\x01 \x03(\t\x12\x0b\n\x03sum\x18\x02 \x03(\t\x12\x0b\n\x03\x61vg\x18\x03 \x03(\t\x12\x0f\n\x07groupBy\x18\x04 \x03(\t\x12\x43\n\x07orderBy\x18\x05 \x03(\x0b\x32\x32.admobilize.query.v1alpha1.QueryFromResult.OrderBy\x1a(\n\x07OrderBy\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\t\"4\n\rEncoderParams\x12\x0f\n\x07metrics\x18\x01 \x03(\t\x12\x12\n\ndimensions\x18\x02 \x03(\t\"?\n\x07\x44\x61taset\x12\r\n\x05label\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value\")\n\x0bSchemaField\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x80\x01\n\nClassifier\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\x12\r\n\x05\x66ield\x18\x03 \x01(\t\x12\x42\n\nconditions\x18\x04 \x03(\x0b\x32..admobilize.query.v1alpha1.ClassifierCondition\"+\n\nOrderField\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\t\"M\n\x13\x43lassifierCondition\x12\x0c\n\x04when\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x02\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x02\x12\x0c\n\x04then\x18\x04 \x01(\t\"5\n\x06Status\x12\x13\n\x0bstatus_code\x18\x01 \x01(\t\x12\x16\n\x0estatus_message\x18\x02 \x01(\t\"3\n\tDeviceMap\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x02 \x01(\t\"\xc0\x01\n\x03Job\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x35\n\x06status\x18\x02 \x01(\x0e\x32%.admobilize.query.v1alpha1.Job.Status\x12\x0e\n\x06\x64\x65tail\x18\x03 \x01(\t\x12\x16\n\x0estatus_message\x18\x04 \x01(\t\x12\x11\n\tself_link\x18\x05 \x01(\t\"7\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\x08\n\x04\x44ONE\x10\x03\x12\t\n\x05\x45RROR\x10\x04\"\xc9\x04\n\x06Report\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x64vertisers\x18\x02 \x03(\t\x12.\n\ncreated_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x64\x61ys_to_send\x18\x04 \x03(\t\x12\x12\n\ndevice_ids\x18\x05 \x03(\t\x12\r\n\x05\x65mail\x18\x06 \x03(\t\x12\x0e\n\x06\x66ields\x18\x07 \x03(\t\x12\x0e\n\x06\x66ormat\x18\x08 \x01(\t\x12\x11\n\tfrequency\x18\t \x01(\t\x12\x10\n\x08interval\x18\n \x01(\t\x12-\n\tlast_sent\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0flast_report_url\x18\x0c \x01(\t\x12\r\n\x05media\x18\r \x03(\t\x12\x0c\n\x04name\x18\x0e \x01(\t\x12\x12\n\nproject_id\x18\x0f \x01(\t\x12.\n\nstart_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_date\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x19\n\x11\x66ilter_by_weekday\x18\x16 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x17 \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x0e\n\x06status\x18\x11 \x01(\t\x12\r\n\x05table\x18\x12 \x01(\t\x12\x10\n\x08timezone\x18\x13 \x01(\t\x12\x0c\n\x04type\x18\x14 \x01(\t\"*\n\x0c\x46ilterByTime\x12\r\n\x05start\x18\x01 \x01(\t\x12\x0b\n\x03\x65nd\x18\x02 \x01(\t\")\n\x08\x46ilterBy\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"(\n\x0c\x43MSDimension\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02\x61s\x18\x02 \x01(\t\"~\n\rCMSDescriptor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x15\n\rplaylog_table\x18\x03 \x01(\t\x12\x39\n\x07\x63olumns\x18\x04 \x01(\x0b\x32(.admobilize.query.v1alpha1.CMSColumnsMap\"V\n\rCMSColumnsMap\x12\x13\n\x0b\x61\x64vertisers\x18\x01 \x01(\t\x12\r\n\x05sites\x18\x02 \x01(\t\x12\x0e\n\x06medias\x18\x03 \x01(\t\x12\x11\n\ttimestamp\x18\x04 \x01(\tB\x93\x01\n\x1d\x63om.admobilize.query.v1alpha1B\nQueryProtoP\x01Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\xa2\x02\x05\x41\x44MQY\xaa\x02\x19\x41\x64Mobilize.Query.V1Alpha1b\x06proto3')
 
 
 
 _PROJECT = DESCRIPTOR.message_types_by_name['Project']
+_HEATMAPDATA = DESCRIPTOR.message_types_by_name['HeatmapData']
+_HEATMAP = DESCRIPTOR.message_types_by_name['Heatmap']
 _METRIC = DESCRIPTOR.message_types_by_name['Metric']
 _AGGREGATERESULT = DESCRIPTOR.message_types_by_name['AggregateResult']
 _QUERYFROMRESULT = DESCRIPTOR.message_types_by_name['QueryFromResult']
 _QUERYFROMRESULT_ORDERBY = _QUERYFROMRESULT.nested_types_by_name['OrderBy']
 _ENCODERPARAMS = DESCRIPTOR.message_types_by_name['EncoderParams']
 _DATASET = DESCRIPTOR.message_types_by_name['Dataset']
 _SCHEMAFIELD = DESCRIPTOR.message_types_by_name['SchemaField']
@@ -46,14 +48,28 @@
 Project = _reflection.GeneratedProtocolMessageType('Project', (_message.Message,), {
   'DESCRIPTOR' : _PROJECT,
   '__module__' : 'admobilize.query.v1alpha1.resources_pb2'
   # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.Project)
   })
 _sym_db.RegisterMessage(Project)
 
+HeatmapData = _reflection.GeneratedProtocolMessageType('HeatmapData', (_message.Message,), {
+  'DESCRIPTOR' : _HEATMAPDATA,
+  '__module__' : 'admobilize.query.v1alpha1.resources_pb2'
+  # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.HeatmapData)
+  })
+_sym_db.RegisterMessage(HeatmapData)
+
+Heatmap = _reflection.GeneratedProtocolMessageType('Heatmap', (_message.Message,), {
+  'DESCRIPTOR' : _HEATMAP,
+  '__module__' : 'admobilize.query.v1alpha1.resources_pb2'
+  # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.Heatmap)
+  })
+_sym_db.RegisterMessage(Heatmap)
+
 Metric = _reflection.GeneratedProtocolMessageType('Metric', (_message.Message,), {
   'DESCRIPTOR' : _METRIC,
   '__module__' : 'admobilize.query.v1alpha1.resources_pb2'
   # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.Metric)
   })
 _sym_db.RegisterMessage(Metric)
 
@@ -186,48 +202,52 @@
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\035com.admobilize.query.v1alpha1B\nQueryProtoP\001Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\242\002\005ADMQY\252\002\031AdMobilize.Query.V1Alpha1'
   _PROJECT._serialized_start=199
   _PROJECT._serialized_end=265
-  _METRIC._serialized_start=268
-  _METRIC._serialized_end=396
-  _AGGREGATERESULT._serialized_start=398
-  _AGGREGATERESULT._serialized_end=462
-  _QUERYFROMRESULT._serialized_start=465
-  _QUERYFROMRESULT._serialized_end=652
-  _QUERYFROMRESULT_ORDERBY._serialized_start=612
-  _QUERYFROMRESULT_ORDERBY._serialized_end=652
-  _ENCODERPARAMS._serialized_start=654
-  _ENCODERPARAMS._serialized_end=706
-  _DATASET._serialized_start=708
-  _DATASET._serialized_end=771
-  _SCHEMAFIELD._serialized_start=773
-  _SCHEMAFIELD._serialized_end=814
-  _CLASSIFIER._serialized_start=817
-  _CLASSIFIER._serialized_end=945
-  _ORDERFIELD._serialized_start=947
-  _ORDERFIELD._serialized_end=990
-  _CLASSIFIERCONDITION._serialized_start=992
-  _CLASSIFIERCONDITION._serialized_end=1069
-  _STATUS._serialized_start=1071
-  _STATUS._serialized_end=1124
-  _DEVICEMAP._serialized_start=1126
-  _DEVICEMAP._serialized_end=1177
-  _JOB._serialized_start=1180
-  _JOB._serialized_end=1372
-  _JOB_STATUS._serialized_start=1317
-  _JOB_STATUS._serialized_end=1372
-  _REPORT._serialized_start=1375
-  _REPORT._serialized_end=1960
-  _FILTERBYTIME._serialized_start=1962
-  _FILTERBYTIME._serialized_end=2004
-  _FILTERBY._serialized_start=2006
-  _FILTERBY._serialized_end=2047
-  _CMSDIMENSION._serialized_start=2049
-  _CMSDIMENSION._serialized_end=2089
-  _CMSDESCRIPTOR._serialized_start=2091
-  _CMSDESCRIPTOR._serialized_end=2217
-  _CMSCOLUMNSMAP._serialized_start=2219
-  _CMSCOLUMNSMAP._serialized_end=2305
+  _HEATMAPDATA._serialized_start=267
+  _HEATMAPDATA._serialized_end=317
+  _HEATMAP._serialized_start=319
+  _HEATMAP._serialized_end=382
+  _METRIC._serialized_start=385
+  _METRIC._serialized_end=513
+  _AGGREGATERESULT._serialized_start=515
+  _AGGREGATERESULT._serialized_end=579
+  _QUERYFROMRESULT._serialized_start=582
+  _QUERYFROMRESULT._serialized_end=769
+  _QUERYFROMRESULT_ORDERBY._serialized_start=729
+  _QUERYFROMRESULT_ORDERBY._serialized_end=769
+  _ENCODERPARAMS._serialized_start=771
+  _ENCODERPARAMS._serialized_end=823
+  _DATASET._serialized_start=825
+  _DATASET._serialized_end=888
+  _SCHEMAFIELD._serialized_start=890
+  _SCHEMAFIELD._serialized_end=931
+  _CLASSIFIER._serialized_start=934
+  _CLASSIFIER._serialized_end=1062
+  _ORDERFIELD._serialized_start=1064
+  _ORDERFIELD._serialized_end=1107
+  _CLASSIFIERCONDITION._serialized_start=1109
+  _CLASSIFIERCONDITION._serialized_end=1186
+  _STATUS._serialized_start=1188
+  _STATUS._serialized_end=1241
+  _DEVICEMAP._serialized_start=1243
+  _DEVICEMAP._serialized_end=1294
+  _JOB._serialized_start=1297
+  _JOB._serialized_end=1489
+  _JOB_STATUS._serialized_start=1434
+  _JOB_STATUS._serialized_end=1489
+  _REPORT._serialized_start=1492
+  _REPORT._serialized_end=2077
+  _FILTERBYTIME._serialized_start=2079
+  _FILTERBYTIME._serialized_end=2121
+  _FILTERBY._serialized_start=2123
+  _FILTERBY._serialized_end=2164
+  _CMSDIMENSION._serialized_start=2166
+  _CMSDIMENSION._serialized_end=2206
+  _CMSDESCRIPTOR._serialized_start=2208
+  _CMSDESCRIPTOR._serialized_end=2334
+  _CMSCOLUMNSMAP._serialized_start=2336
+  _CMSCOLUMNSMAP._serialized_end=2422
 # @@protoc_insertion_point(module_scope)
```

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,19 @@
                 response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Report.FromString,
                 )
         self.GetTableData = channel.unary_unary(
                 '/admobilize.query.v1alpha1.QueryService/GetTableData',
                 request_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableDataRequest.SerializeToString,
                 response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableDataResponse.FromString,
                 )
+        self.GetDeviceHeatmap = channel.unary_unary(
+                '/admobilize.query.v1alpha1.QueryService/GetDeviceHeatmap',
+                request_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetDeviceHeatmapRequest.SerializeToString,
+                response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Heatmap.FromString,
+                )
         self.CreateJob = channel.unary_unary(
                 '/admobilize.query.v1alpha1.QueryService/CreateJob',
                 request_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.CreateJobRequest.SerializeToString,
                 response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Job.FromString,
                 )
         self.GetJob = channel.unary_unary(
                 '/admobilize.query.v1alpha1.QueryService/GetJob',
@@ -196,14 +201,20 @@
         """Get raw table data  <br/>
         Required permissions: `queryapi.datasets.getTableData`
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetDeviceHeatmap(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def CreateJob(self, request, context):
         """
         DATA API METHODS
 
         Starts a job do retrieve user datapoints. <br/>
         Required permissions: `queryapi.jobs.create`
         """
@@ -294,14 +305,19 @@
                     response_serializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Report.SerializeToString,
             ),
             'GetTableData': grpc.unary_unary_rpc_method_handler(
                     servicer.GetTableData,
                     request_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableDataRequest.FromString,
                     response_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableDataResponse.SerializeToString,
             ),
+            'GetDeviceHeatmap': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetDeviceHeatmap,
+                    request_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetDeviceHeatmapRequest.FromString,
+                    response_serializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Heatmap.SerializeToString,
+            ),
             'CreateJob': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateJob,
                     request_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.CreateJobRequest.FromString,
                     response_serializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Job.SerializeToString,
             ),
             'GetJob': grpc.unary_unary_rpc_method_handler(
                     servicer.GetJob,
@@ -531,14 +547,31 @@
         return grpc.experimental.unary_unary(request, target, '/admobilize.query.v1alpha1.QueryService/GetTableData',
             admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableDataRequest.SerializeToString,
             admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableDataResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetDeviceHeatmap(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/admobilize.query.v1alpha1.QueryService/GetDeviceHeatmap',
+            admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetDeviceHeatmapRequest.SerializeToString,
+            admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Heatmap.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def CreateJob(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from admobilize.proto.query.v1alpha1 import resources_pb2 as admobilize_dot_query_dot_v1alpha1_dot_resources__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-admobilize/query/v1alpha1/query_service.proto\x12\x19\x61\x64mobilize.query.v1alpha1\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a google/protobuf/field_mask.proto\x1a)admobilize/query/v1alpha1/resources.proto\".\n\x1b\x43reateProjectDatasetRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\"\xdc\x07\n\x0cQueryRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x32\n\x07metrics\x18\x03 \x03(\x0b\x32!.admobilize.query.v1alpha1.Metric\x12\x12\n\ndimensions\x18\x04 \x03(\t\x12\r\n\x05\x65poch\x18\x05 \x01(\t\x12\x16\n\x0ehas_comparison\x18\x06 \x01(\x08\x12\x44\n\x10\x61ggregate_result\x18\x0b \x01(\x0b\x32*.admobilize.query.v1alpha1.AggregateResult\x12\x45\n\x11query_from_result\x18( \x01(\x0b\x32*.admobilize.query.v1alpha1.QueryFromResult\x12:\n\x0b\x63lassifiers\x18\x0c \x03(\x0b\x32%.admobilize.query.v1alpha1.Classifier\x12\x0f\n\x07timeout\x18\t \x01(\r\x12\r\n\x05limit\x18\n \x01(\r\x12\x1a\n\x12\x64imensions_encoder\x18\r \x01(\x08\x12@\n\x0e\x65ncoder_params\x18* \x01(\x0b\x32(.admobilize.query.v1alpha1.EncoderParams\x12\x37\n\x08order_by\x18\x0f \x03(\x0b\x32%.admobilize.query.v1alpha1.OrderField\x12\x16\n\x0e\x66ilter_by_hour\x18\x10 \x03(\r\x12\x19\n\x11\x66ilter_by_weekday\x18\x11 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x12 \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x36\n\x0b\x63ms_metrics\x18\x13 \x03(\x0b\x32!.admobilize.query.v1alpha1.Metric\x12>\n\rcms_dimension\x18\x14 \x01(\x0b\x32\'.admobilize.query.v1alpha1.CMSDimension\x12@\n\x0e\x63ms_descriptor\x18\x1e \x01(\x0b\x32(.admobilize.query.v1alpha1.CMSDescriptor\x12.\n\nstart_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x0e \x01(\t\x12\x0c\n\x03wid\x18\xe6\x07 \x01(\t\x12\x11\n\x08previous\x18\xe7\x07 \x01(\x08\"R\n\rQueryResponse\x12\x34\n\x08\x64\x61tasets\x18\x01 \x03(\x0b\x32\".admobilize.query.v1alpha1.Dataset\x12\x0b\n\x03tid\x18\x02 \x01(\t\"$\n\x11ListTablesRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\"$\n\x12ListTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"7\n\x15GetTableSchemaRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"\x91\x01\n\x16GetTableSchemaResponse\x12\x36\n\x06schema\x18\x01 \x03(\x0b\x32&.admobilize.query.v1alpha1.SchemaField\x12\x10\n\x08num_rows\x18\x02 \x01(\x04\x12\x11\n\tnum_bytes\x18\x03 \x01(\x03\x12\x1a\n\x12last_modified_time\x18\x04 \x01(\x06\"\xba\x03\n\x10GetReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\r\n\x05\x65poch\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\t \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\n \x01(\t\x12\x12\n\nspeed_unit\x18\x0b \x01(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\x0c \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\r \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x0e\n\x06\x66ields\x18\x0e \x03(\t\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x07\x64\x65vices\x18\x08 \x03(\x0b\x32$.admobilize.query.v1alpha1.DeviceMap\x12\x13\n\x0b\x61\x64vertisers\x18\x0f \x03(\t\x12\x0e\n\x06medias\x18\x10 \x03(\t\"Z\n\x11GetReportResponse\x12\x31\n\x06status\x18\x01 \x01(\x0b\x32!.admobilize.query.v1alpha1.Status\x12\x12\n\nreport_url\x18\x02 \x01(\t\"\xdf\x01\n\x10\x43reateJobRequest\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nproject_id\x18\x03 \x01(\t\x12\x12\n\nproduct_id\x18\x04 \x01(\t\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12\x12\n\nspeed_unit\x18\x08 \x01(\t\x12\x12\n\ndevice_ids\x18\x05 \x03(\t\x12\x0b\n\x03\x63ms\x18\x06 \x01(\t\"G\n\rGetJobRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x66ields\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"I\n\x14GetJobResultRequests\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"2\n\x14\x45xportResultsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"j\n\x15GetDatapointsResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x14\n\x0cjob_complete\x18\x02 \x01(\x08\x12\x17\n\x0fnext_page_token\x18\x03 \x01(\t\x12\x12\n\ndatapoints\x18\x04 \x01(\t\"K\n\x15\x45xportResultsResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x14\n\x0cjob_complete\x18\x02 \x01(\x08\x12\x0c\n\x04urls\x18\x03 \x03(\t\"\xca\x03\n\x13GetTableDataRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06layout\x18\x03 \x01(\t\x12\x13\n\x0bmax_results\x18\x04 \x01(\r\x12\x12\n\npage_token\x18\x05 \x01(\t\x12\r\n\x05\x65poch\x18\x06 \x01(\t\x12\x35\n\x07\x64\x65vices\x18\x07 \x03(\x0b\x32$.admobilize.query.v1alpha1.DeviceMap\x12\x19\n\x11\x66ilter_by_weekday\x18\x08 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\t \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x10\n\x08group_by\x18\n \x03(\t\x12\x36\n\tfilter_by\x18\x0b \x01(\x0b\x32#.admobilize.query.v1alpha1.FilterBy\x12.\n\nstart_time\x18\x61 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x62 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x63 \x01(\t\"T\n\x14GetTableDataResponse\x12\x12\n\npage_token\x18\x02 \x01(\t\x12(\n\x04rows\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"4\n\x12ListReportsRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"I\n\x13ListReportsResponse\x12\x32\n\x07reports\x18\x01 \x03(\x0b\x32!.admobilize.query.v1alpha1.Report\"\xb3\x03\n\x13\x43reateReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\t \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\n \x01(\t\x12\x12\n\nspeed_unit\x18\x0b \x01(\t\x12\x11\n\tfrequency\x18\x0c \x01(\t\x12\x14\n\x0c\x64\x61ys_to_send\x18\r \x03(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\x0e \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x0f \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x64\x65vices\x18\x08 \x03(\t\x12\x13\n\x0b\x61\x64vertisers\x18\x10 \x03(\t\x12\x0e\n\x06medias\x18\x11 \x03(\t\"\xdc\x02\n\x13UpdateReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x0e\n\x06report\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x0c \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x03(\t\x12\x0c\n\x04type\x18\x06 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x07 \x01(\t\x12\x12\n\nspeed_unit\x18\x08 \x01(\t\x12\x11\n\tfrequency\x18\t \x01(\t\x12\x14\n\x0c\x64\x61ys_to_send\x18\n \x03(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\r \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x0e \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12,\n\x08\x65nd_time\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x12PauseReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"F\n\x14RestartReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"E\n\x13\x43\x61ncelReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t2\x98\x14\n\x0cQueryService\x12\x91\x01\n\x14\x43reateProjectDataset\x12\x36.admobilize.query.v1alpha1.CreateProjectDatasetRequest\x1a\".admobilize.query.v1alpha1.Project\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1alpha1/projects:\x01*\x12\x9c\x01\n\x05Query\x12\'.admobilize.query.v1alpha1.QueryRequest\x1a(.admobilize.query.v1alpha1.QueryResponse\"@\x82\xd3\xe4\x93\x02:\"5/v1alpha1/projects/{project=*}/tables/{table=*}/query:\x01*\x12\x98\x01\n\nListTables\x12,.admobilize.query.v1alpha1.ListTablesRequest\x1a-.admobilize.query.v1alpha1.ListTablesResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/v1alpha1/projects/{project=*}/tables\x12\xae\x01\n\x0eGetTableSchema\x12\x30.admobilize.query.v1alpha1.GetTableSchemaRequest\x1a\x31.admobilize.query.v1alpha1.GetTableSchemaResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//v1alpha1/projects/{project=*}/tables/{table=*}\x12\xa9\x01\n\tGetReport\x12+.admobilize.query.v1alpha1.GetReportRequest\x1a,.admobilize.query.v1alpha1.GetReportResponse\"A\x82\xd3\xe4\x93\x02;\"6/v1alpha1/projects/{project=*}/tables/{table=*}/report:\x01*\x12\xa5\x01\n\x0c\x43reateReport\x12..admobilize.query.v1alpha1.CreateReportRequest\x1a!.admobilize.query.v1alpha1.Report\"B\x82\xd3\xe4\x93\x02<\"7/v1alpha1/projects/{project=*}/tables/{table=*}/reports:\x01*\x12\x9f\x01\n\x0cUpdateReport\x12..admobilize.query.v1alpha1.UpdateReportRequest\x1a!.admobilize.query.v1alpha1.Report\"<\x82\xd3\xe4\x93\x02\x36\x1a\x31/v1alpha1/projects/{project=*}/reports/{report=*}:\x01*\x12\x9c\x01\n\x0bListReports\x12-.admobilize.query.v1alpha1.ListReportsRequest\x1a..admobilize.query.v1alpha1.ListReportsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v1alpha1/projects/{project=*}/reports\x12\xb4\x01\n\x0bPauseReport\x12-.admobilize.query.v1alpha1.PauseReportRequest\x1a!.admobilize.query.v1alpha1.Report\"S\x82\xd3\xe4\x93\x02M\"H/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:pause:\x01*\x12\xba\x01\n\rRestartReport\x12/.admobilize.query.v1alpha1.RestartReportRequest\x1a!.admobilize.query.v1alpha1.Report\"U\x82\xd3\xe4\x93\x02O\"J/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:restart:\x01*\x12\xb0\x01\n\x0c\x43\x61ncelReport\x12..admobilize.query.v1alpha1.CancelReportRequest\x1a!.admobilize.query.v1alpha1.Report\"M\x82\xd3\xe4\x93\x02G*B/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:\x01*\x12\xb0\x01\n\x0cGetTableData\x12..admobilize.query.v1alpha1.GetTableDataRequest\x1a/.admobilize.query.v1alpha1.GetTableDataResponse\"?\x82\xd3\xe4\x93\x02\x39\"4/v1alpha1/projects/{project=*}/tables/{table=*}/data:\x01*\x12p\n\tCreateJob\x12+.admobilize.query.v1alpha1.CreateJobRequest\x1a\x1e.admobilize.query.v1alpha1.Job\"\x16\x82\xd3\xe4\x93\x02\x10\"\x0e/v1alpha1/jobs\x12q\n\x06GetJob\x12(.admobilize.query.v1alpha1.GetJobRequest\x1a\x1e.admobilize.query.v1alpha1.Job\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/v1alpha1/{id=jobs/*}\x12\x99\x01\n\rGetJobResults\x12/.admobilize.query.v1alpha1.GetJobResultRequests\x1a\x30.admobilize.query.v1alpha1.GetDatapointsResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v1alpha1/{id=jobs/*}/results\x12\x98\x01\n\rExportResults\x12/.admobilize.query.v1alpha1.ExportResultsRequest\x1a\x30.admobilize.query.v1alpha1.ExportResultsResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1alpha1/{id=jobs/*}/exportB\x9c\x01\n\x1d\x63om.admobilize.query.v1alpha1B\x13QueryResourcesProtoP\x01Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\xa2\x02\x05\x41\x44MQY\xaa\x02\x19\x41\x64Mobilize.Query.V1Alpha1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-admobilize/query/v1alpha1/query_service.proto\x12\x19\x61\x64mobilize.query.v1alpha1\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a google/protobuf/field_mask.proto\x1a)admobilize/query/v1alpha1/resources.proto\".\n\x1b\x43reateProjectDatasetRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\"\xdc\x07\n\x0cQueryRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x32\n\x07metrics\x18\x03 \x03(\x0b\x32!.admobilize.query.v1alpha1.Metric\x12\x12\n\ndimensions\x18\x04 \x03(\t\x12\r\n\x05\x65poch\x18\x05 \x01(\t\x12\x16\n\x0ehas_comparison\x18\x06 \x01(\x08\x12\x44\n\x10\x61ggregate_result\x18\x0b \x01(\x0b\x32*.admobilize.query.v1alpha1.AggregateResult\x12\x45\n\x11query_from_result\x18( \x01(\x0b\x32*.admobilize.query.v1alpha1.QueryFromResult\x12:\n\x0b\x63lassifiers\x18\x0c \x03(\x0b\x32%.admobilize.query.v1alpha1.Classifier\x12\x0f\n\x07timeout\x18\t \x01(\r\x12\r\n\x05limit\x18\n \x01(\r\x12\x1a\n\x12\x64imensions_encoder\x18\r \x01(\x08\x12@\n\x0e\x65ncoder_params\x18* \x01(\x0b\x32(.admobilize.query.v1alpha1.EncoderParams\x12\x37\n\x08order_by\x18\x0f \x03(\x0b\x32%.admobilize.query.v1alpha1.OrderField\x12\x16\n\x0e\x66ilter_by_hour\x18\x10 \x03(\r\x12\x19\n\x11\x66ilter_by_weekday\x18\x11 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x12 \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x36\n\x0b\x63ms_metrics\x18\x13 \x03(\x0b\x32!.admobilize.query.v1alpha1.Metric\x12>\n\rcms_dimension\x18\x14 \x01(\x0b\x32\'.admobilize.query.v1alpha1.CMSDimension\x12@\n\x0e\x63ms_descriptor\x18\x1e \x01(\x0b\x32(.admobilize.query.v1alpha1.CMSDescriptor\x12.\n\nstart_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x0e \x01(\t\x12\x0c\n\x03wid\x18\xe6\x07 \x01(\t\x12\x11\n\x08previous\x18\xe7\x07 \x01(\x08\"R\n\rQueryResponse\x12\x34\n\x08\x64\x61tasets\x18\x01 \x03(\x0b\x32\".admobilize.query.v1alpha1.Dataset\x12\x0b\n\x03tid\x18\x02 \x01(\t\"$\n\x11ListTablesRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\"$\n\x12ListTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"7\n\x15GetTableSchemaRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"\x91\x01\n\x16GetTableSchemaResponse\x12\x36\n\x06schema\x18\x01 \x03(\x0b\x32&.admobilize.query.v1alpha1.SchemaField\x12\x10\n\x08num_rows\x18\x02 \x01(\x04\x12\x11\n\tnum_bytes\x18\x03 \x01(\x03\x12\x1a\n\x12last_modified_time\x18\x04 \x01(\x06\"\xba\x03\n\x10GetReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\r\n\x05\x65poch\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\t \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\n \x01(\t\x12\x12\n\nspeed_unit\x18\x0b \x01(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\x0c \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\r \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x0e\n\x06\x66ields\x18\x0e \x03(\t\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x07\x64\x65vices\x18\x08 \x03(\x0b\x32$.admobilize.query.v1alpha1.DeviceMap\x12\x13\n\x0b\x61\x64vertisers\x18\x0f \x03(\t\x12\x0e\n\x06medias\x18\x10 \x03(\t\"Z\n\x11GetReportResponse\x12\x31\n\x06status\x18\x01 \x01(\x0b\x32!.admobilize.query.v1alpha1.Status\x12\x12\n\nreport_url\x18\x02 \x01(\t\"\xdf\x01\n\x10\x43reateJobRequest\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nproject_id\x18\x03 \x01(\t\x12\x12\n\nproduct_id\x18\x04 \x01(\t\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12\x12\n\nspeed_unit\x18\x08 \x01(\t\x12\x12\n\ndevice_ids\x18\x05 \x03(\t\x12\x0b\n\x03\x63ms\x18\x06 \x01(\t\"G\n\rGetJobRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x66ields\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"I\n\x14GetJobResultRequests\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"2\n\x14\x45xportResultsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"j\n\x15GetDatapointsResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x14\n\x0cjob_complete\x18\x02 \x01(\x08\x12\x17\n\x0fnext_page_token\x18\x03 \x01(\t\x12\x12\n\ndatapoints\x18\x04 \x01(\t\"K\n\x15\x45xportResultsResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x14\n\x0cjob_complete\x18\x02 \x01(\x08\x12\x0c\n\x04urls\x18\x03 \x03(\t\"\xca\x03\n\x13GetTableDataRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06layout\x18\x03 \x01(\t\x12\x13\n\x0bmax_results\x18\x04 \x01(\r\x12\x12\n\npage_token\x18\x05 \x01(\t\x12\r\n\x05\x65poch\x18\x06 \x01(\t\x12\x35\n\x07\x64\x65vices\x18\x07 \x03(\x0b\x32$.admobilize.query.v1alpha1.DeviceMap\x12\x19\n\x11\x66ilter_by_weekday\x18\x08 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\t \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x10\n\x08group_by\x18\n \x03(\t\x12\x36\n\tfilter_by\x18\x0b \x01(\x0b\x32#.admobilize.query.v1alpha1.FilterBy\x12.\n\nstart_time\x18\x61 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x62 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x63 \x01(\t\"T\n\x14GetTableDataResponse\x12\x12\n\npage_token\x18\x02 \x01(\t\x12(\n\x04rows\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"4\n\x12ListReportsRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"I\n\x13ListReportsResponse\x12\x32\n\x07reports\x18\x01 \x03(\x0b\x32!.admobilize.query.v1alpha1.Report\"\xb3\x03\n\x13\x43reateReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\t \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\n \x01(\t\x12\x12\n\nspeed_unit\x18\x0b \x01(\t\x12\x11\n\tfrequency\x18\x0c \x01(\t\x12\x14\n\x0c\x64\x61ys_to_send\x18\r \x03(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\x0e \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x0f \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x64\x65vices\x18\x08 \x03(\t\x12\x13\n\x0b\x61\x64vertisers\x18\x10 \x03(\t\x12\x0e\n\x06medias\x18\x11 \x03(\t\"\xdc\x02\n\x13UpdateReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x0e\n\x06report\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x0c \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x03(\t\x12\x0c\n\x04type\x18\x06 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x07 \x01(\t\x12\x12\n\nspeed_unit\x18\x08 \x01(\t\x12\x11\n\tfrequency\x18\t \x01(\t\x12\x14\n\x0c\x64\x61ys_to_send\x18\n \x03(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\r \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x0e \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12,\n\x08\x65nd_time\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x12PauseReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"F\n\x14RestartReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"E\n\x13\x43\x61ncelReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"\x97\x01\n\x17GetDeviceHeatmapRequest\x12\x0e\n\x06\x64\x65vice\x18\x01 \x01(\t\x12.\n\nstart_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\t2\xb3\x15\n\x0cQueryService\x12\x91\x01\n\x14\x43reateProjectDataset\x12\x36.admobilize.query.v1alpha1.CreateProjectDatasetRequest\x1a\".admobilize.query.v1alpha1.Project\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1alpha1/projects:\x01*\x12\x9c\x01\n\x05Query\x12\'.admobilize.query.v1alpha1.QueryRequest\x1a(.admobilize.query.v1alpha1.QueryResponse\"@\x82\xd3\xe4\x93\x02:\"5/v1alpha1/projects/{project=*}/tables/{table=*}/query:\x01*\x12\x98\x01\n\nListTables\x12,.admobilize.query.v1alpha1.ListTablesRequest\x1a-.admobilize.query.v1alpha1.ListTablesResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/v1alpha1/projects/{project=*}/tables\x12\xae\x01\n\x0eGetTableSchema\x12\x30.admobilize.query.v1alpha1.GetTableSchemaRequest\x1a\x31.admobilize.query.v1alpha1.GetTableSchemaResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//v1alpha1/projects/{project=*}/tables/{table=*}\x12\xa9\x01\n\tGetReport\x12+.admobilize.query.v1alpha1.GetReportRequest\x1a,.admobilize.query.v1alpha1.GetReportResponse\"A\x82\xd3\xe4\x93\x02;\"6/v1alpha1/projects/{project=*}/tables/{table=*}/report:\x01*\x12\xa5\x01\n\x0c\x43reateReport\x12..admobilize.query.v1alpha1.CreateReportRequest\x1a!.admobilize.query.v1alpha1.Report\"B\x82\xd3\xe4\x93\x02<\"7/v1alpha1/projects/{project=*}/tables/{table=*}/reports:\x01*\x12\x9f\x01\n\x0cUpdateReport\x12..admobilize.query.v1alpha1.UpdateReportRequest\x1a!.admobilize.query.v1alpha1.Report\"<\x82\xd3\xe4\x93\x02\x36\x1a\x31/v1alpha1/projects/{project=*}/reports/{report=*}:\x01*\x12\x9c\x01\n\x0bListReports\x12-.admobilize.query.v1alpha1.ListReportsRequest\x1a..admobilize.query.v1alpha1.ListReportsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v1alpha1/projects/{project=*}/reports\x12\xb4\x01\n\x0bPauseReport\x12-.admobilize.query.v1alpha1.PauseReportRequest\x1a!.admobilize.query.v1alpha1.Report\"S\x82\xd3\xe4\x93\x02M\"H/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:pause:\x01*\x12\xba\x01\n\rRestartReport\x12/.admobilize.query.v1alpha1.RestartReportRequest\x1a!.admobilize.query.v1alpha1.Report\"U\x82\xd3\xe4\x93\x02O\"J/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:restart:\x01*\x12\xb0\x01\n\x0c\x43\x61ncelReport\x12..admobilize.query.v1alpha1.CancelReportRequest\x1a!.admobilize.query.v1alpha1.Report\"M\x82\xd3\xe4\x93\x02G*B/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:\x01*\x12\xb0\x01\n\x0cGetTableData\x12..admobilize.query.v1alpha1.GetTableDataRequest\x1a/.admobilize.query.v1alpha1.GetTableDataResponse\"?\x82\xd3\xe4\x93\x02\x39\"4/v1alpha1/projects/{project=*}/tables/{table=*}/data:\x01*\x12\x98\x01\n\x10GetDeviceHeatmap\x12\x32.admobilize.query.v1alpha1.GetDeviceHeatmapRequest\x1a\".admobilize.query.v1alpha1.Heatmap\",\x82\xd3\xe4\x93\x02&\x12$/vialpha1/devices/{device=*}/heatmap\x12p\n\tCreateJob\x12+.admobilize.query.v1alpha1.CreateJobRequest\x1a\x1e.admobilize.query.v1alpha1.Job\"\x16\x82\xd3\xe4\x93\x02\x10\"\x0e/v1alpha1/jobs\x12q\n\x06GetJob\x12(.admobilize.query.v1alpha1.GetJobRequest\x1a\x1e.admobilize.query.v1alpha1.Job\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/v1alpha1/{id=jobs/*}\x12\x99\x01\n\rGetJobResults\x12/.admobilize.query.v1alpha1.GetJobResultRequests\x1a\x30.admobilize.query.v1alpha1.GetDatapointsResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v1alpha1/{id=jobs/*}/results\x12\x98\x01\n\rExportResults\x12/.admobilize.query.v1alpha1.ExportResultsRequest\x1a\x30.admobilize.query.v1alpha1.ExportResultsResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1alpha1/{id=jobs/*}/exportB\x9c\x01\n\x1d\x63om.admobilize.query.v1alpha1B\x13QueryResourcesProtoP\x01Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\xa2\x02\x05\x41\x44MQY\xaa\x02\x19\x41\x64Mobilize.Query.V1Alpha1b\x06proto3')
 
 
 
 _CREATEPROJECTDATASETREQUEST = DESCRIPTOR.message_types_by_name['CreateProjectDatasetRequest']
 _QUERYREQUEST = DESCRIPTOR.message_types_by_name['QueryRequest']
 _QUERYRESPONSE = DESCRIPTOR.message_types_by_name['QueryResponse']
 _LISTTABLESREQUEST = DESCRIPTOR.message_types_by_name['ListTablesRequest']
@@ -43,14 +43,15 @@
 _LISTREPORTSREQUEST = DESCRIPTOR.message_types_by_name['ListReportsRequest']
 _LISTREPORTSRESPONSE = DESCRIPTOR.message_types_by_name['ListReportsResponse']
 _CREATEREPORTREQUEST = DESCRIPTOR.message_types_by_name['CreateReportRequest']
 _UPDATEREPORTREQUEST = DESCRIPTOR.message_types_by_name['UpdateReportRequest']
 _PAUSEREPORTREQUEST = DESCRIPTOR.message_types_by_name['PauseReportRequest']
 _RESTARTREPORTREQUEST = DESCRIPTOR.message_types_by_name['RestartReportRequest']
 _CANCELREPORTREQUEST = DESCRIPTOR.message_types_by_name['CancelReportRequest']
+_GETDEVICEHEATMAPREQUEST = DESCRIPTOR.message_types_by_name['GetDeviceHeatmapRequest']
 CreateProjectDatasetRequest = _reflection.GeneratedProtocolMessageType('CreateProjectDatasetRequest', (_message.Message,), {
   'DESCRIPTOR' : _CREATEPROJECTDATASETREQUEST,
   '__module__' : 'admobilize.query.v1alpha1.query_service_pb2'
   # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.CreateProjectDatasetRequest)
   })
 _sym_db.RegisterMessage(CreateProjectDatasetRequest)
 
@@ -211,14 +212,21 @@
 CancelReportRequest = _reflection.GeneratedProtocolMessageType('CancelReportRequest', (_message.Message,), {
   'DESCRIPTOR' : _CANCELREPORTREQUEST,
   '__module__' : 'admobilize.query.v1alpha1.query_service_pb2'
   # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.CancelReportRequest)
   })
 _sym_db.RegisterMessage(CancelReportRequest)
 
+GetDeviceHeatmapRequest = _reflection.GeneratedProtocolMessageType('GetDeviceHeatmapRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETDEVICEHEATMAPREQUEST,
+  '__module__' : 'admobilize.query.v1alpha1.query_service_pb2'
+  # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.GetDeviceHeatmapRequest)
+  })
+_sym_db.RegisterMessage(GetDeviceHeatmapRequest)
+
 _QUERYSERVICE = DESCRIPTOR.services_by_name['QueryService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\035com.admobilize.query.v1alpha1B\023QueryResourcesProtoP\001Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\242\002\005ADMQY\252\002\031AdMobilize.Query.V1Alpha1'
   _QUERYSERVICE.methods_by_name['CreateProjectDataset']._options = None
   _QUERYSERVICE.methods_by_name['CreateProjectDataset']._serialized_options = b'\202\323\344\223\002\027\"\022/v1alpha1/projects:\001*'
@@ -240,14 +248,16 @@
   _QUERYSERVICE.methods_by_name['PauseReport']._serialized_options = b'\202\323\344\223\002M\"H/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:pause:\001*'
   _QUERYSERVICE.methods_by_name['RestartReport']._options = None
   _QUERYSERVICE.methods_by_name['RestartReport']._serialized_options = b'\202\323\344\223\002O\"J/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:restart:\001*'
   _QUERYSERVICE.methods_by_name['CancelReport']._options = None
   _QUERYSERVICE.methods_by_name['CancelReport']._serialized_options = b'\202\323\344\223\002G*B/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:\001*'
   _QUERYSERVICE.methods_by_name['GetTableData']._options = None
   _QUERYSERVICE.methods_by_name['GetTableData']._serialized_options = b'\202\323\344\223\0029\"4/v1alpha1/projects/{project=*}/tables/{table=*}/data:\001*'
+  _QUERYSERVICE.methods_by_name['GetDeviceHeatmap']._options = None
+  _QUERYSERVICE.methods_by_name['GetDeviceHeatmap']._serialized_options = b'\202\323\344\223\002&\022$/vialpha1/devices/{device=*}/heatmap'
   _QUERYSERVICE.methods_by_name['CreateJob']._options = None
   _QUERYSERVICE.methods_by_name['CreateJob']._serialized_options = b'\202\323\344\223\002\020\"\016/v1alpha1/jobs'
   _QUERYSERVICE.methods_by_name['GetJob']._options = None
   _QUERYSERVICE.methods_by_name['GetJob']._serialized_options = b'\202\323\344\223\002\027\022\025/v1alpha1/{id=jobs/*}'
   _QUERYSERVICE.methods_by_name['GetJobResults']._options = None
   _QUERYSERVICE.methods_by_name['GetJobResults']._serialized_options = b'\202\323\344\223\002\037\022\035/v1alpha1/{id=jobs/*}/results'
   _QUERYSERVICE.methods_by_name['ExportResults']._options = None
@@ -296,10 +306,12 @@
   _UPDATEREPORTREQUEST._serialized_end=4261
   _PAUSEREPORTREQUEST._serialized_start=4263
   _PAUSEREPORTREQUEST._serialized_end=4331
   _RESTARTREPORTREQUEST._serialized_start=4333
   _RESTARTREPORTREQUEST._serialized_end=4403
   _CANCELREPORTREQUEST._serialized_start=4405
   _CANCELREPORTREQUEST._serialized_end=4474
-  _QUERYSERVICE._serialized_start=4477
-  _QUERYSERVICE._serialized_end=7061
+  _GETDEVICEHEATMAPREQUEST._serialized_start=4477
+  _GETDEVICEHEATMAPREQUEST._serialized_end=4628
+  _QUERYSERVICE._serialized_start=4631
+  _QUERYSERVICE._serialized_end=7370
 # @@protoc_insertion_point(module_scope)
```

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/common/entity_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/common/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/common/admobilize_types_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/common/admobilize_types_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/common/job_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/common/job_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py` & `admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/PKG-INFO` & `admobilizeapis-2023.7.10.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admobilizeapis
-Version: 2023.6.29.post1
+Version: 2023.7.10.post1
 Summary: Protobufs used in AdMobilize Ecosystem
 Home-page: https://www.bitbucket.org/admobilize/admobilizeapis
 Author: AdMobilize Team
 Author-email: devel@admobilize.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/SOURCES.txt` & `admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/PKG-INFO` & `admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admobilizeapis
-Version: 2023.6.29.post1
+Version: 2023.7.10.post1
 Summary: Protobufs used in AdMobilize Ecosystem
 Home-page: https://www.bitbucket.org/admobilize/admobilizeapis
 Author: AdMobilize Team
 Author-email: devel@admobilize.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `admobilizeapis-2023.6.29.post1/README.md` & `admobilizeapis-2023.7.10.post1/README.md`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.29.post1/setup.py` & `admobilizeapis-2023.7.10.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 install_requires = ["google-api-core >= 1.6.0, < 2.0.0dev", "protobuf >= 3.6.0, < 4.0"]
 
 extras_require = {"grpc": ["grpcio>=1.2.0"]}
 
 setup(
     name="admobilizeapis",
-    version='2023.06.29r1',
+    version='2023.07.10r1',
     author="AdMobilize Team",
     author_email="devel@admobilize.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
```

