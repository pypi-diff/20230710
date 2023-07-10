# Comparing `tmp/auterion-cli-1.2.0.tar.gz` & `tmp/auterion-cli-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auterion-cli-1.2.0.tar", last modified: Fri Jul  7 12:10:11 2023, max compression
+gzip compressed data, was "auterion-cli-1.2.1.tar", last modified: Mon Jul 10 07:53:08 2023, max compression
```

## Comparing `auterion-cli-1.2.0.tar` & `auterion-cli-1.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/auterion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/auterioncli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/auterioncli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/auterioncli/commands/app_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/auterioncli/commands/app_sdk/app-yml-spec/
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-07 12:10:04.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-07-07 12:10:04.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/app_build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/app_init_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/app_install_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/slimify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8807 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/container_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/device_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/info_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/report_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3690 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/meta_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:08.784307 auterion-cli-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-10 07:53:08.784307 auterion-cli-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:08.780306 auterion-cli-1.2.1/auterion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:08.780306 auterion-cli-1.2.1/auterioncli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:08.780306 auterion-cli-1.2.1/auterioncli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:08.784307 auterion-cli-1.2.1/auterioncli/commands/app_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:08.784307 auterion-cli-1.2.1/auterioncli/commands/app_sdk/app-yml-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-10 07:53:00.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-07-10 07:53:00.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/app_build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/app_init_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/app_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/slimify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8807 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/container_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/device_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/info_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/report_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3690 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/meta_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:53:08.784307 auterion-cli-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/setup.py
```

### Comparing `auterion-cli-1.2.0/README.md` & `auterion-cli-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterion_cli.egg-info/SOURCES.txt` & `auterion-cli-1.2.1/auterion_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/commands/app_command.py` & `auterion-cli-1.2.1/auterioncli/commands/app_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 
         disable_parser = command_subparsers.add_parser('disable', help='Disable an app')
         disable_parser.add_argument('app_name', help='The name of the app to disable')
 
         status_parser = command_subparsers.add_parser('status', help='Get status from an app')
         status_parser.add_argument('app_name', help='The name of the app to get status from')
 
+        version_parser = command_subparsers.add_parser('version', help='Get version from an app')
+        version_parser.add_argument('app_name', help='The name of the app to get version from')
+
         for name, command in self._subcommand_modules.items():
             parser = command_subparsers.add_parser(name, help=command.help())
             command.setup_parser(parser)
 
     def needs_device(self, args):
         command = args.app_command
         if command in self._subcommand_modules:
@@ -162,14 +165,18 @@
         data = requests.post(f'{self._apps_api_endpoint}/apps/{args.app_name}/disable')
         self._print_app_result(data, args.app_name, "disabled")
 
     def status(self, args):
         data = requests.get(f'{self._apps_api_endpoint}/apps/{args.app_name}/status')
         self._print_app_result(data, args.app_name, "status")
 
+    def version(self, args):
+        result = self._get_app(args.app_name)
+        print(result.get('version', 'unknown'))
+
     def _get_app(self, app):
         data = requests.get(f'{self._apps_api_endpoint}/apps/{app}')
         try:
             body = data.json()
         except:
             body = {}
         if data:
```

### Comparing `auterion-cli-1.2.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json` & `auterion-cli-1.2.1/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json` & `auterion-cli-1.2.1/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/commands/app_sdk/app_build_command.py` & `auterion-cli-1.2.1/auterioncli/commands/app_sdk/app_build_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/commands/app_sdk/app_init_command.py` & `auterion-cli-1.2.1/auterioncli/commands/app_sdk/app_init_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/commands/app_sdk/app_install_command.py` & `auterion-cli-1.2.1/auterioncli/commands/app_sdk/app_install_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/commands/app_sdk/environment.py` & `auterion-cli-1.2.1/auterioncli/commands/app_sdk/environment.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/commands/app_sdk/slimify.py` & `auterion-cli-1.2.1/auterioncli/commands/app_sdk/slimify.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/commands/app_sdk/update.py` & `auterion-cli-1.2.1/auterioncli/commands/app_sdk/update.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/commands/container_command.py` & `auterion-cli-1.2.1/auterioncli/commands/container_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/commands/device_command.py` & `auterion-cli-1.2.1/auterioncli/commands/device_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,19 +125,19 @@
 
     def select(self, args):
         devices = _find_devices([args.ip] if args.ip else _get_default_candidates(), 12)
         serial = args.serial
 
         if serial not in devices:
             error(f"Device with serial {serial} not reachable. \n"
-                  f"Use \'devices discover\' command to find reachable devices.")
+                  f"Use \'device discover\' command to find reachable devices.")
 
         if args.ip is not None and args.ip not in devices[serial]['addresses']:
             error(f"Device with serial {serial} reachable, but not on {args.ip}. \n"
-                  f"Use \'devices discover\' command to find reachable devices.")
+                  f"Use \'device discover\' command to find reachable devices.")
 
         address = args.ip if args.ip is not None else next(iter(devices[serial]['addresses']))
 
         self._config["persistent"]["selected_serial"] = serial
         self._config["persistent"]["selected_address"] = address
 
         print(f"Selected device with ID {serial} on address {address}")
```

### Comparing `auterion-cli-1.2.0/auterioncli/commands/info_command.py` & `auterion-cli-1.2.1/auterioncli/commands/info_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/commands/report_command.py` & `auterion-cli-1.2.1/auterioncli/commands/report_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/commands/utils.py` & `auterion-cli-1.2.1/auterioncli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/main.py` & `auterion-cli-1.2.1/auterioncli/main.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/auterioncli/meta_util.py` & `auterion-cli-1.2.1/auterioncli/meta_util.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.0/setup.py` & `auterion-cli-1.2.1/setup.py`

 * *Files identical despite different names*

