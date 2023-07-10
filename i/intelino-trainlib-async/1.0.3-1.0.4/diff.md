# Comparing `tmp/intelino-trainlib-async-1.0.3.tar.gz` & `tmp/intelino-trainlib-async-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intelino-trainlib-async-1.0.3.tar", last modified: Tue Apr  4 16:26:17 2023, max compression
+gzip compressed data, was "intelino-trainlib-async-1.0.4.tar", last modified: Mon Jul 10 18:56:27 2023, max compression
```

## Comparing `intelino-trainlib-async-1.0.3.tar` & `intelino-trainlib-async-1.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-04-04 16:26:17.555045 intelino-trainlib-async-1.0.3/
--rw-r--r--   0 oscar      (501) staff       (20)     7541 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/LICENSE
--rw-r--r--   0 oscar      (501) staff       (20)     4037 2023-04-04 16:26:17.555117 intelino-trainlib-async-1.0.3/PKG-INFO
--rw-r--r--   0 oscar      (501) staff       (20)     2721 2021-09-15 21:43:35.000000 intelino-trainlib-async-1.0.3/README.md
-drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-04-04 16:26:17.551272 intelino-trainlib-async-1.0.3/intelino/
-drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-04-04 16:26:17.552158 intelino-trainlib-async-1.0.3/intelino/scan/
--rw-r--r--   0 oscar      (501) staff       (20)     3073 2023-04-04 16:24:33.000000 intelino-trainlib-async-1.0.3/intelino/scan/__main__.py
-drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-04-04 16:26:17.553614 intelino-trainlib-async-1.0.3/intelino/trainlib_async/
--rw-r--r--   0 oscar      (501) staff       (20)      792 2023-04-04 16:24:33.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/__init__.py
-drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-04-04 16:26:17.553892 intelino-trainlib-async-1.0.3/intelino/trainlib_async/drivers/
--rw-r--r--   0 oscar      (501) staff       (20)     3240 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/drivers/bleak_driver.py
--rw-r--r--   0 oscar      (501) staff       (20)     2004 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/drivers/train_ble_driver.py
-drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-04-04 16:26:17.554323 intelino-trainlib-async-1.0.3/intelino/trainlib_async/enums/
--rw-r--r--   0 oscar      (501) staff       (20)      499 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/enums/__init__.py
--rw-r--r--   0 oscar      (501) staff       (20)     3362 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/enums/enums.py
--rw-r--r--   0 oscar      (501) staff       (20)      975 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/enums/internals.py
--rw-r--r--   0 oscar      (501) staff       (20)     1080 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/exc.py
--rw-r--r--   0 oscar      (501) staff       (20)     3000 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/helpers.py
--rw-r--r--   0 oscar      (501) staff       (20)    11330 2021-09-27 16:20:51.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/message_builder.py
--rw-r--r--   0 oscar      (501) staff       (20)    10003 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/messages.py
--rw-r--r--   0 oscar      (501) staff       (20)    11193 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/train.py
--rw-r--r--   0 oscar      (501) staff       (20)     3707 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/train_ble_device.py
--rw-r--r--   0 oscar      (501) staff       (20)     2896 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/train_ble_packet.py
--rw-r--r--   0 oscar      (501) staff       (20)     4981 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/train_factory.py
--rw-r--r--   0 oscar      (501) staff       (20)     3614 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.3/intelino/trainlib_async/train_scanner.py
-drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-04-04 16:26:17.554935 intelino-trainlib-async-1.0.3/intelino_trainlib_async.egg-info/
--rw-r--r--   0 oscar      (501) staff       (20)     4037 2023-04-04 16:26:17.000000 intelino-trainlib-async-1.0.3/intelino_trainlib_async.egg-info/PKG-INFO
--rw-r--r--   0 oscar      (501) staff       (20)      904 2023-04-04 16:26:17.000000 intelino-trainlib-async-1.0.3/intelino_trainlib_async.egg-info/SOURCES.txt
--rw-r--r--   0 oscar      (501) staff       (20)        1 2023-04-04 16:26:17.000000 intelino-trainlib-async-1.0.3/intelino_trainlib_async.egg-info/dependency_links.txt
--rw-r--r--   0 oscar      (501) staff       (20)       27 2023-04-04 16:26:17.000000 intelino-trainlib-async-1.0.3/intelino_trainlib_async.egg-info/requires.txt
--rw-r--r--   0 oscar      (501) staff       (20)        9 2023-04-04 16:26:17.000000 intelino-trainlib-async-1.0.3/intelino_trainlib_async.egg-info/top_level.txt
--rw-r--r--   0 oscar      (501) staff       (20)      458 2023-04-04 16:26:17.555428 intelino-trainlib-async-1.0.3/setup.cfg
--rw-r--r--   0 oscar      (501) staff       (20)     1916 2023-04-04 16:24:33.000000 intelino-trainlib-async-1.0.3/setup.py
+drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-07-10 18:56:27.425746 intelino-trainlib-async-1.0.4/
+-rw-r--r--   0 oscar      (501) staff       (20)     7541 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.4/LICENSE
+-rw-r--r--   0 oscar      (501) staff       (20)     4037 2023-07-10 18:56:27.425820 intelino-trainlib-async-1.0.4/PKG-INFO
+-rw-r--r--   0 oscar      (501) staff       (20)     2721 2021-09-15 21:43:35.000000 intelino-trainlib-async-1.0.4/README.md
+drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-07-10 18:56:27.422376 intelino-trainlib-async-1.0.4/intelino/
+drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-07-10 18:56:27.423162 intelino-trainlib-async-1.0.4/intelino/scan/
+-rw-r--r--   0 oscar      (501) staff       (20)     3277 2023-07-10 18:53:05.000000 intelino-trainlib-async-1.0.4/intelino/scan/__main__.py
+drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-07-10 18:56:27.424382 intelino-trainlib-async-1.0.4/intelino/trainlib_async/
+-rw-r--r--   0 oscar      (501) staff       (20)      792 2023-07-10 18:53:05.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/__init__.py
+drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-07-10 18:56:27.424708 intelino-trainlib-async-1.0.4/intelino/trainlib_async/drivers/
+-rw-r--r--   0 oscar      (501) staff       (20)     3465 2023-07-10 18:53:05.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/drivers/bleak_driver.py
+-rw-r--r--   0 oscar      (501) staff       (20)     2004 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/drivers/train_ble_driver.py
+drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-07-10 18:56:27.425087 intelino-trainlib-async-1.0.4/intelino/trainlib_async/enums/
+-rw-r--r--   0 oscar      (501) staff       (20)      499 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/enums/__init__.py
+-rw-r--r--   0 oscar      (501) staff       (20)     3362 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/enums/enums.py
+-rw-r--r--   0 oscar      (501) staff       (20)      975 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/enums/internals.py
+-rw-r--r--   0 oscar      (501) staff       (20)     1080 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/exc.py
+-rw-r--r--   0 oscar      (501) staff       (20)     3000 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/helpers.py
+-rw-r--r--   0 oscar      (501) staff       (20)    11330 2021-09-27 16:20:51.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/message_builder.py
+-rw-r--r--   0 oscar      (501) staff       (20)    10003 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/messages.py
+-rw-r--r--   0 oscar      (501) staff       (20)    11193 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/train.py
+-rw-r--r--   0 oscar      (501) staff       (20)     3709 2023-07-10 18:53:05.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/train_ble_device.py
+-rw-r--r--   0 oscar      (501) staff       (20)     2896 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/train_ble_packet.py
+-rw-r--r--   0 oscar      (501) staff       (20)     4981 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/train_factory.py
+-rw-r--r--   0 oscar      (501) staff       (20)     3614 2021-09-15 13:29:11.000000 intelino-trainlib-async-1.0.4/intelino/trainlib_async/train_scanner.py
+drwxr-xr-x   0 oscar      (501) staff       (20)        0 2023-07-10 18:56:27.425643 intelino-trainlib-async-1.0.4/intelino_trainlib_async.egg-info/
+-rw-r--r--   0 oscar      (501) staff       (20)     4037 2023-07-10 18:56:27.000000 intelino-trainlib-async-1.0.4/intelino_trainlib_async.egg-info/PKG-INFO
+-rw-r--r--   0 oscar      (501) staff       (20)      904 2023-07-10 18:56:27.000000 intelino-trainlib-async-1.0.4/intelino_trainlib_async.egg-info/SOURCES.txt
+-rw-r--r--   0 oscar      (501) staff       (20)        1 2023-07-10 18:56:27.000000 intelino-trainlib-async-1.0.4/intelino_trainlib_async.egg-info/dependency_links.txt
+-rw-r--r--   0 oscar      (501) staff       (20)       27 2023-07-10 18:56:27.000000 intelino-trainlib-async-1.0.4/intelino_trainlib_async.egg-info/requires.txt
+-rw-r--r--   0 oscar      (501) staff       (20)        9 2023-07-10 18:56:27.000000 intelino-trainlib-async-1.0.4/intelino_trainlib_async.egg-info/top_level.txt
+-rw-r--r--   0 oscar      (501) staff       (20)      458 2023-07-10 18:56:27.426063 intelino-trainlib-async-1.0.4/setup.cfg
+-rw-r--r--   0 oscar      (501) staff       (20)     1916 2023-07-10 18:53:31.000000 intelino-trainlib-async-1.0.4/setup.py
```

### Comparing `intelino-trainlib-async-1.0.3/LICENSE` & `intelino-trainlib-async-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/PKG-INFO` & `intelino-trainlib-async-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelino-trainlib-async
-Version: 1.0.3
+Version: 1.0.4
 Summary: Asynchronous Python library (SDK) for interacting with the intelino smart train.
 Home-page: https://intelino.com
 Author: intelino
 Author-email: developer@intelino.com
 License: Intelino Public License
 Project-URL: Documentation, https://intelino-trainlib-async-py.readthedocs.io/
 Project-URL: Source Code, https://github.com/intelino-code/intelino-trainlib-async-py
```

### Comparing `intelino-trainlib-async-1.0.3/README.md` & `intelino-trainlib-async-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/intelino/scan/__main__.py` & `intelino-trainlib-async-1.0.4/intelino/scan/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 # https://intelino.com/intelino-public-license.
 # BY INSTALLING, DOWNLOADING, ACCESSING, USING OR DISTRIBUTING ANY OF
 # THE SOFTWARE, YOU AGREE TO THE TERMS OF SUCH LICENSE AGREEMENT.
 
 """BLE scanning utility to find nearby intelino trains."""
 
 import asyncio
-from typing import List
+from typing import List, Dict, Tuple
 from bleak import BleakScanner
 from bleak.backends.device import BLEDevice
+from bleak.backends.scanner import AdvertisementData
 from intelino.trainlib_async import TrainScanner, Train
 
 
 async def print_info_card(train: Train, full: bool = True):
     print(f'{"="*40}')
     print(f'{"Train info":^40s}')
     print(f'{"="*40}')
@@ -58,25 +59,25 @@
         await print_info_card(train, full=True)
         await train.disconnect()
 
     if len(trains) == 0:
         print("No trains found.")
 
 
-def list_devices(title: str, devices: List[BLEDevice]) -> None:
+def list_devices(title: str, devices: List[Tuple[BLEDevice, AdvertisementData]]) -> None:
     print(f"{title} ({len(devices)}):")
-    for d in devices:
-        print(f"{d.address} : {d.name} (RSSI {d.rssi})")
+    for dev, adv_data in devices:
+        print(f"{dev.address} : {dev.name} (RSSI {adv_data.rssi})")
 
 
 async def general_scan(timeout: float) -> None:
-    devices = await BleakScanner.discover(timeout)
+    devices: Dict[str, Tuple[BLEDevice, AdvertisementData]] = await BleakScanner.discover(timeout, return_adv=True)
 
-    trains = list(filter(lambda d: str(d.name).startswith("intelino"), devices))
-    others = list(filter(lambda d: not str(d.name).startswith("intelino"), devices))
+    trains = list(filter(lambda t: str(t[0].name).startswith("intelino"), devices.values()))
+    others = list(filter(lambda t: not str(t[0].name).startswith("intelino"), devices.values()))
 
     list_devices("Trains", trains)
     print()
     list_devices("Others", others)
 
 
 if __name__ == "__main__":
```

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/__init__.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 the :class:`TrainScanner` and :class:`Train` classes.
 """
 
 from .train import Train
 from .train_scanner import TrainScanner
 
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
```

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/drivers/bleak_driver.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/drivers/bleak_driver.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,32 +25,41 @@
     ):
         super().__init__()
         if isinstance(address_or_ble_device, BLEDevice) and name is None:
             self.__name: str = address_or_ble_device.name
         else:
             self.__name: str = name if name else "intelino J-1"
 
-        self.__bleak_client: BleakClient = BleakClient(address_or_ble_device, **kwargs)
+        self.__bleak_client: BleakClient = BleakClient(
+            address_or_ble_device,
+            disconnected_callback=self._on_disconnected,
+            **kwargs
+        )
         self.__response_callback: Union[Callable[[TrainBlePacket], None], None] = None
+        self._disconnected_callback = None
 
     async def connect(self, **kwargs) -> bool:
         connected = await self.__bleak_client.connect(**kwargs)
 
         if connected:
 
-            def callback(_: int, data: bytearray):
+            def callback(_, data: bytearray):
                 if self.__response_callback:
                     self.__response_callback(TrainBlePacket(data))
 
             await self.__bleak_client.start_notify(
                 self.RESPONSE_CHARACTERISTIC, callback
             )
 
         return connected and self.__bleak_client.is_connected
 
+    def _on_disconnected(self, *args):
+        if self._disconnected_callback:
+            self._disconnected_callback(*args)
+
     async def disconnect(self) -> bool:
         if self.__bleak_client.is_connected:
             await self.__bleak_client.stop_notify(self.RESPONSE_CHARACTERISTIC)
         return await self.__bleak_client.disconnect()
 
     @property
     def is_connected(self) -> bool:
@@ -82,12 +91,12 @@
             async_callback = callback
 
             def wrapped_callback(packet: TrainBlePacket):
                 asyncio.create_task(async_callback(packet))
 
             self.__response_callback = wrapped_callback
 
-        elif is_not_coroutine_function((callback)):
+        elif is_not_coroutine_function(callback):
             self.__response_callback = callback
 
     def set_disconnect_listener(self, callback: Callable[[], None]) -> None:
-        self.__bleak_client.set_disconnected_callback(lambda _: callback())
+        self._disconnected_callback = callback
```

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/drivers/train_ble_driver.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/drivers/train_ble_driver.py`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/enums/enums.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/enums/enums.py`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/enums/internals.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/enums/internals.py`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/exc.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/exc.py`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/helpers.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/helpers.py`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/message_builder.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/message_builder.py`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/messages.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/messages.py`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/train.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/train.py`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/train_ble_device.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/train_ble_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self._driver: TrainBleDriver = driver
 
         self.__connection_status: BehaviorSubject[bool] = BehaviorSubject(False)
         self.__notifications: Subject[TrainBlePacket, TrainBlePacket] = Subject()
         self.__writes: Subject[TrainBlePacket, TrainBlePacket] = Subject()
 
         driver.set_response_listener(self.__notifications.on_next)
-        driver.set_disconnect_listener(lambda: self.__connection_status.on_next(False))
+        driver.set_disconnect_listener(lambda _: self.__connection_status.on_next(False))
 
     @property
     def id(self) -> str:
         """Connection ID / address."""
         return self._driver.id
 
     @property
```

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/train_ble_packet.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/train_ble_packet.py`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/train_factory.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/train_factory.py`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/intelino/trainlib_async/train_scanner.py` & `intelino-trainlib-async-1.0.4/intelino/trainlib_async/train_scanner.py`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/intelino_trainlib_async.egg-info/PKG-INFO` & `intelino-trainlib-async-1.0.4/intelino_trainlib_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelino-trainlib-async
-Version: 1.0.3
+Version: 1.0.4
 Summary: Asynchronous Python library (SDK) for interacting with the intelino smart train.
 Home-page: https://intelino.com
 Author: intelino
 Author-email: developer@intelino.com
 License: Intelino Public License
 Project-URL: Documentation, https://intelino-trainlib-async-py.readthedocs.io/
 Project-URL: Source Code, https://github.com/intelino-code/intelino-trainlib-async-py
```

### Comparing `intelino-trainlib-async-1.0.3/intelino_trainlib_async.egg-info/SOURCES.txt` & `intelino-trainlib-async-1.0.4/intelino_trainlib_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intelino-trainlib-async-1.0.3/setup.py` & `intelino-trainlib-async-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "bleak",
     "Rx",
     "typing-extensions",
 ]
 
 setup(
     name="intelino-trainlib-async",
-    version="1.0.3",
+    version="1.0.4",
     description="Asynchronous Python library (SDK) for interacting with the intelino smart train.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="intelino",
     author_email="developer@intelino.com",
     license="Intelino Public License",
     url="https://intelino.com",
```

