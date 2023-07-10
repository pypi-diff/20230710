# Comparing `tmp/Pysor-0.1.tar.gz` & `tmp/pysor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pysor-0.1.tar", last modified: Sun Jul  9 19:00:31 2023, max compression
+gzip compressed data, was "pysor-0.1.1.tar", last modified: Mon Jul 10 14:55:25 2023, max compression
```

## Comparing `Pysor-0.1.tar` & `pysor-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 19:00:31.090345 Pysor-0.1/
--rw-rw-rw-   0        0        0     1090 2023-06-18 19:48:38.000000 Pysor-0.1/LICENSE
--rw-rw-rw-   0        0        0     4058 2023-07-09 19:00:31.089346 Pysor-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-09 19:00:31.050639 Pysor-0.1/Pysor.egg-info/
--rw-rw-rw-   0        0        0     4058 2023-07-09 19:00:30.000000 Pysor-0.1/Pysor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1083 2023-07-09 19:00:30.000000 Pysor-0.1/Pysor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 19:00:30.000000 Pysor-0.1/Pysor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-09 19:00:30.000000 Pysor-0.1/Pysor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-09 19:00:30.000000 Pysor-0.1/Pysor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3348 2023-06-27 13:44:12.000000 Pysor-0.1/README.md
--rw-rw-rw-   0        0        0      516 2023-06-24 16:00:23.000000 Pysor-0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-09 19:00:31.054643 Pysor-0.1/sensor_simulation/
--rw-rw-rw-   0        0        0      207 2023-06-20 22:46:01.000000 Pysor-0.1/sensor_simulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:00:31.057599 Pysor-0.1/sensor_simulation/config/
--rw-rw-rw-   0        0        0        0 2023-06-20 02:27:31.000000 Pysor-0.1/sensor_simulation/config/__init__.py
--rw-rw-rw-   0        0        0      799 2023-06-20 23:14:27.000000 Pysor-0.1/sensor_simulation/config/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:00:31.060599 Pysor-0.1/sensor_simulation/config/parsers/
--rw-rw-rw-   0        0        0       97 2023-06-20 02:27:31.000000 Pysor-0.1/sensor_simulation/config/parsers/__init__.py
--rw-rw-rw-   0        0        0     1158 2023-06-24 15:47:22.000000 Pysor-0.1/sensor_simulation/config/parsers/toml_parser.py
--rw-rw-rw-   0        0        0     2094 2023-07-09 15:41:40.000000 Pysor-0.1/sensor_simulation/mqtt_client.py
--rw-rw-rw-   0        0        0     1527 2023-07-09 16:32:55.000000 Pysor-0.1/sensor_simulation/sensor_manager.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:00:31.072770 Pysor-0.1/sensor_simulation/sensors/
--rw-rw-rw-   0        0        0      374 2023-06-26 14:40:37.000000 Pysor-0.1/sensor_simulation/sensors/__init__.py
--rw-rw-rw-   0        0        0     1798 2023-07-09 15:50:34.000000 Pysor-0.1/sensor_simulation/sensors/base_sensor.py
--rw-rw-rw-   0        0        0     1558 2023-06-22 14:42:21.000000 Pysor-0.1/sensor_simulation/sensors/humidity_sensor.py
--rw-rw-rw-   0        0        0     1786 2023-06-22 14:42:02.000000 Pysor-0.1/sensor_simulation/sensors/light_intensity_sensor.py
--rw-rw-rw-   0        0        0     1366 2023-06-26 14:43:13.000000 Pysor-0.1/sensor_simulation/sensors/ph_sensor.py
--rw-rw-rw-   0        0        0     1717 2023-06-22 14:42:21.000000 Pysor-0.1/sensor_simulation/sensors/temperature_sensor.py
--rw-rw-rw-   0        0        0     1403 2023-06-22 14:42:21.000000 Pysor-0.1/sensor_simulation/sensors/water_level_sensor.py
--rw-rw-rw-   0        0        0       42 2023-07-09 19:00:31.090345 Pysor-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2023-07-09 18:54:57.000000 Pysor-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:00:31.075538 Pysor-0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-06-20 15:06:16.000000 Pysor-0.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:00:31.077990 Pysor-0.1/tests/config/
--rw-rw-rw-   0        0        0        0 2023-06-24 15:00:42.000000 Pysor-0.1/tests/config/__init__.py
--rw-rw-rw-   0        0        0     1978 2023-06-24 15:53:07.000000 Pysor-0.1/tests/config/test_parser.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:00:31.087341 Pysor-0.1/tests/sensors/
--rw-rw-rw-   0        0        0        0 2023-06-20 15:08:31.000000 Pysor-0.1/tests/sensors/__init__.py
--rw-rw-rw-   0        0        0     1838 2023-07-09 16:36:50.000000 Pysor-0.1/tests/sensors/test_humidity_sensor.py
--rw-rw-rw-   0        0        0     2042 2023-07-09 16:36:47.000000 Pysor-0.1/tests/sensors/test_light_intensity_sensor.py
--rw-rw-rw-   0        0        0     1692 2023-07-09 16:36:39.000000 Pysor-0.1/tests/sensors/test_ph_sensor.py
--rw-rw-rw-   0        0        0     5127 2023-07-09 16:36:18.000000 Pysor-0.1/tests/sensors/test_temperature_sensor.py
--rw-rw-rw-   0        0        0     1912 2023-07-09 16:36:35.000000 Pysor-0.1/tests/sensors/test_water_level_sensor.py
--rw-rw-rw-   0        0        0     3299 2023-07-09 16:29:59.000000 Pysor-0.1/tests/test_sensor_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:55:25.268413 pysor-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-06-18 19:48:38.000000 pysor-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3845 2023-07-10 14:55:25.267407 pysor-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-10 14:55:25.220803 pysor-0.1.1/Pysor.egg-info/
+-rw-rw-rw-   0        0        0     3845 2023-07-10 14:55:25.000000 pysor-0.1.1/Pysor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1227 2023-07-10 14:55:25.000000 pysor-0.1.1/Pysor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 14:55:25.000000 pysor-0.1.1/Pysor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-10 14:55:25.000000 pysor-0.1.1/Pysor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-10 14:55:25.000000 pysor-0.1.1/Pysor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3135 2023-07-10 14:52:23.000000 pysor-0.1.1/README.md
+-rw-rw-rw-   0        0        0      516 2023-06-24 16:00:23.000000 pysor-0.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-10 14:55:25.228224 pysor-0.1.1/sensor_simulation/
+-rw-rw-rw-   0        0        0      207 2023-06-20 22:46:01.000000 pysor-0.1.1/sensor_simulation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:55:25.230262 pysor-0.1.1/sensor_simulation/config/
+-rw-rw-rw-   0        0        0        0 2023-06-20 02:27:31.000000 pysor-0.1.1/sensor_simulation/config/__init__.py
+-rw-rw-rw-   0        0        0      799 2023-06-20 23:14:27.000000 pysor-0.1.1/sensor_simulation/config/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:55:25.233803 pysor-0.1.1/sensor_simulation/config/parsers/
+-rw-rw-rw-   0        0        0       97 2023-06-20 02:27:31.000000 pysor-0.1.1/sensor_simulation/config/parsers/__init__.py
+-rw-rw-rw-   0        0        0     1158 2023-06-24 15:47:22.000000 pysor-0.1.1/sensor_simulation/config/parsers/toml_parser.py
+-rw-rw-rw-   0        0        0     2094 2023-07-09 15:41:40.000000 pysor-0.1.1/sensor_simulation/mqtt_client.py
+-rw-rw-rw-   0        0        0     1527 2023-07-09 16:32:55.000000 pysor-0.1.1/sensor_simulation/sensor_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:55:25.248418 pysor-0.1.1/sensor_simulation/sensors/
+-rw-rw-rw-   0        0        0      374 2023-06-26 14:40:37.000000 pysor-0.1.1/sensor_simulation/sensors/__init__.py
+-rw-rw-rw-   0        0        0     1798 2023-07-09 15:50:34.000000 pysor-0.1.1/sensor_simulation/sensors/base_sensor.py
+-rw-rw-rw-   0        0        0     1558 2023-06-22 14:42:21.000000 pysor-0.1.1/sensor_simulation/sensors/humidity_sensor.py
+-rw-rw-rw-   0        0        0     1786 2023-06-22 14:42:02.000000 pysor-0.1.1/sensor_simulation/sensors/light_intensity_sensor.py
+-rw-rw-rw-   0        0        0     1366 2023-06-26 14:43:13.000000 pysor-0.1.1/sensor_simulation/sensors/ph_sensor.py
+-rw-rw-rw-   0        0        0     1717 2023-06-22 14:42:21.000000 pysor-0.1.1/sensor_simulation/sensors/temperature_sensor.py
+-rw-rw-rw-   0        0        0     1403 2023-06-22 14:42:21.000000 pysor-0.1.1/sensor_simulation/sensors/water_level_sensor.py
+-rw-rw-rw-   0        0        0       42 2023-07-10 14:55:25.268413 pysor-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2023-07-10 14:43:47.000000 pysor-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:55:25.251922 pysor-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-20 15:06:16.000000 pysor-0.1.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:55:25.254926 pysor-0.1.1/tests/config/
+-rw-rw-rw-   0        0        0        0 2023-06-24 15:00:42.000000 pysor-0.1.1/tests/config/__init__.py
+-rw-rw-rw-   0        0        0     1978 2023-06-24 15:53:07.000000 pysor-0.1.1/tests/config/test_parser.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:55:25.265837 pysor-0.1.1/tests/sensors/
+-rw-rw-rw-   0        0        0        0 2023-06-20 15:08:31.000000 pysor-0.1.1/tests/sensors/__init__.py
+-rw-rw-rw-   0        0        0     1838 2023-07-09 16:36:50.000000 pysor-0.1.1/tests/sensors/test_humidity_sensor.py
+-rw-rw-rw-   0        0        0     2042 2023-07-09 16:36:47.000000 pysor-0.1.1/tests/sensors/test_light_intensity_sensor.py
+-rw-rw-rw-   0        0        0     1692 2023-07-09 16:36:39.000000 pysor-0.1.1/tests/sensors/test_ph_sensor.py
+-rw-rw-rw-   0        0        0     5127 2023-07-09 16:36:18.000000 pysor-0.1.1/tests/sensors/test_temperature_sensor.py
+-rw-rw-rw-   0        0        0     1912 2023-07-09 16:36:35.000000 pysor-0.1.1/tests/sensors/test_water_level_sensor.py
+-rw-rw-rw-   0        0        0     3299 2023-07-09 16:29:59.000000 pysor-0.1.1/tests/test_sensor_manager.py
```

### Comparing `Pysor-0.1/LICENSE` & `pysor-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/PKG-INFO` & `pysor-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Pysor
-Version: 0.1
+Name: pysor
+Version: 0.1.1
 Summary: A Python package for sensor simulations
 Home-page: https://github.com/CodeSwallow/pysor
 Author: Isai Ramirez
 Author-email: isai.ramirez.stamaria15@gmail.com
 License: MIT
 Keywords: mqtt sensor simulation
 Classifier: Development Status :: 3 - Alpha
@@ -23,45 +23,54 @@
 </div>
 
 <div align="center">
 <img src="https://github.com/CodeSwallow/pysor/actions/workflows/python-package.yml/badge.svg" alt="workflow status"/>
 <img src="artwork/coverage.svg" alt="coverage"/>
 </div>
 
-Pysor is a Python library for the simulation of various sensors. It is designed to be used with the broker of your choice.
-It uses the Paho MQTT library to communicate with the broker.
+Pysor is a Python library for the simulation of various sensors. It is designed to be used with an MQTT broker of your choice, providing an easy and flexible way to simulate sensor data for IoT applications. 
 
 ## Installation
-Not yet available on PyPi. To install, clone the repository and run `pip install -r requirements.txt` in the root directory.
+Pysor is available on PyPi. You can install it via pip:
+
+```shell
+pip install pysor
+```
 
 ## Quickstart
-Import the MqttClient class to create a client object. The client object can be used to publish messages to the broker.
+Here's a quick example showing how to simulate a temperature sensor using Pysor:
 
 ```python
 from sensor_simulation import MqttClient, SensorManager
 from sensor_simulation.sensors import TemperatureSensor
 
 
 if __name__ == '__main__':
-    mqtt_client = MqttClient('test.mosquitto.org')
+    mqtt_client = MqttClient('your.broker.org')
 
     temperature_sensor = TemperatureSensor(mqtt_client, 'sensor/temperature')
 
     sensor_manager = SensorManager()
     sensor_manager.add_sensor(temperature_sensor)
-    sensor_manager.run()
+
+    try:
+        sensor_manager.run()
+    except KeyboardInterrupt:
+        sensor_manager.stop_all()
+
 ```
 
-## Sensors
-Sensors are classes that inherit from the Sensor class. They can be added to the SensorManager to be run.
-### Currently available sensors:
+## Available Sensors
+Pysor comes with a variety of pre-built sensor simulations:
+
 - TemperatureSensor
 - HumiditySensor
 - LightIntensitySensor
 - WaterLevelSensor
+- PhSensor
 
 All sensors have parameters to set the mqtt client, the topic and the interval at which the sensor should publish messages.
 
 ### Example of parameters for HumiditySensor
 ```python
 class HumiditySensor(BaseSensor):
     """
@@ -80,48 +89,38 @@
                  ) -> None:
         ...
 ```
 
 ## Custom Sensors
 Extend the BaseSensor class and implement the 'generate_data' method. This method should return the data to be published.
 ```python
-@abstractmethod
-def generate_data(self) -> Any:
-    """
-    Generate data to be published to the broker
-
-    :return: Data
-    """
-    pass
+class MyCustomSensor(BaseSensor):
+    
+    def generate_data(self) -> Any:
+        # Your custom data generation logic here
+        ...
 ```
 
 ## SensorManager
 The SensorManager class is used to run the sensors. It has a method to add sensors and a method to run the sensors.
 ```python
 sensor_manager = SensorManager()
 
 sensor_manager.add_sensor(temperature_sensor)
 sensor_manager.add_sensor(humidity_sensor)
 sensor_manager.add_sensor(water_level_sensor)
 sensor_manager.add_sensor(light_intensity_sensor)
 
-sensor_manager.run()
+try:
+    sensor_manager.run()
+except KeyboardInterrupt:
+    sensor_manager.stop_all()
 ```
 
 ## MqttClient
 The MqttClient class is used to publish messages to the broker. It uses the Paho MQTT library to communicate with the broker.
 ```python
-mqtt_client = MqttClient('test.mosquitto.org')
+mqtt_client = MqttClient('your.broker.org')
 ```
 
-### Options
-The MqttClient class has a few options that can be set.
-```python
-    def __init__(self,
-                 broker_address: str,
-                 port: int = 1883,
-                 keepalive: int = 60,
-                 bind_address: str = "",
-                 bind_port: int = 0,
-                 ) -> None:
-    ...
-```
+### License
+Pysor is licensed under the MIT License. See the LICENSE file for more details
```

### Comparing `Pysor-0.1/Pysor.egg-info/PKG-INFO` & `pysor-0.1.1/Pysor.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Pysor
-Version: 0.1
+Name: pysor
+Version: 0.1.1
 Summary: A Python package for sensor simulations
 Home-page: https://github.com/CodeSwallow/pysor
 Author: Isai Ramirez
 Author-email: isai.ramirez.stamaria15@gmail.com
 License: MIT
 Keywords: mqtt sensor simulation
 Classifier: Development Status :: 3 - Alpha
@@ -23,45 +23,54 @@
 </div>
 
 <div align="center">
 <img src="https://github.com/CodeSwallow/pysor/actions/workflows/python-package.yml/badge.svg" alt="workflow status"/>
 <img src="artwork/coverage.svg" alt="coverage"/>
 </div>
 
-Pysor is a Python library for the simulation of various sensors. It is designed to be used with the broker of your choice.
-It uses the Paho MQTT library to communicate with the broker.
+Pysor is a Python library for the simulation of various sensors. It is designed to be used with an MQTT broker of your choice, providing an easy and flexible way to simulate sensor data for IoT applications. 
 
 ## Installation
-Not yet available on PyPi. To install, clone the repository and run `pip install -r requirements.txt` in the root directory.
+Pysor is available on PyPi. You can install it via pip:
+
+```shell
+pip install pysor
+```
 
 ## Quickstart
-Import the MqttClient class to create a client object. The client object can be used to publish messages to the broker.
+Here's a quick example showing how to simulate a temperature sensor using Pysor:
 
 ```python
 from sensor_simulation import MqttClient, SensorManager
 from sensor_simulation.sensors import TemperatureSensor
 
 
 if __name__ == '__main__':
-    mqtt_client = MqttClient('test.mosquitto.org')
+    mqtt_client = MqttClient('your.broker.org')
 
     temperature_sensor = TemperatureSensor(mqtt_client, 'sensor/temperature')
 
     sensor_manager = SensorManager()
     sensor_manager.add_sensor(temperature_sensor)
-    sensor_manager.run()
+
+    try:
+        sensor_manager.run()
+    except KeyboardInterrupt:
+        sensor_manager.stop_all()
+
 ```
 
-## Sensors
-Sensors are classes that inherit from the Sensor class. They can be added to the SensorManager to be run.
-### Currently available sensors:
+## Available Sensors
+Pysor comes with a variety of pre-built sensor simulations:
+
 - TemperatureSensor
 - HumiditySensor
 - LightIntensitySensor
 - WaterLevelSensor
+- PhSensor
 
 All sensors have parameters to set the mqtt client, the topic and the interval at which the sensor should publish messages.
 
 ### Example of parameters for HumiditySensor
 ```python
 class HumiditySensor(BaseSensor):
     """
@@ -80,48 +89,38 @@
                  ) -> None:
         ...
 ```
 
 ## Custom Sensors
 Extend the BaseSensor class and implement the 'generate_data' method. This method should return the data to be published.
 ```python
-@abstractmethod
-def generate_data(self) -> Any:
-    """
-    Generate data to be published to the broker
-
-    :return: Data
-    """
-    pass
+class MyCustomSensor(BaseSensor):
+    
+    def generate_data(self) -> Any:
+        # Your custom data generation logic here
+        ...
 ```
 
 ## SensorManager
 The SensorManager class is used to run the sensors. It has a method to add sensors and a method to run the sensors.
 ```python
 sensor_manager = SensorManager()
 
 sensor_manager.add_sensor(temperature_sensor)
 sensor_manager.add_sensor(humidity_sensor)
 sensor_manager.add_sensor(water_level_sensor)
 sensor_manager.add_sensor(light_intensity_sensor)
 
-sensor_manager.run()
+try:
+    sensor_manager.run()
+except KeyboardInterrupt:
+    sensor_manager.stop_all()
 ```
 
 ## MqttClient
 The MqttClient class is used to publish messages to the broker. It uses the Paho MQTT library to communicate with the broker.
 ```python
-mqtt_client = MqttClient('test.mosquitto.org')
+mqtt_client = MqttClient('your.broker.org')
 ```
 
-### Options
-The MqttClient class has a few options that can be set.
-```python
-    def __init__(self,
-                 broker_address: str,
-                 port: int = 1883,
-                 keepalive: int = 60,
-                 bind_address: str = "",
-                 bind_port: int = 0,
-                 ) -> None:
-    ...
-```
+### License
+Pysor is licensed under the MIT License. See the LICENSE file for more details
```

### Comparing `Pysor-0.1/Pysor.egg-info/SOURCES.txt` & `pysor-0.1.1/Pysor.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 pyproject.toml
 setup.py
 Pysor.egg-info/PKG-INFO
 Pysor.egg-info/SOURCES.txt
 Pysor.egg-info/dependency_links.txt
 Pysor.egg-info/requires.txt
 Pysor.egg-info/top_level.txt
+pysor.egg-info/PKG-INFO
+pysor.egg-info/SOURCES.txt
+pysor.egg-info/dependency_links.txt
+pysor.egg-info/requires.txt
+pysor.egg-info/top_level.txt
 sensor_simulation/__init__.py
 sensor_simulation/mqtt_client.py
 sensor_simulation/sensor_manager.py
 sensor_simulation/config/__init__.py
 sensor_simulation/config/logger.py
 sensor_simulation/config/parsers/__init__.py
 sensor_simulation/config/parsers/toml_parser.py
```

### Comparing `Pysor-0.1/README.md` & `pysor-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,45 +3,54 @@
 </div>
 
 <div align="center">
 <img src="https://github.com/CodeSwallow/pysor/actions/workflows/python-package.yml/badge.svg" alt="workflow status"/>
 <img src="artwork/coverage.svg" alt="coverage"/>
 </div>
 
-Pysor is a Python library for the simulation of various sensors. It is designed to be used with the broker of your choice.
-It uses the Paho MQTT library to communicate with the broker.
+Pysor is a Python library for the simulation of various sensors. It is designed to be used with an MQTT broker of your choice, providing an easy and flexible way to simulate sensor data for IoT applications. 
 
 ## Installation
-Not yet available on PyPi. To install, clone the repository and run `pip install -r requirements.txt` in the root directory.
+Pysor is available on PyPi. You can install it via pip:
+
+```shell
+pip install pysor
+```
 
 ## Quickstart
-Import the MqttClient class to create a client object. The client object can be used to publish messages to the broker.
+Here's a quick example showing how to simulate a temperature sensor using Pysor:
 
 ```python
 from sensor_simulation import MqttClient, SensorManager
 from sensor_simulation.sensors import TemperatureSensor
 
 
 if __name__ == '__main__':
-    mqtt_client = MqttClient('test.mosquitto.org')
+    mqtt_client = MqttClient('your.broker.org')
 
     temperature_sensor = TemperatureSensor(mqtt_client, 'sensor/temperature')
 
     sensor_manager = SensorManager()
     sensor_manager.add_sensor(temperature_sensor)
-    sensor_manager.run()
+
+    try:
+        sensor_manager.run()
+    except KeyboardInterrupt:
+        sensor_manager.stop_all()
+
 ```
 
-## Sensors
-Sensors are classes that inherit from the Sensor class. They can be added to the SensorManager to be run.
-### Currently available sensors:
+## Available Sensors
+Pysor comes with a variety of pre-built sensor simulations:
+
 - TemperatureSensor
 - HumiditySensor
 - LightIntensitySensor
 - WaterLevelSensor
+- PhSensor
 
 All sensors have parameters to set the mqtt client, the topic and the interval at which the sensor should publish messages.
 
 ### Example of parameters for HumiditySensor
 ```python
 class HumiditySensor(BaseSensor):
     """
@@ -60,48 +69,38 @@
                  ) -> None:
         ...
 ```
 
 ## Custom Sensors
 Extend the BaseSensor class and implement the 'generate_data' method. This method should return the data to be published.
 ```python
-@abstractmethod
-def generate_data(self) -> Any:
-    """
-    Generate data to be published to the broker
-
-    :return: Data
-    """
-    pass
+class MyCustomSensor(BaseSensor):
+    
+    def generate_data(self) -> Any:
+        # Your custom data generation logic here
+        ...
 ```
 
 ## SensorManager
 The SensorManager class is used to run the sensors. It has a method to add sensors and a method to run the sensors.
 ```python
 sensor_manager = SensorManager()
 
 sensor_manager.add_sensor(temperature_sensor)
 sensor_manager.add_sensor(humidity_sensor)
 sensor_manager.add_sensor(water_level_sensor)
 sensor_manager.add_sensor(light_intensity_sensor)
 
-sensor_manager.run()
+try:
+    sensor_manager.run()
+except KeyboardInterrupt:
+    sensor_manager.stop_all()
 ```
 
 ## MqttClient
 The MqttClient class is used to publish messages to the broker. It uses the Paho MQTT library to communicate with the broker.
 ```python
-mqtt_client = MqttClient('test.mosquitto.org')
+mqtt_client = MqttClient('your.broker.org')
 ```
 
-### Options
-The MqttClient class has a few options that can be set.
-```python
-    def __init__(self,
-                 broker_address: str,
-                 port: int = 1883,
-                 keepalive: int = 60,
-                 bind_address: str = "",
-                 bind_port: int = 0,
-                 ) -> None:
-    ...
-```
+### License
+Pysor is licensed under the MIT License. See the LICENSE file for more details
```

### Comparing `Pysor-0.1/pyproject.toml` & `pysor-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/sensor_simulation/config/logger.py` & `pysor-0.1.1/sensor_simulation/config/logger.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/sensor_simulation/config/parsers/toml_parser.py` & `pysor-0.1.1/sensor_simulation/config/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/sensor_simulation/mqtt_client.py` & `pysor-0.1.1/sensor_simulation/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/sensor_simulation/sensor_manager.py` & `pysor-0.1.1/sensor_simulation/sensor_manager.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/sensor_simulation/sensors/base_sensor.py` & `pysor-0.1.1/sensor_simulation/sensors/base_sensor.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/sensor_simulation/sensors/humidity_sensor.py` & `pysor-0.1.1/sensor_simulation/sensors/humidity_sensor.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/sensor_simulation/sensors/light_intensity_sensor.py` & `pysor-0.1.1/sensor_simulation/sensors/light_intensity_sensor.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/sensor_simulation/sensors/ph_sensor.py` & `pysor-0.1.1/sensor_simulation/sensors/ph_sensor.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/sensor_simulation/sensors/temperature_sensor.py` & `pysor-0.1.1/sensor_simulation/sensors/temperature_sensor.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/sensor_simulation/sensors/water_level_sensor.py` & `pysor-0.1.1/sensor_simulation/sensors/water_level_sensor.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/setup.py` & `pysor-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="Pysor",
-    version="0.1",
+    name="pysor",
+    version="0.1.1",
     packages=find_packages(),
     description="A Python package for sensor simulations",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/CodeSwallow/pysor",
     author="Isai Ramirez",
     author_email="isai.ramirez.stamaria15@gmail.com",
```

### Comparing `Pysor-0.1/tests/config/test_parser.py` & `pysor-0.1.1/tests/config/test_parser.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/tests/sensors/test_humidity_sensor.py` & `pysor-0.1.1/tests/sensors/test_humidity_sensor.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/tests/sensors/test_light_intensity_sensor.py` & `pysor-0.1.1/tests/sensors/test_light_intensity_sensor.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/tests/sensors/test_ph_sensor.py` & `pysor-0.1.1/tests/sensors/test_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/tests/sensors/test_temperature_sensor.py` & `pysor-0.1.1/tests/sensors/test_temperature_sensor.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/tests/sensors/test_water_level_sensor.py` & `pysor-0.1.1/tests/sensors/test_water_level_sensor.py`

 * *Files identical despite different names*

### Comparing `Pysor-0.1/tests/test_sensor_manager.py` & `pysor-0.1.1/tests/test_sensor_manager.py`

 * *Files identical despite different names*

