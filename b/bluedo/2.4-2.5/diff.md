# Comparing `tmp/bluedo-2.4.tar.gz` & `tmp/bluedo-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluedo-2.4.tar", last modified: Sun Jul  9 09:20:03 2023, max compression
+gzip compressed data, was "bluedo-2.5.tar", last modified: Mon Jul 10 17:44:40 2023, max compression
```

## Comparing `bluedo-2.4.tar` & `bluedo-2.5.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.991805 bluedo-2.4/
--rw-rw-r--   0 lars      (1000) lars      (1000)    35149 2022-11-05 18:15:30.000000 bluedo-2.4/LICENSE
--rw-rw-r--   0 lars      (1000) lars      (1000)      487 2022-11-05 18:15:30.000000 bluedo-2.4/MANIFEST.in
--rw-rw-r--   0 lars      (1000) lars      (1000)     4101 2023-07-09 09:20:03.991805 bluedo-2.4/PKG-INFO
--rw-rw-r--   0 lars      (1000) lars      (1000)     3181 2023-07-09 09:14:35.000000 bluedo-2.4/README.md
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.987805 bluedo-2.4/applications/
--rw-rw-r--   0 lars      (1000) lars      (1000)      251 2022-11-05 18:15:30.000000 bluedo-2.4/applications/bluedo.desktop
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.987805 bluedo-2.4/bluedo/
--rwxrwxr-x   0 lars      (1000) lars      (1000)      252 2022-11-04 22:23:57.000000 bluedo-2.4/bluedo/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2022-11-04 22:23:57.000000 bluedo-2.4/bluedo/bluedo.png
--rw-rw-r--   0 lars      (1000) lars      (1000)    27528 2023-07-09 09:16:36.000000 bluedo-2.4/bluedo/bluedoapp.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    79675 2022-11-04 22:23:57.000000 bluedo-2.4/bluedo/lock_animation.gif
--rw-rw-r--   0 lars      (1000) lars      (1000)     8631 2022-11-04 22:23:57.000000 bluedo-2.4/bluedo/unlocked.png
--rw-rw-r--   0 lars      (1000) lars      (1000)    21441 2023-07-07 23:38:29.000000 bluedo-2.4/bluedo/window.glade
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.991805 bluedo-2.4/bluedo.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)     4101 2023-07-09 09:20:03.000000 bluedo-2.4/bluedo.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      415 2023-07-09 09:20:03.000000 bluedo-2.4/bluedo.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-07-09 09:20:03.000000 bluedo-2.4/bluedo.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       40 2023-07-09 09:20:03.000000 bluedo-2.4/bluedo.egg-info/entry_points.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       48 2023-07-09 09:20:03.000000 bluedo-2.4/bluedo.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        7 2023-07-09 09:20:03.000000 bluedo-2.4/bluedo.egg-info/top_level.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)       38 2023-07-09 09:20:03.991805 bluedo-2.4/setup.cfg
--rw-rw-r--   0 lars      (1000) lars      (1000)     2313 2023-07-09 09:14:03.000000 bluedo-2.4/setup.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.987805 bluedo-2.4/share/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.987805 bluedo-2.4/share/icons/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.987805 bluedo-2.4/share/icons/hicolor/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.987805 bluedo-2.4/share/icons/hicolor/256x256/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.991805 bluedo-2.4/share/icons/hicolor/256x256/apps/
--rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2022-11-05 18:15:30.000000 bluedo-2.4/share/icons/hicolor/256x256/apps/bluedo.png
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-10 17:44:40.991999 bluedo-2.5/
+-rw-rw-r--   0 lars      (1000) lars      (1000)    35149 2020-09-10 12:34:08.000000 bluedo-2.5/LICENSE
+-rw-r--r--   0 lars      (1000) lars      (1000)      487 2021-08-29 08:11:16.000000 bluedo-2.5/MANIFEST.in
+-rw-rw-r--   0 lars      (1000) lars      (1000)     4370 2023-07-10 17:44:40.987999 bluedo-2.5/PKG-INFO
+-rw-rw-r--   0 lars      (1000) lars      (1000)     3450 2023-07-10 17:38:17.000000 bluedo-2.5/README.md
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-10 17:44:40.983998 bluedo-2.5/applications/
+-rw-rw-r--   0 lars      (1000) lars      (1000)      251 2020-09-22 18:04:05.000000 bluedo-2.5/applications/bluedo.desktop
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-10 17:44:40.987999 bluedo-2.5/bluedo/
+-rwxrwxr-x   0 lars      (1000) lars      (1000)      252 2020-09-30 09:35:02.000000 bluedo-2.5/bluedo/__init__.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2020-09-30 15:05:40.000000 bluedo-2.5/bluedo/bluedo.png
+-rw-rw-r--   0 lars      (1000) lars      (1000)    27528 2023-07-10 17:43:41.000000 bluedo-2.5/bluedo/bluedoapp.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    79675 2020-10-06 20:43:31.000000 bluedo-2.5/bluedo/lock_animation.gif
+-rw-rw-r--   0 lars      (1000) lars      (1000)      296 2020-10-12 15:26:21.000000 bluedo-2.5/bluedo/phonelink-white-18dp.svg
+-rw-rw-r--   0 lars      (1000) lars      (1000)      405 2020-10-12 15:26:53.000000 bluedo-2.5/bluedo/phonelink_off-white-18dp.svg
+-rw-rw-r--   0 lars      (1000) lars      (1000)     8631 2020-10-06 21:00:26.000000 bluedo-2.5/bluedo/unlocked.png
+-rw-rw-r--   0 lars      (1000) lars      (1000)    21441 2023-07-09 09:33:52.000000 bluedo-2.5/bluedo/window.glade
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-10 17:44:40.987999 bluedo-2.5/bluedo.egg-info/
+-rw-rw-r--   0 lars      (1000) lars      (1000)     4370 2023-07-10 17:44:40.000000 bluedo-2.5/bluedo.egg-info/PKG-INFO
+-rw-rw-r--   0 lars      (1000) lars      (1000)      501 2023-07-10 17:44:40.000000 bluedo-2.5/bluedo.egg-info/SOURCES.txt
+-rw-rw-r--   0 lars      (1000) lars      (1000)        1 2023-07-10 17:44:40.000000 bluedo-2.5/bluedo.egg-info/dependency_links.txt
+-rw-rw-r--   0 lars      (1000) lars      (1000)       40 2023-07-10 17:44:40.000000 bluedo-2.5/bluedo.egg-info/entry_points.txt
+-rw-rw-r--   0 lars      (1000) lars      (1000)       48 2023-07-10 17:44:40.000000 bluedo-2.5/bluedo.egg-info/requires.txt
+-rw-rw-r--   0 lars      (1000) lars      (1000)        7 2023-07-10 17:44:40.000000 bluedo-2.5/bluedo.egg-info/top_level.txt
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-10 17:44:40.987999 bluedo-2.5/images/
+-rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2020-09-30 15:05:40.000000 bluedo-2.5/images/bluedo.png
+-rw-rw-r--   0 lars      (1000) lars      (1000)       38 2023-07-10 17:44:40.991999 bluedo-2.5/setup.cfg
+-rw-rw-r--   0 lars      (1000) lars      (1000)     2313 2023-07-09 09:33:52.000000 bluedo-2.5/setup.py
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-10 17:44:40.979998 bluedo-2.5/share/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-10 17:44:40.979998 bluedo-2.5/share/icons/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-10 17:44:40.979998 bluedo-2.5/share/icons/hicolor/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-10 17:44:40.979998 bluedo-2.5/share/icons/hicolor/256x256/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-10 17:44:40.987999 bluedo-2.5/share/icons/hicolor/256x256/apps/
+-rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2020-09-30 15:05:40.000000 bluedo-2.5/share/icons/hicolor/256x256/apps/bluedo.png
```

### Comparing `bluedo-2.4/LICENSE` & `bluedo-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bluedo-2.4/PKG-INFO` & `bluedo-2.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluedo
-Version: 2.4
+Version: 2.5
 Summary: Bluetooth proximity automation
 Home-page: https://github.com/ways/BlueDo/
 Author: Lars Falk-Petersen
 Author-email: dev@falkp.no
 License: GPLv3+
 Keywords: bluetooth
 Platform: UNKNOWN
@@ -44,28 +44,36 @@
 # Installation
 
 ## From pip
 
     sudo apt install python3-pip gir1.2-appindicator3-0.1
     pip3 install --upgrade bluedo
 
+  Optional apt packages `playerctl` (pause music), `amixer` (for mute/unmute).
+
 ## From deb
 
     Fetch deb file from https://github.com/ways/BlueDo/releases
 
+## From source
+
+    sudo apt install python3-dev libbluetooth-dev playerctl libgirepository1.0-dev libcairo2-dev gir1.2-appindicator3-0.1
+
+Then install requirements: `pip install -r requirements.txt`
+
 # Requirements
 
 Use these system commands:
 
 * bluetoothctl
 * hcitool
 * loginctl
 * gsettings
-* amixer (if using mute)
-* playerctl (if using pause)
+* amixer (mute)
+* playerctl (pause music)
 
 Version > 2.0 is only tested on Ubuntu 22.04 with GNOME.
 
 Version < 2.0 is only tested on Ubuntu 20.04-21.04 with GNOME.
 
 # Command line options
```

### Comparing `bluedo-2.4/README.md` & `bluedo-2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,28 +18,36 @@
 # Installation
 
 ## From pip
 
     sudo apt install python3-pip gir1.2-appindicator3-0.1
     pip3 install --upgrade bluedo
 
+  Optional apt packages `playerctl` (pause music), `amixer` (for mute/unmute).
+
 ## From deb
 
     Fetch deb file from https://github.com/ways/BlueDo/releases
 
+## From source
+
+    sudo apt install python3-dev libbluetooth-dev playerctl libgirepository1.0-dev libcairo2-dev gir1.2-appindicator3-0.1
+
+Then install requirements: `pip install -r requirements.txt`
+
 # Requirements
 
 Use these system commands:
 
 * bluetoothctl
 * hcitool
 * loginctl
 * gsettings
-* amixer (if using mute)
-* playerctl (if using pause)
+* amixer (mute)
+* playerctl (pause music)
 
 Version > 2.0 is only tested on Ubuntu 22.04 with GNOME.
 
 Version < 2.0 is only tested on Ubuntu 20.04-21.04 with GNOME.
 
 # Command line options
```

### Comparing `bluedo-2.4/bluedo/bluedo.png` & `bluedo-2.5/bluedo/bluedo.png`

 * *Files identical despite different names*

### Comparing `bluedo-2.4/bluedo/bluedoapp.py` & `bluedo-2.5/bluedo/bluedoapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import syslog
 import appdirs
 import configparser
 
 
 class BlueDo(Gtk.Application):
     project_name = 'bluedo'
-    project_version = 2.4
+    project_version = 2.5
     config_path = appdirs.user_config_dir(project_name) + '/' + project_name + '.ini'
     config_section = 'CONFIG'
     run_path = os.path.dirname(os.path.realpath(__file__)) + '/'
     autostart_dir = os.getenv("HOME") + '/.config/autostart/'
 
     builder = None
     enabled = False
```

### Comparing `bluedo-2.4/bluedo/lock_animation.gif` & `bluedo-2.5/bluedo/lock_animation.gif`

 * *Files identical despite different names*

### Comparing `bluedo-2.4/bluedo/unlocked.png` & `bluedo-2.5/bluedo/unlocked.png`

 * *Files identical despite different names*

### Comparing `bluedo-2.4/bluedo/window.glade` & `bluedo-2.5/bluedo/window.glade`

 * *Files identical despite different names*

### Comparing `bluedo-2.4/bluedo.egg-info/PKG-INFO` & `bluedo-2.5/bluedo.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluedo
-Version: 2.4
+Version: 2.5
 Summary: Bluetooth proximity automation
 Home-page: https://github.com/ways/BlueDo/
 Author: Lars Falk-Petersen
 Author-email: dev@falkp.no
 License: GPLv3+
 Keywords: bluetooth
 Platform: UNKNOWN
@@ -44,28 +44,36 @@
 # Installation
 
 ## From pip
 
     sudo apt install python3-pip gir1.2-appindicator3-0.1
     pip3 install --upgrade bluedo
 
+  Optional apt packages `playerctl` (pause music), `amixer` (for mute/unmute).
+
 ## From deb
 
     Fetch deb file from https://github.com/ways/BlueDo/releases
 
+## From source
+
+    sudo apt install python3-dev libbluetooth-dev playerctl libgirepository1.0-dev libcairo2-dev gir1.2-appindicator3-0.1
+
+Then install requirements: `pip install -r requirements.txt`
+
 # Requirements
 
 Use these system commands:
 
 * bluetoothctl
 * hcitool
 * loginctl
 * gsettings
-* amixer (if using mute)
-* playerctl (if using pause)
+* amixer (mute)
+* playerctl (pause music)
 
 Version > 2.0 is only tested on Ubuntu 22.04 with GNOME.
 
 Version < 2.0 is only tested on Ubuntu 20.04-21.04 with GNOME.
 
 # Command line options
```

### Comparing `bluedo-2.4/setup.py` & `bluedo-2.5/setup.py`

 * *Files identical despite different names*

### Comparing `bluedo-2.4/share/icons/hicolor/256x256/apps/bluedo.png` & `bluedo-2.5/images/bluedo.png`

 * *Files identical despite different names*

