# Comparing `tmp/sdss-lvmieb-0.4.0.tar.gz` & `tmp/sdss_lvmieb-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss-lvmieb-0.4.0.tar", max compression
+gzip compressed data, was "sdss_lvmieb-0.5.0.tar", max compression
```

## Comparing `sdss-lvmieb-0.4.0.tar` & `sdss_lvmieb-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1504 2022-05-02 01:11:20.871801 sdss-lvmieb-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     1604 2022-05-16 02:19:43.704290 sdss-lvmieb-0.4.0/README.md
--rw-r--r--   0        0        0     2456 2022-05-29 00:07:37.663934 sdss-lvmieb-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      342 2022-05-16 02:16:45.552494 sdss-lvmieb-0.4.0/python/lvmieb/__init__.py
--rw-r--r--   0        0        0     1528 2022-05-16 02:16:45.553478 sdss-lvmieb-0.4.0/python/lvmieb/__main__.py
--rw-r--r--   0        0        0      264 2022-05-16 02:16:45.554538 sdss-lvmieb-0.4.0/python/lvmieb/actor/__init__.py
--rw-r--r--   0        0        0     3715 2022-05-16 02:16:45.555592 sdss-lvmieb-0.4.0/python/lvmieb/actor/actor.py
--rw-r--r--   0        0        0     1023 2022-05-16 02:16:45.556627 sdss-lvmieb-0.4.0/python/lvmieb/actor/commands/__init__.py
--rw-r--r--   0        0        0     1472 2022-05-16 02:16:45.558506 sdss-lvmieb-0.4.0/python/lvmieb/actor/commands/depth.py
--rw-r--r--   0        0        0     5470 2022-05-16 02:16:45.559359 sdss-lvmieb-0.4.0/python/lvmieb/actor/commands/hartmann.py
--rw-r--r--   0        0        0     4353 2022-05-16 02:16:45.560139 sdss-lvmieb-0.4.0/python/lvmieb/actor/commands/shutter.py
--rw-r--r--   0        0        0     1609 2022-05-16 02:16:45.561110 sdss-lvmieb-0.4.0/python/lvmieb/actor/commands/transducer.py
--rw-r--r--   0        0        0     3959 2022-05-16 02:16:45.562266 sdss-lvmieb-0.4.0/python/lvmieb/actor/commands/wago.py
--rw-r--r--   0        0        0       86 2022-05-16 02:16:45.563764 sdss-lvmieb-0.4.0/python/lvmieb/controller/__init__.py
--rw-r--r--   0        0        0     1548 2022-05-16 02:16:45.566207 sdss-lvmieb-0.4.0/python/lvmieb/controller/controller.py
--rw-r--r--   0        0        0     1393 2022-05-16 02:16:45.567632 sdss-lvmieb-0.4.0/python/lvmieb/controller/depth.py
--rw-r--r--   0        0        0      349 2022-05-16 02:16:45.568309 sdss-lvmieb-0.4.0/python/lvmieb/controller/maskbits.py
--rw-r--r--   0        0        0     7296 2022-05-16 02:16:45.569615 sdss-lvmieb-0.4.0/python/lvmieb/controller/motor.py
--rw-r--r--   0        0        0     2157 2022-05-16 02:16:45.570416 sdss-lvmieb-0.4.0/python/lvmieb/controller/pressure.py
--rw-r--r--   0        0        0     2245 2022-05-16 02:16:45.571844 sdss-lvmieb-0.4.0/python/lvmieb/controller/wago.py
--rw-r--r--   0        0        0     3160 2022-05-16 02:16:45.573583 sdss-lvmieb-0.4.0/python/lvmieb/etc/lvmieb.yml
--rw-r--r--   0        0        0     1835 2022-05-16 02:16:45.574624 sdss-lvmieb-0.4.0/python/lvmieb/etc/schema.json
--rw-r--r--   0        0        0      926 2022-05-16 02:16:45.575954 sdss-lvmieb-0.4.0/python/lvmieb/exceptions.py
--rw-r--r--   0        0        0     2755 1970-01-01 00:00:00.000000 sdss-lvmieb-0.4.0/setup.py
--rw-r--r--   0        0        0     2865 1970-01-01 00:00:00.000000 sdss-lvmieb-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-10 09:43:41.025796 sdss_lvmieb-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     1604 2023-07-10 09:43:41.025796 sdss_lvmieb-0.5.0/README.md
+-rw-r--r--   0        0        0     2391 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      342 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/__init__.py
+-rw-r--r--   0        0        0     1954 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/__main__.py
+-rw-r--r--   0        0        0      264 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/actor/__init__.py
+-rw-r--r--   0        0        0     3721 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/actor/actor.py
+-rw-r--r--   0        0        0     1109 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1472 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/actor/commands/depth.py
+-rw-r--r--   0        0        0     6860 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/actor/commands/hartmann.py
+-rw-r--r--   0        0        0     5529 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/actor/commands/shutter.py
+-rw-r--r--   0        0        0     1636 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/actor/commands/transducer.py
+-rw-r--r--   0        0        0     4195 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/actor/commands/wago.py
+-rw-r--r--   0        0        0       86 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/controller/__init__.py
+-rw-r--r--   0        0        0     1547 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/controller/controller.py
+-rw-r--r--   0        0        0     1392 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/controller/depth.py
+-rw-r--r--   0        0        0      349 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/controller/maskbits.py
+-rw-r--r--   0        0        0     7296 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/controller/motor.py
+-rw-r--r--   0        0        0     2157 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/controller/pressure.py
+-rw-r--r--   0        0        0     2244 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/controller/wago.py
+-rw-r--r--   0        0        0     3682 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/etc/lvmieb.yml
+-rw-r--r--   0        0        0     1834 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/etc/schema.json
+-rw-r--r--   0        0        0      925 2023-07-10 09:43:41.045796 sdss_lvmieb-0.5.0/python/lvmieb/exceptions.py
+-rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 sdss_lvmieb-0.5.0/PKG-INFO
```

### Comparing `sdss-lvmieb-0.4.0/LICENSE.md` & `sdss_lvmieb-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-lvmieb-0.4.0/README.md` & `sdss_lvmieb-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss-lvmieb-0.4.0/pyproject.toml` & `sdss_lvmieb-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmieb"
-version = "0.4.0"
+version = "0.5.0"
 description = "Control software for the Local Volume Mapper Instrument Electronics Box"
 authors = ["Changgon Kim <changgonkim@khu.ac.kr>"]
 maintainers = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmieb"
 repository = "https://github.com/sdss/lvmieb"
@@ -20,66 +20,63 @@
 ]
 packages = [
     { include = "lvmieb", from = "python" }
 ]
 include = ["python/lvmieb/etc/*"]
 
 [tool.poetry.scripts]
-lvmieb = "lvmieb.__main__:lvmieb"
+lvmieb = "lvmieb.__main__:main"
 
 [tool.poetry.dependencies]
-python = "^3.9,<3.11"
+python = "^3.9,<3.12"
 sdsstools = ">=0.4.0"
-sdss-clu = "^1.6.1"
+sdss-clu = "^2.0.0"
 click-default-group = "^1.2.2"
 numpy = "^1.20.3"
-sdss-drift = "^0.4.2"
+sdss-drift = "1.0.2"
 
 [tool.poetry.dev-dependencies]
 ipython = ">=7.11.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
 pytest = ">=5.2.2"
 pytest-asyncio = ">=0.10.0"
 pytest-cov = ">=2.8.1"
 pytest-mock = ">=1.13.0"
 pytest-sugar = ">=0.9.2"
 isort = ">=4.3.21"
-codecov = ">=2.0.15"
 coverage = {version = ">=5.0", extras = ["toml"]}
 ipdb = ">=0.12.3"
 rstcheck = "^3.3.1"
 Sphinx = ">=3.0.0"
 black = ">=21.7b0"
 sphinx-click = ">=2.6.0"
 sphinx-jsonschema = ">=1.16.7"
 myst-parser = ">=0.14.0"
 furo = "^2021.6.18-beta.36"
 nox = "^2021.6.12"
 sphinx-autobuild = "^2021.3.14"
 sphinx-copybutton = "^0.3.3"
 
 [tool.isort]
-line_length = 79
-sections = ["FUTURE", "STDLIB", "THIRDPARTY", "SDSS", "FIRSTPARTY", "LOCALFOLDER"]
+profile = "black"
+sections = ["FUTURE", "STDLIB", "TYPING", "THIRDPARTY", "SDSS", "FIRSTPARTY", "LOCALFOLDER"]
 default_section = "THIRDPARTY"
 known_first_party = "lvmieb"
+known_typing = ["typing"]
 known_sdss = ["sdsstools", "clu", "drift"]
-balanced_wrapping = true
-include_trailing_comma = false
 lines_after_imports = 2
-use_parentheses = true
 
 [tool.pytest.ini_options]
 addopts = "--cov lvmieb --cov-report xml --cov-report html --cov-report term"
 asyncio_mode = "auto"
 
 [tool.black]
 line-length = 88
-target-version = ['py39']
+target-version = ['py311']
 fast = true
 
 [tool.coverage.run]
 branch = true
 include = ["python/lvmieb/*"]
 omit = [
     "python/lvmieb/__main__.py",
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/__main__.py` & `sdss_lvmieb-0.5.0/python/lvmieb/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,25 +3,39 @@
 # @Author: Changging Kim, Mingyeong Yang, Taeeun Kim
 # @Date: 2020-10-26
 # @Filename: __main__.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
+import asyncio
+import functools
 import os
 
 import click
 from click_default_group import DefaultGroup
 
-from clu.tools import cli_coro as cli_coro_lvm
 from sdsstools.daemonizer import DaemonGroup
 
 from lvmieb.actor.actor import IEBActor
 
 
+def cli_coro(f):
+    """Decorator function that allows defining coroutines with click."""
+
+    if hasattr(asyncio, "coroutine"):
+        f = getattr(asyncio, "coroutine")(f)
+
+    def wrapper(*args, **kwargs):
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(f(*args, **kwargs))
+
+    return functools.update_wrapper(wrapper, f)
+
+
 @click.group(cls=DefaultGroup, default="actor", default_if_no_args=True)
 @click.option(
     "-c",
     "--config",
     "config_file",
     type=click.Path(exists=True, dir_okay=False),
     help="Path to the user configuration file.",
@@ -37,26 +51,31 @@
     """LVM Electronics Box Controller."""
 
     ctx.obj = {"verbose": verbose, "config_file": config_file}
 
 
 @lvmieb.group(cls=DaemonGroup, prog="lvmieb_actor", workdir=os.getcwd())
 @click.pass_context
-@cli_coro_lvm
+@cli_coro
 async def actor(ctx):
     """Runs the actor."""
 
     default_config_file = os.path.join(os.path.dirname(__file__), "etc/lvmieb.yml")
     config_file = ctx.obj["config_file"] or default_config_file
 
     lvmieb_obj = IEBActor.from_config(config_file)
 
     if ctx.obj["verbose"]:
-        lvmieb_obj.log.fh.setLevel(0)
         lvmieb_obj.log.sh.setLevel(0)
+        if lvmieb_obj.log.fh:
+            lvmieb_obj.log.fh.setLevel(0)
 
     await lvmieb_obj.start()
     await lvmieb_obj.run_forever()
 
 
+def main():
+    lvmieb(auto_envvar_prefix="LVMIEB")
+
+
 if __name__ == "__main__":
-    lvmieb()
+    main()
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/actor/actor.py` & `sdss_lvmieb-0.5.0/python/lvmieb/actor/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 # @Filename: actor.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import os
 import pathlib
+import warnings
 from copy import deepcopy
-from typing import ClassVar
 
-from yaml import warnings
+from typing import ClassVar
 
 from clu import Command
 from clu.actor import AMQPActor
 from sdsstools.configuration import read_yaml_file
 
 from lvmieb import __version__, config
 from lvmieb.controller.controller import IEBController
@@ -49,15 +49,14 @@
     def __init__(
         self,
         *args,
         controllers: tuple[IEBController, ...] = (),
         depth_gauges: DepthGauges | None = None,
         **kwargs,
     ):
-
         self.controllers = {c.spec: c for c in controllers}
         self.depth_gauges = depth_gauges
 
         self.version = __version__
 
         super().__init__(*args, **kwargs)
 
@@ -87,15 +86,15 @@
             if not os.path.isabs(schema):
                 schema = os.path.join(
                     os.path.abspath(os.path.join(os.path.dirname(__file__), "../")),
                     schema,
                 )
             config["actor"]["schema"] = schema
 
-        instance = super().from_config(config["actor"])
+        instance = super().from_config(config["actor"], *args, **kwargs)
 
         controllers: list[IEBController] = []
 
         for spec in config.get("enabled_specs", []):
             if "specs" not in config or spec not in config["specs"]:
                 warnings.warn(
                     f"Cannot find configuration for {spec!r}.",
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/actor/commands/__init__.py` & `sdss_lvmieb-0.5.0/python/lvmieb/actor/commands/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,33 @@
 import glob
 import importlib
 import os
 
 import click
 
 from clu.command import Command
-from clu.parsers.click import CluGroup, command_parser, help_, ping, version
+from clu.parsers.click import (
+    CluGroup,
+    command_parser,
+    get_command_model,
+    help_,
+    ping,
+    version,
+)
 
 
 @click.group(cls=CluGroup)
 def parser(*args):
     pass
 
 
 parser.add_command(ping)
 parser.add_command(version)
 parser.add_command(help_)
+parser.add_command(get_command_model)
 
 
 # Autoimport all modules in this directory so that they are added to the parser.
 
 exclusions = ["__init__.py"]
 
 cwd = os.getcwd()
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/actor/commands/depth.py` & `sdss_lvmieb-0.5.0/python/lvmieb/actor/commands/depth.py`

 * *Files identical despite different names*

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/actor/commands/hartmann.py` & `sdss_lvmieb-0.5.0/python/lvmieb/actor/commands/shutter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,199 +1,209 @@
 # -*- coding: utf-8 -*-
+#
 # @Author: Changgon Kim, Mingyeong Yang, Taeeun Kim
 # @Date: 2021-05-12
-# @Filename: hartmann.py
+# @Filename: shutter.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 # added by CK 2021/03/30
 
 from __future__ import annotations
 
 import asyncio
+
 from typing import TYPE_CHECKING
 
 import click
 
 from lvmieb.controller.maskbits import MotorStatus
 from lvmieb.exceptions import MotorControllerError
 
 from . import parser
 
 
 if TYPE_CHECKING:
     from lvmieb.actor import ControllersType, IEBCommand
 
 
-__all__ = ["hartmann"]
+__all__ = ["shutter"]
 
 
 @parser.group()
-def hartmann(*args):
-    """Control the hartmann doors."""
+def shutter(*args):
+    """Control the shutter."""
 
     pass
 
 
-@hartmann.command()
-@click.option(
-    "-s",
-    "--side",
-    type=click.Choice(["all", "right", "left"]),
-    default="all",
-    help="all, right, or left",
-)
-@click.argument("spectro", type=click.Choice(["sp1", "sp2", "sp3"]))
+@shutter.command()
+@click.argument("spectro", type=click.Choice(["sp1", "sp2", "sp3"]), required=False)
 async def open(
     command: IEBCommand,
     controllers: ControllersType,
-    side: str,
-    spectro: str,
+    spectro: str | None = None,
 ):
-    """Open the Hartmann doors."""
+    """Open the shutter."""
+
+    if spectro is None:
+        if len(controllers) > 1:
+            return command.fail("Multiple controllers present, SPECTRO is required.")
+        spectro = list(controllers.keys())[0]
 
     if spectro not in controllers:
         return command.fail(error=f"Spectrograph {spectro!r} is not available.")
 
     controller = controllers[spectro]
 
     tasks = []
-    if side == "all" or side == "left":
-        tasks.append(controller.motors["hartmann_left"].move(open=True))
-    if side == "all" or side == "right":
-        tasks.append(controller.motors["hartmann_right"].move(open=True))
+    tasks.append(controller.motors["shutter"].move(open=True))
 
-    command.info(text=f"Opening {side} hartmanns")
+    command.info(text="Opening shutter")
     try:
         await asyncio.gather(*tasks)
     except MotorControllerError as err:
         return command.fail(error=err)
 
-    await (await command.child_command(f"hartmann status {spectro}"))
+    await (await command.child_command(f"shutter status {spectro}"))
 
     return command.finish()
 
 
-@hartmann.command()
-@click.option(
-    "-s",
-    "--side",
-    type=click.Choice(["all", "right", "left"]),
-    default="all",
-    help="all, right, or left",
-)
-@click.argument("spectro", type=click.Choice(["sp1", "sp2", "sp3"]))
+@shutter.command()
+@click.argument("spectro", type=click.Choice(["sp1", "sp2", "sp3"]), required=False)
 async def close(
     command: IEBCommand,
     controllers: ControllersType,
-    side: str,
-    spectro: str,
+    spectro: str | None = None,
 ):
-    """Close the Hartmann doors."""
+    """Close the shutter."""
+
+    if spectro is None:
+        if len(controllers) > 1:
+            return command.fail("Multiple controllers present, SPECTRO is required.")
+        spectro = list(controllers.keys())[0]
 
     if spectro not in controllers:
         return command.fail(error=f"Spectrograph {spectro!r} is not available.")
 
     controller = controllers[spectro]
 
     tasks = []
-    if side == "all" or side == "left":
-        tasks.append(controller.motors["hartmann_left"].move(open=False))
-    if side == "all" or side == "right":
-        tasks.append(controller.motors["hartmann_right"].move(open=False))
+    tasks.append(controller.motors["shutter"].move(open=False))
 
-    command.info(text=f"Closing {side} hartmanns")
+    command.info(text="Closing shutter")
     try:
         await asyncio.gather(*tasks)
     except MotorControllerError as err:
         return command.fail(error=err)
 
-    await (await command.child_command(f"hartmann status {spectro}"))
+    await (await command.child_command(f"shutter status {spectro}"))
 
     return command.finish()
 
 
-@hartmann.command()
-@click.argument("spectro", type=click.Choice(["sp1", "sp2", "sp3"]))
-async def status(command: IEBCommand, controllers: ControllersType, spectro: str):
-    """Reports the position of the Hartmann doors."""
+@shutter.command()
+@click.argument("spectro", type=click.Choice(["sp1", "sp2", "sp3"]), required=False)
+async def status(
+    command: IEBCommand,
+    controllers: ControllersType,
+    spectro: str | None = None,
+):
+    """Reports the position of the shutter."""
+
+    if spectro is None:
+        if len(controllers) > 1:
+            return command.fail("Multiple controllers present, SPECTRO is required.")
+        spectro = list(controllers.keys())[0]
 
     if spectro not in controllers:
         return command.fail(error=f"Spectrograph {spectro!r} is not available.")
 
     controller = controllers[spectro]
 
     tasks = []
-    tasks.append(controller.motors["hartmann_left"].get_status())
-    tasks.append(controller.motors["hartmann_right"].get_status())
+    tasks.append(controller.motors["shutter"].get_status())
 
-    result_hartmann = await asyncio.gather(*tasks)
+    result_shutter = await asyncio.gather(*tasks)
 
-    hd_status = {}
-    for i, name in enumerate(["left", "right"]):
-        motor_status, bits = result_hartmann[i]
-
-        power = motor_status & MotorStatus.POWER_ON
-        open = motor_status & MotorStatus.OPEN
-        invalid = motor_status & (
-            MotorStatus.POSITION_INVALID
-            | MotorStatus.POSITION_UNKNOWN
-            | MotorStatus.POWER_UNKNOWN
-        )
-
-        hd_status[name] = {
-            "power": power.value > 0,
-            "open": open.value > 0,
-            "invalid": invalid.value > 0,
-            "bits": bits or "?",
-        }
-
-    command.info({f"{spectro}_hartmann_left": hd_status["left"]})
-    command.info({f"{spectro}_hartmann_right": hd_status["right"]})
-
-    return command.finish()
+    shutter_status = {}
+    motor_status, bits = result_shutter[0]
 
+    power = motor_status & MotorStatus.POWER_ON
+    open = motor_status & MotorStatus.OPEN
+    invalid = motor_status & (
+        MotorStatus.POSITION_INVALID
+        | MotorStatus.POSITION_UNKNOWN
+        | MotorStatus.POWER_UNKNOWN
+    )
+
+    shutter_status = {
+        "power": power.value > 0,
+        "open": open.value > 0,
+        "invalid": invalid.value > 0,
+        "bits": bits or "?",
+    }
+
+    return command.finish({f"{spectro}_shutter": shutter_status})
+
+
+@shutter.command()
+@click.argument("spectro", type=click.Choice(["sp1", "sp2", "sp3"]), required=False)
+async def init(
+    command: IEBCommand,
+    controllers: ControllersType,
+    spectro: str | None = None,
+):
+    """Initialise the shutter."""
 
-@hartmann.command()
-@click.argument("spectro", type=click.Choice(["sp1", "sp2", "sp3"]))
-async def init(command: IEBCommand, controllers: ControllersType, spectro: str):
-    """Initialise the hartmanns."""
+    if spectro is None:
+        if len(controllers) > 1:
+            return command.fail("Multiple controllers present, SPECTRO is required.")
+        spectro = list(controllers.keys())[0]
 
     if spectro not in controllers:
         return command.fail(error=f"Spectrograph {spectro!r} is not available.")
 
     controller = controllers[spectro]
 
-    command.info(text="Initializing all hartmanns")
+    command.info(text="Initializing shutter")
 
     tasks = []
-    for hd in ["hartmann_left", "hartmann_right"]:
-        tasks.append(controller.motors[hd].send_command("init"))
+    tasks.append(controller.motors["shutter"].send_command("init"))
 
     try:
         await asyncio.gather(*tasks)
     except MotorControllerError as err:
         return command.fail(error=err)
 
     return command.finish()
 
 
-@hartmann.command()
-@click.argument("spectro", type=click.Choice(["sp1", "sp2", "sp3"]))
-async def home(command: IEBCommand, controllers: ControllersType, spectro: str):
-    """Home the hartmann doors."""
+@shutter.command()
+@click.argument("spectro", type=click.Choice(["sp1", "sp2", "sp3"]), required=False)
+async def home(
+    command: IEBCommand,
+    controllers: ControllersType,
+    spectro: str | None = None,
+):
+    """Home the shutter."""
+
+    if spectro is None:
+        if len(controllers) > 1:
+            return command.fail("Multiple controllers present, SPECTRO is required.")
+        spectro = list(controllers.keys())[0]
 
     if spectro not in controllers:
         return command.fail(error=f"Spectrograph {spectro!r} is not available.")
 
     controller = controllers[spectro]
 
-    command.info(text="Home all hartmanns")
+    command.info(text="Homing shutter")
 
     tasks = []
-    for hd in ["hartmann_left", "hartmann_right"]:
-        tasks.append(controller.motors[hd].send_command("home"))
+    tasks.append(controller.motors["shutter"].send_command("home"))
 
     try:
         await asyncio.gather(*tasks)
     except MotorControllerError as err:
         return command.fail(error=err)
 
     return command.finish()
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/actor/commands/transducer.py` & `sdss_lvmieb-0.5.0/python/lvmieb/actor/commands/transducer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+
 from typing import TYPE_CHECKING
 
 import click
 
 from . import parser
 
 
@@ -43,13 +44,13 @@
 
     pres_list = await asyncio.gather(*tasks, return_exceptions=True)
 
     for ii, camera in enumerate(camera_order):
         camera_results = pres_list[2 * ii : 2 * ii + 2]
         for jj, measurement in enumerate(["pressure", "temperature"]):
             camera_result = camera_results[jj]
-            if isinstance(camera_result, Exception):
+            if camera_result is False or isinstance(camera_result, Exception):
                 command.warning(f"Failed getting {camera} {measurement}.")
                 camera_result = -999.0
             pres_result[f"{camera}_{measurement}"] = camera_result
 
     command.finish(transducer=pres_result)
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/actor/commands/wago.py` & `sdss_lvmieb-0.5.0/python/lvmieb/actor/commands/wago.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # @Date: 2021-03-22
 # @Filename: telemetry.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import asyncio
+
 from typing import TYPE_CHECKING
 
 import click
 
 from . import parser
 
 
@@ -104,15 +105,19 @@
 
 
 @wago.command()
 @click.argument(
     "DEVICE",
     type=click.Choice(["shutter", "hartmann_left", "hartmann_right"]),
 )
-@click.argument("SPECTRO", type=click.Choice(["sp1", "sp2", "sp3"]))
+@click.argument(
+    "SPECTRO",
+    type=click.Choice(["sp1", "sp2", "sp3"]),
+    required=False,
+)
 @click.option(
     "--on",
     "action",
     flag_value="ON",
     required=True,
     help="Turn on device",
 )
@@ -124,18 +129,23 @@
     help="Turn off device",
 )
 async def setpower(
     command: IEBCommand,
     controllers: ControllersType,
     device: str,
     action: str,
-    spectro: str,
+    spectro: str | None = None,
 ):
     """Switches power on/off to a device."""
 
+    if spectro is None:
+        if len(controllers) > 1:
+            return command.fail("Multiple controllers present, SPECTRO is required.")
+        spectro = list(controllers.keys())[0]
+
     if spectro not in controllers:
         return command.fail(error=f"Spectrograph {spectro!r} is not available.")
 
     controller = controllers[spectro]
 
     try:
         closed = True if action == "ON" else False
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/controller/controller.py` & `sdss_lvmieb-0.5.0/python/lvmieb/controller/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     def __init__(
         self,
         spec: str,
         wago: IEBWAGO,
         pressure: list[PressureTransducer] = [],
         motors: list[MotorController] = [],
     ):
-
         self.spec = spec
 
         self.wago = wago
         self.pressure = {p.camera: p for p in pressure}
         self.motors = {m.type: m for m in motors}
 
     @classmethod
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/controller/depth.py` & `sdss_lvmieb-0.5.0/python/lvmieb/controller/depth.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 __all__ = ["DepthGauges"]
 
 
 class DepthGauges:
     """Reads the value of Heidenhain depth gauges."""
 
     def __init__(self, host: str, port: int, camera: str | None = None):
-
         self.host = host
         self.port = port
         self.camera = camera
 
     async def read(self):
         """Returns the measured values from the depth probes."""
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/controller/motor.py` & `sdss_lvmieb-0.5.0/python/lvmieb/controller/motor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from __future__ import annotations
 
 import asyncio
 import re
 import warnings
 from dataclasses import dataclass
+
 from typing import TYPE_CHECKING, Optional
 
 from lvmieb.controller.maskbits import MotorStatus
 from lvmieb.exceptions import LvmIebUserWarning, MotorControllerError
 
 
 if TYPE_CHECKING:
@@ -54,15 +55,14 @@
     host: str
     port: int
     wago: Optional[IEBWAGO] = None
 
     TIMEOUT: float = 5
 
     def __post_init__(self):
-
         if self.type not in DEVLIST:
             raise ValueError(f"Device type {self.type} is not valid.")
 
     async def get_power_status(self):
         """Returns the power status of a motor controller."""
 
         if self.wago is None:
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/controller/pressure.py` & `sdss_lvmieb-0.5.0/python/lvmieb/controller/pressure.py`

 * *Files identical despite different names*

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/controller/wago.py` & `sdss_lvmieb-0.5.0/python/lvmieb/controller/wago.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         The port serving the TCP modbus service.
     name
         The name associated with this WAGO controller.
 
     """
 
     def __init__(self, host: str, port: int = 502, name: str = ""):
-
         super().__init__(host, port)
 
         self.name = name
 
     async def read_sensors(
         self,
         units: bool = False,
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/etc/lvmieb.yml` & `sdss_lvmieb-0.5.0/python/lvmieb/etc/lvmieb.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-enabled_specs: [sp2]
+enabled_specs: [sp2, sp3]
 
 specs:
   sp1:
     wago:
       address: 10.7.45.28
       port: 502
     motor_controllers:
@@ -40,25 +40,52 @@
         host: 10.7.45.27
         port: 7777
       hartmann_right:
         host: 10.7.45.27
         port: 7778
     pressure:
       r2:
-        host: 10.7.45.33
+        host: 10.7.45.30
         port: 1112
         device_id: 253
       b2:
         host: 10.7.45.33
         port: 1114
         device_id: 253
       z2:
         host: 10.7.45.33
         port: 1115
         device_id: 253
+  sp3:
+    wago:
+      address: 10.7.45.37
+      port: 502
+    motor_controllers:
+      shutter:
+        host: 10.7.45.37
+        port: 7776
+      hartmann_left:
+        host: 10.7.45.37
+        port: 7777
+      hartmann_right:
+        host: 10.7.45.37
+        port: 7778
+    pressure:
+      r2:
+        host: 10.7.45.30
+        port: 1112
+        device_id: 253
+      b2:
+        host: 10.7.45.30
+        port: 1114
+        device_id: 253
+      z2:
+        host: 10.7.45.30
+        port: 1115
+        device_id: 253
 
 wago_modules:
   ANALOG1:
     model: 750-497
     mode: input_register
     channels: 8
     description: E+E temperature and humidity sensors
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/etc/schema.json` & `sdss_lvmieb-0.5.0/python/lvmieb/etc/schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333334%*

 * *Differences: {"'patternProperties'": "{'sp[0-9]_sensors': {'additionalProperties': True}}"}*

```diff
@@ -31,15 +31,15 @@
                 "shutter": {
                     "type": "boolean"
                 }
             },
             "type": "object"
         },
         "sp[0-9]_sensors": {
-            "additionalProperties": false,
+            "additionalProperties": true,
             "properties": {
                 "rh1": {
                     "type": "number"
                 },
                 "rh2": {
                     "type": "number"
                 },
```

### Comparing `sdss-lvmieb-0.4.0/python/lvmieb/exceptions.py` & `sdss_lvmieb-0.5.0/python/lvmieb/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from __future__ import annotations
 
 
 class LvmIebError(Exception):
     """A custom core LvmIeb exception"""
 
     def __init__(self, message=None):
-
         message = "There has been an error" if not message else message
 
         super(LvmIebError, self).__init__(message)
 
 
 class MotorControllerError(LvmIebError):
     """A motor controller error."""
```

### Comparing `sdss-lvmieb-0.4.0/setup.py` & `sdss_lvmieb-0.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,93 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-package_dir = \
-{'': 'python'}
-
-packages = \
-['lvmieb', 'lvmieb.actor', 'lvmieb.actor.commands', 'lvmieb.controller']
-
-package_data = \
-{'': ['*'], 'lvmieb': ['etc/*']}
-
-install_requires = \
-['click-default-group>=1.2.2,<2.0.0',
- 'numpy>=1.20.3,<2.0.0',
- 'sdss-clu>=1.6.1,<2.0.0',
- 'sdss-drift>=0.4.2,<0.5.0',
- 'sdsstools>=0.4.0']
-
-entry_points = \
-{'console_scripts': ['lvmieb = lvmieb.__main__:lvmieb']}
-
-setup_kwargs = {
-    'name': 'sdss-lvmieb',
-    'version': '0.4.0',
-    'description': 'Control software for the Local Volume Mapper Instrument Electronics Box',
-    'long_description': '# lvmieb\n\n![Versions](https://img.shields.io/badge/python->3.8-blue)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Documentation Status](https://readthedocs.org/projects/lvmieb/badge/?version=latest)](https://lvmieb.readthedocs.io/en/latest/?badge=latest)\n[![Test](https://github.com/sdss/lvmieb/actions/workflows/test.yml/badge.svg)](https://github.com/sdss/lvmieb/actions/workflows/test.yml)\n[![Docker](https://github.com/sdss/lvmieb/actions/workflows/docker.yml/badge.svg)](https://github.com/sdss/lvmieb/actions/workflows/docker.yml)\n[![codecov](https://codecov.io/gh/sdss/lvmieb/branch/main/graph/badge.svg?token=IyQglaQYSF)](https://codecov.io/gh/sdss/lvmieb)\n\nControl software for the SDSS-V LVM (Local Volume Mapper) spectrograph Instrument Electronics Box (IEB).\n\n## Quick Start\n\n### Installation\n\n`lvmieb` uses the [CLU](https://clu.readthedocs.io/en/latest/) framework and requires a RabbitMQ instance running in the background.\n\n`lvmieb` can be installed using `pip`\n\n```console\npip install sdss-lvmieb\n```\n\nor by cloning this repository\n\n```console\ngit clone https://github.com/sdss/lvmieb\n```\n\nThe preferred installation for development is using [poetry](https://python-poetry.org/)\n\n```console\ncd lvmieb\npoetry install\n```\n\n\n### Basic ping-pong test\n\nStart the `lvmieb` actor.\n\n```console\nlvmieb start\n```\n\nIn another terminal, type `clu` and `lvmieb ping` for test.\n\n```console\n$ clu\nlvmieb ping\n07:41:22.636 lvmieb >\n07:41:22.645 lvmieb : {\n    "text": "Pong."\n}\n```\n\nStop `lvmieb` actor.\n\n```console\nlvmieb stop\n```\n',
-    'author': 'Changgon Kim',
-    'author_email': 'changgonkim@khu.ac.kr',
-    'maintainer': 'José Sánchez-Gallego',
-    'maintainer_email': 'gallegoj@uw.edu',
-    'url': 'https://github.com/sdss/lvmieb',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<3.11',
+Metadata-Version: 2.1
+Name: sdss-lvmieb
+Version: 0.5.0
+Summary: Control software for the Local Volume Mapper Instrument Electronics Box
+Home-page: https://github.com/sdss/lvmieb
+License: BSD-3-Clause
+Keywords: astronomy,software
+Author: Changgon Kim
+Author-email: changgonkim@khu.ac.kr
+Maintainer: José Sánchez-Gallego
+Maintainer-email: gallegoj@uw.edu
+Requires-Python: >=3.9,<3.12
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Documentation :: Sphinx
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
+Requires-Dist: numpy (>=1.20.3,<2.0.0)
+Requires-Dist: sdss-clu (>=2.0.0,<3.0.0)
+Requires-Dist: sdss-drift (==1.0.2)
+Requires-Dist: sdsstools (>=0.4.0)
+Project-URL: Documentation, https://sdss-lvmieb.readthedocs.org
+Project-URL: Repository, https://github.com/sdss/lvmieb
+Description-Content-Type: text/markdown
+
+# lvmieb
+
+![Versions](https://img.shields.io/badge/python->3.8-blue)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/lvmieb/badge/?version=latest)](https://lvmieb.readthedocs.io/en/latest/?badge=latest)
+[![Test](https://github.com/sdss/lvmieb/actions/workflows/test.yml/badge.svg)](https://github.com/sdss/lvmieb/actions/workflows/test.yml)
+[![Docker](https://github.com/sdss/lvmieb/actions/workflows/docker.yml/badge.svg)](https://github.com/sdss/lvmieb/actions/workflows/docker.yml)
+[![codecov](https://codecov.io/gh/sdss/lvmieb/branch/main/graph/badge.svg?token=IyQglaQYSF)](https://codecov.io/gh/sdss/lvmieb)
+
+Control software for the SDSS-V LVM (Local Volume Mapper) spectrograph Instrument Electronics Box (IEB).
+
+## Quick Start
+
+### Installation
+
+`lvmieb` uses the [CLU](https://clu.readthedocs.io/en/latest/) framework and requires a RabbitMQ instance running in the background.
+
+`lvmieb` can be installed using `pip`
+
+```console
+pip install sdss-lvmieb
+```
+
+or by cloning this repository
+
+```console
+git clone https://github.com/sdss/lvmieb
+```
+
+The preferred installation for development is using [poetry](https://python-poetry.org/)
+
+```console
+cd lvmieb
+poetry install
+```
+
+
+### Basic ping-pong test
+
+Start the `lvmieb` actor.
+
+```console
+lvmieb start
+```
+
+In another terminal, type `clu` and `lvmieb ping` for test.
+
+```console
+$ clu
+lvmieb ping
+07:41:22.636 lvmieb >
+07:41:22.645 lvmieb : {
+    "text": "Pong."
 }
+```
+
+Stop `lvmieb` actor.
 
+```console
+lvmieb stop
+```
 
-setup(**setup_kwargs)
```

