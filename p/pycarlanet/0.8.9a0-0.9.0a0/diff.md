# Comparing `tmp/pycarlanet-0.8.9a0.tar.gz` & `tmp/pycarlanet-0.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycarlanet-0.8.9a0.tar", last modified: Fri Mar 10 11:01:38 2023, max compression
+gzip compressed data, was "pycarlanet-0.9.0a0.tar", last modified: Mon Jul 10 07:53:45 2023, max compression
```

## Comparing `pycarlanet-0.8.9a0.tar` & `pycarlanet-0.9.0a0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/pycarlanet/
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/pycarlanet/CarlanetActor.py
--rw-r--r--   0 runner    (1001) docker     (122)     7053 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/pycarlanet/CarlanetManager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/pycarlanet/EventListener.py
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/pycarlanet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/pycarlanet/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/pycarlanet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/pycarlanet/utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/pycarlanet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-03-10 11:01:38.000000 pycarlanet-0.8.9a0/pycarlanet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      402 2023-03-10 11:01:38.000000 pycarlanet-0.8.9a0/pycarlanet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-10 11:01:38.000000 pycarlanet-0.8.9a0/pycarlanet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-03-10 11:01:38.000000 pycarlanet-0.8.9a0/pycarlanet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-10 11:01:38.000000 pycarlanet-0.8.9a0/pycarlanet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     5759 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/tests/test_communication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 07:53:45.136344 pycarlanet-0.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1091 2023-07-10 07:53:33.000000 pycarlanet-0.9.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     7554 2023-07-10 07:53:45.136344 pycarlanet-0.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-07-10 07:53:33.000000 pycarlanet-0.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 07:53:45.136344 pycarlanet-0.9.0a0/pycarlanet/
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-07-10 07:53:33.000000 pycarlanet-0.9.0a0/pycarlanet/CarlanetActor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-07-10 07:53:33.000000 pycarlanet-0.9.0a0/pycarlanet/CarlanetEventListener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8052 2023-07-10 07:53:33.000000 pycarlanet-0.9.0a0/pycarlanet/CarlanetManager.py
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-10 07:53:33.000000 pycarlanet-0.9.0a0/pycarlanet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 07:53:45.136344 pycarlanet-0.9.0a0/pycarlanet/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-10 07:53:33.000000 pycarlanet-0.9.0a0/pycarlanet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-07-10 07:53:33.000000 pycarlanet-0.9.0a0/pycarlanet/utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 07:53:45.136344 pycarlanet-0.9.0a0/pycarlanet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7554 2023-07-10 07:53:45.000000 pycarlanet-0.9.0a0/pycarlanet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-07-10 07:53:45.000000 pycarlanet-0.9.0a0/pycarlanet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 07:53:45.000000 pycarlanet-0.9.0a0/pycarlanet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-10 07:53:45.000000 pycarlanet-0.9.0a0/pycarlanet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-10 07:53:45.000000 pycarlanet-0.9.0a0/pycarlanet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-10 07:53:45.136344 pycarlanet-0.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-07-10 07:53:33.000000 pycarlanet-0.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 07:53:45.136344 pycarlanet-0.9.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     6420 2023-07-10 07:53:33.000000 pycarlanet-0.9.0a0/tests/test_communication.py
```

### Comparing `pycarlanet-0.8.9a0/LICENSE` & `pycarlanet-0.9.0a0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Valerio Cislaghi
+Copyright (c) 2023 Valerio Cislaghi, Christian Quadri
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `pycarlanet-0.8.9a0/pycarlanet/CarlanetActor.py` & `pycarlanet-0.9.0a0/pycarlanet/CarlanetActor.py`

 * *Files identical despite different names*

### Comparing `pycarlanet-0.8.9a0/pycarlanet/CarlanetManager.py` & `pycarlanet-0.9.0a0/pycarlanet/CarlanetManager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,79 @@
 import abc
 import json
 import os
 import carla
 import zmq
+from carla.libcarla import World
 
-from pycarlanet import EventListener, SimulatorStatus
+from pycarlanet import CarlanetEventListener, SimulatorStatus
 from pycarlanet import CarlanetActor
 from pycarlanet.utils import preconditions
 
 
 class UnknownMessageCarlanetError(RuntimeError):
     def __init__(self, unknown_msg):
         self.unknown_msg = unknown_msg
 
     def __repr__(self) -> str:
         return "I don't know how to handle the following msg: " + self.unknown_msg['message_type']
 
 
+# .get_snapshot().timestamp.elapsed_seconds
 class CarlanetManager:
-    def __init__(self, listening_port, omnet_world_listener: EventListener, save_config_path=None):
+    def __init__(self, listening_port, omnet_world_listener: CarlanetEventListener, save_config_path=None,
+                 socket_options=None, log_messages=False):
         self._listening_port = listening_port
         self._omnet_world_listener = omnet_world_listener
         self._message_handler: MessageHandlerState = None
         self._carlanet_actors = dict()
+        self._log_messages = log_messages
         self._save_config_path = save_config_path
+        self.socket_options = socket_options if socket_options else {}
+        self.carla_world: World = None
 
     def _start_server(self):
         context = zmq.Context()
+        for opt_name, opt_value in self.socket_options.items():
+            context.setsockopt(opt_name, opt_value)
         self.socket = context.socket(zmq.REP)
         self.socket.setsockopt(zmq.CONFLATE, 1)
         self.socket.setsockopt(zmq.LINGER, 100)
         self.socket.bind(f"tcp://*:{self._listening_port}")
         print("server running")
 
     def _receive_data_from_omnet(self):
         message = self.socket.recv()
         json_data = json.loads(message.decode("utf-8"))
         self.timestamp = json_data['timestamp']
+        if self._log_messages:
+            print(f'Received msg: {json_data}\n')
         return json_data
 
     def start_simulation(self):
         self._start_server()
         self.set_message_handler_state(InitMessageHandlerState)
         try:
             while not isinstance(self._message_handler, FinishedMessageHandlerState):
                 msg = self._receive_data_from_omnet()
                 answer = self._message_handler.handle_message(msg)
                 self._send_data_to_omnet(answer)
-            self._omnet_world_listener.on_simulation_finished()
-
+            self._omnet_world_listener.simulation_finished(self._message_handler.simulator_status_code)
         except Exception as e:
-            self._omnet_world_listener.on_simulation_error(e)
+            self._omnet_world_listener.simulation_error(e)
         finally:
             self.socket.close()
 
     def _send_data_to_omnet(self, answer):
+        if self._log_messages:
+            print(f'Sending msg: {answer}\n')
         self.socket.send(json.dumps(answer).encode('utf-8'))
 
-    def set_message_handler_state(self, msg_handler_cls):
-        self._message_handler = msg_handler_cls(self)
+    def set_message_handler_state(self, msg_handler_cls, *args):
+        self._message_handler = msg_handler_cls(self, *args)
 
     def add_dynamic_actor(self, actor_id: str, carlanet_actor: CarlanetActor):
         """
         Used to create dynamically a new actor, both active and passive, and send its position to OMNeT
         :param actor_id:
         :param carlanet_actor:
         :return:
@@ -73,19 +84,22 @@
         """
         Remove actor from OMNeT world
         :param actor_id:
         :return:
         """
         del self._carlanet_actors[actor_id]
 
+    def get_curr_sim_timestamp(self):
+        return self.carla_world.get_snapshot().timestamp.elapsed_seconds
+
 
 class MessageHandlerState(abc.ABC):
     def __init__(self, carlanet_manager: CarlanetManager):
         self._manager = carlanet_manager
-        self.omnet_world_listener: EventListener = self._manager._omnet_world_listener
+        self.omnet_world_listener: CarlanetEventListener = self._manager._omnet_world_listener
         self._carlanet_actors = self._manager._carlanet_actors
 
     def handle_message(self, message):
         message_type = message['message_type']
         if hasattr(self, message_type):
             meth = getattr(self, message_type)
             return meth(message)
@@ -118,58 +132,70 @@
         if self._save_config_path:
             if not os.path.exists(self._save_config_path):
                 os.makedirs(self._save_config_path)
             with open(os.path.join(self._save_config_path, 'init.json'), 'w') as f:
                 json.dump(message, f)
 
     def INIT(self, message):
+
         self._save_config(message)
         res = dict()
         res['message_type'] = 'INIT_COMPLETED'
-        carla_timestamp, sim_status = self.omnet_world_listener.on_finished_creation_omnet_world(
+
+        sim_status, carla_world = self.omnet_world_listener.omnet_init_completed(
             run_id=message['run_id'],
-            seed=message['carla_configuration']['seed'],
-            carla_timestep=message['carla_configuration']['carla_timestep'],
-            sim_time_limit=message['carla_configuration']['sim_time_limit'],
-            custom_params=message['user_defined'])
+            carla_configuration=message['carla_configuration'],
+            user_defined=message['user_defined'])
+
+        self._manager.carla_world = carla_world
+
         for static_carlanet_actor in message['moving_actors']:
             actor_id = static_carlanet_actor['actor_id']
-            carla_timestamp, self._carlanet_actors[actor_id] = self.omnet_world_listener.on_static_actor_created(
+            self._carlanet_actors[actor_id] = self.omnet_world_listener.actor_created(
                 actor_id,
                 static_carlanet_actor['actor_type'],
                 static_carlanet_actor['actor_configuration']
             )
-        res['initial_timestamp'] = carla_timestamp
+
+        res['initial_timestamp'] = self._manager.get_curr_sim_timestamp()
         res['simulation_status'] = sim_status.value
-        res['actors_positions'] = self._generate_carla_nodes_positions()
+        res['actor_positions'] = self._generate_carla_nodes_positions()
+
+        self.omnet_world_listener.carla_init_completed()
+
         if sim_status == SimulatorStatus.RUNNING:
             self._manager.set_message_handler_state(RunningMessageHandlerState)
+
         return res
 
 
 class RunningMessageHandlerState(MessageHandlerState):
     def SIMULATION_STEP(self, message):
         res = dict()
+        self.omnet_world_listener.before_world_tick(message['timestamp'])
+        self._manager.carla_world.tick()
         res['message_type'] = 'UPDATED_POSITIONS'
-        sim_status = self.omnet_world_listener.on_carla_simulation_step(message['timestamp'])
+        sim_status = self.omnet_world_listener.carla_simulation_step(message['timestamp'])
         res['simulation_status'] = sim_status.value
-        res['actors_positions'] = self._generate_carla_nodes_positions()
+        res['actor_positions'] = self._generate_carla_nodes_positions()
         if sim_status != SimulatorStatus.RUNNING:
-            self._manager.set_message_handler_state(FinishedMessageHandlerState)
+            self._manager.set_message_handler_state(FinishedMessageHandlerState, sim_status)
         return res
 
     def GENERIC_MESSAGE(self, message):
         res = dict()
         res['message_type'] = 'GENERIC_RESPONSE'
-        sim_status, user_defined_response = self.omnet_world_listener.on_generic_message(message['timestamp'], message[
-            'user_defined_message'])
+        sim_status, user_defined_response = self.omnet_world_listener.generic_message(message['timestamp'], message[
+            'user_defined'])
 
         res['simulation_status'] = sim_status.value
-        res['user_defined_response'] = user_defined_response
+        res['user_defined'] = user_defined_response
 
         if sim_status != SimulatorStatus.RUNNING:
-            self._manager.set_message_handler_state(FinishedMessageHandlerState)
+            self._manager.set_message_handler_state(FinishedMessageHandlerState, sim_status)
         return res
 
 
 class FinishedMessageHandlerState(MessageHandlerState):
-    ...
+    def __init__(self, carlanet_manager: CarlanetManager, simulator_status_code: SimulatorStatus):
+        super().__init__(carlanet_manager)
+        self.simulator_status_code = simulator_status_code
```

### Comparing `pycarlanet-0.8.9a0/pycarlanet/EventListener.py` & `pycarlanet-0.9.0a0/pycarlanet/CarlanetEventListener.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,83 @@
 import abc
 import enum
 
 from pycarlanet import CarlanetActor
+from carla.libcarla import World
 
 """
 Listener for OMNeT world, note, every parameters gave as in input is a String, so eventually you need to use cast
 """
 
 
 class SimulatorStatus(enum.Enum):
     RUNNING = 0
     FINISHED_OK = 1
+    FINISHED_TIME_LIMIT = 2
     FINISHED_ERROR = -1
 
 
-class EventListener(abc.ABC):
+class CarlanetEventListener(abc.ABC):
 
-    def on_static_actor_created(self, actor_id: str, actor_type: str, actor_config) -> (float, CarlanetActor):
+    def omnet_init_completed(self, run_id, carla_configuration, user_defined) -> (SimulatorStatus, World):
         """
-        Callback called at the beginning of the simulation, OMNeT says which actors it has and communicate
+        :param run_id: id corresponding to the one in OMNeT++
+        :param carla_configuration:
+        :param user_defined:
+        :return: current carla world, current simulator status
+        """
+        ...
+
+    def actor_created(self, actor_id: str, actor_type: str, actor_config) -> CarlanetActor:
+        """
+        Called at the beginning of the simulation, OMNeT says which actors it has and communicate
         with carla to create those actors in the world
         :param actor_id:
         :param actor_type:
         :param actor_config:
-        :return: current carla world timestamp (see Snapshot class of CarlaAPI), new actor created from carlaWorld
+        :return: new actor created from carlaWorld
         """
         ...
         ##return Actor
 
-    def on_finished_creation_omnet_world(self, run_id, seed, carla_timestep, sim_time_limit, custom_params) -> (
-            float, SimulatorStatus):
+    def carla_init_completed(self):
+        """Called when the initialization of CARLA World is finished"""
+        ...
+
+    def before_world_tick(self, timestamp) -> None:
         """
-        :param run_id:
-        :param seed:
-        :param carla_timestep:
-        :param sim_time_limit:
-        :param custom_params:
-        :return: current carla world timestamp (see Snapshot class of CarlaAPI), current simulator status
+        Method called before a world tick called by OMNeT++
+        :param timestamp
+        :return: current simulator status
         """
         ...
 
-    def on_carla_simulation_step(self, timestamp) -> SimulatorStatus:
+    def carla_simulation_step(self, timestamp) -> SimulatorStatus:
         """
-        Method called every times OMNeT call simulation_step of Carla
+        Method called after a world tick called by OMNeT++
         :param timestamp
         :return: current simulator status
         """
         ...
 
-    def on_generic_message(self, timestamp, user_defined_message) -> (SimulatorStatus, dict):
+    def generic_message(self, timestamp, user_defined_message) -> (SimulatorStatus, dict):
         """
         :param timestamp:
         :param user_defined_message:
         :return: (current simulator status, dict contained custom parameters not None)
         """
         ...
 
-    def on_simulation_finished(self):
+    def simulation_finished(self, status_code: SimulatorStatus):
         """
         Callback called upon successful completion of the simulation
         :return:
         """
         ...
 
-    def on_simulation_error(self, exception):
+    def simulation_error(self, exception):
         """
 
         :param exception:
         :return:
         """
         ...
```

### Comparing `pycarlanet-0.8.9a0/pycarlanet/utils/decorators.py` & `pycarlanet-0.9.0a0/pycarlanet/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pycarlanet-0.8.9a0/setup.py` & `pycarlanet-0.9.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 import sys
 from pathlib import Path
 
 setup(
     name="pycarlanet",
     packages=find_packages(include=['pycarlanet', 'pycarlanet.utils']),
-    version="0.8.9-alpha",
+    version="0.9.0-alpha",
     long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type='text/markdown',
     author="Valerio Cislaghi, Christian Quadri",
     license='MIT',
     python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.9',
     install_requires=[
         'pyzmq==23.2.1',
```

### Comparing `pycarlanet-0.8.9a0/tests/test_communication.py` & `pycarlanet-0.9.0a0/tests/test_communication.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import json
 import multiprocessing
 import os
+import shutil
 from time import sleep
-from unittest.mock import MagicMock
+from unittest.mock import MagicMock, Mock, PropertyMock
 import pytest
 import carla
 import zmq
 
 import random
 
 from pycarlanet import CarlanetManager
 from pycarlanet import SimulatorStatus
 
 
 def test_creation_of_server():
-    port = random.randint(5000, 6000)
+    port = random.randint(5000, 8000)
 
     p = _start_server(port, None)
     assert p.is_alive()
     _end_server(p)
 
 
 def _create_init_listener():
@@ -30,65 +31,82 @@
 
     omnet_worl_listener.on_finished_creation_omnet_world.return_value = 10, SimulatorStatus.RUNNING
     omnet_worl_listener.on_static_actor_created.return_value = carla_actor
     return omnet_worl_listener
 
 
 def test_init_with_my_client():
-    port = random.randint(5000, 6000)
+    port = random.randint(5000, 8000)
 
     omnet_worl_listener = MagicMock()
+    omnet_worl_listener.carla_init_completed = MagicMock()
     carla_timestamp = random.randint(1, 100) / 100
 
+    omnet_world = MagicMock()
+    omnet_world.get_snapshot = MagicMock()
+    snapshot = MagicMock()
+    snapshot.timestamp.elapsed_seconds = carla_timestamp
+    omnet_world.get_snapshot.return_value = snapshot
+
+
     carla_actor = MagicMock()
     carla_actor.get_transform.return_value = carla.Transform(carla.Location(1, 2, 3), carla.Rotation(1, 2, 3))
     carla_actor.get_velocity.return_value = carla.Vector3D(1, 2, 3)
     # carla_actor.alive.return_value = True
     carla_actor.alive = True
-    omnet_worl_listener.on_finished_creation_omnet_world.return_value = carla_timestamp, SimulatorStatus.RUNNING
-    omnet_worl_listener.on_static_actor_created.return_value = carla_timestamp, carla_actor
+    omnet_worl_listener.omnet_init_completed.return_value = SimulatorStatus.RUNNING, omnet_world
+    omnet_worl_listener.actor_created.return_value = carla_actor
 
     p = _start_server(port, omnet_worl_listener)
     init_request = _read_request('init')
 
     s = _connect('localhost', port)
     _send_message(s, init_request)
     msg = _receive_message(s)  # omnet_worl_listener.on_finished_creation_omnet_world.assert_called_once()
+
     assert msg['initial_timestamp'] == carla_timestamp
-    assert msg['actors_positions'][0]['position'][0] == 1
+    assert msg['actor_positions'][0]['position'][0] == 1
+    # assert omnet_worl_listener.carla_init_completed.assert_called_once()
     # assert omnet_worl_listener.on_finished_creation_omnet_world.call_count == 1
     _end_server(p)
 
 
 def test_save_configuration():
-    port = random.randint(5000, 6000)
+    port = random.randint(5000, 8000)
     save_config_path = "tests/tmp"
 
     omnet_worl_listener = MagicMock()
     carla_timestamp = random.randint(1, 100) / 100
 
+    omnet_world = MagicMock()
+    omnet_world.get_snapshot = MagicMock()
+    snapshot = MagicMock()
+    snapshot.timestamp.elapsed_seconds = carla_timestamp
+    omnet_world.get_snapshot.return_value = snapshot
+
     carla_actor = MagicMock()
     carla_actor.get_transform.return_value = carla.Transform(carla.Location(1, 2, 3), carla.Rotation(1, 2, 3))
     carla_actor.get_velocity.return_value = carla.Vector3D(1, 2, 3)
     # carla_actor.alive.return_value = True
     carla_actor.alive = True
-    omnet_worl_listener.on_finished_creation_omnet_world.return_value = carla_timestamp, SimulatorStatus.RUNNING
-    omnet_worl_listener.on_static_actor_created.return_value = carla_timestamp, carla_actor
+    omnet_worl_listener.omnet_init_completed.return_value = SimulatorStatus.RUNNING, omnet_world
+    omnet_worl_listener.actor_created.return_value = carla_actor
 
     p = _start_server(port, omnet_worl_listener, save_config_path=save_config_path)
     init_request = _read_request('init')
     init_request['run_id'] = f'run{carla_timestamp}'
 
     s = _connect('localhost', port)
     _send_message(s, init_request)
     _ = _receive_message(s)  # omnet_worl_listener.on_finished_creation_omnet_world.assert_called_once()
 
-    with open(os.path.join(save_config_path, 'init.json'), 'r') as f:        # Load the JSON data into a Python object
+    with open(os.path.join(save_config_path, 'init.json'), 'r') as f:  # Load the JSON data into a Python object
         data = json.load(f)
         assert data == init_request
+    shutil.rmtree(save_config_path)
     # assert omnet_worl_listener.on_finished_creation_omnet_world.call_count == 1
     _end_server(p)
 
 
 # def test_init_with_omnet():
 #     omnet_worl_listener = MagicMock()
 #     carla_timestamp = 0.76
@@ -106,27 +124,32 @@
 
 def test_simulation_step_with_my_client():
     port = random.randint(5000, 6000)
 
     s = _connect('localhost', port)
     carla_timestamp = 0.76
 
+    omnet_world = MagicMock()
+    omnet_world.get_snapshot = MagicMock()
+    snapshot = MagicMock()
+    snapshot.timestamp.elapsed_seconds = carla_timestamp
+    omnet_world.get_snapshot.return_value = snapshot
+
     omnet_worl_listener = _create_init_listener()
-    omnet_worl_listener.on_carla_simulation_step.return_value = SimulatorStatus.RUNNING
-    # omnet_worl_listener.on_carla_simulation_step.return_value = carla_timestamp, SimulatorStatus.RUNNING
+    omnet_worl_listener.omnet_init_completed.return_value = SimulatorStatus.RUNNING, omnet_world
+    omnet_worl_listener.carla_simulation_step.return_value = SimulatorStatus.RUNNING
     p = _start_server(port, omnet_worl_listener)
     init_request = _read_request('init')
     init_request['moving_actors'] = []
     _send_message(s, init_request)
     _ = _receive_message(s)  # omnet_worl_listener.on_finished_creation_omnet_world.assert_called_once()
 
     simulation_step_request = _read_request('simulation_step')
     _send_message(s, simulation_step_request)
     msg = _receive_message(s)
-    # omnet_worl_listener.on_carla_simulation_step.assert_called_once()
     _end_server(p)
 
 
 def _start_server(port, omnet_world_listener, save_config_path=None):
     carlanet_manager = CarlanetManager(port, omnet_world_listener, save_config_path)
     p = multiprocessing.Process(target=carlanet_manager.start_simulation, args=())
     p.start()
```

