# Comparing `tmp/sphractal-0.8.1.tar.gz` & `tmp/sphractal-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphractal-0.8.1.tar", max compression
+gzip compressed data, was "sphractal-0.9.0.tar", max compression
```

## Comparing `sphractal-0.8.1.tar` & `sphractal-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1082 2023-07-08 10:21:27.636502 sphractal-0.8.1/LICENSE
--rw-r--r--   0        0        0     4017 2023-07-08 10:21:27.636502 sphractal-0.8.1/README.md
--rw-r--r--   0        0        0     2056 2023-07-08 10:22:11.617038 sphractal-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      736 2023-07-08 10:22:11.617038 sphractal-0.8.1/setup.py
--rw-r--r--   0        0        0     1429 2023-07-08 10:21:27.692502 sphractal-0.8.1/src/sphractal/__init__.py
--rw-r--r--   0        0        0    23050 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/boxCnt.py
--rw-r--r--   0        0        0     4382 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/constants.py
--rw-r--r--   0        0        0        0 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/data/__init__.py
--rw-r--r--   0        0        0    20105 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/data/example.xyz
--rw-r--r--   0        0        0      264 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/datasets.py
--rw-r--r--   0        0        0     8750 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/surfExact.py
--rw-r--r--   0        0        0     8121 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/surfPointClouds.py
--rw-r--r--   0        0        0    11515 2023-07-08 10:21:27.696502 sphractal-0.8.1/src/sphractal/utils.py
--rw-r--r--   0        0        0    94032 2023-07-08 10:21:27.696502 sphractal-0.8.1/tests/fixtures.py
--rw-r--r--   0        0        0    17618 2023-07-08 10:21:27.696502 sphractal-0.8.1/tests/test_sphractal.py
--rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 sphractal-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-10 06:35:37.325830 sphractal-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4017 2023-07-10 06:35:37.325830 sphractal-0.9.0/README.md
+-rw-r--r--   0        0        0     2056 2023-07-10 06:36:20.890169 sphractal-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      736 2023-07-10 06:36:20.890169 sphractal-0.9.0/setup.py
+-rw-r--r--   0        0        0     1429 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/__init__.py
+-rw-r--r--   0        0        0    23389 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/boxCnt.py
+-rw-r--r--   0        0        0     4382 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/constants.py
+-rw-r--r--   0        0        0        0 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/data/__init__.py
+-rw-r--r--   0        0        0    20105 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/data/example.xyz
+-rw-r--r--   0        0        0      264 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/datasets.py
+-rw-r--r--   0        0        0     8929 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/surfExact.py
+-rw-r--r--   0        0        0     8121 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/surfPointClouds.py
+-rw-r--r--   0        0        0    11511 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/utils.py
+-rw-r--r--   0        0        0    94032 2023-07-10 06:35:37.385831 sphractal-0.9.0/tests/fixtures.py
+-rw-r--r--   0        0        0    17618 2023-07-10 06:35:37.385831 sphractal-0.9.0/tests/test_sphractal.py
+-rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 sphractal-0.9.0/PKG-INFO
```

### Comparing `sphractal-0.8.1/LICENSE` & `sphractal-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.1/README.md` & `sphractal-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.1/pyproject.toml` & `sphractal-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphractal"
-version = "0.8.1"
+version = "0.9.0"
 description = "Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/sphractal"
 repository = "https://github.com/Jon-Ting/sphractal"
 documentation = "https://sphractal.readthedocs.io/en/latest/"
```

### Comparing `sphractal-0.8.1/setup.py` & `sphractal-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '0.8.1'
+__version__ = '0.9.0'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sphractal",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `sphractal-0.8.1/src/sphractal/__init__.py` & `sphractal-0.9.0/src/sphractal/__init__.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.1/src/sphractal/boxCnt.py` & `sphractal-0.9.0/src/sphractal/boxCnt.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import matplotlib.pyplot as plt
 from matplotlib.ticker import FormatStrFormatter
 import numpy as np
 from statsmodels.api import OLS, add_constant
 
 from sphractal.constants import PLT_PARAMS
 from sphractal.surfPointClouds import genSurfPoints
-from sphractal.surfExact import findTargetAtoms, MIN_VAL_FROM_BOUND, scanAllAtoms, writeBoxCoords
+from sphractal.surfExact import findTargetAtoms, scanAllAtoms, writeBoxCoords
 from sphractal.utils import findNN, findSurf, readXYZ
 # from sphractal.utils import estDuration, annotate
 
 
 # @annotate('getVoxelBoxCnts', color='blue')
 def getVoxelBoxCnts(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
                     npName, writeFileDir='boxCntOutputs', exePath='$FASTBC_EXE',
@@ -104,15 +104,16 @@
             scales.append(log10(1 / int(line.split()[0])))
             counts.append(log10(int(line.split()[1])))
     return scales[::-1], counts[::-1]
 
 
 # @annotate('getSphereBoxCnts', color='blue')
 def getSphereBoxCnts(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
-                     maxRange, minMaxBoxLens, minXYZ, npName, writeFileDir='boxCntOutputs', numBoxLenSample=10,
+                     maxRange, minMaxBoxLens, minXYZ, npName, 
+                     writeFileDir='boxCntOutputs', numBoxLenSample=10, minValFromBound=5.0,
                      rmInSurf=True, writeBox=True, verbose=False):
     """
     Count the boxes that cover the outer surface of a set of overlapping spheres represented as exact spheres for
     different box sizes.
     
     Parameters
     ----------
@@ -134,14 +135,16 @@
         Minimum values of each dimension in the Cartesian space.
     npName : str
         Identifier of the measured object, which forms part of the output file name, ideally unique.
     writeFileDir : str, optional
         Path to the directory to store the output files.
     numBoxLenSample : int, optional
         Number of box lengths to use for the collection of the box count data, spaced evenly on logarithmic scale.
+    minValFromBound : Union[int,float]
+        Buffer distance from the borders of the largest box in Angstrom.
     rmInSurf : bool, optional
         Whether to remove the surface points on the inner surface.
     writeBox : bool, optional
         Whether to generate output files for visualisation.
     verbose : bool, optional
         Whether to display the details.
     
@@ -170,23 +173,23 @@
         print(f"    Parallelised with {atomScanMaxWorkers} out of {numCPUs} cores for scanning over {len(atomsIdxs)} "
               f"atoms, the rest over {numBoxLenSample} box lengths...")
         print(f"    (1/eps)    (# bulk)    (# surf)")
     if writeBox:
         if not isdir(writeFileDir):
             mkdir(writeFileDir)
 
-    overallBoxLen = maxRange + MIN_VAL_FROM_BOUND * 2
+    overallBoxLen = maxRange + minValFromBound * 2
     allLensSurfBoxs, allLensBulkBoxs, allLensSurfCnts, allLensBulkCnts = [], [], [], []
     scales, scanBoxLens, scanAllAtomsInps = [], [], []
     approxScanBoxLens = np.geomspace(minMaxBoxLens[1], minMaxBoxLens[0], num=numBoxLenSample)
     for approxScanBoxLen in approxScanBoxLens:  # Evenly reduced box lengths on log scale
         magnFac = int(overallBoxLen / approxScanBoxLen)
         scanBoxLen = overallBoxLen / magnFac
         scanAllAtomsInp = (magnFac, scanBoxLen, atomsIdxs, minXYZ,
-                           atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, 
+                           atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, minValFromBound,
                            rmInSurf, verbose, atomScanMaxWorkers)
         if boxLenConc:
             scanAllAtomsInps.append(scanAllAtomsInp) 
         else:
             scanAllAtomsResult = scanAllAtoms(scanAllAtomsInp) 
             allAtomsSurfBoxs, allAtomsBulkBoxs = scanAllAtomsResult
             allLensSurfBoxs.append(allAtomsSurfBoxs)
@@ -203,15 +206,16 @@
                 allAtomsSurfBoxs, allAtomsBulkBoxs = scanAllAtomsResult
                 allLensSurfBoxs.append(allAtomsSurfBoxs)
                 allLensBulkBoxs.append(allAtomsBulkBoxs)
                 allLensSurfCnts.append(len(allAtomsSurfBoxs))
     counts = [log10(sCnt) if sCnt != 0 else np.nan for sCnt in allLensSurfCnts]
 
     if writeBox:
-        writeBoxCoords(atomsEle, atomsXYZ, allLensSurfBoxs, allLensBulkBoxs, minXYZ, scanBoxLens, writeFileDir, npName)
+        writeBoxCoords(atomsEle, atomsXYZ, allLensSurfBoxs, allLensBulkBoxs, minXYZ, scanBoxLens, minValFromBound, 
+                       writeFileDir, npName)
     return scales, counts
 
 
 # @annotate('findSlope', color='green')
 def findSlope(scales, counts, npName='', writeFileDir='boxCntOutputs', lenRange='trim',
               minSampleNum=5, confLvl=95, 
               visReg=True, figType='paper', saveFig=False, showPlot=False):
@@ -349,15 +353,15 @@
 # @annotate('runCase', color='cyan')
 # @estDuration
 def runBoxCnt(xyzFilePath, 
               radType='atomic', calcBL=False, findSurfOption='alphaShape', alphaMult=2.0,
               writeFileDir='boxCntOutputs', lenRange='trim', minSampleNum=5, confLvl=95, 
               rmInSurf=True, vis=True, figType='paper', saveFig=False, showPlot=False, verbose=False,
               runPointCloudBoxCnt=True, numPoints=300, gridNum=1024, exePath='$FASTBC_EXE', genPCD=False,
-              runExactSphereBoxCnt=True, minLenMult=0.25, maxLenMult=1, numBoxLenSample=10, writeBox=True): 
+              runExactSphereBoxCnt=True, minLenMult=0.25, maxLenMult=1, numBoxLenSample=10, minValFromBound=5.0, writeBox=True): 
     """
     Run box-counting algorithm on the surface of a given object consisting of a set of spheres represented as either
     point clouds or exact spherical surface.
     
     Parameters
     ----------
     xyzFilePath : str
@@ -406,14 +410,16 @@
         Whether to represent the surface as exact spheres.
     minLenMult : float, optional
         Multiplier to the minimum radii to determine the minimum box length for box-counting dimension estimation.
     maxLenMult : float, optional
         Multiplier to the minimum radii to determine the maximum box length for box-counting dimension estimation.
     numBoxLenSample : int, optional
         Number of box lengths to use for the collection of the box count data, spaced evenly on logarithmic scale.
+    minValFromBound : Union[int,float]
+        Buffer distance from the borders of the largest box in Angstrom.
     writeBox : bool, optional
         Whether to generate output files for visualisation.
     
     Returns
     -------
     r2PC : float
         Coefficient of determination from determination of the dimension of point clouds surface.
@@ -451,15 +457,15 @@
                                              rmInSurf, vis, verbose, genPCD)
         r2PC, bcDimPC, confIntPC = findSlope(scalesPC, countsPC, f"{testCase}_PC", writeFileDir, lenRange,
                                              minSampleNum, confLvl, vis, figType, saveFig, showPlot)
     if runExactSphereBoxCnt:
         minAtomRad = atomsRad.min()
         scalesES, countsES = getSphereBoxCnts(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
                                               maxRange, (minAtomRad * minLenMult, minAtomRad * maxLenMult),
-                                              minXYZ, testCase, writeFileDir, numBoxLenSample,
+                                              minXYZ, testCase, writeFileDir, numBoxLenSample, minValFromBound,
                                               rmInSurf, writeBox, verbose)
         r2ES, bcDimES, confIntES = findSlope(scalesES, countsES, f"{testCase}_ES", writeFileDir, lenRange,
                                              minSampleNum, confLvl, vis, figType, saveFig, showPlot)
     if verbose:
         if runPointCloudBoxCnt:
             print(f"  Point clouds  D_Box: {bcDimPC:.4f} [{confIntPC[0]:.4f}, {confIntPC[1]:.4f}],  R2: {r2PC:.4f}")
         if runExactSphereBoxCnt:
```

### Comparing `sphractal-0.8.1/src/sphractal/constants.py` & `sphractal-0.9.0/src/sphractal/constants.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.1/src/sphractal/data/example.xyz` & `sphractal-0.9.0/src/sphractal/data/example.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.1/src/sphractal/surfExact.py` & `sphractal-0.9.0/src/sphractal/surfExact.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,21 +6,18 @@
 from numba import njit
 import numpy as np
 
 from sphractal.utils import calcDist, oppositeInnerAtoms
 # from sphractal.utils import annotate
 
 
-MIN_VAL_FROM_BOUND = 5.0  # Angstrom
-
-
 @njit(fastmath=True, cache=True)
-def getNearFarCoord(scanBoxIdx, boxLen, lowBound, atomCoord):
+def getNearFarCoord(scanBoxIdx, boxLen, lowBound, atomCoord, minValFromBound=5.0):
     """Find the nearest and furthest point of a given box from a given atom."""
-    scanBoxMax = lowBound - MIN_VAL_FROM_BOUND + (scanBoxIdx+1)*boxLen
+    scanBoxMax = lowBound - minValFromBound + (scanBoxIdx+1)*boxLen
     scanBoxMin = scanBoxMax - boxLen
     if atomCoord < scanBoxMin:
         scanBoxNear, scanBoxFar = scanBoxMin, scanBoxMax
     elif atomCoord > scanBoxMax:
         scanBoxNear, scanBoxFar = scanBoxMax, scanBoxMin
     else:
         scanBoxNear = atomCoord
@@ -29,21 +26,21 @@
     return scanBoxNear, scanBoxFar
 
 
 @njit(fastmath=True, cache=True)
 def scanBox(minXYZ, scanBoxIdxs, scanBoxNearFarXYZs, boxLen,
             atomIdx, atomRad, atomXYZ, atomNeighIdxs,
             atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
-            rmInSurf=True):
+            minValFromBound=5.0, rmInSurf=True):
     """Find the nearest and furthest point of a given box from a given atom."""
     # Remove the box if it covers the inner surface
     if rmInSurf:
-        scanBoxX = minXYZ[0] - MIN_VAL_FROM_BOUND + (scanBoxIdxs[0]+1)*boxLen - boxLen*0.5
-        scanBoxY = minXYZ[1] - MIN_VAL_FROM_BOUND + (scanBoxIdxs[1]+1)*boxLen - boxLen*0.5
-        scanBoxZ = minXYZ[2] - MIN_VAL_FROM_BOUND + (scanBoxIdxs[2]+1)*boxLen - boxLen*0.5
+        scanBoxX = minXYZ[0] - minValFromBound + (scanBoxIdxs[0]+1)*boxLen - boxLen*0.5
+        scanBoxY = minXYZ[1] - minValFromBound + (scanBoxIdxs[1]+1)*boxLen - boxLen*0.5
+        scanBoxZ = minXYZ[2] - minValFromBound + (scanBoxIdxs[2]+1)*boxLen - boxLen*0.5
         if not oppositeInnerAtoms(np.array((scanBoxX, scanBoxY, scanBoxZ)), atomXYZ, atomNeighIdxs,
                                   atomsSurfIdxs, atomsXYZ, atomsNeighIdxs):
             return 'none'
 
     # Check what does the box cover
     distNear = calcDist(atomXYZ, np.array(scanBoxNearFarXYZs[:3]))
     distFar = calcDist(atomXYZ, np.array(scanBoxNearFarXYZs[-3:]))
@@ -61,95 +58,96 @@
             return 'none'
 
 
 # @annotate('scanAtom', color='cyan')
 @njit(fastmath=True, cache=True)
 def scanAtom(args):
     """Count the number of boxes that cover the outer spherical surface of a given atom."""
-    magn, boxLen, minXYZ, atomIdx, atomRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, rmInSurf = args
+    magn, boxLen, minXYZ, atomIdx, atomRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, minValFromBound, rmInSurf = args
     atomXYZ, atomNeighIdxsPadded = atomsXYZ[atomIdx], atomsNeighIdxs[atomIdx]
     atomNeighIdxs = atomNeighIdxsPadded[atomNeighIdxsPadded > -1]
 
     atomX, atomY, atomZ = atomXYZ
     minX, minY, minZ = minXYZ
-    atomBoxIdxX = int((atomX - minX + MIN_VAL_FROM_BOUND)/boxLen)
-    atomBoxIdxY = int((atomY - minY + MIN_VAL_FROM_BOUND)/boxLen)
-    atomBoxIdxZ = int((atomZ - minZ + MIN_VAL_FROM_BOUND)/boxLen)
+    atomBoxIdxX = int((atomX - minX + minValFromBound)/boxLen)
+    atomBoxIdxY = int((atomY - minY + minValFromBound)/boxLen)
+    atomBoxIdxZ = int((atomZ - minZ + minValFromBound)/boxLen)
     numScan = ceil((atomRad + boxLen)/boxLen)
     atomSurfBoxs, atomBulkBoxs = [], []
     for i in range(-numScan, numScan + 1):
         scanBoxIdxX = atomBoxIdxX + i
         if scanBoxIdxX < 0 or scanBoxIdxX >= magn:
             continue
-        scanBoxNearX, scanBoxFarX = getNearFarCoord(scanBoxIdxX, boxLen, minX, atomX)
+        scanBoxNearX, scanBoxFarX = getNearFarCoord(scanBoxIdxX, boxLen, minX, atomX, minValFromBound)
         for j in range(-numScan, numScan + 1):
             scanBoxIdxY = atomBoxIdxY + j
             if scanBoxIdxY < 0 or scanBoxIdxY >= magn:
                 continue
-            scanBoxNearY, scanBoxFarY = getNearFarCoord(scanBoxIdxY, boxLen, minY, atomY)
+            scanBoxNearY, scanBoxFarY = getNearFarCoord(scanBoxIdxY, boxLen, minY, atomY, minValFromBound)
             for k in range(-numScan, numScan + 1):
                 scanBoxIdxZ = atomBoxIdxZ + k
                 if scanBoxIdxZ < 0 or scanBoxIdxZ >= magn:
                     continue
-                scanBoxNearZ, scanBoxFarZ = getNearFarCoord(scanBoxIdxZ, boxLen, minZ, atomZ)
+                scanBoxNearZ, scanBoxFarZ = getNearFarCoord(scanBoxIdxZ, boxLen, minZ, atomZ, minValFromBound)
 
                 belong = scanBox(minXYZ, (scanBoxIdxX, scanBoxIdxY, scanBoxIdxZ),
                                  (scanBoxNearX, scanBoxNearY, scanBoxNearZ, scanBoxFarX, scanBoxFarY, scanBoxFarZ),
                                  boxLen,
                                  atomIdx, atomRad, atomXYZ, atomNeighIdxs,
                                  atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
-                                 rmInSurf)
+                                 minValFromBound, rmInSurf)
                 if belong == 'surf':
                     atomSurfBoxs.append((scanBoxIdxX, scanBoxIdxY, scanBoxIdxZ))
                 elif belong == 'bulk':
                     atomBulkBoxs.append((scanBoxIdxX, scanBoxIdxY, scanBoxIdxZ))
     return atomSurfBoxs, atomBulkBoxs
 
 
 # @annotate('scanAtomsForLoop', color='cyan')
 @njit(fastmath=True, cache=True)
 def scanAtomsForLoop(atomsIdxs, magn, boxLen, minXYZ,
                      atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
-                     rmInSurf=True):
+                     minValFromBound=5.0, rmInSurf=True):
     """Serialised loop to scan the atoms for timing comparison with the parallelised version."""
     allAtomsSurfBoxs, allAtomsBulkBoxs = [], []
     for atomIdx in atomsIdxs:
         scanAtomInp = (magn, boxLen, minXYZ, atomIdx,
-                       atomsRad[atomIdx], atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, rmInSurf)
+                       atomsRad[atomIdx], atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, 
+                       minValFromBound, rmInSurf)
         atomSurfBoxs, atomBulkBoxs = scanAtom(scanAtomInp)
         allAtomsSurfBoxs.extend(atomSurfBoxs)
         allAtomsBulkBoxs.extend(atomBulkBoxs)
     return allAtomsSurfBoxs, allAtomsBulkBoxs
 
 
 # @annotate('scanAllAtoms', color='magenta')
 def scanAllAtoms(args):
     """Count the number of boxes that cover the outer spherical surface of a set of atoms for a given box size."""
-    magn, boxLen, atomsIdxs, minXYZ, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, rmInSurf, verbose, maxCPU = args
+    magn, boxLen, atomsIdxs, minXYZ, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, minValFromBound, rmInSurf, verbose, maxCPU = args
     scanAtomInps = [(magn, boxLen, minXYZ, atomIdx, atomsRad[atomIdx],
-                     atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, rmInSurf) for atomIdx in atomsIdxs]
+                     atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, minValFromBound, rmInSurf) for atomIdx in atomsIdxs]
     allAtomsSurfBoxs, allAtomsBulkBoxs = [], []
     with Pool(max_workers=maxCPU) as pool:
         for scanAtomResult in pool.map(scanAtom, scanAtomInps, chunksize=ceil(len(atomsIdxs) / maxCPU)):
             allAtomsSurfBoxs.extend(scanAtomResult[0])
             allAtomsBulkBoxs.extend(scanAtomResult[1])
     # allAtomsSurfBoxs, allAtomsBulkBoxs = scanAtomsForLoop(atomsIdxs, magn, boxLen, minXYZ,
     #                                                       atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
-    #                                                       rmInSurf)
+    #                                                       minValFromBound, rmInSurf)
     allAtomsSurfBoxs, allAtomsBulkBoxs = set(allAtomsSurfBoxs), set(allAtomsBulkBoxs)
     allAtomsSurfBoxs.difference_update(allAtomsBulkBoxs)
 
     if verbose:
         epsInvStr = f"{1 / boxLen:.2f}"
         print(f"{epsInvStr.rjust(10)}{str(len(allAtomsBulkBoxs)).rjust(12)}{str(len(allAtomsSurfBoxs)).rjust(12)}")
     return allAtomsSurfBoxs, allAtomsBulkBoxs
 
 
 # @annotate('writeBoxCoords', color='yellow')
-def writeBoxCoords(atomsEle, atomsXYZ, allSurfBoxs, allBulkBoxs, minXYZ, boxLens,
+def writeBoxCoords(atomsEle, atomsXYZ, allSurfBoxs, allBulkBoxs, minXYZ, boxLens, minValFromBound,
                    writeFileDir, npName):
     """Write out coordinates of scanned boxes."""
     minX, minY, minZ = minXYZ
     boxCoordsDir = f"{writeFileDir}/boxCoords"
     if not isdir(boxCoordsDir):
         if not isdir(writeFileDir):
             mkdir(writeFileDir)
@@ -158,22 +156,22 @@
         for (i, boxLen) in enumerate(boxLens):
             if i != 0:
                 f.write('\n')
             f.write(f"{len(atomsEle) + len(allSurfBoxs[i]) + len(allBulkBoxs[i])}\n")
             for (j, atomXYZ) in enumerate(atomsXYZ):
                 f.write(f"\n{atomsEle[j]}\t{atomXYZ[0]} {atomXYZ[1]} {atomXYZ[2]}")
             for (boxIDX, boxIDY, boxIDZ) in allSurfBoxs[i]:
-                boxX = minX - MIN_VAL_FROM_BOUND + boxIDX*boxLen + boxLen/2
-                boxY = minY - MIN_VAL_FROM_BOUND + boxIDY*boxLen + boxLen/2
-                boxZ = minZ - MIN_VAL_FROM_BOUND + boxIDZ*boxLen + boxLen/2
+                boxX = minX - minValFromBound + boxIDX*boxLen + boxLen/2
+                boxY = minY - minValFromBound + boxIDY*boxLen + boxLen/2
+                boxZ = minZ - minValFromBound + boxIDZ*boxLen + boxLen/2
                 f.write(f"\nOV\t{boxX:.6f} {boxY:.6f} {boxZ:.6f}")
             for (boxIDX, boxIDY, boxIDZ) in allBulkBoxs[i]:
-                boxX = minX - MIN_VAL_FROM_BOUND + boxIDX*boxLen + boxLen/2
-                boxY = minY - MIN_VAL_FROM_BOUND + boxIDY*boxLen + boxLen/2
-                boxZ = minZ - MIN_VAL_FROM_BOUND + boxIDZ*boxLen + boxLen/2
+                boxX = minX - minValFromBound + boxIDX*boxLen + boxLen/2
+                boxY = minY - minValFromBound + boxIDY*boxLen + boxLen/2
+                boxZ = minZ - minValFromBound + boxIDZ*boxLen + boxLen/2
                 f.write(f"\nIV\t{boxX:.6f} {boxY:.6f} {boxZ:.6f}")
 
 
 # @annotate('findTargetAtoms', color='cyan')
 @njit(fastmath=True, cache=True)
 def findTargetAtoms(atomsNeighIdxs):
     """Find atoms to be scanned if not removing inner surfaces (atoms with neighbours that are on the surface)."""
```

### Comparing `sphractal-0.8.1/src/sphractal/surfPointClouds.py` & `sphractal-0.9.0/src/sphractal/surfPointClouds.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.1/src/sphractal/utils.py` & `sphractal-0.9.0/src/sphractal/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             for z in range(-1, 2):
                 dirVecs.append((x, y, z))
     return dirVecs
 
 
 # @annotate('findNN', color='magenta')
 @njit(fastmath=True, cache=True)
-def findNN(atomsRad, atomsXYZ, minXYZ, maxXYZ, maxAtomRad, alphaMult, calcBL=False):
+def findNN(atomsRad, atomsXYZ, minXYZ, maxXYZ, maxAtomRad, radMult, calcBL=False):
     """Compute the nearest neighbour list and average bond length for each atom."""
     (minX, minY, minZ), (maxX, maxY, maxZ) = minXYZ, maxXYZ
     atomsNeighIdxs = [[int(j) for j in range(0)] for _ in range(len(atomsRad))]
     atomsAvgBondLen = np.zeros_like(atomsRad)
     stepSize = ceil(maxAtomRad * 2)
     numX, numY, numZ = ceil((maxX-minX) / stepSize), ceil((maxY-minY) / stepSize), ceil((maxZ-minZ) / stepSize)
     boxes = [[[[int(i) for i in range(0)] for _ in range(numZ)] for _ in range(numY)] for _ in range(numX)]
@@ -87,15 +87,15 @@
             if 0 <= x + dirX < numX and 0 <= y + dirY < numY and 0 <= z + dirZ < numZ:
                 for j in boxes[x + dirX][y + dirY][z + dirZ]:
                     atom2X, atom2Y, atom2Z = atomsXYZ[j]
                     atom2rad = atomsRad[j]
 
                     diffX, diffY, diffZ = abs(atom1X - atom2X), abs(atom1Y - atom2Y), abs(atom1Z - atom2Z)
                     sumOfSquares = diffX * diffX + diffY * diffY + diffZ * diffZ
-                    if sumOfSquares < ((atom1rad+atom2rad)*alphaMult) ** 2:
+                    if sumOfSquares < ((atom1rad+atom2rad)*radMult) ** 2:
                         atomsNeighIdxs[i].append(j)
                         atomsNeighIdxs[j].append(i)
                         if calcBL:
                             atomsAvgBondLen[i] += sqrt(diffX * diffX + diffY * diffY + diffZ * diffZ)
                             atomsAvgBondLen[j] += sqrt(diffX * diffX + diffY * diffY + diffZ * diffZ)
         boxes[x][y][z].append(i)
```

### Comparing `sphractal-0.8.1/tests/fixtures.py` & `sphractal-0.9.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.1/tests/test_sphractal.py` & `sphractal-0.9.0/tests/test_sphractal.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.8.1/PKG-INFO` & `sphractal-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphractal
-Version: 0.8.1
+Version: 0.9.0
 Summary: Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm.
 Home-page: https://github.com/Jon-Ting/sphractal
 License: MIT
 Keywords: box-counting,box-count,fractal,dimension,sphere,surface
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
```

