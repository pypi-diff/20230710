# Comparing `tmp/tud_sumo-1.2.0.tar.gz` & `tmp/tud_sumo-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tud_sumo-1.2.0.tar", last modified: Wed Jul  5 12:19:47 2023, max compression
+gzip compressed data, was "tud_sumo-1.2.1.tar", last modified: Mon Jul 10 12:41:08 2023, max compression
```

## Comparing `tud_sumo-1.2.0.tar` & `tud_sumo-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-05 12:19:47.466483 tud_sumo-1.2.0/
--rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.2.0/.gitattributes
--rw-r--r--   0 callumevans (50765939) 1653728465       78 2023-05-26 14:50:47.000000 tud_sumo-1.2.0/.gitignore
--rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.2.0/LICENSE
--rw-r--r--   0 callumevans (50765939) 1653728465     2849 2023-07-05 12:19:47.466357 tud_sumo-1.2.0/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465     1242 2023-05-26 14:58:45.000000 tud_sumo-1.2.0/README.md
--rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-07-05 12:17:49.000000 tud_sumo-1.2.0/pyproject.toml
--rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-07-05 12:19:47.466525 tud_sumo-1.2.0/setup.cfg
--rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.2.0/setup.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-05 12:19:47.465475 tud_sumo-1.2.0/tud_sumo/
--rw-r--r--   0 callumevans (50765939) 1653728465    18021 2023-07-05 12:08:53.000000 tud_sumo-1.2.0/tud_sumo/tud_sumo.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-05 12:19:47.466161 tud_sumo-1.2.0/tud_sumo.egg-info/
--rw-r--r--   0 callumevans (50765939) 1653728465     2849 2023-07-05 12:19:47.000000 tud_sumo-1.2.0/tud_sumo.egg-info/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465      247 2023-07-05 12:19:47.000000 tud_sumo-1.2.0/tud_sumo.egg-info/SOURCES.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-07-05 12:19:47.000000 tud_sumo-1.2.0/tud_sumo.egg-info/dependency_links.txt
--rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-07-05 12:19:47.000000 tud_sumo-1.2.0/tud_sumo.egg-info/requires.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-07-05 12:19:47.000000 tud_sumo-1.2.0/tud_sumo.egg-info/top_level.txt
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-10 12:41:08.392556 tud_sumo-1.2.1/
+-rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.2.1/.gitattributes
+-rw-r--r--   0 callumevans (50765939) 1653728465       78 2023-05-26 14:50:47.000000 tud_sumo-1.2.1/.gitignore
+-rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.2.1/LICENSE
+-rw-r--r--   0 callumevans (50765939) 1653728465     4843 2023-07-10 12:41:08.392414 tud_sumo-1.2.1/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465     3236 2023-07-10 12:40:39.000000 tud_sumo-1.2.1/README.md
+-rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-07-10 12:38:40.000000 tud_sumo-1.2.1/pyproject.toml
+-rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-07-10 12:41:08.392600 tud_sumo-1.2.1/setup.cfg
+-rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.2.1/setup.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-10 12:41:08.391305 tud_sumo-1.2.1/tud_sumo/
+-rw-r--r--   0 callumevans (50765939) 1653728465    18624 2023-07-10 12:12:30.000000 tud_sumo-1.2.1/tud_sumo/tud_sumo.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-10 12:41:08.392208 tud_sumo-1.2.1/tud_sumo.egg-info/
+-rw-r--r--   0 callumevans (50765939) 1653728465     4843 2023-07-10 12:41:08.000000 tud_sumo-1.2.1/tud_sumo.egg-info/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465      247 2023-07-10 12:41:08.000000 tud_sumo-1.2.1/tud_sumo.egg-info/SOURCES.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-07-10 12:41:08.000000 tud_sumo-1.2.1/tud_sumo.egg-info/dependency_links.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-07-10 12:41:08.000000 tud_sumo-1.2.1/tud_sumo.egg-info/requires.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-07-10 12:41:08.000000 tud_sumo-1.2.1/tud_sumo.egg-info/top_level.txt
```

### Comparing `tud_sumo-1.2.0/LICENSE` & `tud_sumo-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tud_sumo-1.2.0/pyproject.toml` & `tud_sumo-1.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tud_sumo"
-version = "1.2.0"
+version = "1.2.1"
 description = "TU Delft SUMO wrapper"
 readme = "README.md"
 authors = [{ name = "Callum Evans", email = "c.evans@tudelft.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `tud_sumo-1.2.0/tud_sumo/tud_sumo.py` & `tud_sumo-1.2.1/tud_sumo/tud_sumo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-
-import os, sys, traci, json, warnings, math
+import os, sys, traci, json, math
 from functools import reduce
 from tqdm import tqdm
 from random import randint
 from copy import copy
+from warnings import warn
 import matplotlib.pyplot as plt
 
 class Simulation:
     def __init__(self, main_junction = None, verbose = False) -> None:
         path_tools = os.path.join(os.environ.get("SUMO_HOME"), 'tools')
 
         if path_tools in sys.path: pass
@@ -20,14 +20,15 @@
         self.junc_phases = None
         self.def_junc = main_junction
 
         self.available_detectors = {}
         self.step_length = 0.5
 
         self.get_individual_vehicle_data = True
+        self.all_curr_vehicle_ids = []
         self.known_vehicles = {}
         self.light_changes = 0
 
     def start(self, config_file = None, net_file = None, route_file = None, add_file = None, cmd_options = None, step_len = None, warnings = False, gui = False) -> None:
         """
         Intialises SUMO simulation.
         :param config_file: Location of '.sumocfg' file (can be given instead of net_file)
@@ -76,20 +77,20 @@
         
         return True
 
     def end(self):
         traci.close()
         self.running = False
 
-    def step_to(self, end_step = None, n_steps = None, sim_dur = None, n_light_changes = None, detector_list = None, prev_data = None, vTypes = None, cumulative_data = False) -> dict:
+    def step_through(self, n_steps = 1, end_step = None, sim_dur = None, n_light_changes = None, detector_list = None, prev_data = None, vTypes = None, cumulative_data = False) -> dict:
         """
         Step through simulation from the current time until end_step, aggregating
         data during this period.
-        :param end_step:        End point for stepping through simulation
-        :param n_steps:         Perform n steps of the simulation (given instead of end_steps)
+        :param n_steps:         Perform n steps of the simulation (defaults to 1)
+        :param end_step:        End point for stepping through simulation (given instead of end_step)
         :param sim_dur:         Simulation duration
         :param n_light_changes: Run for n light changes (across all junctions)
         :param detector_list:   List of detector IDs to collect data from (defaults to all)
         :param prev_data:       If given, new data is appended to this dictionary
         :param vTypes:          Vehicle type(s) to collect data of (list of types or string, defaults to all)
         :param cumulative_data: Denotes whether to get cumulative veh count and TTS values
         :return dict:           All data collected through the time period, separated by detector
@@ -97,15 +98,15 @@
 
         if detector_list == None: detector_list = list(self.available_detectors.keys())
         start_time = self.curr_step
 
         if end_step == None and n_steps != None: end_step = self.curr_step + n_steps
         elif end_step == None and sim_dur != None: end_step = self.curr_step + (sim_dur / self.step_length)
         elif end_step == None and n_light_changes != None: end_step, init_changes = math.inf, self.light_changes
-        elif end_step == None: raise ValueError("No time value given for step_to() function.")
+        elif end_step == None: raise ValueError("No time value given for step_through() function.")
 
         if prev_data == None:
             prev_steps, all_data = 0, {"data": {"detector": {}, "vehicle": {}, "all_vehicles": []}, "step_len": self.step_length, "start": start_time}
         else: 
             prev_steps = set([len(data_arr) for data_arr in prev_data["data"]["vehicle"].values()] +
                             [len(detector_data["speeds"]) for detector_data in prev_data["data"]["detector"].values()] +
                             [len(detector_data["veh_counts"]) for detector_data in prev_data["data"]["detector"].values()])
@@ -159,14 +160,16 @@
 
         data = {"detector": {}, "vehicle": {}}
         
         traci.simulationStep()
         time_diff = traci.simulation.getTime() - self.time_val
         self.time_val = traci.simulation.getTime()
 
+        self.all_curr_vehicle_ids = list(traci.vehicle.getIDList())
+
         if self.junc_phases != None:
             update_junc_lights = []
             for junction_id, phases in self.junc_phases.items():
                 phases["curr_time"] += time_diff
                 if phases["curr_time"] >= phases["cycle_len"]:
                     phases["curr_time"] = 0
                     phases["curr_phase"] = 0
@@ -185,15 +188,15 @@
                 data["detector"][detector_id]["speeds"] = traci.multientryexit.getLastStepMeanSpeed(detector_id)
                 data["detector"][detector_id]["veh_counts"] = traci.multientryexit.getLastStepVehicleNumber(detector_id)
             elif self.available_detectors[detector_id] == "inductionloop":
                 data["detector"][detector_id]["speeds"] = traci.inductionloop.getLastStepMeanSpeed(detector_id)
                 data["detector"][detector_id]["veh_counts"] = traci.inductionloop.getLastStepVehicleNumber(detector_id)
                 data["detector"][detector_id]["occupancies"] = traci.inductionloop.getLastStepOccupancy(detector_id)
             else:
-                print("Warning: Unknown detector type '"+self.available_detectors[detector_id]+"'")
+                warn("Warning: Unknown detector type '"+self.available_detectors[detector_id]+"'")
 
         total_v_data, all_v_data = self.get_all_vehicle_data(types=vTypes)
         data["vehicle"]["no_vehicles"] = total_v_data["no_vehicles"]
         data["vehicle"]["tts"] = total_v_data["no_vehicles"] * self.step_length
         data["vehicle"]["delay"] = total_v_data["no_waiting"] * self.step_length
 
         self.curr_step += 1
@@ -262,14 +265,21 @@
             self.light_changes += 1
             new_phase = self.junc_phases[junction_id]["phases"][self.junc_phases[junction_id]["curr_phase"]].lower()
             if '-' in new_phase:
                 new_phase = new_phase.split()
                 new_phase = "".join([new_phase[i] if new_phase[i] != '-' else curr_setting[i] for i in range(len(new_phase))])
             traci.trafficlight.setRedYellowGreenState(junction_id, new_phase)
 
+    def vehicle_exists(self, vehicle_id):
+        """
+        Tests if vehicle exists in the network
+        :return bool: True if ID in list of current vehicle IDs 
+        """
+        return vehicle_id in self.all_curr_vehicle_ids
+
     def get_last_step_vehicles(self, detector_ids = None) -> dict:
         """
         Get the IDs of vehicles that passed over the specified detectors
         :param detector_ids: detector ID or list of detector IDs (defaults to all)
         :return dict: Dict containing vehicle IDs for each detector
         """
 
@@ -283,73 +293,76 @@
             detector_type = self.available_detectors[detector_id]
 
             if detector_type == "inductionloop":
                 vehicle_ids[detector_id] = list(traci.inductionloop.getLastStepVehicleIDs(detector_id))
             elif detector_type == "multientryexit":
                 vehicle_ids[detector_id] = list(traci.multientryexit.getLastStepVehicleIDs(detector_id))
             else:
-                print("Warning: Unknown detector type '"+detector_type+"'")
+                warn("Warning: Unknown detector type '"+detector_type+"'")
 
         return vehicle_ids
     
     def get_vehicle_data(self, vehicle_id, vehicle_type = None):
         """
         Get data for specified vehicle, updating known_vehicles dict
         :param vehicle_id: vehicle ID
         :param vehicle_type: Vehicle type if known
-        :return dict: Vehicle data dictionary
+        :return dict: Vehicle data dictionary, returns None if does not exist in simulation
         """
 
+        if vehicle_id not in self.all_curr_vehicle_ids: return None
+
         if vehicle_type == None:
             if "cbikes" in vehicle_id: vehicle_type = "cbikes"
             elif "bikes" in vehicle_id: vehicle_type = "bikes"
             else: vehicle_type = "cars"
 
         speed = traci.vehicle.getSpeed(vehicle_id)
         lon, lat, alt = traci.vehicle.getPosition3D(vehicle_id)
+        heading, ts = traci.vehicle.getAngle(vehicle_id), traci.vehicle.getDeparture(vehicle_id)
 
         if vehicle_id not in self.known_vehicles.keys():
-            self.known_vehicles[vehicle_id] = {"type": vehicle_type,
+            self.known_vehicles[vehicle_id] = {"type":      vehicle_type,
                                                "longitude": lon,
-                                               "latitude": lat,
-                                               "speed": speed,
-                                               "length": traci.vehicle.getLength(vehicle_id),
-                                               "heading": traci.vehicle.getAngle(vehicle_id),
-                                               "ts": traci.vehicle.getDeparture(vehicle_id),
-                                               "altitude": alt,
+                                               "latitude":  lat,
+                                               "speed":     speed,
+                                               "length":    traci.vehicle.getLength(vehicle_id),
+                                               "heading":   heading,
+                                               "ts":        ts,
+                                               "altitude":  alt,
                                                "last_seen": self.curr_step
                                               }
         else:
-            self.known_vehicles[vehicle_id]["speed"] = speed
+            self.known_vehicles[vehicle_id]["speed"]     = speed
             self.known_vehicles[vehicle_id]["longitude"] = lon
-            self.known_vehicles[vehicle_id]["latitude"] = lat
-            self.known_vehicles[vehicle_id]["altitude"] = alt
+            self.known_vehicles[vehicle_id]["latitude"]  = lat
+            self.known_vehicles[vehicle_id]["heading"]   = heading
+            self.known_vehicles[vehicle_id]["ts"]        = ts
+            self.known_vehicles[vehicle_id]["altitude"]  = alt
             self.known_vehicles[vehicle_id]["last_seen"] = self.curr_step
 
         vehicle_data = copy(self.known_vehicles[vehicle_id])
         del vehicle_data['last_seen']
 
         return vehicle_data
 
-    def get_all_vehicle_data(self, ids = None, types = None, type_from_id = True) -> dict:
+    def get_all_vehicle_data(self, types = None, type_from_id = True) -> dict:
         """
         Collects vehicle data from SUMO, by id and/or type (defaults to all vehicles)
-        :param ids: IDs of vehicles to fetch
         :param types: Type(s) of vehicles to fetch
         :return dict: Vehicle data by id
         """
-        if ids == None: ids = list(traci.vehicle.getIDList())
 
         all_vehicle_data = {}
         total_vehicle_data = {"no_vehicles": 0, "no_waiting": 0}
 
-        for vehicle_id in ids:
+        for vehicle_id in self.all_curr_vehicle_ids:
 
             # Saving known vehicles reduces calls to traci by not
-            # fetching already known data
+            # fetching already known (& unchanging!) data
             if vehicle_id in self.known_vehicles.keys(): vehicle_type = self.known_vehicles[vehicle_id]["type"]
             else:
                 vehicle_type = traci.vehicle.getVehicleClass(vehicle_id)
 
             if types is None or (isinstance(types, list) and vehicle_type in types) or (isinstance(types, str) and vehicle_type == types):
 
                 if self.get_individual_vehicle_data: vehicle_data = self.get_vehicle_data(vehicle_id, vehicle_type)
```

