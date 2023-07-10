# Comparing `tmp/enocean_ble-0.1.0.tar.gz` & `tmp/enocean_ble-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enocean_ble-0.1.0.tar", last modified: Sun Jul  2 19:33:27 2023, max compression
+gzip compressed data, was "enocean_ble-0.1.1.tar", last modified: Mon Jul 10 21:04:12 2023, max compression
```

## Comparing `enocean_ble-0.1.0.tar` & `enocean_ble-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-02 19:25:15.742226 enocean_ble-0.1.0/LICENSE
--rw-r--r--   0        0        0      137 2023-07-02 19:25:15.758226 enocean_ble-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-02 19:25:15.742226 enocean_ble-0.1.0/enocean_ble/__init__.py
--rw-r--r--   0        0        0     1140 2023-07-02 19:25:15.754226 enocean_ble-0.1.0/enocean_ble/__main__.py
--rw-r--r--   0        0        0     5514 2023-07-02 19:25:15.758226 enocean_ble-0.1.0/enocean_ble/decoder.py
--rw-r--r--   0        0        0     2449 2023-07-02 19:25:15.758226 enocean_ble-0.1.0/enocean_ble/parser.py
--rw-r--r--   0        0        0      652 2023-07-02 19:33:27.023768 enocean_ble-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-02 19:25:15.758226 enocean_ble-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3477 2023-07-02 19:25:15.758226 enocean_ble-0.1.0/tests/test_decoder.py
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 enocean_ble-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-02 19:25:15.742226 enocean_ble-0.1.1/LICENSE
+-rw-r--r--   0        0        0      137 2023-07-02 19:25:15.758226 enocean_ble-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-02 19:25:15.742226 enocean_ble-0.1.1/enocean_ble/__init__.py
+-rw-r--r--   0        0        0     1170 2023-07-10 21:00:55.929469 enocean_ble-0.1.1/enocean_ble/__main__.py
+-rw-r--r--   0        0        0     5516 2023-07-10 21:00:30.589570 enocean_ble-0.1.1/enocean_ble/decoder.py
+-rw-r--r--   0        0        0     2449 2023-07-02 19:25:15.758226 enocean_ble-0.1.1/enocean_ble/parser.py
+-rw-r--r--   0        0        0      652 2023-07-10 21:04:12.104970 enocean_ble-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-02 19:25:15.758226 enocean_ble-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     3477 2023-07-02 19:25:15.758226 enocean_ble-0.1.1/tests/test_decoder.py
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 enocean_ble-0.1.1/PKG-INFO
```

### Comparing `enocean_ble-0.1.0/LICENSE` & `enocean_ble-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enocean_ble-0.1.0/enocean_ble/__main__.py` & `enocean_ble-0.1.1/enocean_ble/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 def simple_callback(device: BLEDevice, advertisement_data: AdvertisementData):
     if device.address.startswith("E2:15"):
         decoder = PTM215BDecoder(
             BluetoothServiceInfo.from_advertisement(device, advertisement_data, "")
         )
+        print(device.address)
         print(
             "signature_valid: "
             + str(decoder.is_signature_valid(b'D\x18\xe4\x0c{{\x05na\xaa"\\C.\xa8\xad'))
         )
         print(f"a0: {decoder.a0_action}")
         print(f"b0: {decoder.b0_action}")
         print(f"a1: {decoder.a1_action}")
```

### Comparing `enocean_ble-0.1.0/enocean_ble/decoder.py` & `enocean_ble-0.1.1/enocean_ble/decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,18 +47,18 @@
         # Calculate signature and verify against submitted signature
         cipher = AES.new(
             sec_key,
             AES.MODE_CCM,
             nonce=self._get_nonce(),
             mac_len=4,
             msg_len=0,
-            assoc_len=len(self.input_data),
+            assoc_len=len(self._input_data),
         )
 
-        cipher.update(self.input_data)
+        cipher.update(self._input_data)
         try:
             cipher.verify(self.signature)
         except ValueError:
             return False
         return True
 
     def _get_nonce(self) -> bytes:
```

### Comparing `enocean_ble-0.1.0/enocean_ble/parser.py` & `enocean_ble-0.1.1/enocean_ble/parser.py`

 * *Files identical despite different names*

### Comparing `enocean_ble-0.1.0/pyproject.toml` & `enocean_ble-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "enocean-ble"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = [
     { name = "Christian Ohde", email = "christian.s1989@gmail.com" },
 ]
 dependencies = [
     "bleak>=0.20.2",
     "typer>=0.9.0",
```

### Comparing `enocean_ble-0.1.0/tests/test_decoder.py` & `enocean_ble-0.1.1/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `enocean_ble-0.1.0/PKG-INFO` & `enocean_ble-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enocean-ble
-Version: 0.1.0
+Version: 0.1.1
 Author-Email: Christian Ohde <christian.s1989@gmail.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: bleak>=0.20.2
 Requires-Dist: typer>=0.9.0
 Requires-Dist: bluetooth-sensor-state-data>=1.6.1
 Requires-Dist: bluetooth-data-tools>=1.2.0
```

