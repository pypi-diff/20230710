# Comparing `tmp/chainbench-0.3.0.tar.gz` & `tmp/chainbench-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.3.0.tar", max compression
+gzip compressed data, was "chainbench-0.3.1.tar", max compression
```

## Comparing `chainbench-0.3.0.tar` & `chainbench-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-05-31 16:05:21.018361 chainbench-0.3.0/LICENSE
--rw-r--r--   0        0        0     7715 2023-05-31 16:05:21.018361 chainbench-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/__main__.py
--rw-r--r--   0        0        0     7638 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/main.py
--rw-r--r--   0        0        0        0 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     3597 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/avalanche/general.py
--rw-r--r--   0        0        0     2693 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/bsc/general.py
--rw-r--r--   0        0        0     2912 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/ethereum/general.py
--rw-r--r--   0        0        0      361 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/evm/get_logs.py
--rw-r--r--   0        0        0      803 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/evm/heavy.py
--rw-r--r--   0        0        0     1645 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/evm/light.py
--rw-r--r--   0        0        0     1838 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/oasis/general.py
--rw-r--r--   0        0        0     2845 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/polygon/general.py
--rw-r--r--   0        0        0      168 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     4705 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/test_data/base.py
--rw-r--r--   0        0        0      166 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/test_data/dummy.py
--rw-r--r--   0        0        0     2979 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/test_data/evm.py
--rw-r--r--   0        0        0        0 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/user/__init__.py
--rw-r--r--   0        0        0     3511 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/user/base.py
--rw-r--r--   0        0        0     1225 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/user/evm.py
--rw-r--r--   0        0        0        0 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/util/__init__.py
--rw-r--r--   0        0        0     3840 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/util/cli.py
--rw-r--r--   0        0        0     2512 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/util/event.py
--rw-r--r--   0        0        0     3463 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/util/notify.py
--rw-r--r--   0        0        0      320 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/util/rpc.py
--rw-r--r--   0        0        0      438 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/util/timer.py
--rw-r--r--   0        0        0      772 2023-05-31 16:05:21.022361 chainbench-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8228 1970-01-01 00:00:00.000000 chainbench-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-10 07:23:02.669200 chainbench-0.3.1/LICENSE
+-rw-r--r--   0        0        0     8428 2023-07-10 07:23:02.669200 chainbench-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/__main__.py
+-rw-r--r--   0        0        0     8401 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     3597 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/avalanche/general.py
+-rw-r--r--   0        0        0     2693 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/bsc/general.py
+-rw-r--r--   0        0        0     2912 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/ethereum/general.py
+-rw-r--r--   0        0        0      361 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/evm/get_logs.py
+-rw-r--r--   0        0        0     4158 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/evm/heavy.py
+-rw-r--r--   0        0        0     1645 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/evm/light.py
+-rw-r--r--   0        0        0     1838 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/oasis/general.py
+-rw-r--r--   0        0        0     2845 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/polygon/general.py
+-rw-r--r--   0        0        0      168 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     4705 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/test_data/base.py
+-rw-r--r--   0        0        0      166 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/test_data/dummy.py
+-rw-r--r--   0        0        0     2979 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0        0 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     3511 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/user/base.py
+-rw-r--r--   0        0        0     2740 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/user/evm.py
+-rw-r--r--   0        0        0        0 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     3907 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/cli.py
+-rw-r--r--   0        0        0     2511 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/event.py
+-rw-r--r--   0        0        0     3436 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/monitor.py
+-rw-r--r--   0        0        0     3463 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/notify.py
+-rw-r--r--   0        0        0      279 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/rpc.py
+-rw-r--r--   0        0        0      438 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/timer.py
+-rw-r--r--   0        0        0      771 2023-07-10 07:23:02.673200 chainbench-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8941 1970-01-01 00:00:00.000000 chainbench-0.3.1/PKG-INFO
```

### Comparing `chainbench-0.3.0/LICENSE` & `chainbench-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.0/README.md` & `chainbench-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 To learn about the parameters and flags, run the following command:
 ```shell
 chainbench start --help
 ```
 
 Basic usage is:
 ```shell
-chainbench start --profile bsc --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
+chainbench start --profile bsc.general --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
 ```
 
 This will run a load test for BSC with 2 workers, 50 users and 12 hours test time in headless mode.
 After the test is finished, the tool will automatically quit.
 
 ### Parameters and Flags
 - `-p, --profile`: Specifies the profile to use for the benchmark. Available profiles can be found in the profile directory. Sample usage `-p bsc.general`
@@ -126,34 +126,45 @@
 There are built-in `evm.light` and `evm.heavy` profiles for EVM-compatible chains.
 
 Here's an example of how to run a load test for Ethereum using the `evm.light` profile:
 ```shell
 chainbench start --profile evm.light --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
 ```
 
+### Monitors
+Monitors are separate processes that run during the test to collect or process some additional data and metrics relevant to the test.
+For example, head-lag-monitor will collect the latest block information from the node under test, check the timestamp and compare it to current time to calculate how much the node lags behind.
+You may include monitors in your test by using the `-m` or `--monitor` option and specifying the name of the monitor. At the moment, monitors only work in headless mode.
+
+Here's an example:
+```shell
+chainbench start --profile evm.light --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit -m head-lag-monitor
+```
+
+
 ### Web UI Mode
 
 Run the following command to run a load test for BSC in UI mode. It will start a web server on port 8089. 
 Target is required to initialize the test data, however you may change the target endpoint later in the UI, along with the number of users, spawn rate and test time.
 
 ```shell
 chainbench start --profile bsc.general --workers 1 --target https://any-working-node-endpoint.com
 ```
 
 ### Headless Mode
 
 If you want to run a load test for BSC in headless mode, run the following command:
 
 ```shell
-chainbench start --profile bsc --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit
+chainbench start --profile bsc.general --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit
 ```
 
 It will run a load test for BSC with 4 workers, 100 users and 1 hour test time.
 
 In practice, you will probably want to run the benchmark on a remote server. Here's the example utilizing `nohup`:
 
 ```shell
-nohup chainbench start --profile bsc --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit &
+nohup chainbench start --profile bsc.general --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit &
 ```
 
 ## License
 This project is licensed under the [Apache 2.0 License](LICENSE).
```

### Comparing `chainbench-0.3.0/chainbench/main.py` & `chainbench-0.3.1/chainbench/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import logging
 import os
 import shlex
 import subprocess
 import sys
+from multiprocessing import Process
 from pathlib import Path
 
 import click
+from locust import runners
 
 from chainbench.util.cli import (
     ContextData,
     ensure_results_dir,
     get_base_path,
     get_master_command,
     get_profile_path,
     get_worker_command,
 )
+from chainbench.util.monitor import monitors
 from chainbench.util.notify import NoopNotifier, Notifier
 
 # Default values for arguments
 MASTER_HOST = "127.0.0.1"
 MASTER_PORT = "5557"
 WORKER_COUNT = 16
 TEST_TIME = "1h"
 USERS = 1000
 SPAWN_RATE = 10
 LOG_LEVEL = "DEBUG"
 DEFAULT_PROFILE = "ethereum.general"
 NOTIFY_URL_TEMPLATE = "https://ntfy.sh/{topic}"
+runners.HEARTBEAT_INTERVAL = 60
 
 logger = logging.getLogger(__name__)
 
 
 @click.group(
     help="Tool for flexible blockchain infrastructure benchmarking.",
 )
@@ -90,14 +94,23 @@
 )
 @click.option("--headless", is_flag=True, help="Run in headless mode")
 @click.option("--autoquit", is_flag=True, help="Auto quit after test")
 @click.option("--target", default=None, help="Endpoint to test")
 @click.option("--run-id", default=None, help="ID of the test")
 @click.option("--notify", default=None, help="Notify when test is finished")
 @click.option(
+    "-m",
+    "--monitor",
+    default=[],
+    help="Add a monitor to collect additional data or metrics. "
+    "You may specify this option multiple times for different monitors",
+    type=click.Choice(["head-lag-monitor"], case_sensitive=False),
+    multiple=True,
+)
+@click.option(
     "--debug-trace-methods",
     is_flag=True,
     help="Enable tasks tagged with debug or trace to be executed",
 )
 @click.option(
     "-E",
     "--exclude-tags",
@@ -136,14 +149,15 @@
     log_level: str,
     results_dir: Path,
     headless: bool,
     autoquit: bool,
     target: str | None,
     run_id: str | None,
     notify: str | None,
+    monitor: list[str],
     debug_trace_methods: bool,
     exclude_tags: list[str],
     timescale: bool,
     pg_host: str | None,
     pg_port: int,
     pg_username: str,
     pg_password: str | None,
@@ -222,14 +236,15 @@
         click.echo(f"Starting master for {profile}")
 
     is_posix = os.name == "posix"
 
     master_args = shlex.split(master_command, posix=is_posix)
     master_process = subprocess.Popen(master_args)
     ctx.obj.master = master_process
+
     # Start the Locust workers
     for worker_id in range(workers):
         worker_command = get_worker_command(
             profile_path=profile_path,
             host=host,
             port=port,
             results_path=results_path,
@@ -255,17 +270,27 @@
             message=f"Running test in headless mode for {profile}",
             tags=["loudspeaker"],
         )
     else:
         # Print out the URL to access the test
         click.echo(f"Run test: http://{host}:8089 {profile}")
 
+    unique_monitors: set[str] = set(monitor)
+    for m in unique_monitors:
+        p = Process(target=monitors[m], args=(target, results_path, test_time))
+        click.echo(f"Starting monitor {m}")
+        p.start()
+        ctx.obj.monitors.append(p)
+
     for process in ctx.obj.workers:
         process.wait()
 
+    for process in ctx.obj.monitors:
+        process.join()
+
     if autoquit:
         ctx.obj.master.wait()
         click.echo("Quitting...")
         ctx.obj.master.terminate()
 
     ctx.obj.notifier.notify(
         title="Test finished", message=f"Test finished for {profile}", tags=["tada"]
```

### Comparing `chainbench-0.3.0/chainbench/profile/avalanche/general.py` & `chainbench-0.3.1/chainbench/profile/avalanche/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.0/chainbench/profile/bsc/general.py` & `chainbench-0.3.1/chainbench/profile/bsc/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.0/chainbench/profile/ethereum/general.py` & `chainbench-0.3.1/chainbench/profile/ethereum/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.0/chainbench/profile/evm/light.py` & `chainbench-0.3.1/chainbench/profile/evm/light.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.0/chainbench/profile/oasis/general.py` & `chainbench-0.3.1/chainbench/profile/oasis/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.0/chainbench/profile/polygon/general.py` & `chainbench-0.3.1/chainbench/profile/polygon/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.0/chainbench/test_data/base.py` & `chainbench-0.3.1/chainbench/test_data/base.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.0/chainbench/test_data/evm.py` & `chainbench-0.3.1/chainbench/test_data/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.0/chainbench/user/base.py` & `chainbench-0.3.1/chainbench/user/base.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.0/chainbench/util/cli.py` & `chainbench-0.3.1/chainbench/util/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,8 +134,9 @@
     return command
 
 
 @dataclass
 class ContextData:
     workers: list[subprocess.Popen] = field(default_factory=list)
     master: subprocess.Popen | None = None
+    monitors: list[subprocess.Popen] = field(default_factory=list)
     notifier: Notifier = field(default_factory=NoopNotifier)
```

### Comparing `chainbench-0.3.0/chainbench/util/event.py` & `chainbench-0.3.1/chainbench/util/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 logger = logging.getLogger(__name__)
 
 
 def on_test_start(environment, **_kwargs):
     # It will be called for any runner (master, worker, local)
     if not isinstance(environment.runner, MasterRunner):
         # Print worker details to the log
-        logger.debug(
+        logger.info(
             f"Worker[{environment.runner.worker_index:02d}]: "
             f"The test is started, Environment: {environment.runner}",
         )
         Timer.set_timer(environment.runner.worker_index)
     else:
         # Print master details to the log
         logger.info(
```

### Comparing `chainbench-0.3.0/chainbench/util/notify.py` & `chainbench-0.3.1/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.0/pyproject.toml` & `chainbench-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "chainbench"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Egor Molodik <egor.molodik@chainstack.com>"]
 readme = "README.md"
 packages = [{include = "chainbench"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = "^0.24.0"
 locust = "^2.15.0"
 click = "^8.1.3"
 locust-plugins = "^3.3.0"
 
-
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.2.0"
 pre-commit = "^3.2.2"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 flake8-pyproject = "^1.2.3"
```

### Comparing `chainbench-0.3.0/PKG-INFO` & `chainbench-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -99,15 +99,15 @@
 To learn about the parameters and flags, run the following command:
 ```shell
 chainbench start --help
 ```
 
 Basic usage is:
 ```shell
-chainbench start --profile bsc --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
+chainbench start --profile bsc.general --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
 ```
 
 This will run a load test for BSC with 2 workers, 50 users and 12 hours test time in headless mode.
 After the test is finished, the tool will automatically quit.
 
 ### Parameters and Flags
 - `-p, --profile`: Specifies the profile to use for the benchmark. Available profiles can be found in the profile directory. Sample usage `-p bsc.general`
@@ -142,34 +142,45 @@
 There are built-in `evm.light` and `evm.heavy` profiles for EVM-compatible chains.
 
 Here's an example of how to run a load test for Ethereum using the `evm.light` profile:
 ```shell
 chainbench start --profile evm.light --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
 ```
 
+### Monitors
+Monitors are separate processes that run during the test to collect or process some additional data and metrics relevant to the test.
+For example, head-lag-monitor will collect the latest block information from the node under test, check the timestamp and compare it to current time to calculate how much the node lags behind.
+You may include monitors in your test by using the `-m` or `--monitor` option and specifying the name of the monitor. At the moment, monitors only work in headless mode.
+
+Here's an example:
+```shell
+chainbench start --profile evm.light --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit -m head-lag-monitor
+```
+
+
 ### Web UI Mode
 
 Run the following command to run a load test for BSC in UI mode. It will start a web server on port 8089. 
 Target is required to initialize the test data, however you may change the target endpoint later in the UI, along with the number of users, spawn rate and test time.
 
 ```shell
 chainbench start --profile bsc.general --workers 1 --target https://any-working-node-endpoint.com
 ```
 
 ### Headless Mode
 
 If you want to run a load test for BSC in headless mode, run the following command:
 
 ```shell
-chainbench start --profile bsc --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit
+chainbench start --profile bsc.general --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit
 ```
 
 It will run a load test for BSC with 4 workers, 100 users and 1 hour test time.
 
 In practice, you will probably want to run the benchmark on a remote server. Here's the example utilizing `nohup`:
 
 ```shell
-nohup chainbench start --profile bsc --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit &
+nohup chainbench start --profile bsc.general --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit &
 ```
 
 ## License
 This project is licensed under the [Apache 2.0 License](LICENSE).
```

