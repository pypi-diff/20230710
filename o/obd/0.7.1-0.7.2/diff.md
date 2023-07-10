# Comparing `tmp/obd-0.7.1.tar.gz` & `tmp/obd-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/obd-0.7.1.tar", last modified: Wed May 15 05:05:41 2019, max compression
+gzip compressed data, was "obd-0.7.2.tar", last modified: Mon Jul 10 03:14:36 2023, max compression
```

## Comparing `obd-0.7.1.tar` & `obd-0.7.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 brendan   (1000) brendan   (1000)        0 2019-05-15 05:05:41.000000 obd-0.7.1/
-drwxr-xr-x   0 brendan   (1000) brendan   (1000)        0 2019-05-15 05:05:41.000000 obd-0.7.1/obd.egg-info/
--rw-r--r--   0 brendan   (1000) brendan   (1000)        1 2019-05-15 05:05:41.000000 obd-0.7.1/obd.egg-info/not-zip-safe
--rw-r--r--   0 brendan   (1000) brendan   (1000)        1 2019-05-15 05:05:41.000000 obd-0.7.1/obd.egg-info/dependency_links.txt
--rw-r--r--   0 brendan   (1000) brendan   (1000)        4 2019-05-15 05:05:41.000000 obd-0.7.1/obd.egg-info/top_level.txt
--rw-r--r--   0 brendan   (1000) brendan   (1000)       26 2019-05-15 05:05:41.000000 obd-0.7.1/obd.egg-info/requires.txt
--rw-r--r--   0 brendan   (1000) brendan   (1000)      525 2019-05-15 05:05:41.000000 obd-0.7.1/obd.egg-info/SOURCES.txt
--rw-r--r--   0 brendan   (1000) brendan   (1000)     3014 2019-05-15 05:05:41.000000 obd-0.7.1/obd.egg-info/PKG-INFO
--rw-r--r--   0 brendan   (1000) brendan   (1000)     1161 2019-05-15 04:56:21.000000 obd-0.7.1/setup.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)       38 2019-05-15 05:05:41.000000 obd-0.7.1/setup.cfg
-drwxr-xr-x   0 brendan   (1000) brendan   (1000)        0 2019-05-15 05:05:41.000000 obd-0.7.1/obd/
--rw-r--r--   0 brendan   (1000) brendan   (1000)    20401 2019-05-15 02:24:25.000000 obd-0.7.1/obd/elm327.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)     6098 2019-05-15 02:24:25.000000 obd-0.7.1/obd/OBDResponse.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)     2856 2019-05-15 02:24:25.000000 obd-0.7.1/obd/__init__.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)    12335 2019-05-15 02:24:25.000000 obd-0.7.1/obd/obd.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)     6075 2019-05-15 02:24:25.000000 obd-0.7.1/obd/utils.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)   129662 2019-05-15 02:24:25.000000 obd-0.7.1/obd/codes.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)       22 2019-05-15 04:50:52.000000 obd-0.7.1/obd/__version__.py
-drwxr-xr-x   0 brendan   (1000) brendan   (1000)        0 2019-05-15 05:05:41.000000 obd-0.7.1/obd/protocols/
--rw-r--r--   0 brendan   (1000) brendan   (1000)    10992 2019-05-15 02:24:25.000000 obd-0.7.1/obd/protocols/protocol.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)     7164 2019-05-15 02:24:25.000000 obd-0.7.1/obd/protocols/protocol_legacy.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)     2705 2019-05-15 02:24:25.000000 obd-0.7.1/obd/protocols/__init__.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)     2519 2019-05-15 02:24:25.000000 obd-0.7.1/obd/protocols/protocol_unknown.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)    12348 2019-05-15 02:24:25.000000 obd-0.7.1/obd/protocols/protocol_can.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)     6615 2019-05-15 02:24:25.000000 obd-0.7.1/obd/OBDCommand.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)     7296 2019-05-15 02:24:25.000000 obd-0.7.1/obd/UnitsAndScaling.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)     9075 2019-05-15 02:24:25.000000 obd-0.7.1/obd/asynchronous.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)    12890 2019-05-15 02:24:25.000000 obd-0.7.1/obd/decoders.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)    35095 2019-05-15 02:24:25.000000 obd-0.7.1/obd/commands.py
--rw-r--r--   0 brendan   (1000) brendan   (1000)     1632 2018-11-05 06:20:40.000000 obd-0.7.1/README.md
--rw-r--r--   0 brendan   (1000) brendan   (1000)     3014 2019-05-15 05:05:41.000000 obd-0.7.1/PKG-INFO
+drwxr-xr-x   0 brendan   (1000) brendan   (1000)        0 2023-07-10 03:14:36.579970 obd-0.7.2/
+-rw-r--r--   0 brendan   (1000) brendan   (1000)    18027 2020-07-27 03:23:22.000000 obd-0.7.2/LICENSE
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     2771 2023-07-10 03:14:36.579970 obd-0.7.2/PKG-INFO
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     1990 2023-06-12 02:27:39.000000 obd-0.7.2/README.md
+drwxr-xr-x   0 brendan   (1000) brendan   (1000)        0 2023-07-10 03:14:36.578971 obd-0.7.2/obd/
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     6615 2020-07-27 03:23:34.000000 obd-0.7.2/obd/OBDCommand.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     6098 2020-07-27 03:23:34.000000 obd-0.7.2/obd/OBDResponse.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     7296 2020-07-27 03:23:34.000000 obd-0.7.2/obd/UnitsAndScaling.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     2856 2020-07-27 03:23:34.000000 obd-0.7.2/obd/__init__.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)       22 2023-07-10 03:07:43.000000 obd-0.7.2/obd/__version__.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     9075 2020-07-27 03:23:34.000000 obd-0.7.2/obd/asynchronous.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)   129662 2020-07-27 03:23:34.000000 obd-0.7.2/obd/codes.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)    37192 2023-06-12 02:27:39.000000 obd-0.7.2/obd/commands.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)    13759 2023-06-12 02:27:39.000000 obd-0.7.2/obd/decoders.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)    20970 2023-06-12 02:27:39.000000 obd-0.7.2/obd/elm327.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)    12335 2020-07-27 03:23:34.000000 obd-0.7.2/obd/obd.py
+drwxr-xr-x   0 brendan   (1000) brendan   (1000)        0 2023-07-10 03:14:36.579970 obd-0.7.2/obd/protocols/
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     2705 2020-07-27 03:23:34.000000 obd-0.7.2/obd/protocols/__init__.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)    11214 2023-06-12 02:27:39.000000 obd-0.7.2/obd/protocols/protocol.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)    12348 2020-07-27 03:23:34.000000 obd-0.7.2/obd/protocols/protocol_can.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     7164 2020-07-27 03:23:34.000000 obd-0.7.2/obd/protocols/protocol_legacy.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     2519 2020-07-27 03:23:34.000000 obd-0.7.2/obd/protocols/protocol_unknown.py
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     6075 2020-07-27 03:23:34.000000 obd-0.7.2/obd/utils.py
+drwxr-xr-x   0 brendan   (1000) brendan   (1000)        0 2023-07-10 03:14:36.578971 obd-0.7.2/obd.egg-info/
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     2771 2023-07-10 03:14:36.000000 obd-0.7.2/obd.egg-info/PKG-INFO
+-rw-r--r--   0 brendan   (1000) brendan   (1000)      533 2023-07-10 03:14:36.000000 obd-0.7.2/obd.egg-info/SOURCES.txt
+-rw-r--r--   0 brendan   (1000) brendan   (1000)        1 2023-07-10 03:14:36.000000 obd-0.7.2/obd.egg-info/dependency_links.txt
+-rw-r--r--   0 brendan   (1000) brendan   (1000)        1 2020-07-27 03:23:35.000000 obd-0.7.2/obd.egg-info/not-zip-safe
+-rw-r--r--   0 brendan   (1000) brendan   (1000)       27 2023-07-10 03:14:36.000000 obd-0.7.2/obd.egg-info/requires.txt
+-rw-r--r--   0 brendan   (1000) brendan   (1000)        4 2023-07-10 03:14:36.000000 obd-0.7.2/obd.egg-info/top_level.txt
+-rw-r--r--   0 brendan   (1000) brendan   (1000)       38 2023-07-10 03:14:36.579970 obd-0.7.2/setup.cfg
+-rw-r--r--   0 brendan   (1000) brendan   (1000)     1162 2023-07-10 03:07:48.000000 obd-0.7.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `obd-0.7.1/obd.egg-info/SOURCES.txt` & `obd-0.7.2/obd.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 obd/OBDCommand.py
 obd/OBDResponse.py
 obd/UnitsAndScaling.py
 obd/__init__.py
 obd/__version__.py
```

### Comparing `obd-0.7.1/setup.py` & `obd-0.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(
     name="obd",
-    version="0.7.1",
+    version="0.7.2",
     description=("Serial module for handling live sensor data from a vehicle's OBD-II port"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Operating System :: POSIX :: Linux",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Topic :: System :: Monitoring",
@@ -26,9 +26,9 @@
     author="Brendan Whitfield",
     author_email="brendanw@windworksdesign.com",
     url="http://github.com/brendan-w/python-OBD",
     license="GNU GPLv2",
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
-    install_requires=["pyserial==3.*", "pint==0.7.*"],
+    install_requires=["pyserial==3.*", "pint==0.20.*"],
 )
```

### Comparing `obd-0.7.1/obd/elm327.py` & `obd-0.7.2/obd/elm327.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,17 @@
             close()
             status()
             port_name()
             protocol_name()
             ecus()
     """
 
+    # chevron (ELM prompt character)
     ELM_PROMPT = b'>'
+    # an 'OK' which indicates we are entering low power state
     ELM_LP_ACTIVE = b'OK'
 
     _SUPPORTED_PROTOCOLS = {
         # "0" : None,
         # Automatic Mode. This isn't an actual protocol. If the
         # ELM reports this, then we don't have enough
         # information. see auto_protocol()
@@ -206,15 +208,17 @@
                 logger.error("Connected to the adapter, "
                              "but failed to connect to the vehicle")
 
     def set_protocol(self, protocol_):
         if protocol_ is not None:
             # an explicit protocol was specified
             if protocol_ not in self._SUPPORTED_PROTOCOLS:
-                logger.error("%s is not a valid protocol. Please use \"1\" through \"A\"")
+                logger.error(
+                    "{:} is not a valid protocol. ".format(protocol_) +
+                    "Please use \"1\" through \"A\"")
                 return False
             return self.manual_protocol(protocol_)
         else:
             # auto detect the protocol
             return self.auto_protocol()
 
     def manual_protocol(self, protocol_):
@@ -235,18 +239,18 @@
             If no protocol is specified, then protocols at tried with `ATTP`
 
             Upon success, the appropriate protocol parser is loaded,
             and this function returns True
         """
 
         # -------------- try the ELM's auto protocol mode --------------
-        r = self.__send(b"ATSP0")
+        r = self.__send(b"ATSP0", delay=1)
 
         # -------------- 0100 (first command, SEARCH protocols) --------------
-        r0100 = self.__send(b"0100")
+        r0100 = self.__send(b"0100", delay=1)
         if self.__has_message(r0100, "UNABLE TO CONNECT"):
             logger.error("Failed to query protocol 0100: unable to connect")
             return False
 
         # ------------------- ATDPN (list protocol number) -------------------
         r = self.__send(b"ATDPN")
         if len(r) != 1:
@@ -385,15 +389,15 @@
             is going to become active.
         """
 
         if self.__status == OBDStatus.NOT_CONNECTED:
             logger.info("cannot enter low power when unconnected")
             return None
 
-        lines = self.__send(b"ATLP", delay=1)
+        lines = self.__send(b"ATLP", delay=1, end_marker=self.ELM_LP_ACTIVE)
 
         if 'OK' in lines:
             logger.debug("Successfully entered low power mode")
             self.__low_power = True
         else:
             logger.debug("Failed to enter low power mode")
 
@@ -460,30 +464,39 @@
         if self.__low_power == True:
             self.normal_power()
 
         lines = self.__send(cmd)
         messages = self.__protocol(lines)
         return messages
 
-    def __send(self, cmd, delay=None):
+    def __send(self, cmd, delay=None, end_marker=ELM_PROMPT):
         """
             unprotected send() function
 
             will __write() the given string, no questions asked.
             returns result of __read() (a list of line strings)
-            after an optional delay.
+            after an optional delay, until the end marker (by
+            default, the prompt) is seen
         """
-
         self.__write(cmd)
 
+        delayed = 0.0
         if delay is not None:
             logger.debug("wait: %d seconds" % delay)
             time.sleep(delay)
+            delayed += delay
 
-        return self.__read()
+        r = self.__read(end_marker=end_marker)
+        while delayed < 1.0 and len(r) <= 0:
+            d = 0.1
+            logger.debug("no response; wait: %f seconds" % d)
+            time.sleep(d)
+            delayed += d
+            r = self.__read(end_marker=end_marker)
+        return r
 
     def __write(self, cmd):
         """
             "low-level" function to write a string to the port
         """
 
         if self.__port:
@@ -498,19 +511,20 @@
                 self.__port.close()
                 self.__port = None
                 logger.critical("Device disconnected while writing")
                 return
         else:
             logger.info("cannot perform __write() when unconnected")
 
-    def __read(self):
+    def __read(self, end_marker=ELM_PROMPT):
         """
             "low-level" read function
 
-            accumulates characters until the prompt character is seen
+            accumulates characters until the end marker (by
+            default, the prompt character) is seen
             returns a list of [/r/n] delimited strings
         """
         if not self.__port:
             logger.info("cannot perform __read() when unconnected")
             return []
 
         buffer = bytearray()
@@ -529,17 +543,16 @@
             # if nothing was received
             if not data:
                 logger.warning("Failed to read port")
                 break
 
             buffer.extend(data)
 
-            # end on chevron (ELM prompt character) or an 'OK' which
-            # indicates we are entering low power state
-            if self.ELM_PROMPT in buffer or self.ELM_LP_ACTIVE in buffer:
+            # end on specified end-marker sequence
+            if end_marker in buffer:
                 break
 
         # log, and remove the "bytearray(   ...   )" part
         logger.debug("read: " + repr(buffer)[10:-1])
 
         # clean out any null characters
         buffer = re.sub(b"\x00", b"", buffer)
```

### Comparing `obd-0.7.1/obd/OBDResponse.py` & `obd-0.7.2/obd/OBDResponse.py`

 * *Files identical despite different names*

### Comparing `obd-0.7.1/obd/__init__.py` & `obd-0.7.2/obd/__init__.py`

 * *Files identical despite different names*

### Comparing `obd-0.7.1/obd/obd.py` & `obd-0.7.2/obd/obd.py`

 * *Files identical despite different names*

### Comparing `obd-0.7.1/obd/utils.py` & `obd-0.7.2/obd/utils.py`

 * *Files identical despite different names*

### Comparing `obd-0.7.1/obd/codes.py` & `obd-0.7.2/obd/codes.py`

 * *Files identical despite different names*

### Comparing `obd-0.7.1/obd/protocols/protocol.py` & `obd-0.7.2/obd/protocols/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,20 @@
             car to determine the ECU layout.
         """
 
         # create the default, empty map
         # for example: self.TX_ID_ENGINE : ECU.ENGINE
         self.ecu_map = {}
 
+        if (self.TX_ID_ENGINE is not None):
+            self.ecu_map[self.TX_ID_ENGINE] = ECU.ENGINE
+
+        if (self.TX_ID_TRANSMISSION is not None):
+            self.ecu_map[self.TX_ID_TRANSMISSION] = ECU.TRANSMISSION
+
         # parse the 0100 data into messages
         # NOTE: at this point, their "ecu" property will be UNKNOWN
         messages = self(lines_0100)
 
         # read the messages and assemble the map
         # subsequent runs will now be tagged correctly
         self.populate_ecu_map(messages)
```

### Comparing `obd-0.7.1/obd/protocols/protocol_legacy.py` & `obd-0.7.2/obd/protocols/protocol_legacy.py`

 * *Files identical despite different names*

### Comparing `obd-0.7.1/obd/protocols/__init__.py` & `obd-0.7.2/obd/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `obd-0.7.1/obd/protocols/protocol_unknown.py` & `obd-0.7.2/obd/protocols/protocol_unknown.py`

 * *Files identical despite different names*

### Comparing `obd-0.7.1/obd/protocols/protocol_can.py` & `obd-0.7.2/obd/protocols/protocol_can.py`

 * *Files identical despite different names*

### Comparing `obd-0.7.1/obd/OBDCommand.py` & `obd-0.7.2/obd/OBDCommand.py`

 * *Files identical despite different names*

### Comparing `obd-0.7.1/obd/UnitsAndScaling.py` & `obd-0.7.2/obd/UnitsAndScaling.py`

 * *Files identical despite different names*

### Comparing `obd-0.7.1/obd/asynchronous.py` & `obd-0.7.2/obd/asynchronous.py`

 * *Files identical despite different names*

### Comparing `obd-0.7.1/obd/decoders.py` & `obd-0.7.2/obd/decoders.py`

 * *Files 7% similar despite different names*

```diff
@@ -90,14 +90,18 @@
 
 
 """
 General sensor decoders
 Return pint Quantities
 """
 
+def count(messages):
+    d = messages[0].data[2:]
+    v = bytes_to_int(d)
+    return v * Unit.count
 
 # 0 to 100 %
 def percent(messages):
     d = messages[0].data[2:]
     v = d[0]
     v = v * 100.0 / 255.0
     return v * Unit.percent
@@ -480,7 +484,32 @@
     for n in range(0, len(d), 9):
         # extract the 9 byte block, and parse a new MonitorTest
         test = parse_monitor_test(d[n:n + 9], mon)
         if test is not None:
             mon.add_test(test)
 
     return mon
+
+
+def encoded_string(length):
+    """ Extract an encoded string from multi-part messages """
+    return functools.partial(decode_encoded_string, length=length)
+
+
+def decode_encoded_string(messages, length):
+    d = messages[0].data[2:]
+
+    if len(d) < length:
+        logger.debug("Invalid string {}. Discarding...", d)
+        return None
+
+    # Encoded strings come in bundles of messages with leading null values to
+    # pad out the string to the next full message size. We strip off the
+    # leading null characters here and return the resulting string.
+    return d.strip().strip(b'\x00' b'\x01' b'\x02' b'\\x00' b'\\x01' b'\\x02')
+
+
+def cvn(messages):
+    d = decode_encoded_string(messages, 4)
+    if d is None:
+        return None
+    return bytes_to_hex(d)
```

### Comparing `obd-0.7.1/obd/commands.py` & `obd-0.7.2/obd/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,14 +275,35 @@
     OBDCommand("MONITOR_PM_FILTER_B2"        , "PM Filter Monitor Bank 2"                       , b"06B1",   0, monitor,               ECU.ALL,     False),
 ]
 
 __mode7__ = [
     OBDCommand("GET_CURRENT_DTC", "Get DTCs from the current/last driving cycle", b"07", 0, dtc, ECU.ALL, False),
 ]
 
+
+__mode9__ = [
+    #                      name                             description                            cmd     bytes       decoder       ECU        fast
+    OBDCommand("PIDS_9A"                    , "Supported PIDs [01-20]"                            , b"0900",  7, pid,                ECU.ALL,     True),
+    OBDCommand("VIN_MESSAGE_COUNT"          , "VIN Message Count"                                 , b"0901",  3, count,              ECU.ENGINE,  True),
+    OBDCommand("VIN"                        , "Vehicle Identification Number"                     , b"0902", 22, encoded_string(17), ECU.ENGINE,  True),
+    OBDCommand("CALIBRATION_ID_MESSAGE_COUNT","Calibration ID message count for PID 04"           , b"0903",  3, count,              ECU.ALL,     True),
+    OBDCommand("CALIBRATION_ID"             , "Calibration ID"                                    , b"0904", 18, encoded_string(16), ECU.ALL,     True),
+    OBDCommand("CVN_MESSAGE_COUNT"          , "CVN Message Count for PID 06"                      , b"0905",  3, count,              ECU.ALL,     True),
+    OBDCommand("CVN"                        , "Calibration Verification Numbers"                  , b"0906", 10, cvn,                ECU.ALL,     True),
+
+#
+# NOTE: The following are untested
+#
+#    OBDCommand("PERF_TRACKING_MESSAGE_COUNT", "Performance tracking message count"                , b"0907",  3, count,              ECU.ALL,     True),
+#    OBDCommand("PERF_TRACKING_SPARK"        , "In-use performance tracking (spark ignition)"      , b"0908",  4, raw_string,         ECU.ALL,     True),
+#    OBDCommand("ECU_NAME_MESSAGE_COUNT"     , "ECU Name Message Count for PID 0A"                 , b"0909",  3, count,              ECU.ALL,     True),
+#    OBDCommand("ECU_NAME"                   , "ECU Name"                                          , b"090a", 20, raw_string,         ECU.ALL,     True),
+#    OBDCommand("PERF_TRACKING_COMPRESSION"  , "In-use performance tracking (compression ignition)", b"090b",  4, raw_string,         ECU.ALL,     True),
+]
+
 __misc__ = [
     OBDCommand("ELM_VERSION", "ELM327 version string", b"ATI", 0, raw_string, ECU.UNKNOWN, False),
     OBDCommand("ELM_VOLTAGE", "Voltage detected by OBD-II adapter", b"ATRV", 0, elm_voltage, ECU.UNKNOWN, False),
 ]
 
 """
 Assemble the command tables by mode, and allow access by name
@@ -299,14 +320,15 @@
             __mode2__,
             __mode3__,
             __mode4__,
             [],
             __mode6__,
             __mode7__,
             [],
+            __mode9__,
         ]
 
         # allow commands to be accessed by name
         for m in self.modes:
             for c in m:
                 if c is not None:
                     self.__dict__[c.name] = c
@@ -346,14 +368,15 @@
     def base_commands(self):
         """
             returns the list of commands that should always be
             supported by the ELM327
         """
         return [
             self.PIDS_A,
+            self.PIDS_9A,
             self.MIDS_A,
             self.GET_DTC,
             self.CLEAR_DTC,
             self.GET_CURRENT_DTC,
             self.ELM_VERSION,
             self.ELM_VOLTAGE,
         ]
```

### Comparing `obd-0.7.1/README.md` & `obd-0.7.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -56,14 +56,26 @@
 -   Barometric Pressure
 -   Ambient air temperature
 -   Commanded throttle actuator
 -   Time run with MIL on
 -   Time since trouble codes cleared
 -   Hybrid battery pack remaining life
 -   Engine fuel rate
+-   Vehicle Identification Number (VIN)
+
+Common Issues
+-------------
+
+### Bluetooth OBD-II Adapters
+
+There are sometimes connection issues when using a Bluetooth OBD-II adapter with some devices (the Raspberry Pi is a common problem). This can be fixed by setting the following arguments when setting up the connection:
+
+```Python
+fast=False, timeout=30
+```
 
 License
 -------
 
 GNU GPL v2
 
 This library is forked from:
```

