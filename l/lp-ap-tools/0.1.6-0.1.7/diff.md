# Comparing `tmp/lp_ap_tools-0.1.6.tar.gz` & `tmp/lp_ap_tools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lp_ap_tools-0.1.6.tar", last modified: Fri Jun 16 01:01:15 2023, max compression
+gzip compressed data, was "lp_ap_tools-0.1.7.tar", last modified: Mon Jul 10 00:45:26 2023, max compression
```

## Comparing `lp_ap_tools-0.1.6.tar` & `lp_ap_tools-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-06-16 01:01:15.961594 lp_ap_tools-0.1.6/
--rw-r--r--   0 eller      (501) staff       (20)      759 2023-06-16 01:01:15.961420 lp_ap_tools-0.1.6/PKG-INFO
--rw-r--r--   0 eller      (501) staff       (20)      339 2023-05-30 22:31:42.000000 lp_ap_tools-0.1.6/README.md
-drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-06-16 01:01:15.959867 lp_ap_tools-0.1.6/lp_ap_tools/
--rw-r--r--   0 eller      (501) staff       (20)       15 2023-05-29 02:44:23.000000 lp_ap_tools-0.1.6/lp_ap_tools/__init__.py
--rw-r--r--   0 eller      (501) staff       (20)    10711 2023-06-16 00:58:23.000000 lp_ap_tools-0.1.6/lp_ap_tools/lp_ap_tools.py
-drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-06-16 01:01:15.960667 lp_ap_tools-0.1.6/lp_ap_tools.egg-info/
--rw-r--r--   0 eller      (501) staff       (20)      759 2023-06-16 01:01:15.000000 lp_ap_tools-0.1.6/lp_ap_tools.egg-info/PKG-INFO
--rw-r--r--   0 eller      (501) staff       (20)      287 2023-06-16 01:01:15.000000 lp_ap_tools-0.1.6/lp_ap_tools.egg-info/SOURCES.txt
--rw-r--r--   0 eller      (501) staff       (20)        1 2023-06-16 01:01:15.000000 lp_ap_tools-0.1.6/lp_ap_tools.egg-info/dependency_links.txt
--rw-r--r--   0 eller      (501) staff       (20)       30 2023-06-16 01:01:15.000000 lp_ap_tools-0.1.6/lp_ap_tools.egg-info/requires.txt
--rw-r--r--   0 eller      (501) staff       (20)       18 2023-06-16 01:01:15.000000 lp_ap_tools-0.1.6/lp_ap_tools.egg-info/top_level.txt
--rw-r--r--   0 eller      (501) staff       (20)       38 2023-06-16 01:01:15.961645 lp_ap_tools-0.1.6/setup.cfg
--rw-r--r--   0 eller      (501) staff       (20)      801 2023-06-16 00:59:03.000000 lp_ap_tools-0.1.6/setup.py
-drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-06-16 01:01:15.960902 lp_ap_tools-0.1.6/tests/
--rw-r--r--   0 eller      (501) staff       (20)        0 2023-05-29 02:51:18.000000 lp_ap_tools-0.1.6/tests/__init__.py
--rw-r--r--   0 eller      (501) staff       (20)      104 2023-05-29 03:34:42.000000 lp_ap_tools-0.1.6/tests/lp_ap_tools_test.py
+drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-07-10 00:45:26.555425 lp_ap_tools-0.1.7/
+-rw-r--r--   0 eller      (501) staff       (20)      759 2023-07-10 00:45:26.555242 lp_ap_tools-0.1.7/PKG-INFO
+-rw-r--r--   0 eller      (501) staff       (20)      339 2023-05-30 22:31:42.000000 lp_ap_tools-0.1.7/README.md
+drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-07-10 00:45:26.553269 lp_ap_tools-0.1.7/lp_ap_tools/
+-rw-r--r--   0 eller      (501) staff       (20)       15 2023-05-29 02:44:23.000000 lp_ap_tools-0.1.7/lp_ap_tools/__init__.py
+-rw-r--r--   0 eller      (501) staff       (20)    10768 2023-07-10 00:42:09.000000 lp_ap_tools-0.1.7/lp_ap_tools/lp_ap_tools.py
+drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-07-10 00:45:26.554326 lp_ap_tools-0.1.7/lp_ap_tools.egg-info/
+-rw-r--r--   0 eller      (501) staff       (20)      759 2023-07-10 00:45:26.000000 lp_ap_tools-0.1.7/lp_ap_tools.egg-info/PKG-INFO
+-rw-r--r--   0 eller      (501) staff       (20)      287 2023-07-10 00:45:26.000000 lp_ap_tools-0.1.7/lp_ap_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 eller      (501) staff       (20)        1 2023-07-10 00:45:26.000000 lp_ap_tools-0.1.7/lp_ap_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 eller      (501) staff       (20)       30 2023-07-10 00:45:26.000000 lp_ap_tools-0.1.7/lp_ap_tools.egg-info/requires.txt
+-rw-r--r--   0 eller      (501) staff       (20)       18 2023-07-10 00:45:26.000000 lp_ap_tools-0.1.7/lp_ap_tools.egg-info/top_level.txt
+-rw-r--r--   0 eller      (501) staff       (20)       38 2023-07-10 00:45:26.555472 lp_ap_tools-0.1.7/setup.cfg
+-rw-r--r--   0 eller      (501) staff       (20)      801 2023-07-10 00:44:01.000000 lp_ap_tools-0.1.7/setup.py
+drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-07-10 00:45:26.554755 lp_ap_tools-0.1.7/tests/
+-rw-r--r--   0 eller      (501) staff       (20)        0 2023-05-29 02:51:18.000000 lp_ap_tools-0.1.7/tests/__init__.py
+-rw-r--r--   0 eller      (501) staff       (20)      104 2023-05-29 03:34:42.000000 lp_ap_tools-0.1.7/tests/lp_ap_tools_test.py
```

### Comparing `lp_ap_tools-0.1.6/PKG-INFO` & `lp_ap_tools-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lp_ap_tools
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python decorator for creating ActionProvider RO-crates within a Globus flow
 Home-page: https://github.com/GusEllerm/lp_tools.git
 Author: Augustus Ellerm
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lp_ap_tools-0.1.6/lp_ap_tools/lp_ap_tools.py` & `lp_ap_tools-0.1.7/lp_ap_tools/lp_ap_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # possible schema for container description in ROcrate
 # https://openschemas.github.io/specifications/ContainerRecipe/
 
 # LP fields to be included within AP input_schema
 # TODO: Build schema, and provide flexibility in chosen fields. 
 LP_FIELDS = {
-   'management_ep_id': (str, Field(..., title="Some required input", description="A useful description")),
+   'orchestration_node': (str, Field(..., title="Orchestration Node UUID", description="Collects LP artefacts and produces the final Orchestration crate artefact")),
 }
 
 # returns a new model with the union of the original class 
 # and the LP fields
 def add_lp_params(origin_class: BaseModel):
    original_fields = {name: (field.outer_type_, field.field_info) for name, field in origin_class.__fields__.items()}
    return create_model(type(origin_class).__name__, **{**original_fields, **LP_FIELDS})
@@ -148,30 +148,30 @@
 def create_method(crate: ROCrate,
                   dir_struct: dict):
    method_files = crate.add_tree(dir_struct['method'])
    return method_files
 
 def transfer_crate(ap_auth: AuthState,
                    crate_path: str,
-                   management_ep_id: str,
+                   orchestration_node: str,
                    ap_status: ActionStatus,
                    ap_apbt: ActionProviderBlueprint):
    
    # Get local running globus connect personal endpoint
    local_gcp = LocalGlobusConnectPersonal()
    # Get dependent token for globus transfer API
    dependent_tokens = ap_auth.auth_client.oauth2_get_dependent_tokens(ap_auth.bearer_token)
    transfer_token = dependent_tokens.by_resource_server['transfer.api.globus.org']['access_token']
    # Transfer crate to management endpoint
    transfer_client = TransferClient(authorizer=globus_sdk.AccessTokenAuthorizer(transfer_token))
    data = TransferData(transfer_client,
                        source_endpoint=local_gcp.endpoint_id,
-                       destination_endpoint=management_ep_id,
+                       destination_endpoint=orchestration_node,
                        label=f"{ap_apbt.name}_AP crate transfer: crate_{ap_status.action_id}")
-   data.add_item(crate_path, f"CRATE_DIR/crate_{ap_status.action_id}", recursive=True)
+   data.add_item(crate_path, f"crate_{ap_status.action_id}", recursive=True)
    transfer_result = transfer_client.submit_transfer(data)
    print(f"Transfering crate for job {ap_status.action_id}. Transfer Job ID: {transfer_result['task_id']}")
 
 # -----------------------------------------------
 # ------------ Primary decorator  ---------------
 # -----------------------------------------------
 
@@ -238,13 +238,13 @@
          action["total_time"] = total_time
 
          # Write RO-Crate to disk
          crate.write_crate(os.path.join(dir_struct["crates"], f"crate_{ap_status.action_id}"))
          # # Transfer crate to management endpoint
          transfer_crate(ap_auth=ap_auth,
                         crate_path=os.path.join(dir_struct["crates"], crate_name), 
-                        management_ep_id=ap_request.body["management_ep_id"],
+                        orchestration_node=ap_request.body["orchestration_node"],
                         ap_status=ap_status,
                         ap_apbt=ap_apbt)
          return computation
       return create_ROcrate
     return middle
```

### Comparing `lp_ap_tools-0.1.6/lp_ap_tools.egg-info/PKG-INFO` & `lp_ap_tools-0.1.7/lp_ap_tools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lp-ap-tools
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python decorator for creating ActionProvider RO-crates within a Globus flow
 Home-page: https://github.com/GusEllerm/lp_tools.git
 Author: Augustus Ellerm
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lp_ap_tools-0.1.6/setup.py` & `lp_ap_tools-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name='lp_ap_tools',
     packages=find_packages(),
-    version='0.1.6',
+    version='0.1.7',
     description='A python decorator for creating ActionProvider RO-crates within a Globus flow',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Augustus Ellerm',
     license='MIT',
     install_requires=['rocrate', 
                       'pydantic',
```

