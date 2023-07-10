# Comparing `tmp/sdss-lvmnps-0.3.0.tar.gz` & `tmp/sdss_lvmnps-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss-lvmnps-0.3.0.tar", max compression
+gzip compressed data, was "sdss_lvmnps-0.4.0.tar", max compression
```

## Comparing `sdss-lvmnps-0.3.0.tar` & `sdss_lvmnps-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,37 @@
--rw-r--r--   0        0        0     1504 2021-09-13 19:15:16.592272 sdss-lvmnps-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     5319 2022-05-28 23:36:17.188290 sdss-lvmnps-0.3.0/README.md
--rw-r--r--   0        0        0     2747 2022-05-28 23:44:04.504215 sdss-lvmnps-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      539 2022-05-28 23:36:17.192070 sdss-lvmnps-0.3.0/python/lvmnps/__init__.py
--rw-r--r--   0        0        0     1258 2022-05-28 23:36:17.192264 sdss-lvmnps-0.3.0/python/lvmnps/__main__.py
--rw-r--r--   0        0        0      257 2022-05-28 23:36:17.192450 sdss-lvmnps-0.3.0/python/lvmnps/actor/__init__.py
--rw-r--r--   0        0        0     4211 2022-05-28 23:36:17.192669 sdss-lvmnps-0.3.0/python/lvmnps/actor/actor.py
--rw-r--r--   0        0        0     1072 2022-05-28 23:36:17.192886 sdss-lvmnps-0.3.0/python/lvmnps/actor/commands/__init__.py
--rw-r--r--   0        0        0     4683 2022-05-28 23:36:17.193140 sdss-lvmnps-0.3.0/python/lvmnps/actor/commands/onoff.py
--rw-r--r--   0        0        0     1209 2022-05-28 23:36:17.193277 sdss-lvmnps-0.3.0/python/lvmnps/actor/commands/outlets.py
--rw-r--r--   0        0        0     1757 2022-05-28 23:36:17.193592 sdss-lvmnps-0.3.0/python/lvmnps/actor/commands/status.py
--rw-r--r--   0        0        0      638 2022-05-28 23:36:17.193773 sdss-lvmnps-0.3.0/python/lvmnps/actor/commands/switches.py
--rw-r--r--   0        0        0      908 2022-05-28 23:36:17.194002 sdss-lvmnps-0.3.0/python/lvmnps/etc/lvmnps.yml
--rw-r--r--   0        0        0      716 2022-05-28 23:36:17.194268 sdss-lvmnps-0.3.0/python/lvmnps/etc/lvmnps_dummy.yml
--rw-r--r--   0        0        0      633 2022-05-28 23:36:17.194467 sdss-lvmnps-0.3.0/python/lvmnps/etc/lvmnps_pwi.yml
--rw-r--r--   0        0        0      680 2022-05-28 23:36:17.194780 sdss-lvmnps-0.3.0/python/lvmnps/etc/schema.json
--rw-r--r--   0        0        0      817 2022-05-28 23:36:17.195266 sdss-lvmnps-0.3.0/python/lvmnps/exceptions.py
--rw-r--r--   0        0        0        0 2022-05-28 23:36:17.195362 sdss-lvmnps-0.3.0/python/lvmnps/switch/dli/__init__.py
--rw-r--r--   0        0        0     5854 2022-05-28 23:36:17.195697 sdss-lvmnps-0.3.0/python/lvmnps/switch/dli/dli.py
--rw-r--r--   0        0        0     4670 2022-05-28 23:36:17.195968 sdss-lvmnps-0.3.0/python/lvmnps/switch/dli/powerswitch.py
--rw-r--r--   0        0        0        0 2022-05-28 23:36:17.196027 sdss-lvmnps-0.3.0/python/lvmnps/switch/dummy/__init__.py
--rw-r--r--   0        0        0     1381 2022-05-28 23:36:17.196273 sdss-lvmnps-0.3.0/python/lvmnps/switch/dummy/powerswitch.py
--rw-r--r--   0        0        0     1500 2022-05-28 23:36:17.196718 sdss-lvmnps-0.3.0/python/lvmnps/switch/factory.py
--rw-r--r--   0        0        0     2458 2022-05-28 23:36:17.196967 sdss-lvmnps-0.3.0/python/lvmnps/switch/outlet.py
--rw-r--r--   0        0        0     7784 2022-05-28 23:36:17.197298 sdss-lvmnps-0.3.0/python/lvmnps/switch/powerswitchbase.py
--rw-r--r--   0        0        0     6611 1970-01-01 00:00:00.000000 sdss-lvmnps-0.3.0/setup.py
--rw-r--r--   0        0        0     6663 1970-01-01 00:00:00.000000 sdss-lvmnps-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-10 09:55:59.806696 sdss_lvmnps-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     5512 2023-07-10 09:55:59.806696 sdss_lvmnps-0.4.0/README.md
+-rw-r--r--   0        0        0     2747 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      539 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/__init__.py
+-rw-r--r--   0        0        0     2189 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/__main__.py
+-rw-r--r--   0        0        0      257 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/actor/__init__.py
+-rw-r--r--   0        0        0     4382 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/actor/actor.py
+-rw-r--r--   0        0        0     1129 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/actor/commands/__init__.py
+-rw-r--r--   0        0        0     4921 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/actor/commands/onoff.py
+-rw-r--r--   0        0        0     1209 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/actor/commands/outlets.py
+-rw-r--r--   0        0        0     1842 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/actor/commands/status.py
+-rw-r--r--   0        0        0      638 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/actor/commands/switches.py
+-rw-r--r--   0        0        0      908 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/etc/lvmnps.yml
+-rw-r--r--   0        0        0     1076 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/etc/lvmnps_dummy.yml
+-rw-r--r--   0        0        0      493 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/etc/lvmnps_netio.yml
+-rw-r--r--   0        0        0      633 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/etc/lvmnps_pwi.yml
+-rw-r--r--   0        0        0     1465 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/etc/lvmnps_telescope.yml
+-rw-r--r--   0        0        0      680 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/etc/schema.json
+-rw-r--r--   0        0        0      816 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/dli/__init__.py
+-rw-r--r--   0        0        0     6183 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/dli/dli.py
+-rw-r--r--   0        0        0     4669 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/dli/powerswitch.py
+-rw-r--r--   0        0        0        0 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/dummy/__init__.py
+-rw-r--r--   0        0        0     1438 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/dummy/powerswitch.py
+-rw-r--r--   0        0        0     1815 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/factory.py
+-rw-r--r--   0        0        0    10582 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/iboot/iboot.py
+-rw-r--r--   0        0        0     2428 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/iboot/powerswitch.py
+-rw-r--r--   0        0        0     6300 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/netio/Netio/Device.py
+-rw-r--r--   0        0        0       58 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/netio/Netio/__init__.py
+-rw-r--r--   0        0        0       62 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/netio/Netio/__main__.py
+-rw-r--r--   0        0        0    11727 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/netio/Netio/cli.py
+-rw-r--r--   0        0        0      305 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/netio/Netio/exceptions.py
+-rw-r--r--   0        0        0      211 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/netio/__init__.py
+-rw-r--r--   0        0        0     2765 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/netio/powerswitch.py
+-rw-r--r--   0        0        0     2457 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/outlet.py
+-rw-r--r--   0        0        0     7783 2023-07-10 09:55:59.818697 sdss_lvmnps-0.4.0/python/lvmnps/switch/powerswitchbase.py
+-rw-r--r--   0        0        0     6796 1970-01-01 00:00:00.000000 sdss_lvmnps-0.4.0/PKG-INFO
```

### Comparing `sdss-lvmnps-0.3.0/LICENSE.md` & `sdss_lvmnps-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-lvmnps-0.3.0/README.md` & `sdss_lvmnps-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 ## Features
 
 - CLU Actor based interface
 - Supports a Dummy PDU
 - Supports [iBOOT g2](https://dataprobe.com/iboot-g2/) with python code from [here](https://github.com/dprince/python-iboot)
 - Supports [Digital Loggers Web Power](https://www.digital-loggers.com/lpc7.html) with python code from [here](https://github.com/dwighthubbard/python-dlipower)
+- Supports [netio](https://shop.netio.eu/netio-power-sockets/powerpdu-4ps--iec-320-c13-switched-power-distribution-unit/) with python code from [here](https://github.com/netioproducts/PyNetio)
 
 
 ## Installation
 
 Clone this repository.
 
 ```console
```

### Comparing `sdss-lvmnps-0.3.0/pyproject.toml` & `sdss_lvmnps-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmnps"
-version = "0.3.0"
+version = "0.4.0"
 description = "A library and actor to communicate with an SDSS-V LVM network power switch"
 authors = ["Florian Briegel <briegel@mpia.de>", "José Sánchez-Gallego <gallegoj@uw.edu>", "Changgon Kim <changgonkim@khu.ac.kr>", "Mingyeong Yang <mingyeong@khu.ac.kr>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmnps"
 repository = "https://github.com/sdss/lvmnps"
 documentation = "https://lvmnps.readthedocs.org"
@@ -21,22 +21,23 @@
 ]
 packages = [
     { include = "lvmnps", from = "python" }
 ]
 include = ["python/lvmnps/etc/*"]
 
 [tool.poetry.scripts]
-lvmnps = "lvmnps.__main__:lvmnps"
+lvmnps = "lvmnps.__main__:main"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-sdsstools = ">=0.4.0"
+python = ">=3.8,<4.0"
+sdsstools = "^1.0.0"
 click-default-group = "^1.2.2"
-sdss-clu = "^1.0.3"
+sdss-clu = "^2.0.0"
 httpx = "^0.18.1"
+requests = ">2.20"
 
 [tool.poetry.group.helpers.dependencies]
 ipython = ">=7.11.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
 isort = ">=4.3.21"
 ipdb = ">=0.12.3"
@@ -48,15 +49,14 @@
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=5.2.2"
 pytest-asyncio = ">=0.10.0"
 pytest-cov = ">=2.8.1"
 pytest-mock = ">=1.13.0"
 pytest-sugar = ">=0.9.2"
-codecov = ">=2.0.15"
 coverage = {version = ">=5.0", extras = ["toml"]}
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = ">=4.1.2"
@@ -77,15 +77,15 @@
 balanced_wrapping = true
 include_trailing_comma = false
 lines_after_imports = 2
 use_parentheses = true
 
 [tool.black]
 line-length = 88
-target-version = ['py39']
+target-version = ['py311']
 fast = true
 
 [tool.pytest.ini_options]
 addopts = "--cov lvmnps --cov-report xml --cov-report html --cov-report term"
 asyncio_mode = "auto"
 
 [tool.coverage.run]
@@ -98,9 +98,9 @@
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING"
 ]
 
 [build-system]
-requires = ["poetry-core>=1.1.0a7"]
+requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/__init__.py` & `sdss_lvmnps-0.4.0/python/lvmnps/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/actor/actor.py` & `sdss_lvmnps-0.4.0/python/lvmnps/actor/actor.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
     """
 
     parser: ClassVar[click.Group] = nps_command_parser
     BASE_CONFIG: ClassVar[str | Dict | None] = None
 
     def __init__(self, *args, **kwargs):
-
         if "schema" not in kwargs:
             kwargs["schema"] = os.path.join(
                 os.path.dirname(__file__),
                 "../etc/schema.json",
             )
 
         super().__init__(*args, **kwargs)
@@ -99,15 +98,15 @@
                 await asyncio.wait_for(switch.stop(), timeout=self.connect_timeout)
             except Exception as ex:
                 self.log.error(f"Unexpected exception of {type(ex)}: {ex}")
 
         return await super().stop()
 
     @classmethod
-    def from_config(cls, config, *args, **kwargs):
+    def from_config(cls, config, *args, simulate: bool = False, **kwargs):
         """Creates an actor from a configuration file."""
 
         if config is None:
             if cls.BASE_CONFIG is None:
                 raise RuntimeError("The class does not have a base configuration.")
             config = cls.BASE_CONFIG
 
@@ -115,23 +114,27 @@
 
         assert isinstance(instance, NPSActor)
         assert isinstance(instance.config, dict)
 
         switches = {}
 
         if "switches" in instance.config:
-            for (key, swconfig) in instance.config["switches"].items():
+            if simulate:
+                instance.log.warn("In simulation mode !!!")
+            for key, swconfig in instance.config["switches"].items():
                 if "name" in swconfig:
                     name = swconfig["name"]
                 else:
                     name = key
 
                 instance.log.info(f"Instance {name}: {swconfig}")
                 try:
-                    switches[name] = powerSwitchFactory(name, swconfig, instance.log)
+                    switches[name] = powerSwitchFactory(
+                        name, swconfig, instance.log, simulate=simulate
+                    )
                 except Exception as ex:
                     instance.log.error(f"Power switch factory error {type(ex)}: {ex}")
 
         instance.parser_args = [switches]
 
         return instance
```

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/actor/commands/__init__.py` & `sdss_lvmnps-0.4.0/python/lvmnps/actor/commands/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import glob
 import importlib
 import os
 
 import click
 
 from clu.command import Command
-from clu.parsers.click import CluGroup, help_, ping, version
+from clu.parsers.click import CluGroup, get_command_model, help_, ping, version
 
 
 @click.group(cls=CluGroup)
 def parser(*args):
     pass
 
 
 parser.add_command(ping)
 parser.add_command(version)
 parser.add_command(help_)
+parser.add_command(get_command_model)
 
 
 @parser.command(name="__commands")
 @click.pass_context
 def __commands(ctx, command: Command, *args):
     # Returns all commands.
```

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/actor/commands/onoff.py` & `sdss_lvmnps-0.4.0/python/lvmnps/actor/commands/onoff.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,21 @@
     command: NPSCommand,
     switches: dict[str, PowerSwitchBase],
     outlet: str,
     portnum: int | None = None,
     switch: str | None = None,
     off_after: float | None = None,
 ):
-    """Turn on the outlet."""
+    """
+    Turn on the outlet.
+
+    \b
+    :param OUTLET: Outlet or switch name.
+    :param PORTNUM: Portnumber if switch name is provided.
+    """
 
     if portnum:
         command.info(text=f"Turning on {outlet} port {portnum} ...")
     else:
         command.info(text=f"Turning on outlet {outlet} ...")
 
     the_switch: PowerSwitchBase | None = None
@@ -80,15 +86,15 @@
 
     if current_status is None or the_switch is None:
         return command.fail(f"Could not find a match for {outlet}:{portnum}.")
 
     outletname_list = list(current_status.keys())
     outletname = outletname_list[0]
 
-    if current_status[outletname]["state"] == 0:
+    if current_status[outletname]["state"] != 1:
         current_status = await switch_control("on", the_switch, True, outlet, portnum)
     elif current_status[outletname]["state"] == 1:
         return command.finish(text=f"The outlet {outletname} is already ON")
     else:
         return command.fail(text=f"The outlet {outletname} returns wrong value")
 
     command.info(status=current_status)
@@ -114,15 +120,21 @@
 async def off(
     command: NPSCommand,
     switches: dict[str, PowerSwitchBase],
     outlet: str,
     portnum: int | None = None,
     switch: str | None = None,
 ):
-    """Turn off the outlet."""
+    """
+    Turn off the outlet.
+
+    \b
+    :param OUTLET: Outlet or switch name.
+    :param PORTNUM: Portnumber if switch name is provided.
+    """
 
     if portnum:
         command.info(text=f"Turning off {outlet} port {portnum} ...")
     else:
         command.info(text=f"Turning off outlet {outlet} ...")
 
     the_switch: PowerSwitchBase | None = None
@@ -138,15 +150,15 @@
 
     if current_status is None or the_switch is None:
         return command.fail(f"Could not find a match for {outlet}:{portnum}.")
 
     outletname_list = list(current_status.keys())
     outletname = outletname_list[0]
 
-    if current_status[outletname]["state"] == 1:
+    if current_status[outletname]["state"] != 0:
         current_status = await switch_control("off", the_switch, False, outlet, portnum)
     elif current_status[outletname]["state"] == 0:
         return command.finish(text=f"The outlet {outletname} is already OFF")
     else:
         return command.fail(text=f"The outlet {outletname} returns wrong value")
 
     command.info(status=current_status)
```

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/actor/commands/outlets.py` & `sdss_lvmnps-0.4.0/python/lvmnps/actor/commands/outlets.py`

 * *Files identical despite different names*

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/actor/commands/status.py` & `sdss_lvmnps-0.4.0/python/lvmnps/actor/commands/status.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,21 @@
 async def status(
     command: NPSCommand,
     switches: dict[str, PowerSwitchBase],
     switchname: str | None = None,
     portnum: int | None = None,
     outlet: str | None = None,
 ):
-    """Returns the dictionary of a specific outlet."""
+    """
+    Returns the dictionary of a specific outlet.
 
+    \b
+    :param SWITCHNAME: Switch name.
+    :param PORTNUM: Portnumber.
+    """
     if switchname and switchname not in switches:
         return command.fail(f"Unknown switch {switchname}.")
 
     status = {}
     if switchname is None:
         for switch in switches.values():
             if not await switch.isReachable():
```

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/actor/commands/switches.py` & `sdss_lvmnps-0.4.0/python/lvmnps/actor/commands/switches.py`

 * *Files identical despite different names*

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/etc/lvmnps.yml` & `sdss_lvmnps-0.4.0/python/lvmnps/etc/lvmnps.yml`

 * *Files identical despite different names*

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/etc/lvmnps_dummy.yml` & `sdss_lvmnps-0.4.0/python/lvmnps/etc/lvmnps_pwi.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 # A dictionary of controller name to NPS controller connection parameters.
 switches:
-  nps_dummy_1:
-    type: dummy
-    num: 8
-    ports:
-      1:
-        desc: 'was 1'
-      2:
-        name: 'skye.what.ever'
-        desc: 'whatever is connected to skye'
-      4:
-        name: 'skyw.what.ever'
-        desc: 'Something @ skyw'
   skye.nps:
-    type: dummy
+    type: iboot
+    hostname: '192.168.178.52'
+    username: 'admin'
+    password: 'admin'
     ports:
+      num: 1
       1:
         name: 'skye.pwi'
         desc: 'PlaneWavemount Skye'
-  nps_dummy_3:
-    type: dummy
+  skyw.nps:
+    type: iboot
+    hostname: '192.168.178.53'
+    username: 'admin'
+    password: 'admin'
     ports:
-      num: 2
+      num: 1
       1:
         name: 'skyw.pwi'
-        desc: 'PlaneWavemount Skyw'
+        desc: 'PlaneWavemount Skye'
 
 timeouts:
   switch_connect: 1
 
 # Actor configuration for the AMQPActor class
 actor:
   name: lvmnps
```

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/etc/schema.json` & `sdss_lvmnps-0.4.0/python/lvmnps/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/exceptions.py` & `sdss_lvmnps-0.4.0/python/lvmnps/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from __future__ import absolute_import, division, print_function
 
 
 class NpsActorError(Exception):
     """A custom core NpsActor exception"""
 
     def __init__(self, message=None):
-
         message = "There has been an error" if not message else message
 
         super(NpsActorError, self).__init__(message)
 
 
 class NpsActorWarning(Warning):
     """Base warning for NpsActor."""
```

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/switch/dli/dli.py` & `sdss_lvmnps-0.4.0/python/lvmnps/switch/dli/dli.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,26 +47,27 @@
         hostname: str,
         user: str,
         password: str,
         name: str | None = None,
         log: SDSSLogger | None = None,
         onoff_timeout=3,
     ):
-
         self.user = user
         self.hostname = hostname
         self.name = name or hostname
 
         self.log = log or logging.getLogger(f"{self.__class__.__name__}_{self.name}")
 
         self.onoff_timeout = onoff_timeout
 
         self.client: httpx.AsyncClient
         self.add_client(password)
 
+        self.lock = asyncio.Lock()
+
     def add_client(self, password: str):
         """Add the `httpx.AsyncClient` to the DLI object."""
 
         try:
             auth = httpx.DigestAuth(self.user, password)
             self.client = httpx.AsyncClient(
                 auth=auth,
@@ -87,20 +88,21 @@
         outlets
             The list of `.Outlet` instance to check.
 
         """
 
         result = False
 
-        async with self.client as client:
-            r = await client.get("relay/outlets/")
-            if r.status_code != 200:
-                raise RuntimeError(f"GET returned code {r.status_code}.")
-            else:
-                result = self.compare(r.json(), outlets)
+        async with self.lock:
+            async with self.client as client:
+                r = await client.get("relay/outlets/")
+                if r.status_code != 200:
+                    raise RuntimeError(f"GET returned code {r.status_code}.")
+                else:
+                    result = self.compare(r.json(), outlets)
 
         return result
 
     def compare(self, json: dict, outlets: list[Outlet]):
         """Compares the names of the outlets with the response JSON object.
 
         Parameters
@@ -134,25 +136,26 @@
         outlet
             The number indicating the outlet (1-indexed).
 
         """
 
         outlet = outlet - 1
 
-        async with self.client as client:
-            r = await asyncio.wait_for(
-                client.put(
-                    f"relay/outlets/{outlet}/state/",
-                    data={"value": True},
-                    headers={"X-CSRF": "x"},
-                ),
-                self.onoff_timeout,
-            )
-            if r.status_code != 204:
-                raise RuntimeError(f"PUT returned code {r.status_code}.")
+        async with self.lock:
+            async with self.client as client:
+                r = await asyncio.wait_for(
+                    client.put(
+                        f"relay/outlets/{outlet}/state/",
+                        data={"value": True},
+                        headers={"X-CSRF": "x"},
+                    ),
+                    self.onoff_timeout,
+                )
+                if r.status_code != 204:
+                    raise RuntimeError(f"PUT returned code {r.status_code}.")
 
     async def off(self, outlet=0):
         """Turn off the power to the outlet.
 
         Set the value of the outlet state by using a PUT request. Note that the
         outlets in the RESTful API are zero-indexed.
 
@@ -161,48 +164,51 @@
         outlet
             The number indicating the outlet (1-indexed).
 
         """
 
         outlet = outlet - 1
 
-        async with self.client as client:
-            r = await asyncio.wait_for(
-                client.put(
-                    f"relay/outlets/{outlet}/state/",
-                    data={"value": False},
-                    headers={"X-CSRF": "x"},
-                ),
-                self.onoff_timeout,
-            )
-            if r.status_code != 204:
-                raise RuntimeError(f"PUT returned code {r.status_code}.")
+        async with self.lock:
+            async with self.client as client:
+                r = await asyncio.wait_for(
+                    client.put(
+                        f"relay/outlets/{outlet}/state/",
+                        data={"value": False},
+                        headers={"X-CSRF": "x"},
+                    ),
+                    self.onoff_timeout,
+                )
+                if r.status_code != 204:
+                    raise RuntimeError(f"PUT returned code {r.status_code}.")
 
     async def get_outlets_response(self):
         """Returns the raw response to a ``relay/outlets`` GET request.."""
 
-        async with self.client as client:
-            r = await client.get("relay/outlets/")
-            if r.status_code != 200:
-                raise RuntimeError(f"GET returned code {r.status_code}.")
+        async with self.lock:
+            async with self.client as client:
+                r = await client.get("relay/outlets/")
+                if r.status_code != 200:
+                    raise RuntimeError(f"GET returned code {r.status_code}.")
 
         return r.json()
 
     async def status(self):
         """Returns the status as a dictionary.
 
         Receives the data from the switch by the GET method as a JSON. Note that
         this method returns the status of all the outlets (ports 1-8).
 
         """
 
-        async with self.client as client:
-            r = await client.get("relay/outlets/")
-            if r.status_code != 200:
-                raise RuntimeError(f"GET returned code {r.status_code}.")
+        async with self.lock:
+            async with self.client as client:
+                r = await client.get("relay/outlets/")
+                if r.status_code != 200:
+                    raise RuntimeError(f"GET returned code {r.status_code}.")
 
         outlets_dict = {}
 
         data = r.json()
         for n in range(0, 8):
             outlets_dict[n + 1] = data[n]["state"]
```

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/switch/dli/powerswitch.py` & `sdss_lvmnps-0.4.0/python/lvmnps/switch/dli/powerswitch.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         The configuration defined on the .yaml file under ``/etc/lvmnps_dli.yml``.
     log
         The logger for logging.
 
     """
 
     def __init__(self, name: str, config: dict, log: SDSSLogger | None = None):
-
         super().__init__(name, config, log)
 
         hostname = self.config_get("hostname")
         user = self.config_get("user")
         password = self.config_get("password")
 
         onoff_timeout = self.config_get("onoff_timeout", 3)
```

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/switch/dummy/powerswitch.py` & `sdss_lvmnps-0.4.0/python/lvmnps/switch/dummy/powerswitch.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 class PowerSwitch(PowerSwitchBase):
     """Powerswitch class to manage the Digital Loggers Web power switch"""
 
     def __init__(self, name: str, config: dict, log: SDSSLogger):
         super().__init__(name, config, log)
         self.delay = self.config_get("delay", 0.0)
+        for o in self.outlets:
+            o.setState(0)
 
     async def start(self):
         if not await self.isReachable():
             self.log.warning(f"{self.name} not reachable on start up")
         await self.update(self.outlets)
 
     async def stop(self):
```

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/switch/factory.py` & `sdss_lvmnps-0.4.0/python/lvmnps/switch/factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,44 +12,52 @@
 
 from sdsstools.logger import SDSSLogger
 
 from lvmnps.exceptions import PowerException
 
 from .dli.powerswitch import DLIPowerSwitch
 from .dummy.powerswitch import PowerSwitch as DummyPowerSwitch
+from .iboot.powerswitch import PowerSwitch as IBootPowerSwitch
+from .netio.powerswitch import PowerSwitch as NetIOPowerSwitch
 
 
 if TYPE_CHECKING:
     from lvmnps.switch.powerswitchbase import PowerSwitchBase
 
 
 # from .iboot.powerswitch import PowerSwitch as IBootPowerSwitch
 
 
-def powerSwitchFactory(name: str, config: dict, log: SDSSLogger):
+def powerSwitchFactory(
+    name: str, config: dict, log: SDSSLogger, simulate: bool = False
+):
     """Power switch factory method which helps the user to select the `.PowerSwitch`
     class based on the configuration file that is selected.
 
     Parameters
     ----------
     name
         the name of the Dli Controller
     config
         The configuration dictionary from the configuration file .yml
     log
         The logger for logging
+    simulate
+        on True overwrite type from config with dummy
 
     """
 
     def throwError(n, c):
         """The method to throw the Exception."""
         raise PowerException(f"Power switch {n} with type {c['type']} not defined")
 
     factorymap: dict[str, Type[PowerSwitchBase]] = {
         "dli": DLIPowerSwitch,
-        # "iboot": IBootPowerSwitch,
+        "netio": NetIOPowerSwitch,
+        "iboot": IBootPowerSwitch,
         "dummy": DummyPowerSwitch,
     }
 
-    return factorymap.get(config["type"], lambda n, c, _: throwError(n, c))(
-        name, config, log
-    )
+    log.info(f"{simulate:-}")
+    return factorymap.get(
+        config["type"] if not simulate else "dummy", lambda n, c, _: throwError(n, c)
+    )(name, config, log)
```

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/switch/outlet.py` & `sdss_lvmnps-0.4.0/python/lvmnps/switch/outlet.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         self,
         switch: PowerSwitchBase,
         name: str,
         portnum: int,
         description: str | None = None,
         state: int = 0,
     ):
-
         self.switch = switch
         self.name = name if name else f"{self.switch.name}.port{portnum}"
         self.portnum = portnum
 
         default_description = f"{self.switch.name} Port {portnum}"
         self.description = description if description else default_description
```

### Comparing `sdss-lvmnps-0.3.0/python/lvmnps/switch/powerswitchbase.py` & `sdss_lvmnps-0.4.0/python/lvmnps/switch/powerswitchbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         The configuration defined on the .yaml file under ``/etc/lvmnps.yml``.
     log
         The logger for logging.
 
     """
 
     def __init__(self, name: str, config: dict, log: SDSSLogger | None = None):
-
         self.name = name
         self.log = log or SDSSLogger(f"powerswitchbase.{name}")
         self.config = config
 
         numports = self.config_get("ports.number_of_ports", 8)
         if numports is None:
             raise ValueError(f"{name}: unknown number of ports.")
```

### Comparing `sdss-lvmnps-0.3.0/setup.py` & `sdss_lvmnps-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,246 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sdss-lvmnps
+Version: 0.4.0
+Summary: A library and actor to communicate with an SDSS-V LVM network power switch
+Home-page: https://github.com/sdss/lvmnps
+License: BSD-3-Clause
+Keywords: astronomy,software
+Author: Florian Briegel
+Author-email: briegel@mpia.de
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Documentation :: Sphinx
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
+Requires-Dist: httpx (>=0.18.1,<0.19.0)
+Requires-Dist: requests (>2.20)
+Requires-Dist: sdss-clu (>=2.0.0,<3.0.0)
+Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
+Project-URL: Documentation, https://lvmnps.readthedocs.org
+Project-URL: Repository, https://github.com/sdss/lvmnps
+Description-Content-Type: text/markdown
+
+# lvmnps
+
+![Versions](https://img.shields.io/badge/python->3.8-blue)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/lvmnps/badge/?version=latest)](https://lvmnps.readthedocs.io/en/latest/?badge=latest)
+[![Test](https://github.com/sdss/lvmnps/actions/workflows/test.yml/badge.svg)](https://github.com/sdss/lvmnps/actions/workflows/test.yml)
+[![Docker](https://github.com/sdss/lvmnps/actions/workflows/docker.yml/badge.svg)](https://github.com/sdss/lvmnps/actions/workflows/docker.yml)
+[![codecov](https://codecov.io/gh/sdss/lvmnps/branch/main/graph/badge.svg?token=M0RPGO77JH)](https://codecov.io/gh/sdss/lvmnps)
+
+LVM Network Power Switch
+
+## Features
+
+- CLU Actor based interface
+- Supports a Dummy PDU
+- Supports [iBOOT g2](https://dataprobe.com/iboot-g2/) with python code from [here](https://github.com/dprince/python-iboot)
+- Supports [Digital Loggers Web Power](https://www.digital-loggers.com/lpc7.html) with python code from [here](https://github.com/dwighthubbard/python-dlipower)
+- Supports [netio](https://shop.netio.eu/netio-power-sockets/powerpdu-4ps--iec-320-c13-switched-power-distribution-unit/) with python code from [here](https://github.com/netioproducts/PyNetio)
+
+
+## Installation
+
+Clone this repository.
+
+```console
+git clone https://github.com/sdss/lvmnps
+cd lvmnps
+```
+
+## Quick Start
+
+### Start the actor
+
+Start `lvmnps` actor.
+
+```console
+lvmnps start
+```
+
+In another terminal, type `clu` and `lvmnps ping` for test.
+
+```console
+clu
+lvmnps ping
+     07:41:22.636 lvmnps >
+     07:41:22.645 lvmnps : {
+         "text": "Pong."
+         }
+```
+
+Stop `lvmnps` actor.
+
+```console
+lvmnps stop
+```
+
+## Config file structure
+
+```yaml
+switches:
+    name_your_switch_here:    # should be a unique name
+        type: dummy           # currently dummy, iboot, dli
+        num: 8                # number of ports
+        ports:
+            1:
+            name: "skyw.pwi"  # should also be a unique name
+            desc: "Something that make sense"
+    should_be_a_unique_name:
+        type: dummy
+        ports:
+            1:
+            name: "skye.pwi"
+            desc: "PlaneWavemount Skye"
+```
+
+## Status return for all commands
+
+- if `name` is not defined then the port name will be `switch name.port number`, e.g. `nps_dummy_1.port1`. Otherwise `name` from the config file will be used.
+- `STATE: 1: ON, 0: OFF, -1: UNKNOWN`
+
+```yaml
+    "STATUS": {
+    "nps_dummy_1.port1": {
+        "STATE": -1,
+        "DESCR": "was 1",
+        "SWITCH": "nps_dummy_1",
+        "PORT": 1
+    },
+```
+
+## Run the example lvmnps_dummy
+
+```console
+cd lvmnps
+poetry run lvmnps -vvv -c $(pwd)/python/lvmnps/etc/lvmnps_dummy.yml start
+
+poetry run clu
+```
+
+- Status command without parameter returns all ports of all switches.
+- The default is to return only configured ports, otherwise define 'ouo' false in the config file, see [lvmnps_dummy.yml](https://github.com/sdss/lvmnps/blob/main/python/lvmnps/etc/lvmnps_dummy.yml)
+
+```console
+>>> lvmnps status
+
+12:02:08.649 lvmnps >
+12:02:08.660 lvmnps i {
+    "STATUS": {
+        "nps_dummy_1.port1": {
+            "STATE": -1,
+            "DESCR": "was 1",
+            "SWITCH": "nps_dummy_1",
+            "PORT": 1
+        },
+        "skye.what.ever": {
+            "STATE": -1,
+            "DESCR": "whatever is connected to skye",
+            "SWITCH": "nps_dummy_1",
+            "PORT": 2
+        },
+        "skyw.what.ever": {
+            "STATE": -1,
+            "DESCR": "Something @ skyw",
+            "SWITCH": "nps_dummy_1",
+            "PORT": 4
+        },
+        "skye.pwi": {
+            "STATE": -1,
+            "DESCR": "PlaneWavemount Skye",
+            "SWITCH": "skye.nps",
+            "PORT": 1
+        },
+            "skyw.pwi": {
+            "STATE": -1,
+            "DESCR": "PlaneWavemount Skyw",
+            "SWITCH": "nps_dummy_3",
+            "PORT": 1
+        }
+    }
+}
+```
+
+- status command with port name skyw.what.ever
+
+```console
+>>> lvmnps status skyw.what.ever
+
+12:07:12.349 lvmnps >
+12:07:12.377 lvmnps i {
+    "STATUS": {
+        "skyw.what.ever": {
+            "STATE": -1,
+            "DESCR": "Something @ skyw",
+            "SWITCH": "nps_dummy_1",
+            "PORT": 4
+}
+```
+
+- status command with switch name nps_dummy_1
 
-package_dir = \
-{'': 'python'}
+```console
+>>> lvmnps status nps_dummy_1
 
-packages = \
-['lvmnps',
- 'lvmnps.actor',
- 'lvmnps.actor.commands',
- 'lvmnps.switch',
- 'lvmnps.switch.dli',
- 'lvmnps.switch.dummy']
-
-package_data = \
-{'': ['*'], 'lvmnps': ['etc/*']}
-
-install_requires = \
-['click-default-group>=1.2.2,<2.0.0',
- 'httpx>=0.18.1,<0.19.0',
- 'sdss-clu>=1.0.3,<2.0.0',
- 'sdsstools>=0.4.0']
-
-entry_points = \
-{'console_scripts': ['lvmnps = lvmnps.__main__:lvmnps']}
-
-setup_kwargs = {
-    'name': 'sdss-lvmnps',
-    'version': '0.3.0',
-    'description': 'A library and actor to communicate with an SDSS-V LVM network power switch',
-    'long_description': '# lvmnps\n\n![Versions](https://img.shields.io/badge/python->3.8-blue)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Documentation Status](https://readthedocs.org/projects/lvmnps/badge/?version=latest)](https://lvmnps.readthedocs.io/en/latest/?badge=latest)\n[![Test](https://github.com/sdss/lvmnps/actions/workflows/test.yml/badge.svg)](https://github.com/sdss/lvmnps/actions/workflows/test.yml)\n[![Docker](https://github.com/sdss/lvmnps/actions/workflows/docker.yml/badge.svg)](https://github.com/sdss/lvmnps/actions/workflows/docker.yml)\n[![codecov](https://codecov.io/gh/sdss/lvmnps/branch/main/graph/badge.svg?token=M0RPGO77JH)](https://codecov.io/gh/sdss/lvmnps)\n\nLVM Network Power Switch\n\n## Features\n\n- CLU Actor based interface\n- Supports a Dummy PDU\n- Supports [iBOOT g2](https://dataprobe.com/iboot-g2/) with python code from [here](https://github.com/dprince/python-iboot)\n- Supports [Digital Loggers Web Power](https://www.digital-loggers.com/lpc7.html) with python code from [here](https://github.com/dwighthubbard/python-dlipower)\n\n\n## Installation\n\nClone this repository.\n\n```console\ngit clone https://github.com/sdss/lvmnps\ncd lvmnps\n```\n\n## Quick Start\n\n### Start the actor\n\nStart `lvmnps` actor.\n\n```console\nlvmnps start\n```\n\nIn another terminal, type `clu` and `lvmnps ping` for test.\n\n```console\nclu\nlvmnps ping\n     07:41:22.636 lvmnps >\n     07:41:22.645 lvmnps : {\n         "text": "Pong."\n         }\n```\n\nStop `lvmnps` actor.\n\n```console\nlvmnps stop\n```\n\n## Config file structure\n\n```yaml\nswitches:\n    name_your_switch_here:    # should be a unique name\n        type: dummy           # currently dummy, iboot, dli\n        num: 8                # number of ports\n        ports:\n            1:\n            name: "skyw.pwi"  # should also be a unique name\n            desc: "Something that make sense"\n    should_be_a_unique_name:\n        type: dummy\n        ports:\n            1:\n            name: "skye.pwi"\n            desc: "PlaneWavemount Skye"\n```\n\n## Status return for all commands\n\n- if `name` is not defined then the port name will be `switch name.port number`, e.g. `nps_dummy_1.port1`. Otherwise `name` from the config file will be used.\n- `STATE: 1: ON, 0: OFF, -1: UNKNOWN`\n\n```yaml\n    "STATUS": {\n    "nps_dummy_1.port1": {\n        "STATE": -1,\n        "DESCR": "was 1",\n        "SWITCH": "nps_dummy_1",\n        "PORT": 1\n    },\n```\n\n## Run the example lvmnps_dummy\n\n```console\ncd lvmnps\npoetry run lvmnps -vvv -c $(pwd)/python/lvmnps/etc/lvmnps_dummy.yml start\n\npoetry run clu\n```\n\n- Status command without parameter returns all ports of all switches.\n- The default is to return only configured ports, otherwise define \'ouo\' false in the config file, see [lvmnps_dummy.yml](https://github.com/sdss/lvmnps/blob/main/python/lvmnps/etc/lvmnps_dummy.yml)\n\n```console\n>>> lvmnps status\n\n12:02:08.649 lvmnps >\n12:02:08.660 lvmnps i {\n    "STATUS": {\n        "nps_dummy_1.port1": {\n            "STATE": -1,\n            "DESCR": "was 1",\n            "SWITCH": "nps_dummy_1",\n            "PORT": 1\n        },\n        "skye.what.ever": {\n            "STATE": -1,\n            "DESCR": "whatever is connected to skye",\n            "SWITCH": "nps_dummy_1",\n            "PORT": 2\n        },\n        "skyw.what.ever": {\n            "STATE": -1,\n            "DESCR": "Something @ skyw",\n            "SWITCH": "nps_dummy_1",\n            "PORT": 4\n        },\n        "skye.pwi": {\n            "STATE": -1,\n            "DESCR": "PlaneWavemount Skye",\n            "SWITCH": "skye.nps",\n            "PORT": 1\n        },\n            "skyw.pwi": {\n            "STATE": -1,\n            "DESCR": "PlaneWavemount Skyw",\n            "SWITCH": "nps_dummy_3",\n            "PORT": 1\n        }\n    }\n}\n```\n\n- status command with port name skyw.what.ever\n\n```console\n>>> lvmnps status skyw.what.ever\n\n12:07:12.349 lvmnps >\n12:07:12.377 lvmnps i {\n    "STATUS": {\n        "skyw.what.ever": {\n            "STATE": -1,\n            "DESCR": "Something @ skyw",\n            "SWITCH": "nps_dummy_1",\n            "PORT": 4\n}\n```\n\n- status command with switch name nps_dummy_1\n\n```console\n>>> lvmnps status nps_dummy_1\n\n12:07:12.349 lvmnps >\n12:12:21.349 lvmnps i {\n    "STATUS": {\n        "nps_dummy_1.port1": {\n            "STATE": -1,\n            "DESCR": "was 1",\n            "SWITCH": "nps_dummy_1",\n            "PORT": 1\n        },\n        "skye.what.ever": {\n            "STATE": -1,\n            "DESCR": "whatever is connected to skye",\n            "SWITCH": "nps_dummy_1",\n            "PORT": 2\n        },\n        "skyw.what.ever": {\n            "STATE": -1,\n            "DESCR": "Something @ skyw",\n            "SWITCH": "nps_dummy_1",\n            "PORT": 4\n        }\n    }\n}\n```\n\n- status command with switch name nps_dummy_1 and port 4 returns\n\n```console\n      lvmnps status nps_dummy_1 4\n\n      12:07:12.349 lvmnps >\n      12:12:21.349 lvmnps i {\n          "STATUS": {\n              "skyw.what.ever": {\n                  "STATE": -1,\n                  "DESCR": "Something @ skyw",\n                  "SWITCH": "nps_dummy_1",\n                  "PORT": 4\n              }\n          }\n      }\n\n\n- the commands on and off use the same addressing scheme as status\n\n## Test\n\n```console\npoetry run pytest\npoetry run pytest -p no:logging -s -vv\n```\n',
-    'author': 'Florian Briegel',
-    'author_email': 'briegel@mpia.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/sdss/lvmnps',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+12:07:12.349 lvmnps >
+12:12:21.349 lvmnps i {
+    "STATUS": {
+        "nps_dummy_1.port1": {
+            "STATE": -1,
+            "DESCR": "was 1",
+            "SWITCH": "nps_dummy_1",
+            "PORT": 1
+        },
+        "skye.what.ever": {
+            "STATE": -1,
+            "DESCR": "whatever is connected to skye",
+            "SWITCH": "nps_dummy_1",
+            "PORT": 2
+        },
+        "skyw.what.ever": {
+            "STATE": -1,
+            "DESCR": "Something @ skyw",
+            "SWITCH": "nps_dummy_1",
+            "PORT": 4
+        }
+    }
 }
+```
+
+- status command with switch name nps_dummy_1 and port 4 returns
+
+```console
+      lvmnps status nps_dummy_1 4
 
+      12:07:12.349 lvmnps >
+      12:12:21.349 lvmnps i {
+          "STATUS": {
+              "skyw.what.ever": {
+                  "STATE": -1,
+                  "DESCR": "Something @ skyw",
+                  "SWITCH": "nps_dummy_1",
+                  "PORT": 4
+              }
+          }
+      }
+
+
+- the commands on and off use the same addressing scheme as status
+
+## Test
+
+```console
+poetry run pytest
+poetry run pytest -p no:logging -s -vv
+```
 
-setup(**setup_kwargs)
```

