# Comparing `tmp/cloudshell-cp-vcenter-5.0.4.tar.gz` & `tmp/cloudshell-cp-vcenter-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudshell-cp-vcenter-5.0.4.tar", last modified: Thu Jun 22 08:02:32 2023, max compression
+gzip compressed data, was "cloudshell-cp-vcenter-5.0.5.tar", last modified: Mon Jul 10 15:16:57 2023, max compression
```

## Comparing `cloudshell-cp-vcenter-5.0.4.tar` & `cloudshell-cp-vcenter-5.0.5.tar`

### file list

```diff
@@ -1,162 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.492528 cloudshell-cp-vcenter-5.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.420529 cloudshell-cp-vcenter-5.0.4/.tox/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.436529 cloudshell-cp-vcenter-5.0.4/.tox/build/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-22 08:02:24.000000 cloudshell-cp-vcenter-5.0.4/.tox/build/.tox-info.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-22 08:02:32.492528 cloudshell-cp-vcenter-5.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.436529 cloudshell-cp-vcenter-5.0.4/cloudshell/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.436529 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.436529 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.440528 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/actions/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/actions/vm_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/actions/vm_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.440528 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/common/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.440528 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/common/vcenter/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/common/vcenter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/common/vcenter/data_retrieve_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/common/vcenter/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.448528 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/affinity_rules_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/autoload.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/cluster_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/connectivity_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/customize_guest_os.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/delete_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.452529 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/base_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.452529 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/commands/clone_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/commands/create_custom_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/commands/create_vm_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/commands/deploy_vm_from_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/from_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/from_linked_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/from_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/from_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.456529 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/get_attribute_hints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/get_attribute_hints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/get_attribute_hints/attribute_hints.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/get_attribute_hints/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/get_attribute_hints/deployment_type_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/get_vm_web_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/power_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/reconfigure_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/refresh_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/save_restore_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/validate_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/vm_details.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/vm_uuid_by_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.464528 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/cluster_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/cluster_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/config_spec_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/custom_spec_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/datastore_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/dc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/folder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/managed_entity_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/network_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/resource_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/si_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/snapshot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/storage_pod_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/switch_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/vcenter_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/vcenter_tag_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/virtual_device_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/virtual_disk_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    15130 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/vm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/vnic_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/vsphere_api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/vsphere_sdk_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.468528 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/json_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/json_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/json_schemas/linux_custom_spec.json
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/json_schemas/windows_custom_spec.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.472528 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/DeployDataHolder.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/base_deployment_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/connectivity_action_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/custom_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/deploy_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/deployed_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/vsphere_tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/resource_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.476529 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/bytes_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/client_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/connectivity_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/cs_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/customization_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/get_vm_web_console.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/network_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/ovf_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/split_list_of_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/units_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/vm_console_link_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/vm_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.480528 cloudshell-cp-vcenter-5.0.4/cloudshell_cp_vcenter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-22 08:02:32.000000 cloudshell-cp-vcenter-5.0.4/cloudshell_cp_vcenter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-22 08:02:32.000000 cloudshell-cp-vcenter-5.0.4/cloudshell_cp_vcenter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:02:32.000000 cloudshell-cp-vcenter-5.0.4/cloudshell_cp_vcenter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-22 08:02:32.000000 cloudshell-cp-vcenter-5.0.4/cloudshell_cp_vcenter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 08:02:32.000000 cloudshell-cp-vcenter-5.0.4/cloudshell_cp_vcenter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 08:02:32.492528 cloudshell-cp-vcenter-5.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.480528 cloudshell-cp-vcenter-5.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.480528 cloudshell-cp-vcenter-5.0.4/tests/cp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.480528 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.480528 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/actions/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.484528 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/flows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/flows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.484528 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/flows/deploy_vm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/flows/deploy_vm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.484528 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/flows/deploy_vm/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/flows/deploy_vm/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/flows/deploy_vm/commands/test_clone_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/flows/test_save_restore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.488528 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_cluster_hanlder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_config_spec_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_dc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_si_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_virtual_disk_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_vm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_vnic_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_vsphere_sdk_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.488528 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/models/test_custom_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/models/test_deployed_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/test_resource_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:32.492528 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/utils/test_connectivity_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 08:02:15.000000 cloudshell-cp-vcenter-5.0.4/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.136559 cloudshell-cp-vcenter-5.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.108559 cloudshell-cp-vcenter-5.0.5/.tox/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.112559 cloudshell-cp-vcenter-5.0.5/.tox/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-10 15:16:50.000000 cloudshell-cp-vcenter-5.0.5/.tox/build/.tox-info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-10 15:16:57.136559 cloudshell-cp-vcenter-5.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.112559 cloudshell-cp-vcenter-5.0.5/cloudshell/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.112559 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.116559 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.116559 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/actions/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/actions/vm_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/actions/vm_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.116559 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.116559 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/common/vcenter/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/common/vcenter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/common/vcenter/data_retrieve_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/common/vcenter/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.120559 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/affinity_rules_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/autoload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/cluster_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/connectivity_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/customize_guest_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/delete_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.120559 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/base_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.120559 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/commands/clone_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/commands/create_custom_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/commands/create_vm_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/commands/deploy_vm_from_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/from_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/from_linked_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/from_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/from_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.120559 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/get_attribute_hints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/get_attribute_hints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/get_attribute_hints/attribute_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/get_attribute_hints/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/get_attribute_hints/deployment_type_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/get_vm_web_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/power_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/reconfigure_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/refresh_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/save_restore_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/validate_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/vm_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/vm_uuid_by_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.124559 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/cluster_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/cluster_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/config_spec_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/custom_spec_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/datastore_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/dc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/folder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/managed_entity_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/network_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/resource_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/si_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/snapshot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/storage_pod_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/switch_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/vcenter_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/vcenter_tag_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/virtual_device_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/virtual_disk_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15130 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/vm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/vnic_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/vsphere_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/vsphere_sdk_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.124559 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/json_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/json_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/json_schemas/linux_custom_spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/json_schemas/windows_custom_spec.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.128558 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/DeployDataHolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/base_deployment_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/connectivity_action_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/custom_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/deploy_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/deployed_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/vsphere_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/resource_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.128558 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/client_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/connectivity_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/cs_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/customization_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/get_vm_web_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/network_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/ovf_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/split_list_of_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/units_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/vm_console_link_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/vm_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.132559 cloudshell-cp-vcenter-5.0.5/cloudshell_cp_vcenter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-10 15:16:57.000000 cloudshell-cp-vcenter-5.0.5/cloudshell_cp_vcenter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-10 15:16:57.000000 cloudshell-cp-vcenter-5.0.5/cloudshell_cp_vcenter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:16:57.000000 cloudshell-cp-vcenter-5.0.5/cloudshell_cp_vcenter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-10 15:16:57.000000 cloudshell-cp-vcenter-5.0.5/cloudshell_cp_vcenter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 15:16:57.000000 cloudshell-cp-vcenter-5.0.5/cloudshell_cp_vcenter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:16:57.136559 cloudshell-cp-vcenter-5.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.132559 cloudshell-cp-vcenter-5.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.132559 cloudshell-cp-vcenter-5.0.5/tests/cp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.132559 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.132559 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/actions/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/actions/test_vm_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.132559 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/flows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.132559 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/flows/deploy_vm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/flows/deploy_vm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.132559 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/flows/deploy_vm/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/flows/deploy_vm/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/flows/deploy_vm/commands/test_clone_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/flows/test_save_restore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.136559 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_cluster_hanlder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_config_spec_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_dc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_si_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_virtual_disk_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_vm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_vnic_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_vsphere_sdk_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.136559 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/models/test_custom_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/models/test_deployed_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/test_resource_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:57.136559 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/utils/test_client_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/utils/test_connectivity_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/utils/test_cs_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/utils/test_units_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 15:16:44.000000 cloudshell-cp-vcenter-5.0.5/version.txt
```

### Comparing `cloudshell-cp-vcenter-5.0.4/.tox/build/.tox-info.json` & `cloudshell-cp-vcenter-5.0.5/.tox/build/.tox-info.json`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/PKG-INFO` & `cloudshell-cp-vcenter-5.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudshell-cp-vcenter
-Version: 5.0.4
+Version: 5.0.5
 Summary: This Shell enables setting up vCenter as a cloud provider in CloudShell. It supports connectivity, and adds new deployment types for apps which can be used in CloudShell sandboxes.
 Home-page: http://www.qualisystems.com/
 Author: QualiSystems
 Author-email: info@qualisystems.com
 Requires-Python: ~=3.9
 
 This Shell enables setting up vCenter as a cloud provider in CloudShell. It supports connectivity, and adds new deployment types for apps which can be used in CloudShell sandboxes.
```

### Comparing `cloudshell-cp-vcenter-5.0.4/README.md` & `cloudshell-cp-vcenter-5.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/actions/validation.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/actions/validation.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/actions/vm_details.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/actions/vm_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
+from contextlib import suppress
 from typing import TYPE_CHECKING, Union
 
 from cloudshell.cp.core.request_actions.models import (
     VmDetailsData,
     VmDetailsNetworkInterface,
     VmDetailsProperty,
 )
 
 from cloudshell.cp.vcenter.actions.vm_network import VMNetworkActions
+from cloudshell.cp.vcenter.exceptions import VMIPNotFoundException
 from cloudshell.cp.vcenter.handlers.si_handler import SiHandler
 from cloudshell.cp.vcenter.handlers.vm_handler import PowerState, VmHandler
 from cloudshell.cp.vcenter.models.deploy_app import (
     BaseVCenterDeployApp,
     VMFromImageDeployApp,
     VMFromLinkedCloneDeployApp,
     VMFromTemplateDeployApp,
@@ -22,15 +24,15 @@
     BaseVCenterDeployedApp,
     StaticVCenterDeployedApp,
     VMFromImageDeployedApp,
     VMFromLinkedCloneDeployedApp,
     VMFromTemplateDeployedApp,
     VMFromVMDeployedApp,
 )
-from cloudshell.cp.vcenter.utils.bytes_converter import format_bytes
+from cloudshell.cp.vcenter.utils.units_converter import format_bytes
 
 if TYPE_CHECKING:
     from logging import Logger
 
     from cloudshell.cp.core.cancellation_manager import CancellationContextManager
 
     from cloudshell.cp.vcenter.resource_config import VCenterResourceConfig
@@ -72,32 +74,24 @@
         self,
         vm: VmHandler,
         app_model: APP_MODEL_TYPES,
     ) -> list[VmDetailsNetworkInterface]:
         """Prepare VM Network data."""
         self._logger.info(f"Preparing VM Details network data for the {vm}")
         network_interfaces = []
-
-        if isinstance(app_model, StaticVCenterDeployedApp):
-            # try to get VM IP without waiting
-            primary_ip = self.get_vm_ip(vm, timeout=0)
-        elif vm.power_state is PowerState.ON:
-            # try to get VM IP without waiting, use IP regex if present
-            primary_ip = self.get_vm_ip(vm, ip_regex=app_model.ip_regex, timeout=0)
-        else:
-            primary_ip = None
+        primary_ip = self._get_primary_ip(app_model, vm)
 
         for vnic in vm.vnics:
             network = vnic.network
             is_predefined = network.name in self._resource_conf.reserved_networks
             vlan_id = vm.get_network_vlan_id(network)
 
             if vlan_id and (self.is_quali_network(network.name) or is_predefined):
                 vnic_ip = vnic.ipv4
-                is_primary = primary_ip == vnic_ip if vnic_ip and primary_ip else False
+                is_primary = primary_ip == vnic_ip if primary_ip else False
 
                 network_data = [
                     VmDetailsProperty(key="IP", value=vnic_ip),
                     VmDetailsProperty(key="MAC Address", value=vnic.mac_address),
                     VmDetailsProperty(key="Network Adapter", value=vnic.name),
                     VmDetailsProperty(key="Port Group Name", value=network.name),
                 ]
@@ -110,14 +104,25 @@
                     networkData=network_data,
                     privateIpAddress=vnic_ip,
                 )
                 network_interfaces.append(interface)
 
         return network_interfaces
 
+    def _get_primary_ip(self, app_model, vm) -> str | None:
+        primary_ip = None
+        with suppress(VMIPNotFoundException):
+            if isinstance(app_model, StaticVCenterDeployedApp):
+                # try to get VM IP without waiting
+                primary_ip = self.get_vm_ip(vm, timeout=0)
+            elif vm.power_state is PowerState.ON:
+                # try to get VM IP without waiting, use IP regex if present
+                primary_ip = self.get_vm_ip(vm, ip_regex=app_model.ip_regex, timeout=0)
+        return primary_ip
+
     @staticmethod
     def prepare_vm_from_vm_details(
         deploy_app: VMFromVMDeployApp | VMFromVMDeployedApp,
     ) -> list[VmDetailsProperty]:
         return [
             VmDetailsProperty(
                 key="Cloned VM Name",
```

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/actions/vm_network.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/actions/vm_network.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,19 +38,23 @@
 
     def _find_vm_ip(
         self,
         vm: VmHandler,
         skip_networks: list[NetworkHandler],
         is_ip_pass_regex: callable[[str | None], bool],
     ) -> str | None:
-        self._logger.info(f"Searching for the IPv4 address of the {vm}")
-        ip = vm.primary_ipv4
-        if not ip or not is_ip_pass_regex(ip):
-            self._logger.debug(f"{vm} doesn't have a primary IPv4 address")
+        self._logger.debug(f"Searching for the IPv4 address of the {vm}")
+        ip = None
+        primary_ip = vm.primary_ipv4
+        if is_ip_pass_regex(primary_ip):
+            ip = primary_ip
+            self._logger.debug(f"Use primary IPv4 address of the {vm}")
+        else:
             for vnic in vm.vnics:
+                self._logger.debug(f"Checking {vnic} with ip {vnic.ipv4}")
                 if vnic.network not in skip_networks and is_ip_pass_regex(vnic.ipv4):
                     self._logger.debug(f"Found IP {vnic.ipv4} on {vnic}")
                     ip = vnic.ipv4
                     break
         return ip
 
     def get_vm_ip(
@@ -67,15 +71,15 @@
 
         while True:
             with self._cancellation_manager:
                 ip = self._find_vm_ip(vm, skip_networks, is_ip_pass_regex)
             if ip:
                 break
             if datetime.now() > timeout_time:
-                raise VMIPNotFoundException("Unable to get VM IP")
+                raise VMIPNotFoundException(ip_regex)
             time.sleep(self.DEFAULT_IP_DELAY)
         return ip
 
 
 def get_ip_regex_match_func(ip_regex=None) -> callable[[str | None], bool]:
     """Get Regex Match function for the VM IP address."""
     pattern = re.compile(ip_regex) if ip_regex is not None else None
```

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/common/vcenter/data_retrieve_service.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/common/vcenter/data_retrieve_service.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/common/vcenter/event_manager.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/common/vcenter/event_manager.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/__init__.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/affinity_rules_flow.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/affinity_rules_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/autoload.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/autoload.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/cluster_usage.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/cluster_usage.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/connectivity_flow.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/connectivity_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/customize_guest_os.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/customize_guest_os.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/delete_instance.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/delete_instance.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/__init__.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/base_flow.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/base_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/commands/clone_vm.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/commands/clone_vm.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/commands/create_custom_spec.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/commands/create_custom_spec.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/commands/create_vm_folder.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/commands/create_vm_folder.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/commands/deploy_vm_from_image.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/commands/deploy_vm_from_image.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/from_image.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/from_image.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/from_linked_clone.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/from_linked_clone.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/from_template.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/from_template.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/deploy_vm/from_vm.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/deploy_vm/from_vm.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/get_attribute_hints/attribute_hints.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/get_attribute_hints/attribute_hints.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/get_attribute_hints/command.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/get_attribute_hints/command.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/get_attribute_hints/deployment_type_handlers.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/get_attribute_hints/deployment_type_handlers.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/get_vm_web_console.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/get_vm_web_console.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/power_flow.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/power_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/reconfigure_vm.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/reconfigure_vm.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/refresh_ip.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/refresh_ip.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/save_restore_app.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/save_restore_app.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/snapshots.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/snapshots.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/validate_attributes.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/validate_attributes.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/vm_details.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/vm_details.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/flows/vm_uuid_by_name.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/flows/vm_uuid_by_name.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/cluster_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/cluster_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/cluster_specs.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/cluster_specs.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/config_spec_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/config_spec_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/custom_spec_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/custom_spec_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/datastore_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/datastore_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/dc_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/dc_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/folder_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/folder_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/managed_entity_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/managed_entity_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/network_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/network_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/resource_pool.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/resource_pool.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/si_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/si_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/snapshot_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/snapshot_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/storage_pod_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/storage_pod_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/switch_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/switch_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/task.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/task.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/vcenter_path.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/vcenter_path.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/virtual_device_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/virtual_device_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/virtual_disk_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/virtual_disk_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/vm_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/vm_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/vnic_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/vnic_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/vsphere_api_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/vsphere_api_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/handlers/vsphere_sdk_handler.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/handlers/vsphere_sdk_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,15 @@
 
     def assign_tags(
         self, obj: OBJECTS_WITH_TAGS, tags: dict[str:str] | None = None
     ) -> None:
         """Get/Create tags and assign to provided vCenter object."""
         if not tags:
             tags = self._tags_manager.get_default_tags()
+        tags = _normalize_tags(tags)
 
         tag_ids = []
         for category_name, tag in tags.items():
             category_id = self._get_or_create_tag_category(name=category_name)
             tag_id = self._get_or_create_tag(name=tag, category_id=category_id)
             tag_ids.append(tag_id)
 
@@ -290,7 +291,15 @@
                 self._delete_tag(tag_id)
 
     def _get_object_id_and_type(self, obj: OBJECTS_WITH_TAGS) -> tuple[str, str]:
         object_id = obj._moId
         object_type = obj._wsdl_name
         self._logger.debug(f"Object type: {object_type}, Object ID: {object_id}")
         return object_id, object_type
+
+
+def _normalize_tags(tags: dict[str, str]) -> dict[str, str]:
+    """Normalize tags.
+
+    vCenter automatically removes whitespaces from tag names.
+    """
+    return {key: value.strip() for key, value in tags.items()}
```

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/json_schemas/linux_custom_spec.json` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/json_schemas/linux_custom_spec.json`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/json_schemas/windows_custom_spec.json` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/json_schemas/windows_custom_spec.json`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/DeployDataHolder.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/DeployDataHolder.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/base_deployment_app.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/base_deployment_app.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/connectivity_action_model.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/connectivity_action_model.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/custom_spec.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/custom_spec.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/deploy_app.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/deploy_app.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/deployed_app.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/deployed_app.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/models/vsphere_tagging.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/models/vsphere_tagging.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/resource_config.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/resource_config.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/client_helpers.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/client_helpers.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/connectivity_helpers.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/connectivity_helpers.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/customization_params.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/customization_params.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/get_vm_web_console.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/get_vm_web_console.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/ovf_tool.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/ovf_tool.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/units_converter.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/units_converter.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,31 +15,33 @@
 PREFIX_HZ = "Hz"
 PREFIX_KHZ = "kHz"
 PREFIX_MHZ = "MHz"
 PREFIX_GHZ = "GHz"
 HERTZ_PREFIX_LABELS = [PREFIX_HZ, PREFIX_KHZ, PREFIX_MHZ, PREFIX_GHZ]
 
 
-def _format_units(size, prefix, prefixes, unit_step):
+def _format_units(size: int | float, prefix: str, prefixes: list[str], unit_step: int):
     prefix_idx = prefixes.index(prefix)
 
     while size // unit_step and prefix_idx < len(prefixes) - 1:
         prefix_idx += 1
         size /= unit_step
 
-    return f"{size:.2f} {prefixes[prefix_idx]}"
+    # remove trailing zeros and decimal point
+    num = f"{size:.2f}".strip("0").strip(".") or "0"
+    return f"{num} {prefixes[prefix_idx]}"
 
 
-def format_bytes(size, prefix=PREFIX_B):
+def format_bytes(size: int | float, prefix: str = PREFIX_B):
     return _format_units(
         size=size, prefix=prefix, prefixes=BYTES_PREFIX_LABELS, unit_step=BASE_10
     )
 
 
-def format_hertz(size, prefix=PREFIX_HZ):
+def format_hertz(size: int | float, prefix: str = PREFIX_HZ):
     return _format_units(
         size=size, prefix=prefix, prefixes=HERTZ_PREFIX_LABELS, unit_step=BASE_SI
     )
 
 
 @attr.s(auto_attribs=True)
 class UsageInfo:
```

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/vm_console_link_attr.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/vm_console_link_attr.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell/cp/vcenter/utils/vm_helpers.py` & `cloudshell-cp-vcenter-5.0.5/cloudshell/cp/vcenter/utils/vm_helpers.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell_cp_vcenter.egg-info/PKG-INFO` & `cloudshell-cp-vcenter-5.0.5/cloudshell_cp_vcenter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudshell-cp-vcenter
-Version: 5.0.4
+Version: 5.0.5
 Summary: This Shell enables setting up vCenter as a cloud provider in CloudShell. It supports connectivity, and adds new deployment types for apps which can be used in CloudShell sandboxes.
 Home-page: http://www.qualisystems.com/
 Author: QualiSystems
 Author-email: info@qualisystems.com
 Requires-Python: ~=3.9
 
 This Shell enables setting up vCenter as a cloud provider in CloudShell. It supports connectivity, and adds new deployment types for apps which can be used in CloudShell sandboxes.
```

### Comparing `cloudshell-cp-vcenter-5.0.4/cloudshell_cp_vcenter.egg-info/SOURCES.txt` & `cloudshell-cp-vcenter-5.0.5/cloudshell_cp_vcenter.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 cloudshell/cp/vcenter/models/base_deployment_app.py
 cloudshell/cp/vcenter/models/connectivity_action_model.py
 cloudshell/cp/vcenter/models/custom_spec.py
 cloudshell/cp/vcenter/models/deploy_app.py
 cloudshell/cp/vcenter/models/deployed_app.py
 cloudshell/cp/vcenter/models/vsphere_tagging.py
 cloudshell/cp/vcenter/utils/__init__.py
-cloudshell/cp/vcenter/utils/bytes_converter.py
 cloudshell/cp/vcenter/utils/client_helpers.py
 cloudshell/cp/vcenter/utils/connectivity_helpers.py
 cloudshell/cp/vcenter/utils/cs_helpers.py
 cloudshell/cp/vcenter/utils/customization_params.py
 cloudshell/cp/vcenter/utils/get_vm_web_console.py
 cloudshell/cp/vcenter/utils/network_helpers.py
 cloudshell/cp/vcenter/utils/ovf_tool.py
@@ -107,14 +106,15 @@
 tests/__init__.py
 tests/conftest.py
 tests/cp/__init__.py
 tests/cp/vcenter/__init__.py
 tests/cp/vcenter/test_resource_config.py
 tests/cp/vcenter/actions/__init__.py
 tests/cp/vcenter/actions/test_validation.py
+tests/cp/vcenter/actions/test_vm_network.py
 tests/cp/vcenter/flows/__init__.py
 tests/cp/vcenter/flows/test_save_restore.py
 tests/cp/vcenter/flows/deploy_vm/__init__.py
 tests/cp/vcenter/flows/deploy_vm/commands/__init__.py
 tests/cp/vcenter/flows/deploy_vm/commands/test_clone_vm.py
 tests/cp/vcenter/handlers/__init__.py
 tests/cp/vcenter/handlers/test_cluster_hanlder.py
@@ -125,8 +125,11 @@
 tests/cp/vcenter/handlers/test_vm_handler.py
 tests/cp/vcenter/handlers/test_vnic_handler.py
 tests/cp/vcenter/handlers/test_vsphere_sdk_handler.py
 tests/cp/vcenter/models/__init__.py
 tests/cp/vcenter/models/test_custom_spec.py
 tests/cp/vcenter/models/test_deployed_app.py
 tests/cp/vcenter/utils/__init__.py
-tests/cp/vcenter/utils/test_connectivity_helpers.py
+tests/cp/vcenter/utils/test_client_helpers.py
+tests/cp/vcenter/utils/test_connectivity_helpers.py
+tests/cp/vcenter/utils/test_cs_helpers.py
+tests/cp/vcenter/utils/test_units_converter.py
```

### Comparing `cloudshell-cp-vcenter-5.0.4/setup.py` & `cloudshell-cp-vcenter-5.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/tests/conftest.py` & `cloudshell-cp-vcenter-5.0.5/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from unittest.mock import MagicMock, Mock
+from unittest.mock import MagicMock, Mock, patch
 
 import pytest
 
 from cloudshell.cp.core.cancellation_manager import CancellationContextManager
 from cloudshell.cp.core.request_actions import GetVMDetailsRequestActions
 from cloudshell.shell.core.driver_context import (
     AppContext,
@@ -22,14 +22,20 @@
 
 
 @pytest.fixture()
 def logger():
     return MagicMock()
 
 
+@pytest.fixture
+def sleepless(monkeypatch):
+    with patch("time.sleep"):
+        yield
+
+
 @pytest.fixture()
 def connectivity_context() -> ConnectivityContext:
     return ConnectivityContext(
         server_address="localhost",
         cloudshell_api_port="5000",
         quali_api_port="5001",
         admin_auth_token="token",
```

### Comparing `cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/flows/deploy_vm/commands/test_clone_vm.py` & `cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/flows/deploy_vm/commands/test_clone_vm.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/flows/test_save_restore.py` & `cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/flows/test_save_restore.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_config_spec_handler.py` & `cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_config_spec_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_dc_handler.py` & `cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_dc_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_si_handler.py` & `cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_si_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_vm_handler.py` & `cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_vm_handler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/handlers/test_vsphere_sdk_handler.py` & `cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/handlers/test_vsphere_sdk_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from unittest.mock import Mock
 
+import pytest
+
 from cloudshell.cp.vcenter.handlers.vsphere_api_handler import TagAlreadyExists
-from cloudshell.cp.vcenter.handlers.vsphere_sdk_handler import VSphereSDKHandler
+from cloudshell.cp.vcenter.handlers.vsphere_sdk_handler import (
+    VSphereSDKHandler,
+    _normalize_tags,
+)
 
 
 def test_tag_was_deleted_while_we_searching_for_it(logger):
     # - try to create a tag - get the error that it exists
     # - try to get it - get the error that we can't find it
     #   (it can be deleted in another thread or even Shell's venv)
     # - try to create the tag one more time
@@ -15,7 +20,18 @@
         ),
         get_all_category_tags=Mock(side_effect=([], "tag_id")),
         get_tag_info=Mock(side_effect=({"name": "tag name", "id": "tag_id"},)),
     )
 
     handler = VSphereSDKHandler(client, None, logger)
     assert handler._get_or_create_tag("tag_name", "category_id") == "tag_id"
+
+
+@pytest.mark.parametrize(
+    ("tags", "expected"),
+    [
+        ({"tag1": "value1"}, {"tag1": "value1"}),
+        ({"tag1": " value1 "}, {"tag1": "value1"}),
+    ],
+)
+def test__normalize_tags(tags, expected):
+    assert _normalize_tags(tags) == expected
```

### Comparing `cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/models/test_custom_spec.py` & `cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/models/test_custom_spec.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/models/test_deployed_app.py` & `cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/models/test_deployed_app.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/test_resource_config.py` & `cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/test_resource_config.py`

 * *Files identical despite different names*

### Comparing `cloudshell-cp-vcenter-5.0.4/tests/cp/vcenter/utils/test_connectivity_helpers.py` & `cloudshell-cp-vcenter-5.0.5/tests/cp/vcenter/utils/test_connectivity_helpers.py`

 * *Files identical despite different names*

