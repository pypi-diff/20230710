# Comparing `tmp/vastai-0.1.5.tar.gz` & `tmp/vastai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastai-0.1.5.tar", last modified: Mon Jul 10 19:30:51 2023, max compression
+gzip compressed data, was "vastai-0.1.6.tar", last modified: Mon Jul 10 19:33:16 2023, max compression
```

## Comparing `vastai-0.1.5.tar` & `vastai-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-07-10 19:30:51.079120 vastai-0.1.5/
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1064 2023-06-15 20:54:21.000000 vastai-0.1.5/LICENSE.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 20:55:37.000000 vastai-0.1.5/MANIFEST.in
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33954 2023-07-10 19:30:51.079120 vastai-0.1.5/PKG-INFO
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33343 2023-06-15 21:40:11.000000 vastai-0.1.5/README.md
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      641 2023-07-10 19:30:30.000000 vastai-0.1.5/pyproject.toml
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-07-10 19:30:51.079120 vastai-0.1.5/setup.cfg
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1054 2023-07-10 19:30:36.000000 vastai-0.1.5/setup.py
-drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-07-10 19:30:51.075121 vastai-0.1.5/vastai/
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:02:15.000000 vastai-0.1.5/vastai/__init__.py
--rwxrwxr-x   0 jcannell  (1000) jcannell  (1000)    76750 2023-07-06 22:53:54.000000 vastai-0.1.5/vastai/vast.py
-drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-07-10 19:30:51.079120 vastai-0.1.5/vastai.egg-info/
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33954 2023-07-10 19:30:51.000000 vastai-0.1.5/vastai.egg-info/PKG-INFO
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      283 2023-07-10 19:30:51.000000 vastai-0.1.5/vastai.egg-info/SOURCES.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        1 2023-07-10 19:30:51.000000 vastai-0.1.5/vastai.egg-info/dependency_links.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       44 2023-07-10 19:30:51.000000 vastai-0.1.5/vastai.egg-info/entry_points.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        9 2023-07-10 19:30:51.000000 vastai-0.1.5/vastai.egg-info/requires.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        7 2023-07-10 19:30:51.000000 vastai-0.1.5/vastai.egg-info/top_level.txt
+drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-07-10 19:33:16.778125 vastai-0.1.6/
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1064 2023-06-15 20:54:21.000000 vastai-0.1.6/LICENSE.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 20:55:37.000000 vastai-0.1.6/MANIFEST.in
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33954 2023-07-10 19:33:16.778125 vastai-0.1.6/PKG-INFO
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33343 2023-06-15 21:40:11.000000 vastai-0.1.6/README.md
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      641 2023-07-10 19:33:04.000000 vastai-0.1.6/pyproject.toml
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-07-10 19:33:16.778125 vastai-0.1.6/setup.cfg
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1054 2023-07-10 19:33:05.000000 vastai-0.1.6/setup.py
+drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-07-10 19:33:16.778125 vastai-0.1.6/vastai/
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:02:15.000000 vastai-0.1.6/vastai/__init__.py
+-rwxrwxr-x   0 jcannell  (1000) jcannell  (1000)    77955 2023-07-10 19:28:12.000000 vastai-0.1.6/vastai/vast.py
+drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-07-10 19:33:16.778125 vastai-0.1.6/vastai.egg-info/
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33954 2023-07-10 19:33:16.000000 vastai-0.1.6/vastai.egg-info/PKG-INFO
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      283 2023-07-10 19:33:16.000000 vastai-0.1.6/vastai.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        1 2023-07-10 19:33:16.000000 vastai-0.1.6/vastai.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       44 2023-07-10 19:33:16.000000 vastai-0.1.6/vastai.egg-info/entry_points.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        9 2023-07-10 19:33:16.000000 vastai-0.1.6/vastai.egg-info/requires.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        7 2023-07-10 19:33:16.000000 vastai-0.1.6/vastai.egg-info/top_level.txt
```

### Comparing `vastai-0.1.5/LICENSE.txt` & `vastai-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vastai-0.1.5/PKG-INFO` & `vastai-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastai
-Version: 0.1.5
+Version: 0.1.6
 Summary: Vast.ai Python CLI
 Home-page: https://github.com/vast-ai/vast-python
 Author: Vast.ai
 Author-email: "vast.ai" <support@vast.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/vast-ai/vast-python
 Project-URL: Bug Tracker, https://github.com/vast-ai/vast-python/issues
```

### Comparing `vastai-0.1.5/README.md` & `vastai-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `vastai-0.1.5/pyproject.toml` & `vastai-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vastai"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="vast.ai", email="support@vast.ai" },
 ]
 description = "Vast.ai Python CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vastai-0.1.5/setup.py` & `vastai-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='vastai',
-    version='0.1.5',  # choose your own version
+    version='0.1.6',  # choose your own version
     packages=['vastai'],
     entry_points={
         'console_scripts': [
             'vastai = vastai.vast:main',  # you need a main function in your vast.py file
         ],
     },
     description='Vast.ai Python CLI',
```

### Comparing `vastai-0.1.5/vastai/vast.py` & `vastai-0.1.6/vastai/vast.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,15 +247,15 @@
     ("cuda_max_good", "CUDA", "{:0.1f}", None, True),
     ("num_gpus", "N", "{}x", None, False),
     ("gpu_name", "Model", "{}", None, True),
     ("pcie_bw", "PCIE", "{:0.1f}", None, True),
     ("cpu_cores_effective", "vCPUs", "{:0.1f}", None, True),
     ("cpu_ram", "RAM", "{:0.1f}", lambda x: x / 1000, False),
     ("disk_space", "Disk", "{:.0f}", None, True),
-    ("dph_total", "$/hr", "{:0.4f}", None, True),
+    ("discounted_dph_total", "$/hr", "{:0.4f}", None, True),
     ("dlperf", "DLP", "{:0.1f}", None, True),
     ("dlperf_per_dphtotal", "DLP/$", "{:0.2f}", None, True),
     ("driver_version", "NV Driver", "{}", None, True),
     ("inet_up", "Net_up", "{:0.1f}", None, True),
     ("inet_down", "Net_down", "{:0.1f}", None, True),
     ("reliability2", "R", "{:0.1f}", lambda x: x * 100, True),
     ("duration", "Max_Days", "{:0.1f}", lambda x: x / (24.0 * 60.0 * 60.0), True),
@@ -405,15 +405,15 @@
         "dph": "dph_total",
         "flops_usd": "flops_per_dphtotal",
     };
 
     field_multiplier = {
         "cpu_ram": 1000,
         "gpu_ram": 1000,
-        "duration": 1.0 / (24.0 * 60.0 * 60.0),
+        "duration": 24.0 * 60.0 * 60.0,
     }
 
     fields = {
         "bw_nvlink",
         "compute_cap",
         "cpu_cores",
         "cpu_cores_effective",
@@ -488,19 +488,27 @@
             if field in v:
                 del v[field]
             if field in res:
                 del res[field]
             continue
 
         if field in field_multiplier:
-            value = str(float(value) * field_multiplier[field]);
-        if isinstance(value, str):
-            v[op_name] = value.replace('_', ' ')
+            value = float(value) * field_multiplier[field]
+
+            if isinstance(value, str):
+                v[op_name] = value.replace('_', ' ')
+            else:
+                v[op_name] = value
+
         else:
-            v[op_name] = [v.replace('_', ' ') for v in value]
+            if isinstance(value, str):
+                v[op_name] = value.replace('_', ' ')
+            else:
+                v[op_name] = [v.replace('_', ' ') for v in value]
+
         res[field] = v;
 
     #print(res)
     return res
 
 
 def display_table(rows: list, fields: typing.Tuple) -> None:
@@ -1124,17 +1132,18 @@
     else:
         print(r.text);
         print("failed with error {r.status_code}".format(**locals()));
 
 
 
 @parser.command(
-    argument("-t", "--type", default="on-demand", help="Show 'bid'(interruptible) or 'on-demand' offers. default: on-demand"),
+    argument("-t", "--type", default="on-demand", help="Show 'on-demand', 'reserved', or 'bid'(interruptible) pricing. default: on-demand"),
     argument("-i", "--interruptible", dest="type", const="bid", action="store_const", help="Alias for --type=bid"),
     argument("-b", "--bid", dest="type", const="bid", action="store_const", help="Alias for --type=bid"),
+    argument("-r", "--reserved", dest="type", const="reserved", action="store_const", help="Alias for --type=reserved"),
     argument("-d", "--on-demand", dest="type", const="on-demand", action="store_const", help="Alias for --type=on-demand"),
     argument("-n", "--no-default", action="store_true", help="Disable default query"),
     argument("--disable-bundling", action="store_true", help="Show identical offers. This request is more heavily rate limited."),
     argument("--storage", type=float, default=5.0, help="Amount of storage to use for pricing, in GiB. default=5.0GiB"),
     argument("-o", "--order", type=str, help="Comma-separated list of fields to sort on. postfix field with - to sort desc. ex: -o 'num_gpus,total_flops-'.  default='score-'", default='score-'),
     argument("query", help="Query to search for. default: 'external=false rentable=true verified=true', pass -n to ignore default", nargs="*", default=None),
     usage="./vast search offers [--help] [--api-key API_KEY] [--raw] <query>",
@@ -1247,15 +1256,15 @@
         if query["type"] == 'interruptible':
             query["type"] = 'bid'
         if args.disable_bundling:
             query["disable_bundling"] = True
     except ValueError as e:
         print("Error: ", e)
         return 1
-
+    
     url = apiurl(args, "/bundles", {"q": query})
     r = requests.get(url);
     r.raise_for_status()
     rows = r.json()["offers"]
     # TODO: add this post-query geolocation filter to the database call rather than handling it locally
     if 'geolocation' in query:
         geo_filter = query['geolocation']
@@ -1277,54 +1286,90 @@
     if args.raw:
         print(json.dumps(rows, indent=1, sort_keys=True))
     else:
         display_table(rows, displayable_fields)
 
 
 @parser.command(
-    argument("--id", help="id of instance", type=int),
-    usage="./vast ssh-url",
+    argument("id", help="id of instance", type=int),
+    usage="./vast ssh-url ID",
     help="ssh url helper",
 )
 def ssh_url(args):
     """
 
     :param argparse.Namespace args: should supply all the command-line options
     :rtype:
     """
     return _ssh_url(args, "ssh://")
 
 
 @parser.command(
-    argument("--id", help="id of instance", type=int),
-    usage="./vast scp-url",
+    argument("id",   help="id", type=int),
+    usage="./vast scp-url ID",
     help="scp url helper",
 )
 def scp_url(args):
     """
 
     :param argparse.Namespace args: should supply all the command-line options
     :rtype:
     """
     return _ssh_url(args, "scp://")
 
 
 def _ssh_url(args, protocol):
-    req_url = apiurl(args, "/instances", {"owner": "me"});
-    r = requests.get(req_url);
-    r.raise_for_status()
-    rows = r.json()["instances"]
-    if args.id:
-        instance, = [r for r in rows if r['id'] == args.id]
-    elif len(rows) > 1:
-        print("Found multiple running instances")
-        return 1
-    else:
-        instance, = rows
-    print(f'{protocol}root@{instance["ssh_host"]}:{instance["ssh_port"]}')
+
+    json_object = None
+
+    # Opening JSON file
+    try:
+        with open(f"ssh_{args.id}.json", 'r') as openfile:
+            json_object = json.load(openfile)
+    except:
+        pass
+
+    port      = None
+    ipaddr    = None
+
+    if json_object is not None:
+        ipaddr = json_object["ipaddr"]
+        port   = json_object["port"]
+
+    if ipaddr is None:
+        req_url = apiurl(args, "/instances", {"owner": "me"});
+        r = requests.get(req_url);
+        r.raise_for_status()
+        rows = r.json()["instances"]
+        if args.id:
+            instance, = [r for r in rows if r['id'] == args.id]
+        elif len(rows) > 1:
+            print("Found multiple running instances")
+            return 1
+        else:
+            instance, = rows
+
+        ports     = instance.get("ports",{})
+        port_22d  = ports.get("22/tcp",None)
+        if (port_22d is not None):
+            ipaddr = instance["public_ipaddr"]
+            port   = port_22d[0]["HostPort"]
+        else:        
+            ipaddr = instance["ssh_host"]
+            port   = int(instance["ssh_port"])+1
+
+    print(f'{protocol}root@{ipaddr}:{port}')
+
+   
+    # Writing to sample.json
+    try:
+        with open(f"ssh_{args.id}.json", "w") as outfile:
+            json.dump({"ipaddr":ipaddr, "port":port}, outfile)
+    except:
+        pass
 
 
 @parser.command(
     argument("-q", "--quiet", action="store_true", help="only display numeric ids"),
     argument("-s", "--start_date", help="start date and time for report. Many formats accepted", type=str),
     argument("-e", "--end_date", help="end date and time for report. Many formats accepted ", type=str),
     argument("-m", "--machine_id", help="Machine id (optional)", type=int),
```

### Comparing `vastai-0.1.5/vastai.egg-info/PKG-INFO` & `vastai-0.1.6/vastai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastai
-Version: 0.1.5
+Version: 0.1.6
 Summary: Vast.ai Python CLI
 Home-page: https://github.com/vast-ai/vast-python
 Author: Vast.ai
 Author-email: "vast.ai" <support@vast.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/vast-ai/vast-python
 Project-URL: Bug Tracker, https://github.com/vast-ai/vast-python/issues
```

