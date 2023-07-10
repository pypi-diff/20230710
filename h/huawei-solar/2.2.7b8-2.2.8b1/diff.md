# Comparing `tmp/huawei-solar-2.2.7b8.tar.gz` & `tmp/huawei-solar-2.2.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huawei-solar-2.2.7b8.tar", last modified: Wed Jun 21 06:44:37 2023, max compression
+gzip compressed data, was "huawei-solar-2.2.8b1.tar", last modified: Mon Jul 10 13:26:01 2023, max compression
```

## Comparing `huawei-solar-2.2.7b8.tar` & `huawei-solar-2.2.8b1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:44:37.416512 huawei-solar-2.2.7b8/
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/.codecov.yml
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/.yamllint
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     7719 2023-06-21 06:44:37.416512 huawei-solar-2.2.7b8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7163 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/bridge_tst.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/requirements_test.txt
--rw-rw-rw-   0 root         (0) root         (0)      936 2023-06-21 06:44:37.417512 huawei-solar-2.2.7b8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:44:37.408512 huawei-solar-2.2.7b8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:44:37.414512 huawei-solar-2.2.7b8/src/huawei_solar/
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/bridge.py
--rw-rw-rw-   0 root         (0) root         (0)     1764 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    11325 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/files.py
--rw-rw-rw-   0 root         (0) root         (0)    24956 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     7019 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/modbus.py
--rw-rw-rw-   0 root         (0) root         (0)    18080 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/register_names.py
--rw-rw-rw-   0 root         (0) root         (0)    22487 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/register_values.py
--rw-rw-rw-   0 root         (0) root         (0)    42679 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/registers.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/utils.py
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-21 06:44:37.000000 huawei-solar-2.2.7b8/src/huawei_solar/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:44:37.415512 huawei-solar-2.2.7b8/src/huawei_solar.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7719 2023-06-21 06:44:37.000000 huawei-solar-2.2.7b8/src/huawei_solar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      891 2023-06-21 06:44:37.000000 huawei-solar-2.2.7b8/src/huawei_solar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 06:44:37.000000 huawei-solar-2.2.7b8/src/huawei_solar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-21 06:44:37.000000 huawei-solar-2.2.7b8/src/huawei_solar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 06:44:37.000000 huawei-solar-2.2.7b8/src/huawei_solar.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3578 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:44:37.416512 huawei-solar-2.2.7b8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2611 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tests/mock_huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     3531 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tests/test__registers__peak_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     6245 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tests/test__registers__time_of_use.py
--rw-rw-rw-   0 root         (0) root         (0)    16324 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tests/test_huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tests/test_registers.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:26:01.566200 huawei-solar-2.2.8b1/
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/.codecov.yml
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/.yamllint
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     7719 2023-07-10 13:26:01.566200 huawei-solar-2.2.8b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7163 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/bridge_tst.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/requirements_test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-07-10 13:26:01.567200 huawei-solar-2.2.8b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:26:01.559200 huawei-solar-2.2.8b1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:26:01.564200 huawei-solar-2.2.8b1/src/huawei_solar/
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11325 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/files.py
+-rw-rw-rw-   0 root         (0) root         (0)    25023 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     6983 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/modbus.py
+-rw-rw-rw-   0 root         (0) root         (0)    18080 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/register_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    22487 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/register_values.py
+-rw-rw-rw-   0 root         (0) root         (0)    42677 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/registers.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/utils.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-10 13:26:01.000000 huawei-solar-2.2.8b1/src/huawei_solar/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:26:01.565200 huawei-solar-2.2.8b1/src/huawei_solar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7719 2023-07-10 13:26:01.000000 huawei-solar-2.2.8b1/src/huawei_solar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      891 2023-07-10 13:26:01.000000 huawei-solar-2.2.8b1/src/huawei_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 13:26:01.000000 huawei-solar-2.2.8b1/src/huawei_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-10 13:26:01.000000 huawei-solar-2.2.8b1/src/huawei_solar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 13:26:01.000000 huawei-solar-2.2.8b1/src/huawei_solar.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:26:01.566200 huawei-solar-2.2.8b1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2611 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tests/mock_huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     3531 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tests/test__registers__peak_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tests/test__registers__time_of_use.py
+-rw-rw-rw-   0 root         (0) root         (0)    16324 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tests/test_huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tests/test_registers.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tox.ini
```

### Comparing `huawei-solar-2.2.7b8/.gitignore` & `huawei-solar-2.2.8b1/.gitignore`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/.gitlab-ci.yml` & `huawei-solar-2.2.8b1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/.pre-commit-config.yaml` & `huawei-solar-2.2.8b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/LICENSE.md` & `huawei-solar-2.2.8b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/PKG-INFO` & `huawei-solar-2.2.8b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huawei-solar
-Version: 2.2.7b8
+Version: 2.2.8b1
 Summary: A Python wrapper for the Huawei Inverter modbus TCP API
 Home-page: https://gitlab.com/EmilV2/huawei-solar
 Author: Emil Vanherp
 Author-email: emil@vanherp.me
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `huawei-solar-2.2.7b8/README.md` & `huawei-solar-2.2.8b1/README.md`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/bridge_tst.py` & `huawei-solar-2.2.8b1/bridge_tst.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/pyproject.toml` & `huawei-solar-2.2.8b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/setup.cfg` & `huawei-solar-2.2.8b1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	=src
 packages = find:
 install_requires = 
-	pymodbus>=3.2.2,<3.3
+	pymodbus>=3.3.1,<3.4
 	pyserial-asyncio>=0.6
 	backoff
-	pytz>=2021.3
+	pytz>=2023.3
 python_requires = >=3.9
 setup_requires = 
 	setuptools_scm
 
 [flake8]
 extend-ignore = 
 	E203
```

### Comparing `huawei-solar-2.2.7b8/src/huawei_solar/__init__.py` & `huawei-solar-2.2.8b1/src/huawei_solar/__init__.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/src/huawei_solar/bridge.py` & `huawei-solar-2.2.8b1/src/huawei_solar/bridge.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/src/huawei_solar/exceptions.py` & `huawei-solar-2.2.8b1/src/huawei_solar/exceptions.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/src/huawei_solar/files.py` & `huawei-solar-2.2.8b1/src/huawei_solar/files.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/src/huawei_solar/huawei_solar.py` & `huawei-solar-2.2.8b1/src/huawei_solar/huawei_solar.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 DEFAULT_TCP_PORT = 502
 DEFAULT_BAUDRATE = 9600
 
 DEFAULT_SLAVE = 0
 DEFAULT_TIMEOUT = 10  # especially the SDongle can react quite slowly
 DEFAULT_WAIT = 1
 DEFAULT_COOLDOWN_TIME = 0.05
+WAIT_FOR_CONNECTION_TIMEOUT = 5
 
 HEARTBEAT_REGISTER = 49999
 
 FILE_UPLOAD_MAX_RETRIES = 6
 FILE_UPLOAD_RETRY_TIMEOUT = 10
 
 PERMISSION_DENIED_EXCEPTION_CODE = 0x80
@@ -129,15 +130,15 @@
                 raise rerr
 
     @asynccontextmanager
     async def _communication_lock(self):
         async with self.__communication_lock:
             if not self._client.connected_event.is_set():
                 LOGGER.info("Waiting for connection ...")
-            await self._client.connected_event.wait()
+            await asyncio.wait_for(self._client.connected_event.wait(), WAIT_FOR_CONNECTION_TIMEOUT)
 
             await self.__cooled_down.wait()
             self.__cooled_down.clear()
 
             try:
                 yield
             finally:
@@ -205,19 +206,19 @@
             # if an error occurs, we need to make sure that the Modbus-client is stopped,
             # otherwise it can stay active and cause even more problems ...
             LOGGER.exception("Aborting client creation due to error.")
             raise ConnectionException from err
 
     async def stop(self):
         """Stop the modbus client."""
-        await self._client.close()
+        self._client.close()
 
     async def _reconnect(self):
         """Reconnect to the inverter"""
-        await self._client.close()
+        self._client.close()
         await self._client.connect()
 
     async def _decode_response(self, reg: RegisterDefinition, decoder: BinaryPayloadDecoder):
         """Decodes a modbus register and puts it into a Result object."""
         result = reg.decode(decoder, self)
 
         if not hasattr(reg, "unit") or callable(reg.unit) or isinstance(reg.unit, dict):
```

### Comparing `huawei-solar-2.2.7b8/src/huawei_solar/modbus.py` & `huawei-solar-2.2.8b1/src/huawei_solar/modbus.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,28 +20,28 @@
     connected_event = asyncio.Event()
 
     def __init__(self, *args, **kwargs) -> None:
         """Add support for the custom Huawei modbus messages"""
         super().__init__(*args, **kwargs)
         super().register(PrivateHuaweiModbusResponse)
 
-    def client_made_connection(self, protocol):
+    def connection_made(self, transport):
         """Register that a connection has been made in an asyncio Event"""
-        super().client_made_connection(protocol)
+        super().connection_made(transport)
 
         async def _made_connection_task():
             LOGGER.debug("Waiting for %d milliseconds after connection before performing operations", WAIT_ON_CONNECT)
             await asyncio.sleep(WAIT_ON_CONNECT / 1000)
             self.connected_event.set()
 
         asyncio.create_task(_made_connection_task())
 
-    def client_lost_connection(self, protocol):
+    def connection_lost(self, exc):
         """Register that a connection has been lost in an asyncio Event"""
-        super().client_lost_connection(protocol)
+        super().connection_lost(exc)
         self.connected_event.clear()
 
 
 class AsyncHuaweiSolarModbusSerialClient(ModbusConnectionMixin, AsyncModbusSerialClient):
     """Custom SerialClient with support for custom Huawei modbus messages"""
 
     def __init__(self, port, baudrate, timeout: int, **serial_kwargs):
```

### Comparing `huawei-solar-2.2.7b8/src/huawei_solar/register_names.py` & `huawei-solar-2.2.8b1/src/huawei_solar/register_names.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/src/huawei_solar/register_values.py` & `huawei-solar-2.2.8b1/src/huawei_solar/register_values.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/src/huawei_solar/registers.py` & `huawei-solar-2.2.8b1/src/huawei_solar/registers.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,15 +589,15 @@
     rn.Q_MAX_OUT: I32Register("VAr", 1, 30079, 2),
     rn.Q_MAX_IN: I32Register("VAr", 1, 30081, 2),
     rn.OFFERING_NAME_OF_SOUTHBOUND_DEVICE_1: StringRegister(30561, 15),
     rn.OFFERING_NAME_OF_SOUTHBOUND_DEVICE_2: StringRegister(30576, 15),
     rn.OFFERING_NAME_OF_SOUTHBOUND_DEVICE_3: StringRegister(30591, 15),
     rn.HARDWARE_VERSION: StringRegister(31000, 15),
     rn.MONITORING_BOARD_SN: StringRegister(31015, 10),
-    rn.MONITORING_SOFTWARE_VERSION: StringRegister(31015, 15),
+    rn.MONITORING_SOFTWARE_VERSION: StringRegister(31025, 15),
     rn.MASTER_DSP_VERSION: StringRegister(31040, 15),
     rn.CPLD_VERSION: StringRegister(31070, 15),
     rn.AFCI_VERSION: StringRegister(31085, 15),
     rn.DC_MBUS_VERSION: StringRegister(31115, 15),
     rn.REGKEY: StringRegister(31200, 10),
     rn.STATE_1: U16Register(partial(bitfield_decoder, rv.STATE_CODES_1), 1, 32000, 1),
     rn.STATE_2: U16Register(partial(bitfield_decoder, rv.STATE_CODES_2), 1, 32002, 1),
@@ -830,15 +830,15 @@
     rn.STORAGE_LCOE: U32Register(None, 1000, 47069, 2),
     rn.STORAGE_MAXIMUM_CHARGING_POWER: U32Register("W", 1, 47075, 2, writeable=True),
     rn.STORAGE_MAXIMUM_DISCHARGING_POWER: U32Register("W", 1, 47077, 2, writeable=True),
     rn.STORAGE_POWER_LIMIT_GRID_TIED_POINT: I32Register("W", 1, 47079, 2),
     rn.STORAGE_CHARGING_CUTOFF_CAPACITY: U16Register("%", 10, 47081, 1, writeable=True),
     rn.STORAGE_DISCHARGING_CUTOFF_CAPACITY: U16Register("%", 10, 47082, 1, writeable=True),
     rn.STORAGE_FORCED_CHARGING_AND_DISCHARGING_PERIOD: U16Register("min", 1, 47083, 1, writeable=True),
-    rn.STORAGE_FORCED_CHARGING_AND_DISCHARGING_POWER: I32Register("min", 1, 47084, 2),
+    rn.STORAGE_FORCED_CHARGING_AND_DISCHARGING_POWER: I32Register("W", 1, 47084, 2),
     rn.STORAGE_WORKING_MODE_SETTINGS: U16Register(rv.StorageWorkingModesC, 1, 47086, 1, writeable=True),
     rn.STORAGE_CHARGE_FROM_GRID_FUNCTION: U16Register(bool, 1, 47087, 1, writeable=True),
     rn.STORAGE_GRID_CHARGE_CUTOFF_STATE_OF_CHARGE: U16Register("%", 10, 47088, 1, writeable=True),
     rn.STORAGE_UNIT_2_PRODUCT_MODEL: U16Register(rv.StorageProductModel, 1, 47089, 1),
     rn.STORAGE_FORCIBLE_CHARGE_DISCHARGE_WRITE: U16Register(
         rv.StorageForcibleChargeDischarge, 1, 47100, 1, writeable=True
     ),
@@ -856,15 +856,15 @@
     rn.STORAGE_EXCESS_PV_ENERGY_USE_IN_TOU: U16Register(rv.StorageExcessPvEnergyUseInTOU, 1, 47299, 1, writeable=True),
     rn.ACTIVE_POWER_CONTROL_MODE: U16Register(rv.ActivePowerControlMode, 1, 47415, 1, writeable=True),
     rn.MAXIMUM_FEED_GRID_POWER_WATT: I32Register("W", 1, 47416, 2, writeable=True),
     rn.MAXIMUM_FEED_GRID_POWER_PERCENT: I16Register("%", 10, 47418, 1, writeable=True),
     rn.DONGLE_PLANT_MAXIMUM_CHARGE_FROM_GRID_POWER: U32Register("W", 1, 47590, 2, writeable=True),
     rn.BACKUP_SWITCH_TO_OFF_GRID: U16Register(None, 1, 47604, 1, writeable=True),
     rn.BACKUP_VOLTAGE_INDEPENDEND_OPERATION: U16Register(
-        rv.BackupVoltageIndependentOperation, 1, 47604, 1, writeable=True
+        rv.BackupVoltageIndependentOperation, 1, 47605, 1, writeable=True
     ),
     rn.REMOTE_CHARGE_DISCHARGE_CONTROL_MODE: I16Register(
         rv.RemoteChargeDischargeControlMode, 1, 47589, 1, writeable=True
     ),
     rn.DEFAULT_MAXIMUM_FEED_IN_POWER: I32Register("W", 1, 47675, 2, writeable=True),
     rn.DEFAULT_ACTIVE_POWER_CHANGE_GRADIENT: U32Register("%/s", 1000, 47677, 2),
     rn.STORAGE_UNIT_1_PACK_1_NO: U16Register(None, 1, 47750, 1),
```

### Comparing `huawei-solar-2.2.7b8/src/huawei_solar.egg-info/PKG-INFO` & `huawei-solar-2.2.8b1/src/huawei_solar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huawei-solar
-Version: 2.2.7b8
+Version: 2.2.8b1
 Summary: A Python wrapper for the Huawei Inverter modbus TCP API
 Home-page: https://gitlab.com/EmilV2/huawei-solar
 Author: Emil Vanherp
 Author-email: emil@vanherp.me
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `huawei-solar-2.2.7b8/src/huawei_solar.egg-info/SOURCES.txt` & `huawei-solar-2.2.8b1/src/huawei_solar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/test.py` & `huawei-solar-2.2.8b1/test.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/tests/conftest.py` & `huawei-solar-2.2.8b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/tests/mock_huawei_solar.py` & `huawei-solar-2.2.8b1/tests/mock_huawei_solar.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/tests/test__registers__peak_periods.py` & `huawei-solar-2.2.8b1/tests/test__registers__peak_periods.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/tests/test__registers__time_of_use.py` & `huawei-solar-2.2.8b1/tests/test__registers__time_of_use.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/tests/test_huawei_solar.py` & `huawei-solar-2.2.8b1/tests/test_huawei_solar.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/tests/test_registers.py` & `huawei-solar-2.2.8b1/tests/test_registers.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b8/tox.ini` & `huawei-solar-2.2.8b1/tox.ini`

 * *Files identical despite different names*

