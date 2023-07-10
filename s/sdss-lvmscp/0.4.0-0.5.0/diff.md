# Comparing `tmp/sdss_lvmscp-0.4.0.tar.gz` & `tmp/sdss_lvmscp-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmscp-0.4.0.tar", max compression
+gzip compressed data, was "sdss_lvmscp-0.5.0.tar", max compression
```

## Comparing `sdss_lvmscp-0.4.0.tar` & `sdss_lvmscp-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1504 2023-03-04 21:35:04.790053 sdss_lvmscp-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     1578 2023-03-04 21:35:04.790262 sdss_lvmscp-0.4.0/README.md
--rw-r--r--   0        0        0     2733 2023-03-04 21:35:04.945355 sdss_lvmscp-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      369 2023-03-04 21:35:04.945682 sdss_lvmscp-0.4.0/python/lvmscp/__init__.py
--rw-r--r--   0        0        0     1618 2023-03-04 21:35:05.018453 sdss_lvmscp-0.4.0/python/lvmscp/__main__.py
--rw-r--r--   0        0        0      258 2023-03-04 21:35:05.019399 sdss_lvmscp-0.4.0/python/lvmscp/actor/__init__.py
--rw-r--r--   0        0        0     8161 2023-03-04 21:35:05.019955 sdss_lvmscp-0.4.0/python/lvmscp/actor/actor.py
--rw-r--r--   0        0        0      859 2023-03-04 21:35:05.020264 sdss_lvmscp-0.4.0/python/lvmscp/actor/commands/__init__.py
--rw-r--r--   0        0        0     1515 2023-03-04 21:35:05.020480 sdss_lvmscp-0.4.0/python/lvmscp/actor/commands/expose.py
--rw-r--r--   0        0        0     3827 2023-03-04 21:35:05.020694 sdss_lvmscp-0.4.0/python/lvmscp/actor/commands/focus.py
--rw-r--r--   0        0        0     1272 2023-03-04 21:35:05.020900 sdss_lvmscp-0.4.0/python/lvmscp/actor/commands/hardware_status.py
--rw-r--r--   0        0        0    10418 2023-03-04 21:35:05.021143 sdss_lvmscp-0.4.0/python/lvmscp/delegate.py
--rw-r--r--   0        0        0    40775 2023-03-04 21:35:05.021504 sdss_lvmscp-0.4.0/python/lvmscp/etc/LVM_100kHz.acf
--rw-r--r--   0        0        0     5526 2023-03-04 21:35:05.021742 sdss_lvmscp-0.4.0/python/lvmscp/etc/lvmscp.yml
--rw-r--r--   0        0        0      161 2023-03-04 21:35:05.021918 sdss_lvmscp-0.4.0/python/lvmscp/etc/schema.json
--rw-r--r--   0        0        0     3083 1970-01-01 00:00:00.000000 sdss_lvmscp-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-10 05:47:11.766281 sdss_lvmscp-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     1578 2023-07-10 05:47:11.766723 sdss_lvmscp-0.5.0/README.md
+-rw-r--r--   0        0        0     2714 2023-07-10 05:47:11.810868 sdss_lvmscp-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-07-10 05:47:11.811326 sdss_lvmscp-0.5.0/python/lvmscp/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-10 05:47:11.811631 sdss_lvmscp-0.5.0/python/lvmscp/__main__.py
+-rw-r--r--   0        0        0      258 2023-07-10 05:47:11.812037 sdss_lvmscp-0.5.0/python/lvmscp/actor/__init__.py
+-rw-r--r--   0        0        0     8321 2023-07-10 05:47:11.812308 sdss_lvmscp-0.5.0/python/lvmscp/actor/actor.py
+-rw-r--r--   0        0        0      859 2023-07-10 05:47:11.812630 sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1515 2023-07-10 05:47:11.812852 sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/expose.py
+-rw-r--r--   0        0        0     3827 2023-07-10 05:47:11.813100 sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/focus.py
+-rw-r--r--   0        0        0     1272 2023-07-10 05:47:11.813395 sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/hardware_status.py
+-rw-r--r--   0        0        0      758 2023-07-10 05:47:11.813673 sdss_lvmscp-0.5.0/python/lvmscp/controller.py
+-rw-r--r--   0        0        0    13581 2023-07-10 05:47:11.814001 sdss_lvmscp-0.5.0/python/lvmscp/delegate.py
+-rw-r--r--   0        0        0    40775 2023-07-10 05:47:11.814476 sdss_lvmscp-0.5.0/python/lvmscp/etc/LVM_100kHz.acf
+-rw-r--r--   0        0        0     5466 2023-07-10 05:47:11.814738 sdss_lvmscp-0.5.0/python/lvmscp/etc/lvmscp.yml
+-rw-r--r--   0        0        0      161 2023-07-10 05:47:11.814918 sdss_lvmscp-0.5.0/python/lvmscp/etc/schema.json
+-rw-r--r--   0        0        0    18807 2023-07-10 05:47:11.815206 sdss_lvmscp-0.5.0/python/lvmscp/ln2.py
+-rw-r--r--   0        0        0     2811 1970-01-01 00:00:00.000000 sdss_lvmscp-0.5.0/PKG-INFO
```

### Comparing `sdss_lvmscp-0.4.0/LICENSE.md` & `sdss_lvmscp-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.4.0/README.md` & `sdss_lvmscp-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.4.0/pyproject.toml` & `sdss_lvmscp-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmscp"
-version = "0.4.0"
+version = "0.5.0"
 description = "LVM spectrograph control package."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>", "Changgon Kim <changgonkim@khu.ac.kr>"]
 maintainers = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmscp"
 repository = "https://github.com/sdss/lvmscp"
@@ -23,22 +23,20 @@
 packages = [
     { include = "lvmscp", from = "python" }
 ]
 include = ["python/lvmscp/etc/*"]
 
 [tool.poetry.scripts]
 lvmscp = "lvmscp.__main__:main"
+ln2fill = "lvmscp.ln2:ln2fill"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-sdsstools = "^1.0.0"
-click = "^8.1.2"
 click-default-group = "^1.2.2"
-sdss-clu = "^1.6.1"
-sdss-archon = "^0.8.0"
+sdss-archon = "^0.9.0"
 httpx = ">=0.18.1"
 Authlib = ">=1.0.0rc1"
 
 [tool.poetry.dev-dependencies]
 ipython = ">=7.11.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
@@ -52,15 +50,14 @@
 
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
@@ -70,15 +67,15 @@
 nox = ">=2021.6.12"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-copybutton = ">=0.3.3"
 sphinx-click = ">=3.0.1"
 
 [tool.black]
 line-length = 88
-target-version = ['py39']
+target-version = ['py311']
 fast = true
 
 [tool.isort]
 line_length = 79
 sections = ["FUTURE", "STDLIB", "THIRDPARTY", "SDSS", "FIRSTPARTY", "LOCALFOLDER"]
 default_section = "THIRDPARTY"
 known_first_party = "lvmscp"
@@ -92,14 +89,15 @@
 addopts = "--cov lvmscp --cov-report xml --cov-report html --cov-report term"
 asyncio_mode = "auto"
 
 [tool.coverage.run]
 branch = true
 omit = [
     "python/lvmscp/__main__.py",
+    "python/lvmscp/ln2.py",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING"
 ]
```

### Comparing `sdss_lvmscp-0.4.0/python/lvmscp/__main__.py` & `sdss_lvmscp-0.5.0/python/lvmscp/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.4.0/python/lvmscp/actor/actor.py` & `sdss_lvmscp-0.5.0/python/lvmscp/actor/actor.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from archon.actor import ArchonActor
 from archon.actor.tools import get_schema
 from archon.exceptions import ArchonWarning
 from clu import Command
 from sdsstools.configuration import read_yaml_file
 
 from lvmscp import config
+from lvmscp.controller import SCPController
 from lvmscp.delegate import LVMExposeDelegate
 
 from .commands import parser
 
 
 if TYPE_CHECKING:
     from clu.model import Property
@@ -41,18 +42,22 @@
 
 class SCPActor(ArchonActor):
     """The main actor class of the lvmscp."""
 
     parser = parser
     BASE_CONFIG: ClassVar[str | dict | None] = config
     DELEGATE_CLASS = LVMExposeDelegate
+    CONTROLLER_CLASS = SCPController
 
     def __init__(self, *args, **kwargs):
         schema = self.merge_schemas(kwargs.pop("schema", None))
 
+        # Just for typing.
+        self.controllers: dict[str, SCPController]
+
         super().__init__(*args, schema=schema, **kwargs)
 
         self._log_lock = asyncio.Lock()
         self._log_values = {}
 
         assert self.model
```

### Comparing `sdss_lvmscp-0.4.0/python/lvmscp/actor/commands/__init__.py` & `sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.4.0/python/lvmscp/actor/commands/expose.py` & `sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.4.0/python/lvmscp/actor/commands/focus.py` & `sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/focus.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.4.0/python/lvmscp/actor/commands/hardware_status.py` & `sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/hardware_status.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.4.0/python/lvmscp/delegate.py` & `sdss_lvmscp-0.5.0/python/lvmscp/delegate.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 # @Date: 2021-05-29
 # @Filename: delegate.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import asyncio
-from typing import TYPE_CHECKING, List, Literal, Tuple
+from typing import TYPE_CHECKING, Any, List, Literal, Tuple
 
+import numpy
 from astropy.io import fits
 
 from archon.actor import ExposureDelegate
 from archon.controller.controller import ArchonController
 
 
 if TYPE_CHECKING:
@@ -130,14 +131,17 @@
             for ccd in self.actor.config["controllers"][controller.name]["detectors"]:
                 value = pressure_data.get(f"{ccd}_pressure", -999.0)
                 self.extra_data["pressure"][ccd] = value
 
         # Read depth probes
         self.extra_data["depth"] = await self.read_depth_probes()
 
+        # Get telescope information.
+        self.extra_data["telescope"] = await self.get_telescope_info()
+
         return
 
     async def post_process(
         self,
         controller: ArchonController,
         hdus: List[fits.PrimaryHDU],
     ) -> Tuple[ArchonController, List[fits.PrimaryHDU]]:
@@ -179,97 +183,96 @@
             depth_camera = self.extra_data["depth"].get("camera", "")
             for ch in ["A", "B", "C"]:
                 hdu.header[f"DEPTH{ch}"] = (
                     self.extra_data["depth"][ch] if ccd == depth_camera else -999.0,
                     f"Depth probe {ch} [mm]",
                 )
 
+            for key, value in self.extra_data.get("telescope", {}).items():
+                hdu.header[key.upper()] = value
+
+            if "TILE_ID" not in hdu.header:
+                hdu.header["TILE_ID"] = (-999, "The tile_id of this observation")
+
+            if "DPOS" not in hdu.header:
+                hdu.header["DPOS"] = (0, "The dither position of this observation")
+
         return (controller, hdus)
 
     async def get_shutter_status(self, spec: str) -> dict | Literal[False]:
         """Returns the status of the shutter for a spectrograph."""
 
-        spec_config = self.actor.config["controllers"][spec]
-        lvmieb_name = spec_config.get("lvmieb_actor", "lvmieb")
-
-        cmd = await self.command.send_command(lvmieb_name, f"shutter status {spec}")
+        lvmieb = self.actor.controllers[spec].lvmieb
+        cmd = await self.command.send_command(lvmieb, f"shutter status {spec}")
         await cmd
 
         if cmd.status.did_fail:
             return False
 
         try:
             return cmd.replies.get(f"{spec}_shutter")
         except KeyError:
             return False
 
     async def get_hartmann_status(self, spec: str) -> dict:
         """Returns the status of the hartmann doors."""
 
-        spec_config = self.actor.config["controllers"][spec]
-        lvmieb_name = spec_config.get("lvmieb_actor", "lvmieb")
-
-        cmd = await self.command.send_command(lvmieb_name, f"hartmann status {spec}")
+        lvmieb = self.actor.controllers[spec].lvmieb
+        cmd = await self.command.send_command(lvmieb, f"hartmann status {spec}")
         await cmd
 
         try:
             return {
                 f"{spec}_hartmann_left": cmd.replies.get(f"{spec}_hartmann_left"),
                 f"{spec}_hartmann_right": cmd.replies.get(f"{spec}_hartmann_right"),
             }
         except KeyError:
             self.command.warning(f"{spec}: failed retrieving hartmann door status.")
             return {}
 
     async def move_shutter(self, spec: str, action: str) -> bool:
         """Opens/closes a shutter."""
 
-        spec_config = self.actor.config["controllers"][spec]
-        lvmieb_name = spec_config.get("lvmieb_actor", "lvmieb")
-
-        cmd = await self.command.send_command(lvmieb_name, f"shutter {action} {spec}")
+        lvmieb = self.actor.controllers[spec].lvmieb
+        cmd = await self.command.send_command(lvmieb, f"shutter {action} {spec}")
         await cmd
 
         return cmd.status.did_succeed
 
     async def get_sensors(self, spec: str) -> dict:
         """Returns the spectrograph temepratues and RHs."""
 
-        spec_config = self.actor.config["controllers"][spec]
-        lvmieb_name = spec_config.get("lvmieb_actor", "lvmieb")
-
-        cmd = await self.command.send_command(lvmieb_name, f"wago status {spec}")
+        lvmieb = self.actor.controllers[spec].lvmieb
+        cmd = await self.command.send_command(lvmieb, f"wago status {spec}")
         await cmd
 
         try:
             return cmd.replies.get(f"{spec}_sensors")
         except KeyError:
             self.command.warning(f"{spec}: failed retrieving sensor values.")
             return {}
 
     async def get_pressure(self, spec: str) -> dict:
         """Returns the cryostat pressures."""
 
-        spec_config = self.actor.config["controllers"][spec]
-        lvmieb_name = spec_config.get("lvmieb_actor", "lvmieb")
-
-        cmd = await self.command.send_command(lvmieb_name, f"transducer status {spec}")
+        lvmieb = self.actor.controllers[spec].lvmieb
+        cmd = await self.command.send_command(lvmieb, f"transducer status {spec}")
         await cmd
 
         try:
             return cmd.replies.get("transducer")
         except KeyError:
             self.command.warning(f"{spec}: failed retrieving pressure status.")
             return {}
 
     async def read_depth_probes(self) -> dict:
         """Returns the depth probe measurements."""
 
         spec_config = list(self.actor.config["controllers"].values())[0]
-        lvmieb_name = spec_config.get("lvmieb_actor", "lvmieb")
+        lvmieb_name = spec_config.get("lvmieb", "lvmieb")
 
         cmd = await self.command.send_command(lvmieb_name, "depth status")
         await cmd
 
         try:
             return cmd.replies.get("depth")
         except KeyError:
@@ -277,26 +280,103 @@
             pass
 
         return {}
 
     async def get_lamps(self) -> dict:
         """Retrieves lamp information."""
 
-        cmd = await self.command.send_command("lvmnps", "status")
+        lvmnps = self.actor.config.get("lvmnps", "lvmnps")
+        cmd = await self.command.send_command(lvmnps, "status")
         await cmd
 
-        # Lamp mapping from outlet name in NPS to desired header name.
-        # TODO: eventually make these match.
-        lamp_mapping = self.actor.config.get("lamps", {})
+        # The config file includes the names of the lamps that should be present.
+        lamps = self.actor.config.get("lamps", [])
 
         lamp_status = {}
         try:
             status = cmd.replies.get("status")
             for switch in status:
                 for outlet in status[switch]:
-                    if outlet in lamp_mapping:
+                    if outlet in lamps:
                         state = "ON" if status[switch][outlet]["state"] == 1 else "OFF"
-                        lamp_status[lamp_mapping[outlet]] = state
+                        lamp_status[outlet] = state
         except Exception as err:
             self.command.warning(f"Failed retrieving lamp status: {err}")
 
+        # Make sure all lamps are in the dictionary, even if the NPS did not
+        # return some.
+        for lamp_name in lamps:
+            if lamp_name not in lamp_status:
+                lamp_status[lamp_name] = "?"
+
         return lamp_status
+
+    async def get_telescope_info(self) -> dict:
+        """Retrieve telescope information."""
+
+        data: dict[str, Any] = {"telescop": "SDSS 0.16m", "survey": "LVM"}
+
+        telescopes = ["sci", "skye", "skyw", "spec"]
+        keys = ["ra", "dec", "airm", "km", "foc"]
+
+        for telescope in telescopes:
+            pwi_status: dict = {}
+            km_position: float = -999
+            foc_position: float = -999
+
+            pwi_cmd = await self.command.send_command(
+                f"lvm.{telescope}.pwi",
+                "status",
+                internal=True,
+            )
+            if pwi_cmd.status.did_fail:
+                self.command.warning(f"Failed getting {telescope} PWI status.")
+            else:
+                pwi_status = pwi_cmd.replies[-1].body
+
+            if telescope != "spec":
+                km_cmd = await self.command.send_command(
+                    f"lvm.{telescope}.km",
+                    "status",
+                    internal=True,
+                )
+                if km_cmd.status.did_fail:
+                    self.command.warning(f"Failed getting {telescope} k-mirror status.")
+                else:
+                    km_position = km_cmd.replies.get("Position")
+
+            foc_cmd = await self.command.send_command(
+                f"lvm.{telescope}.foc",
+                "status",
+                internal=True,
+            )
+            if foc_cmd.status.did_fail:
+                self.command.warning(f"Failed getting {telescope} focus status.")
+            else:
+                foc_position = foc_cmd.replies.get("Position")
+
+            for key in keys:
+                if key == "km" and telescope == "spec":
+                    continue
+
+                if key == "km":
+                    data[f"{telescope}km"] = (km_position, "K-mirror position [deg]")
+                elif key == "foc":
+                    data[f"{telescope}foc"] = (foc_position, "Focuser position [deg]")
+                elif key == "ra":
+                    ra_h: float = pwi_status.get("ra_j2000_hours", -999.0)
+                    if ra_h > 0:
+                        ra_h *= 15.0
+                    data[f"{telescope}ra"] = (ra_h, "Telescope pointing RA [deg]")
+                elif key == "dec":
+                    dec = pwi_status.get("dec_j2000_degs", -999.0)
+                    data[f"{telescope}dec"] = (dec, "Telescope pointing Dec [deg]")
+                elif key == "airm":
+                    alt = pwi_status.get("altitude_degs", None)
+                    comment = "Telescope airmass"
+                    if alt is None:
+                        data[f"{telescope}airm"] = (-999.0, comment)
+                    else:
+                        airm = 1 / numpy.cos(numpy.radians(90 - alt))
+                        data[f"{telescope}airm"] = (airm, comment)
+
+        return data
```

### Comparing `sdss_lvmscp-0.4.0/python/lvmscp/etc/LVM_100kHz.acf` & `sdss_lvmscp-0.5.0/python/lvmscp/etc/LVM_100kHz.acf`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.4.0/python/lvmscp/etc/lvmscp.yml` & `sdss_lvmscp-0.5.0/python/lvmscp/etc/lvmscp.yml`

 * *Files 6% similar despite different names*

```diff
@@ -76,22 +76,20 @@
   readout_expected: 40
   readout_max: 60
   fetching_expected: 5
   fetching_max: 10
   flushing: 4.7
 
 lamps:
-  'Argon': 'Argon'
-  'Xenon': 'Xenon'
-  'Hg (Ar)': HgAr
-  'LDLS': 'LDLS'
-  'Krypton': 'Krypton'
-  'Neon': 'Neon'
-  'Hg (Ne)': 'HgNe'
-  'NIR LED': 'NIRLED'
+  - Argon
+  - Xenon
+  - LDLS
+  - Neon
+  - HgNe
+  - Quartz
 
 # Header for each CCD. The key is the header keyword name. The value can
 # be a single string, a tuple with the value and comment, or a dictionary for
 # cases in which the value is retrieved from an archon command or when the
 # value depends on the CCD name.
 header:
   CCDTEMP1:
@@ -150,14 +148,18 @@
 # controls whether the CCD frames from each controller are saved as individual files
 # or as different HDU extensions inside the FITS file.
 files:
   data_dir: '/data/spectro/lvm'
   split: true
   template: 'sdR-{hemisphere}-{ccd}-{exposure_no:08d}.fits.gz'
 
+checksum:
+  write: true
+  mode: md5
+
 credentials_file: ~/.config/sdss/lvmscp_credentials.yml
 
 exposure_list:
   id: 103BNxjlZ59Sob3jDO4EN1z6zp2q5YrYA6nTjGlZM6XY
   sheet:
     sp2: 'Spec 2'
     sp3: 'Spec 3'
```

### Comparing `sdss_lvmscp-0.4.0/PKG-INFO` & `sdss_lvmscp-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmscp
-Version: 0.4.0
+Version: 0.5.0
 Summary: LVM spectrograph control package.
 Home-page: https://github.com/sdss/lvmscp
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Maintainer: José Sánchez-Gallego
@@ -15,26 +15,20 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Authlib (>=1.0.0rc1)
-Requires-Dist: click (>=8.1.2,<9.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: httpx (>=0.18.1)
-Requires-Dist: sdss-archon (>=0.8.0,<0.9.0)
-Requires-Dist: sdss-clu (>=1.6.1,<2.0.0)
-Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
+Requires-Dist: sdss-archon (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://sdss-lvmscp.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/lvmscp
 Description-Content-Type: text/markdown
 
 # lvmscp
 
 ![Versions](https://img.shields.io/badge/python->3.8-blue)
```

