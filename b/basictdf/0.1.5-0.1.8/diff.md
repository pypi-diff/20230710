# Comparing `tmp/basictdf-0.1.5.tar.gz` & `tmp/basictdf-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basictdf-0.1.5.tar", max compression
+gzip compressed data, was "basictdf-0.1.8.tar", max compression
```

## Comparing `basictdf-0.1.5.tar` & `basictdf-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0      321 2023-07-03 21:05:53.181489 basictdf-0.1.5/README.md
--rw-r--r--   0        0        0      579 2023-07-03 21:05:53.185489 basictdf-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2956 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/__init__.py
--rw-r--r--   0        0        0    17639 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/basictdf.py
--rw-r--r--   0        0        0     3499 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfBlock.py
--rw-r--r--   0        0        0    12235 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfCalibrationData.py
--rw-r--r--   0        0        0    12413 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfData3D.py
--rw-r--r--   0        0        0     6907 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfEMG.py
--rw-r--r--   0        0        0     3938 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfEvents.py
--rw-r--r--   0        0        0    10735 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfForce3D.py
--rw-r--r--   0        0        0     7743 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfForcePlatformsCalibration.py
--rw-r--r--   0        0        0     5627 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfOpticalSystem.py
--rw-r--r--   0        0        0     6587 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfTypes.py
--rw-r--r--   0        0        0     1434 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfUtils.py
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 basictdf-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      321 2023-07-10 17:26:48.883559 basictdf-0.1.8/README.md
+-rw-r--r--   0        0        0      579 2023-07-10 17:26:48.887559 basictdf-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2956 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/__init__.py
+-rw-r--r--   0        0        0    17804 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/basictdf.py
+-rw-r--r--   0        0        0     3824 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfBlock.py
+-rw-r--r--   0        0        0    14252 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfCalibrationData.py
+-rw-r--r--   0        0        0     5663 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfData2D.py
+-rw-r--r--   0        0        0    12496 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfData3D.py
+-rw-r--r--   0        0        0     7160 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfEMG.py
+-rw-r--r--   0        0        0     4779 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfEvents.py
+-rw-r--r--   0        0        0    10800 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfForce3D.py
+-rw-r--r--   0        0        0     8432 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfForcePlatformsCalibration.py
+-rw-r--r--   0        0        0     7410 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfForcePlatformsData.py
+-rw-r--r--   0        0        0     5644 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfOpticalSystem.py
+-rw-r--r--   0        0        0     6652 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfTypes.py
+-rw-r--r--   0        0        0     1434 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfUtils.py
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 basictdf-0.1.8/PKG-INFO
```

### Comparing `basictdf-0.1.5/pyproject.toml` & `basictdf-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "basictdf"
-version = "0.1.5"
+version = "0.1.8"
 description = "A basic TDF parser"
 authors = ["Marcos A. Núñez <silver94@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 numpy = "^1.20"
```

### Comparing `basictdf-0.1.5/src/basictdf/__init__.py` & `basictdf-0.1.8/src/basictdf/__init__.py`

 * *Files identical despite different names*

### Comparing `basictdf-0.1.5/src/basictdf/basictdf.py` & `basictdf-0.1.8/src/basictdf/basictdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 from basictdf.tdfBlock import (
     AnalogData,
     AnthropometricData,
     Block,
     BlockType,
     CalibrationData2D,
-    Data2D,
     ForcePlatformsCalibrationData2D,
-    ForcePlatformsData,
     GeneralCalibrationData,
     NotDefinedBlock,
     UnusedBlock,
     VolumetricData,
 )
+from basictdf.tdfForcePlatformsData import ForcePlatformsDataBlock
 from basictdf.tdfCalibrationData import CalibrationDataBlock
+from basictdf.tdfData2D import Data2D
 from basictdf.tdfData3D import Data3D
 from basictdf.tdfEMG import EMG
 from basictdf.tdfEvents import TemporalEventsData
 from basictdf.tdfForce3D import ForceTorque3D
 from basictdf.tdfOpticalSystem import OpticalSetupBlock
 from basictdf.tdfTypes import BTSDate, BTSString, i32, u32
 from basictdf.tdfUtils import (
@@ -47,15 +47,15 @@
     elif block_type == BlockType.opticalSystemConfiguration:
         return OpticalSetupBlock
     elif block_type == BlockType.forcePlatformsCalibrationData:
         return ForcePlatformsCalibrationDataBlock
     elif block_type == BlockType.forcePlatformsCalibrationData2D:
         return ForcePlatformsCalibrationData2D
     elif block_type == BlockType.forcePlatformsData:
-        return ForcePlatformsData
+        return ForcePlatformsDataBlock
     elif block_type == BlockType.anthropometricData:
         return AnthropometricData
     elif block_type == BlockType.electromyographicData:
         return EMG
     elif block_type == BlockType.forceAndTorqueData:
         return ForceTorque3D
     elif block_type == BlockType.volumetricData:
@@ -125,18 +125,18 @@
             last_modification_date,
             last_access_date,
             comment,
         )
 
     def __repr__(self) -> str:
         return (
-            f"TdfEntry({self.type}, {self.format}, {self.offset},"
-            f" {self.size}, {self.creation_date},"
-            f" {self.last_modification_date},"
-            f" {self.last_access_date}, {self.comment})"
+            f"TdfEntry(type={self.type}, format={self.format}, offset={self.offset}, "
+            f"size={self.size}, creation_date={self.creation_date}, "
+            f"last_modification_date={self.last_modification_date}, "
+            f"last_access_date={self.last_access_date}, comment={self.comment})"
         )
 
 
 class Tdf:
     SIGNATURE = b"\x82K`A\xd3\x11\x84\xca`\x00\xb6\xac\x16h\x0c\x08"
 
     def __init__(self, filename: Union[Path, str]) -> None:
@@ -385,15 +385,15 @@
         - Inserting a new unused slot entry at the end
           (with the previous slot offset + size as offset)
         - If there is info after the block, move it
           block_to_remove.size up
 
         """
         if "+" not in self._mode:
-            raise ValueError(
+            raise PermissionError(
                 "Can't remove blocks, this file was opened in read-only mode"
             )
 
         # find block
         try:
             oldEntryPos, oldEntry = next(
                 (n, i) for n, i in enumerate(self.entries) if i.type == type
```

### Comparing `basictdf-0.1.5/src/basictdf/tdfBlock.py` & `basictdf-0.1.8/src/basictdf/tdfBlock.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         pass
 
     @abstractmethod
     def _write(self, file: IO[bytes]):
         pass
 
     def __repr__(self):
-        return self.__class__.__name__ + "(" + str(self.__class__.type) + ")"
+        return f"<{self.__class__.__name__} type={self.type}>"
 
 
 class NotImplementedBlock(Block):
     type = BlockType.notDefined
 
     @classmethod
     def _build(cls, *args, **kwargs):
@@ -115,13 +115,28 @@
     type = BlockType.analogData
 
 
 class GeneralCalibrationData(NotImplementedBlock):
     type = BlockType.generalCalibrationData
 
 
-class UnusedBlock(NotImplementedBlock):
+class UnusedBlock(Block):
     type = BlockType.unusedSlot
+    nBytes = 0
+    format = None
+
+    @staticmethod
+    def _build(*args, **kwargs) -> "UnusedBlock":
+        return UnusedBlock()
+
+    def _write(self, *args, **kwargs) -> None:
+        pass
+
+    def __repr__(self) -> str:
+        return "<UnusedBlock>"
+
+    def __eq__(self, other: "UnusedBlock") -> bool:
+        return isinstance(other, UnusedBlock)
 
 
 class NotDefinedBlock(NotImplementedBlock):
     type = BlockType.notDefined
```

### Comparing `basictdf-0.1.5/src/basictdf/tdfCalibrationData.py` & `basictdf-0.1.8/src/basictdf/tdfCalibrationData.py`

 * *Files 14% similar despite different names*

```diff
@@ -108,26 +108,41 @@
         VEC2D.bwrite(file, self.focus)
         VEC2D.bwrite(file, self.optical_center)
         VEC2D.bwrite(file, self.radial_distortion)
         VEC2D.bwrite(file, self.decentering)
         VEC2D.bwrite(file, self.thin_prism)
         self.view_port.bwrite(file)
 
+    @property
     def nBytes(self) -> int:
         return (
             MAT3X3D.btype.itemsize  # rotation_matrix
             + VEC3D.btype.itemsize  # translation_vector
             + VEC2D.btype.itemsize  # focus
             + VEC2D.btype.itemsize  # optical_center
             + VEC2D.btype.itemsize  # radial_distortion
             + VEC2D.btype.itemsize  # decentering
             + VEC2D.btype.itemsize  # thin_prism
             + CameraViewPort.nBytes  # view_port
         )
 
+    def __eq__(self, o: object) -> bool:
+        if not isinstance(o, SeelabCameraData):
+            return False
+        return (
+            np.array_equal(self.rotation_matrix, o.rotation_matrix)
+            and np.array_equal(self.translation_vector, o.translation_vector)
+            and np.array_equal(self.focus, o.focus)
+            and np.array_equal(self.optical_center, o.optical_center)
+            and np.array_equal(self.radial_distortion, o.radial_distortion)
+            and np.array_equal(self.decentering, o.decentering)
+            and np.array_equal(self.thin_prism, o.thin_prism)
+            and self.view_port == o.view_port
+        )
+
 
 class BTSCameraData:
     max_distorsion_coefficients = 70
 
     def __init__(
         self,
         rotation_matrix,
@@ -215,14 +230,15 @@
         VEC3D.bwrite(file, self.translation_vector)  # translation_vector
         VEC2D.bwrite(file, self.focus)  # focus
         VEC2D.bwrite(file, self.optical_center)  # optical_center
         f64.bwrite(file, self.x_distortion_coefficients)  # x_distortion_coefficients
         f64.bwrite(file, self.y_distortion_coefficients)  # y_distortion_coefficients
         self.view_port.bwrite(file)  # view_port
 
+    @property
     def nBytes(self) -> int:
         return (
             MAT3X3D.btype.itemsize  # rotation_matrix
             + VEC3D.btype.itemsize  # translation_vector
             + VEC2D.btype.itemsize  # focus
             + VEC2D.btype.itemsize  # optical_center
             + f64.btype.itemsize
@@ -256,14 +272,15 @@
         self,
         distorsion_model: DistorsionModel,
         calibration_volume_size: np.ndarray,
         calibration_volume_rotation_matrix: np.ndarray,
         calibration_volume_translation_vector: np.ndarray,
         cameras_calibration_map: np.ndarray,
         cam_data: Union[List[BTSCameraData], List[SeelabCameraData]],
+        format: CalibrationDataBlockFormat = CalibrationDataBlockFormat.Seelab1,
     ) -> None:
         super().__init__()
 
         self.distorsion_model = distorsion_model
         "Distorsion model of the calibration"
 
         if calibration_volume_size.shape != VEC3F.btype.shape:
@@ -305,19 +322,22 @@
             not isinstance(cameras_calibration_map, np.ndarray)
             or len(cameras_calibration_map.shape) != 1
         ):
             raise ValueError("Cameras_calibration_map must be a single row numpy array")
         self.cameras_calibration_map = cameras_calibration_map
 
         self.cam_data = cam_data
+        self.format = format
 
     @staticmethod
     def _build(stream, format) -> "CalibrationDataBlock":
+        format = CalibrationDataBlockFormat(format)
+
         nCams = i32.bread(stream)
-        distosion_model = DistorsionModel(i32.bread(stream))
+        distorsion_model = DistorsionModel(i32.bread(stream))
         calibration_volume = VEC3F.bread(stream)
         rotation_matrix = MAT3X3F.bread(stream)
         translation_vector = VEC3F.bread(stream)
         calibration_map = i16.bread(stream, nCams)
 
         calibration_data = []
 
@@ -325,20 +345,21 @@
             calibration_data = [SeelabCameraData._build(stream) for _ in range(nCams)]
         elif format == CalibrationDataBlockFormat.BTS:
             calibration_data = [BTSCameraData._build(stream) for _ in range(nCams)]
         else:
             raise ValueError(f'"Unknown calibration format "{format}"')
 
         return CalibrationDataBlock(
-            distorsion_model=distosion_model,
+            distorsion_model=distorsion_model,
             calibration_volume_size=calibration_volume,
             calibration_volume_rotation_matrix=rotation_matrix,
             calibration_volume_translation_vector=translation_vector,
             cameras_calibration_map=calibration_map,
             cam_data=calibration_data,
+            format=format,
         )
 
     def _write(self, file) -> None:
         # nCams
         nCams = len(self.cam_data)
         i32.bwrite(file, nCams)
 
@@ -357,17 +378,47 @@
         # calibration map
         i16.bwrite(file, self.cameras_calibration_map)
 
         # calibration data
         for cam in self.cam_data:
             cam._write(file)
 
+    @property
     def nBytes(self) -> int:
         return (
             i32.btype.itemsize  # nCams
             + i32.btype.itemsize  # DistorsionModel
             + VEC3F.btype.itemsize  # calibration_volume
             + MAT3X3F.btype.itemsize  # rotation matrix
             + VEC3F.btype.itemsize  # translation_vector
             + i16.btype.itemsize * len(self.cam_data)  # calibration map
             + sum(cam.nBytes for cam in self.cam_data)  # calibration data
         )
+
+    def __eq__(self, o: object) -> bool:
+        if not isinstance(o, CalibrationDataBlock):
+            return False
+
+        return (
+            self.distorsion_model == o.distorsion_model
+            and np.array_equal(self.calibration_volume_size, o.calibration_volume_size)
+            and np.array_equal(
+                self.calibration_volume_rotation_matrix,
+                o.calibration_volume_rotation_matrix,
+            )
+            and np.array_equal(
+                self.calibration_volume_translation_vector,
+                o.calibration_volume_translation_vector,
+            )
+            and np.array_equal(self.cameras_calibration_map, o.cameras_calibration_map)
+            and all(i == j for i, j in zip(self.cam_data, o.cam_data))
+            and self.format == o.format
+        )
+
+    def __repr__(self) -> str:
+        return (
+            "<CalibrationDataBlock "
+            f"format={self.format.name} "
+            f"nCams={len(self.cam_data)} "
+            f"distorsion_model={self.distorsion_model.name} "
+            f"calibration_volume_size={self.calibration_volume_size} >"
+        )
```

### Comparing `basictdf-0.1.5/src/basictdf/tdfData3D.py` & `basictdf-0.1.8/src/basictdf/tdfData3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     VEC3F,
     BTSString,
     TdfType,
     Volume,
     f32,
     i32,
     u32,
+    SegmentData,
 )
 
 
 class Data3dBlockFormat(Enum):
     """
     Available formats for a Data3D block.
     """
@@ -38,15 +39,14 @@
     """
 
     rawData = 0
     filtered = 1
 
 
 LinkType = TdfType(np.dtype([("Track1", "<u4"), ("Track2", "<u4")]))
-SegmentData = TdfType(np.dtype([("startFrame", "<i4"), ("nFrames", "<i4")]))
 
 TrackType = TdfType(np.dtype("<3f4"))
 
 
 class MarkerTrack:
     """
     A track that collects all the data of a physical marker, such as name and position.
@@ -423,10 +423,15 @@
         for track in self._tracks:
             base += track.nBytes
 
         return base
 
     def __repr__(self) -> str:
         return (
-            f"<Data3D: {self.nFrames} frames, {self.frequency} Hz,"
-            f" {self.nTracks} tracks, tracks={[i.label for i in self._tracks]}>"
+            f"<Data3D "
+            f"format={self.format.name}, "
+            f"nFrames={self.nFrames}, "
+            f"frequency={self.frequency}, "
+            f"startTime={self.startTime}, "
+            f"nTracks={self.nTracks}, "
+            f"tracks={[i.label for i in self._tracks]}>"
         )
```

### Comparing `basictdf-0.1.5/src/basictdf/tdfEMG.py` & `basictdf-0.1.8/src/basictdf/tdfEMG.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 __doc__ = "Electromyography data module."
 
 from enum import Enum
-from io import BytesIO
 from typing import Iterator, Union
 
 import numpy as np
 
 from basictdf.tdfBlock import Block, BlockType
 from basictdf.tdfTypes import BTSString, TdfType, f32, i16, i32
 
@@ -88,32 +87,35 @@
 
 
 class EMG(Block):
     """Electromyography data block"""
 
     type = BlockType.electromyographicData
 
-    def __init__(self, frequency, nSamples, startTime=0.0) -> None:
+    def __init__(
+        self, frequency, nSamples, startTime=0.0, format=EMGBlockFormat.byTrack
+    ) -> None:
         super().__init__()
         self.frequency = frequency
         self.startTime = startTime
         self.nSamples = nSamples
         self._signals = []
         self._emgMap = []
+        self.format = format
 
     @staticmethod
     def _build(stream, format) -> "EMG":
         format = EMGBlockFormat(format)
         nSignals = i32.bread(stream)
         frequency = i32.bread(stream)
         startTime = f32.bread(stream)
         nSamples = i32.bread(stream) + 49  # Why 49??? Whyyyy????
         emgMap = i16.bread(stream, n=nSignals)
 
-        d = EMG(frequency, nSamples, startTime)
+        d = EMG(frequency, nSamples, startTime, format)
         if format == EMGBlockFormat.byTrack:
             for n in range(nSignals):
                 emgSignal = EMGTrack.build(stream, nSamples)
                 d.addSignal(emgSignal, channel=emgMap[n])
         else:
             raise NotImplementedError(f"EMG format {format} not implemented yet")
         return d
@@ -127,20 +129,20 @@
 
         # frequency
         i32.bwrite(file, self.frequency)
 
         # startTime
         f32.bwrite(file, self.startTime)
 
-        # emgMap
-        i16.bwrite(file, self._emgMap)
-
         # nSamples
         i32.bwrite(file, self.nSamples - 49)  # That 49 again
 
+        # emgMap
+        i16.bwrite(file, self._emgMap)
+
         # signals
         for signal in self._signals:
             signal.write(file)
 
     def __getitem__(self, key) -> EMGTrack:
         if isinstance(key, int):
             return self._signals[key]
@@ -161,19 +163,20 @@
     def __iter__(self) -> Iterator[EMGTrack]:
         return iter(self._signals)
 
     def __len__(self) -> int:
         return len(self._signals)
 
     def __eq__(self, other) -> bool:
-        buff1 = BytesIO()
-        buff2 = BytesIO()
-        self.write(buff1)
-        other.write(buff2)
-        return buff1.getvalue() == buff2.getvalue()
+        return (
+            self.frequency == other.frequency
+            and self.startTime == other.startTime
+            and self.nSamples == other.nSamples
+            and all(s1 == s2 for s1, s2 in zip(self._signals, other._signals))
+        )
 
     def addSignal(self, signal: EMGTrack, channel=None) -> None:
         """
         adds a signal to the EMG block. If the channel is not specified,
         it is set to the next one  available
         """
         if not isinstance(signal, EMGTrack):
@@ -216,10 +219,15 @@
 
     @property
     def nSignals(self) -> int:
         return len(self._signals)
 
     def __repr__(self) -> str:
         return (
-            f"EMGBlock(frequency={self.frequency}, nSamples={self.nSamples}, "
-            f"nSignals={self.nSignals}, startTime={self.startTime},)"
+            "<EMGBlock"
+            f" format={self.format.name}"
+            f" frequency={self.frequency}"
+            f" nSamples={self.nSamples}"
+            f" nSignals={self.nSignals}"
+            f" startTime={self.startTime}"
+            ">"
         )
```

### Comparing `basictdf-0.1.5/src/basictdf/tdfEvents.py` & `basictdf-0.1.8/src/basictdf/tdfEvents.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,20 +51,35 @@
         nItems = i32.bread(stream)
         values = np.array([f32.bread(stream) for _ in range(nItems)])
         return Event(label, values, type_)
 
     def __len__(self) -> int:
         return len(self.values)
 
+    def __eq__(self, o: object) -> bool:
+        if not isinstance(o, Event):
+            return False
+        return (
+            self.label == o.label
+            and self.type == o.type
+            and np.array_equal(self.values, o.values)
+        )
+
     @property
     def nBytes(self) -> int:
         return 256 + 4 + 4 + len(self.values) * 4
 
     def __repr__(self) -> str:
-        return f"Event(label={self.label}, type={self.type}, items={self.values})"
+        return (
+            "<Event "
+            f"label={self.label} "
+            f"type={self.type} "
+            f"nItems={len(self.values)} "
+            f"values={self.values}>"
+        )
 
 
 class TemporalEventsData(Block):
     """
     A class to represent a TDF temporal events data block.
     """
 
@@ -116,12 +131,27 @@
     def __contains__(self, value: Union[Event, str]) -> bool:
         if isinstance(value, Event):
             return value in self.events
         elif isinstance(value, str):
             return any(value == event.label for event in self.events)
         raise TypeError(f"Invalid key type: {type(value)}")
 
+    def __eq__(self, other) -> bool:
+        if not isinstance(other, TemporalEventsData):
+            raise TypeError(
+                "Can only compare TemporalEventsData with TemporalEventsData"
+            )
+        return (
+            self.format == other.format
+            and self.start_time == other.start_time
+            and all(e1 == e2 for e1, e2 in zip(self.events, other.events))
+        )
+
     def __repr__(self) -> str:
         return (
-            f"TemporalEventsData(format={self.format}, nEvents={len(self.events)}, "
-            f"start_time={self.start_time}, events={self.events}) size={self.nBytes}"
+            "<TemporalEventsData "
+            f"format={self.format.name} "
+            f"nEvents={len(self.events)} "
+            f"start_time={self.start_time} "
+            f"events={self.events} "
+            f"size={self.nBytes}>"
         )
```

### Comparing `basictdf-0.1.5/src/basictdf/tdfForce3D.py` & `basictdf-0.1.8/src/basictdf/tdfForce3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     VEC3F,
     BTSString,
     TdfType,
     Volume,
     f32,
     i32,
     u32,
+    SegmentData,
 )
 
-SegmentData = TdfType(np.dtype([("startFrame", "<i4"), ("nFrames", "<i4")]))
 ForceType = ApplicationPointType = TorqueType = TdfType(np.dtype("<3f4"))
 
 
 class ForceTorqueTrack:
     def __init__(
         self,
         label: str,
@@ -222,14 +222,42 @@
         )
         if format != ForceTorque3DBlockFormat.byTrack:
             raise NotImplementedError(f"Force3D format {format} not implemented yet")
 
         f._tracks = [ForceTorqueTrack._build(stream, nFrames) for _ in range(nTracks)]
         return f
 
+    def _write(self, file) -> None:
+        if self.format != ForceTorque3DBlockFormat.byTrack:
+            raise NotImplementedError(
+                f"Force3D format {self.format} not implemented yet"
+            )
+
+        # nTracks
+        u32.bwrite(file, len(self._tracks))
+        # frequency
+        i32.bwrite(file, self.frequency)
+        # startTime
+        f32.bwrite(file, self.startTime)
+        # nFrames
+        i32.bwrite(file, self.nFrames)
+
+        # volume
+        Volume.bwrite(file, self.volume)
+        # rotationMatrix
+        MAT3X3F.bwrite(file, self.rotationMatrix)
+        # translationVector
+        VEC3F.bwrite(file, self.translationVector)
+
+        # padding
+        i32.bpad(file)
+
+        for track in self._tracks:
+            track._write(file)
+
     def add_track(self, track: ForceTorqueTrack) -> None:
         """Adds a track to the data block
 
         Args:
             track (MarkerTrack): track to add
 
         Raises:
@@ -316,40 +344,16 @@
             + VEC3F.btype.itemsize
             + 4
         )
         for track in self._tracks:
             base += track.nBytes
         return base
 
-    def _write(self, file) -> None:
-        if self.format != ForceTorque3DBlockFormat.byTrack:
-            raise NotImplementedError(
-                f"Force3D format {self.format} not implemented yet"
-            )
-        # nFrames
-        i32.bwrite(file, self.nFrames)
-
-        # frequency
-        i32.bwrite(file, self.frequency)
-        # startTime
-        f32.bwrite(file, self.startTime)
-        # nTracks
-        u32.bwrite(file, len(self._tracks))
-
-        # volume
-        Volume.bwrite(file, self.volume)
-        # rotationMatrix
-        MAT3X3F.bwrite(file, self.rotationMatrix)
-        # translationVector
-        VEC3F.bwrite(file, self.translationVector)
-
-        # padding
-        i32.bpad(file)
-
-        for track in self._tracks:
-            track._write(file)
-
     def __repr__(self) -> str:
         return (
-            f"<ForceTorque3D: {self.nFrames} frames, {self.frequency} Hz, "
-            f"{self.nTracks} tracks, tracks={[i.label for i in self._tracks]}>"
+            f"<ForceTorque3D format={self.format.name} "
+            f"nFrames={self.nFrames} "
+            f"frequency={self.frequency} Hz "
+            f"startTime={self.startTime} "
+            f"nTracks={self.nTracks} "
+            f"tracks={[i.label for i in self._tracks]}>"
         )
```

### Comparing `basictdf-0.1.5/src/basictdf/tdfForcePlatformsCalibration.py` & `basictdf-0.1.8/src/basictdf/tdfForcePlatformsCalibration.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,88 +16,95 @@
 
 class ForcePlatformCalibrationBlockFormat(Enum):
     unknownFormat = 0
     ISSFormat = 1  # TDF_CALPLAT_FORMAT_ISS
     GRPFormat = 2  # TDF_CALPLAT_FORMAT_GRP? (not documented)
 
 
-class ForcePlatform:
+class ForcePlatformInfo:
     """
     Class that stores the calibration data of a force platform.
     """
 
     def __init__(self, label, size, position) -> None:
         self.label = label
         "Force platform label"
         self.size = size
         "Size in meters (width, length)"
         self.position = position
         "Position of the 4 vertices in x,y,z coordinates"
 
     @staticmethod
-    def _build(stream) -> "ForcePlatform":
+    def _build(stream) -> "ForcePlatformInfo":
         label = BTSString.bread(stream, 256)  # Docs say 32, but it's actually 256
         size = VEC2F.bread(stream)
         position = ForcePlatformVertices.bread(stream)
         BTSString.bread(stream, 256)  # Undocumented padding
 
-        return ForcePlatform(label, size, position)
+        return ForcePlatformInfo(label, size, position)
 
     def _write(self, stream) -> None:
         BTSString.bwrite(stream, 256, self.label)
         VEC2F.bwrite(stream, self.size)
         ForcePlatformVertices.bwrite(stream, self.position)
         BTSString.bwrite(stream, 256, "")  # Undocumented padding
 
     nBytes = 256 + (4 * 2) + (4 * 3 * 4) + 256
 
     def __eq__(self, o: object) -> bool:
-        if not isinstance(o, ForcePlatform):
+        if not isinstance(o, ForcePlatformInfo):
             return False
         return (
             self.label == o.label
             and np.allclose(self.size, o.size)
             and np.allclose(self.position, o.position)
         )
 
     def __repr__(self) -> str:
+        # return (
+        #     f"ForcePlatform(label={self.label}, size={self.size},"
+        #     " position={self.position})"
+        # )
         return (
-            f"ForcePlatform(label={self.label}, size={self.size},"
-            " position={self.position})"
+            "<ForcePlatformInfo "
+            f"label={self.label}, size={self.size}, position={self.position}>"
         )
 
 
 class ForcePlatformsCalibrationDataBlock(Block):
     """
     Block that stores the calibration data of a list of force platforms.
     Each platform is stored as a ForcePlatform object, along with a channel
     number. The channel number links the logical channel of the platform to the
     physical channel of the data acquisition system.
     """
 
     type = BlockType.forcePlatformsCalibrationData
 
-    def __init__(self, platforms=None) -> None:
-        self._platforms: List[ForcePlatform] = platforms or []
+    def __init__(
+        self, platforms=None, format=ForcePlatformCalibrationBlockFormat.GRPFormat
+    ) -> None:
+        self._platforms: List[ForcePlatformInfo] = platforms or []
         self._platformMap = []
+        self.format = format
 
     @staticmethod
     def _build(stream, format) -> "ForcePlatformsCalibrationDataBlock":
         format = ForcePlatformCalibrationBlockFormat(format)
         if format != ForcePlatformCalibrationBlockFormat.GRPFormat:
             raise NotImplementedError(
                 f"Platform calibration format {format} not implemented yet"
             )
         nPlats = i32.bread(stream)
         i32.skip(stream)  # padding
         platMap = i16.bread(stream, n=nPlats)
-        block = ForcePlatformsCalibrationDataBlock()
+        block = ForcePlatformsCalibrationDataBlock(format=format)
         for nPlat in range(nPlats):
-            platform = ForcePlatform._build(stream)
-            block.addPlatform(platform, channel=platMap[nPlat])
+            platform = ForcePlatformInfo._build(stream)
+            block.add_platform(platform, channel=platMap[nPlat])
 
         return block
 
     def _write(
         self, file, format=ForcePlatformCalibrationBlockFormat.GRPFormat
     ) -> None:
         if format != ForcePlatformCalibrationBlockFormat.GRPFormat:
@@ -114,117 +121,131 @@
         # platMap
         i16.bwrite(file, self._platformMap)
 
         # platforms
         for platform in self._platforms:
             platform._write(file)
 
-    def addPlatform(self, platform: ForcePlatform, channel: int = None):
+    def add_platform(self, platform: ForcePlatformInfo, channel: int = None):
         """
         Adds a platform to the list of platforms. Optionally, a channel can be
         specified. If no channel is specified, the next available channel is
         used.
         """
-        if not isinstance(platform, ForcePlatform):
+        if not isinstance(platform, ForcePlatformInfo):
             raise TypeError("platform must be of type ForcePlatform")
 
         if channel is None:
             if len(self._platformMap) == 0:
                 next_channel = 0
             else:
                 next_channel = max(self._platformMap) + 1
             self._platformMap.append(next_channel)
         else:
             if channel in self._platformMap:
                 raise ValueError(f"channel {channel} already in use")
             self._platformMap.append(channel)
         self._platforms.append(platform)
 
-    def removePlatform(self, plat):
+    def remove_platform(self, plat):
         """
         Removes a platform from the list of platforms. The platform can be
         specified either by index or by ForcePlatform object.
         """
-        if isinstance(plat, ForcePlatform):
+        if isinstance(plat, ForcePlatformInfo):
             if plat in self._platforms:
                 index = self._platforms.index(plat)
             else:
                 raise ValueError(f"platform {plat} not in list")
         elif isinstance(plat, int):
             if plat >= len(self._platforms):
                 raise ValueError(f"index {plat} out of range")
             else:
                 index = plat
 
         del self._platforms[index]
         del self._platformMap[index]
 
-    def removePlatforms(self, plats):
+    def remove_platforms(self, plats):
         """
         Removes a list of platforms from the list of platforms. The platforms
         can be specified either by index or by ForcePlatform object.
         """
         for plat in plats:
-            self.removePlatform(plat)
+            self.remove_platform(plat)
 
-    def addPlatforms(self, plats, channels=None):
+    def add_platforms(self, plats, channels=None):
         """
         Adds a list of platforms to the list of platforms. If a list of
         channels is provided, the platforms will be added to the corresponding
         channels. If no list of channels is provided, the platforms will be
         added to the next available channels.
 
         """
         if channels:
             for plat, channel in zip(plats, channels):
-                self.addPlatform(plat, channel)
+                self.add_platform(plat, channel)
         else:
             for plat in plats:
-                self.addPlatform(plat)
+                self.add_platform(plat)
 
     @property
-    def platforms(self) -> List[Tuple[int, ForcePlatform]]:
+    def platforms(self) -> List[Tuple[int, ForcePlatformInfo]]:
         """
         Returns:
             List[Tuple(int, ForcePlatform)]: a list of tuples containing the
             channel and the platform
 
         Settable:
             Iterable[Sequence[Union[int, ForcePlatform]]]: a list of tuples
             containing the channel and the platform
         """
         return list(zip(self._platformMap, self._platforms))
 
     @platforms.setter
-    def platforms(self, channel_plats: Iterable[Sequence[Union[int, ForcePlatform]]]):
+    def platforms(
+        self, channel_plats: Iterable[Sequence[Union[int, ForcePlatformInfo]]]
+    ):
         """
         Replaces the current list of platforms with the one provided. The
         input is a list of tuples containing the channel and the platform.
         """
         self._platformMap = []
         self._platforms = []
         for channel, plat in channel_plats:
-            self.addPlatform(plat, channel)
+            self.add_platform(plat, channel)
 
     @property
     def nBytes(self) -> int:
         return (
             4  # nPlats
             + 4  # padding
             + 2 * len(self._platformMap)
             + sum(platform.nBytes for platform in self._platforms)
         )
 
     def __getitem__(self, key):
         return self._platforms[key]
 
-    def __iter__(self) -> Iterator[ForcePlatform]:
+    def __iter__(self) -> Iterator[ForcePlatformInfo]:
         return iter(self.platforms)
 
-    def __contains__(self, item: ForcePlatform) -> bool:
+    def __contains__(self, item: ForcePlatformInfo) -> bool:
         return item in self._platforms
 
     def __len__(self) -> int:
         return len(self._platforms)
 
+    def __eq__(self, o: object) -> bool:
+        if not isinstance(o, ForcePlatformsCalibrationDataBlock):
+            return False
+        return (
+            self.format == o.format
+            and self._platformMap == o._platformMap
+            and self._platforms == o._platforms
+        )
+
     def __repr__(self) -> str:
-        return f"ForcePlatformsCalibrationDataBlock(platforms={self.platforms})"
+        return (
+            f"<ForcePlatformsCalibrationDataBlock "
+            f"format={self.format.name}, nPlats={len(self)}>"
+        )
```

### Comparing `basictdf-0.1.5/src/basictdf/tdfOpticalSystem.py` & `basictdf-0.1.8/src/basictdf/tdfOpticalSystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,8 +186,8 @@
 
         for channel in self.channels:
             base += channel.nBytes
 
         return base
 
     def __repr__(self) -> str:
-        return f"<OpticalSetupBlock: {len(self.channels)} channels>"
+        return f"<OpticalSetupBlock format={self.format.name} nChannels={len(self)}>"
```

### Comparing `basictdf-0.1.5/src/basictdf/tdfTypes.py` & `basictdf-0.1.8/src/basictdf/tdfTypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,14 +153,15 @@
 
 MAT3X3F = TdfType(np.dtype("(3,3)<f4"))
 MAT3X3D = TdfType(np.dtype("(3,3)<f8"))
 
 i32 = TdfType(np.dtype("<i4"))
 i16 = TdfType(np.dtype("<i2"))
 u32 = TdfType(np.dtype("<u4"))
+u16 = TdfType(np.dtype("<u2"))
 f32 = TdfType(np.dtype("<f4"))
 f64 = TdfType(np.dtype("<f8"))
 
 
 class CameraViewPort:
     def __init__(self, origin, size) -> None:
         if isinstance(origin, np.ndarray) and origin.shape != VEC2I.btype.shape:
@@ -195,18 +196,19 @@
     def write(self) -> bytes:
         return VEC2I.write(self.origin) + VEC2I.write(self.size)
 
     def bwrite(self, stream: BinaryIO) -> None:
         VEC2I.bwrite(stream, self.origin)
         VEC2I.bwrite(stream, self.size)
 
-    @property
-    def nBytes(self) -> int:
-        return 8 + 8
+    nBytes = 8 + 8
 
     def __repr__(self) -> str:
         return f"CameraViewPort(origin={self.origin}, size={self.size})"
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, CameraViewPort):
             raise TypeError("Can only compare CameraViewPort with CameraViewPort")
         return np.all(self.origin == other.origin) and np.all(self.size == other.size)
+
+
+SegmentData = TdfType(np.dtype([("startFrame", "<i4"), ("nFrames", "<i4")]))
```

### Comparing `basictdf-0.1.5/src/basictdf/tdfUtils.py` & `basictdf-0.1.8/src/basictdf/tdfUtils.py`

 * *Files identical despite different names*

### Comparing `basictdf-0.1.5/PKG-INFO` & `basictdf-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basictdf
-Version: 0.1.5
+Version: 0.1.8
 Summary: A basic TDF parser
 Author: Marcos A. Núñez
 Author-email: silver94@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

