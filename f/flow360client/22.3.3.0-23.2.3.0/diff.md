# Comparing `tmp/flow360client-22.3.3.0.tar.gz` & `tmp/flow360client-23.2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow360client-22.3.3.0.tar", last modified: Mon Oct 17 16:02:47 2022, max compression
+gzip compressed data, was "flow360client-23.2.3.0.tar", last modified: Mon Jul 10 14:20:46 2023, max compression
```

## Comparing `flow360client-22.3.3.0.tar` & `flow360client-23.2.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 feilin    (1000) feilin    (1000)        0 2022-10-17 16:02:47.311201 flow360client-22.3.3.0/
--rw-rw-r--   0 feilin    (1000) feilin    (1000)      360 2022-10-17 16:02:47.311201 flow360client-22.3.3.0/PKG-INFO
--rw-rw-r--   0 feilin    (1000) feilin    (1000)    11249 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/README.md
-drwxrwxr-x   0 feilin    (1000) feilin    (1000)        0 2022-10-17 16:02:47.307201 flow360client-22.3.3.0/flow360client/
--rw-rw-r--   0 feilin    (1000) feilin    (1000)      555 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/IOutils.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)    14208 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/__init__.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     2824 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/authentication.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     8934 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/case.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     2442 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/casehelper.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)      954 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/config.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     1143 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/errorHandling.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     5510 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/fun3d_to_flow360.py
-drwxrwxr-x   0 feilin    (1000) feilin    (1000)        0 2022-10-17 16:02:47.311201 flow360client-22.3.3.0/flow360client/generator/
--rw-rw-r--   0 feilin    (1000) feilin    (1000)        0 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/generator/__init__.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     4423 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/generator/case.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     9143 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/generator/caseBoundary.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     5488 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/generator/caseFreestream.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     3203 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/generator/caseGeometry.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     2429 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/generator/caseNavierStokesSolver.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     1164 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/generator/caseOutput.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     1237 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/generator/caseSlidingInterfaces.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     5250 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/generator/caseTimeStepping.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     4267 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/generator/caseTurbulenceSolver.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     2270 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/generator/core.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     3032 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/generator/meshInfo.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     2320 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/httputils.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     6287 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/mesh.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     8637 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/meshUtils.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     5374 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/s3utils.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     1068 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/studio.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     3711 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/surfaceMesh.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)      874 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/task.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)      597 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/validation.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)      994 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/version.py
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     1735 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/flow360client/versionCheck.py
-drwxrwxr-x   0 feilin    (1000) feilin    (1000)        0 2022-10-17 16:02:47.307201 flow360client-22.3.3.0/flow360client.egg-info/
--rw-rw-r--   0 feilin    (1000) feilin    (1000)      360 2022-10-17 16:02:47.000000 flow360client-22.3.3.0/flow360client.egg-info/PKG-INFO
--rw-rw-r--   0 feilin    (1000) feilin    (1000)     1170 2022-10-17 16:02:47.000000 flow360client-22.3.3.0/flow360client.egg-info/SOURCES.txt
--rw-rw-r--   0 feilin    (1000) feilin    (1000)       71 2022-10-17 16:02:47.000000 flow360client-22.3.3.0/flow360client.egg-info/dependency_links.txt
--rw-rw-r--   0 feilin    (1000) feilin    (1000)      133 2022-10-17 16:02:47.000000 flow360client-22.3.3.0/flow360client.egg-info/requires.txt
--rw-rw-r--   0 feilin    (1000) feilin    (1000)       14 2022-10-17 16:02:47.000000 flow360client-22.3.3.0/flow360client.egg-info/top_level.txt
--rw-rw-r--   0 feilin    (1000) feilin    (1000)       38 2022-10-17 16:02:47.311201 flow360client-22.3.3.0/setup.cfg
--rw-rw-r--   0 feilin    (1000) feilin    (1000)      725 2022-10-17 16:01:34.000000 flow360client-22.3.3.0/setup.py
+drwxrwxr-x   0 feilin    (1000) feilin    (1000)        0 2023-07-10 14:20:46.134498 flow360client-23.2.3.0/
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)      285 2023-07-10 14:20:46.134498 flow360client-23.2.3.0/PKG-INFO
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)    11249 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/README.md
+drwxrwxr-x   0 feilin    (1000) feilin    (1000)        0 2023-07-10 14:20:46.130498 flow360client-23.2.3.0/flow360client/
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)      555 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/IOutils.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)    13626 2023-07-10 14:14:37.000000 flow360client-23.2.3.0/flow360client/__init__.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     2824 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/authentication.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     8854 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/case.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     2442 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/casehelper.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)      954 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/config.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     1143 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/errorHandling.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     5510 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/fun3d_to_flow360.py
+drwxrwxr-x   0 feilin    (1000) feilin    (1000)        0 2023-07-10 14:20:46.134498 flow360client-23.2.3.0/flow360client/generator/
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)        0 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/generator/__init__.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     4421 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/generator/case.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     9143 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/generator/caseBoundary.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     5488 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/generator/caseFreestream.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     3203 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/generator/caseGeometry.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     2429 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/generator/caseNavierStokesSolver.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     1164 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/generator/caseOutput.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     1237 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/generator/caseSlidingInterfaces.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     5250 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/generator/caseTimeStepping.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     4267 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/generator/caseTurbulenceSolver.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     2270 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/generator/core.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     3028 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/generator/meshInfo.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     2348 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/httputils.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     7891 2023-07-10 14:14:37.000000 flow360client-23.2.3.0/flow360client/mesh.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     9470 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/meshUtils.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     5344 2023-07-10 14:14:37.000000 flow360client-23.2.3.0/flow360client/s3utils.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     1068 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/studio.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     3657 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/surfaceMesh.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)      874 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/task.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)      597 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/validation.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)      994 2023-07-10 14:20:33.000000 flow360client-23.2.3.0/flow360client/version.py
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     1735 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/flow360client/versionCheck.py
+drwxrwxr-x   0 feilin    (1000) feilin    (1000)        0 2023-07-10 14:20:46.130498 flow360client-23.2.3.0/flow360client.egg-info/
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)      285 2023-07-10 14:20:46.000000 flow360client-23.2.3.0/flow360client.egg-info/PKG-INFO
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)     1170 2023-07-10 14:20:46.000000 flow360client-23.2.3.0/flow360client.egg-info/SOURCES.txt
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)       71 2023-07-10 14:20:46.000000 flow360client-23.2.3.0/flow360client.egg-info/dependency_links.txt
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)      133 2023-07-10 14:20:46.000000 flow360client-23.2.3.0/flow360client.egg-info/requires.txt
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)       14 2023-07-10 14:20:46.000000 flow360client-23.2.3.0/flow360client.egg-info/top_level.txt
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)       38 2023-07-10 14:20:46.134498 flow360client-23.2.3.0/setup.cfg
+-rw-rw-r--   0 feilin    (1000) feilin    (1000)      725 2023-07-10 13:24:55.000000 flow360client-23.2.3.0/setup.py
```

### Comparing `flow360client-22.3.3.0/README.md` & `flow360client-23.2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/IOutils.py` & `flow360client-23.2.3.0/flow360client/IOutils.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/__init__.py` & `flow360client-23.2.3.0/flow360client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,57 +70,38 @@
         print('mesh file {0} does not Exist!'.format(fname), flush=True)
         raise FileDoesNotExist(fname)
     if meshJson is not None:
         meshJson = readJsonFileOrDict(meshJson)
     if meshName is None:
         meshName = os.path.splitext(basename(fname))[0]
 
-    if fmat is None:
-        if fname.endswith('.ugrid') or fname.endswith('.ugrid.gz') or \
-                fname.endswith('.ugrid.bz2'):
-            fmat = 'aflr3'
-        elif fname.endswith('.cgns') or fname.endswith('.cgns.gz') or \
-                fname.endswith('.cgns.bz2'):
-            fmat = 'cgns'
-        else:
-            raise RuntimeError('Unknown format for file {}'.format(fname))
-
-    if endianness is None:
-        try:
-            if fname.find('.b8.') != -1:
-                endianness = 'big'
-
-            elif fname.find('.lb8.') != -1:
-                endianness = 'little'
-            else:
-                endianness = ''
-        except:
-            raise RuntimeError('Unknown endianness for file {}'.format(fname))
+
+    remoteFileName, fmat, endianness, compression = mesh.GetRemoteMeshFileName(fname)
 
     if noSlipWalls is None and meshJson is None:
         raise RuntimeError('Both noSlipWals or meshJson are none')
 
     if noSlipWalls is not None and meshJson is not None:
         noSlipWalls = None
         print('noSlipWalls will be override by meshJson')
 
     if noSlipWalls is not None:
         validateMeshAndMeshJson(fname, { "boundaries": {"noSlipWalls": noSlipWalls }}, solverVersion)
-        resp = mesh.AddMesh(meshName, noSlipWalls, tags, fmat, endianness, solverVersion)
+        resp = mesh.AddMesh(meshName, remoteFileName, noSlipWalls, tags, fmat, endianness, compression, solverVersion)
     else:
         if isinstance(meshJson, str):
             if not os.path.exists(meshJson):
                 print('meshJson file {0} does not Exist!'.format(meshJson), flush=True)
                 raise FileDoesNotExist(meshJson)
             meshJson = json.load(open(meshJson))
         validateMeshAndMeshJson(fname, meshJson, solverVersion)
-        resp = mesh.AddMeshWithJson(meshName, meshJson, tags, fmat, endianness, solverVersion)
+        resp = mesh.AddMeshWithJson(meshName, remoteFileName, meshJson, tags, fmat, endianness, compression, solverVersion)
 
     meshId = resp['meshId']
-    mesh.UploadMesh(meshId, fname)
+    mesh.UploadMesh(meshId, fname, remoteFileName)
     print()
     return meshId
 
 
 def NewMeshFromSurface(surfaceMeshId, config, meshName=None, tags=[], solverVersion=None, validate=True):
     if isinstance(config, str):
         if not os.path.exists(config):
```

### Comparing `flow360client-22.3.3.0/flow360client/authentication.py` & `flow360client-23.2.3.0/flow360client/authentication.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/case.py` & `flow360client-23.2.3.0/flow360client/case.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,23 +64,21 @@
         return None
 
     resp['runtimeParams'] = runtimeContent
     return resp
 
 
 @refreshToken
-def ListCases(name=None, status=None, meshId=None, include_deleted=False):
+def ListCases(meshId=None, include_deleted=False):
     if meshId is None:
         url = "cases"
     else:
         url = f'volumemeshes/{meshId}/cases'
 
-    resp = flow360ApiGet(url)
-    if not include_deleted:
-        resp = list(filter(lambda i: i['caseStatus'] != 'deleted', resp))
+    resp = flow360ApiGet(url, params={"includeDeleted": include_deleted})
     return resp
 
 
 @refreshToken
 def GetCaseResidual(caseId):
     try:
         resp = flow360ApiGet(f'case/{caseId}/result/nonlinear_residual_v2')
@@ -261,7 +259,9 @@
             info = GetCaseInfo(caseId)
             if info['caseStatus'] in ['deleted', 'error', 'preerror', 'unknownError', 'diverged', 'completed']:
                 return info['caseStatus']
         except Exception as e:
             print('Warning : {0}'.format(str(e)))
 
         time.sleep(sleepSeconds)
+
+
```

### Comparing `flow360client-22.3.3.0/flow360client/casehelper.py` & `flow360client-23.2.3.0/flow360client/casehelper.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/config.py` & `flow360client-23.2.3.0/flow360client/config.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/errorHandling.py` & `flow360client-23.2.3.0/flow360client/errorHandling.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/fun3d_to_flow360.py` & `flow360client-23.2.3.0/flow360client/fun3d_to_flow360.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/generator/case.py` & `flow360client-23.2.3.0/flow360client/generator/case.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from requests.exceptions import HTTPError
 from .core import getInput, printHelp, bcolors
 from .meshInfo import getBoundariesAndCoordinates, displayWallBoundaries, \
-                      MeshNotProcessedYetError
+                      MeshNotUploadedYetError
 from .caseBoundary import inputAllBoundaries
 from .caseGeometry import inputGeometry
 from .caseFreestream import inputFreestream
 from .caseSlidingInterfaces import inputSlidingInterfaces
 from .caseTimeStepping import inputTimeStepping
 from .caseNavierStokesSolver import inputNavierStokesSolverOptions
 from .caseTurbulenceSolver import inputTurbulenceSolverOptions
@@ -93,12 +93,12 @@
                      inputTurbulenceSolverOptions, isSteady)
         inputSection(caseJson, ('volumeOutput', 'surfaceOutput'),
                      inputVolumeSurfaceOutputOptions)
     except (KeyboardInterrupt, EOFError):
         print(bcolors.ENDC)
         print(bcolors.FAIL + 'Interrupted, returning incomplete case.')
         print(bcolors.ENDC)
-    except MeshNotProcessedYetError:
+    except MeshNotUploadedYetError:
         print(bcolors.ENDC)
         print(bcolors.FAIL + 'This utility works only for processed mesh.')
         print(bcolors.ENDC)
     return caseJson
```

### Comparing `flow360client-22.3.3.0/flow360client/generator/caseBoundary.py` & `flow360client-23.2.3.0/flow360client/generator/caseBoundary.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/generator/caseFreestream.py` & `flow360client-23.2.3.0/flow360client/generator/caseFreestream.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/generator/caseGeometry.py` & `flow360client-23.2.3.0/flow360client/generator/caseGeometry.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/generator/caseNavierStokesSolver.py` & `flow360client-23.2.3.0/flow360client/generator/caseNavierStokesSolver.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/generator/caseOutput.py` & `flow360client-23.2.3.0/flow360client/generator/caseOutput.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/generator/caseSlidingInterfaces.py` & `flow360client-23.2.3.0/flow360client/generator/caseSlidingInterfaces.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/generator/caseTimeStepping.py` & `flow360client-23.2.3.0/flow360client/generator/caseTimeStepping.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/generator/caseTurbulenceSolver.py` & `flow360client-23.2.3.0/flow360client/generator/caseTurbulenceSolver.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/generator/core.py` & `flow360client-23.2.3.0/flow360client/generator/core.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/generator/meshInfo.py` & `flow360client-23.2.3.0/flow360client/generator/meshInfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 
     with tempfile.TemporaryDirectory() as tmpDir:
         fname = os.path.join(tmpDir, 'tmp.gltf')
         S3TransferType.VolumeMesh.download_file(meshId, f"visualize/{meshId}.gltf", to_file=fname)
         gltf = GLTF2().load(fname)
     return gltf
 
-class MeshNotProcessedYetError(NotImplementedError):
+class MeshNotUploadedYetError(NotImplementedError):
     pass
 
 def getBoundariesAndCoordinates(meshId):
     info = mesh.GetMeshInfo(meshId)
-    if info['status'] != 'processed':
-        print('Mesh not yet processed: ', info['status'])
-        raise MeshNotProcessedYetError
+    if info['status'] != 'uploaded':
+        print('Mesh not yet uploaded: ', info['status'])
+        raise MeshNotUploadedYetError
     gltf = readGLTF(meshId)
     boundaries = []
     for boundary in gltf.meshes:
         vertices = []
         for primitive in boundary.primitives:
             # get the binary data for this boundary primitive from the buffer
             accessor = gltf.accessors[primitive.attributes.POSITION]
```

### Comparing `flow360client-22.3.3.0/flow360client/httputils.py` & `flow360client-23.2.3.0/flow360client/httputils.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,17 +47,17 @@
 def flow360ApiPut(method, data):
     queryUrl = f"{Config.FLOW360_WEB_API_ENDPONT}/{method}"
     headers = {'Authorization': f"Bearer {Config.auth['accessToken']}", 'FLOW360ACCESSUSER': Config.user['accessIdentityId']}
     return requests.put(queryUrl, headers=headers, json=data)
 
 
 @handle_response
-def flow360ApiGet(method):
+def flow360ApiGet(method, params=None):
     queryUrl = f"{Config.FLOW360_WEB_API_ENDPONT}/{method}"
     headers = {'Authorization': f"Bearer {Config.auth['accessToken']}", 'FLOW360ACCESSUSER': Config.user['accessIdentityId']}
-    return requests.get(queryUrl, headers=headers)
+    return requests.get(queryUrl, headers=headers, params=params)
 
 @handle_response
 def flow360ApiDelete(method):
     queryUrl = f"{Config.FLOW360_WEB_API_ENDPONT}/{method}"
     headers = {'Authorization': f"Bearer {Config.auth['accessToken']}", 'FLOW360ACCESSUSER': Config.user['accessIdentityId']}
     return requests.delete(queryUrl, headers=headers)
```

### Comparing `flow360client-22.3.3.0/flow360client/mesh.py` & `flow360client-23.2.3.0/flow360client/mesh.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,46 +9,48 @@
 from .errorHandling import deprecated 
 from .validation import validateJSON
 
 auth = Config.auth
 keys = Config.user
 
 @refreshToken
-def AddMeshWithJson(name, mesh_json, tags, fmat, endianness, solver_version=None):
-    return AddMeshBase(name, mesh_json, tags, fmat, endianness, solver_version)
+def AddMeshWithJson(name, remoteFileName, mesh_json, tags, fmat, endianness, compression=None, solver_version=None):
+    return AddMeshBase(name, remoteFileName, mesh_json, tags, fmat, endianness, compression, solver_version)
 
 
 @refreshToken
-def AddMesh(name, noSlipWalls, tags, fmat, endianness, solver_version=None):
-    return AddMeshBase(name, {
+def AddMesh(name, remoteFileName, noSlipWalls, tags, fmat, endianness, compression=None, solver_version=None):
+    return AddMeshBase(name, remoteFileName, {
         "boundaries":
             {
                 "noSlipWalls": noSlipWalls
             }
-    }, tags, fmat, endianness, solver_version)
+    }, tags, fmat, endianness, compression, solver_version)
 
-def AddMeshBase(name, meshParams, tags, fmat, endianness, solver_version):
+def AddMeshBase(name, remoteFileName, meshParams, tags, fmat, endianness, compression, solver_version):
     '''
        AddMesh(name, noSlipWalls, tags, fmat, endianness, version)
        returns the raw HTTP response
        {
            'meshId' : 'xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx',
            'addTime' : '2019:01:01:01:01:01.000000'
        }
        The returned meshId is need to subsequently call UploadMesh
        Example:
            resp = AddMesh('foo', [1], [], 'aflr3', 'big')
            UploadMesh(resp['meshId'], 'mesh.lb8.ugrid')
        '''
 
     body = {
+        "fileName": remoteFileName,
         "meshName": name,
         "meshTags": tags,
         "meshFormat": fmat,
         "meshEndianness": endianness,
+        "meshCompression": compression,
         "meshParams": json.dumps(meshParams)
     }
 
     if solver_version:
         body['solverVersion'] = solver_version
 
     resp = flow360ApiPost("volumemeshes", data=body)
@@ -93,48 +95,88 @@
     except Exception as e:
         print('invalid meshParams or not exist:' + str(resp['meshParams']))
         pass
     resp['meshParams'] = meshParams
     return resp
 
 @refreshToken
-def CompleteVolumeMeshUpload(meshInfo, fileName):
-    url = f"volumemeshes/{meshInfo['id']}/completeUpload?fileName={fileName}"
-    resp = flow360ApiPost(url, meshInfo)
+def CompleteVolumeMeshUpload(meshId, fileName):
+    url = f"volumemeshes/{meshId}/completeUpload?fileName={fileName}"
+    resp = flow360ApiPost(url)
     return resp
 
 
 @refreshToken
 def ListMeshes(include_deleted=False):
-    resp = flow360ApiGet("volumemeshes")
-    if not include_deleted:
-        resp = list(filter(lambda i: i['meshStatus'] != 'deleted', resp))
+    resp = flow360ApiGet("volumemeshes", params={"includeDeleted": include_deleted})
     return resp
 
 
-@refreshToken
-def UploadMesh(meshId, meshFile):
-    '''
-    UploadMesh(meshId, meshFile)
-    '''
+def MeshFileNameBreakdown(fileName, fmat=None, endianness=None):
+    if fmat is None:
+        if fileName.endswith('.ugrid') or fileName.endswith('.ugrid.gz') or \
+                fileName.endswith('.ugrid.bz2'):
+            fmat = 'aflr3'
+        elif fileName.endswith('.cgns') or fileName.endswith('.cgns.gz') or \
+                fileName.endswith('.cgns.bz2'):
+            fmat = 'cgns'
+        else:
+            raise RuntimeError('Unknown format for file {}'.format(fileName))
+
+    if fmat == 'aflr3' and endianness is None:
+        if fileName.find('.b8.') != -1:
+            endianness = 'big'
+        elif fileName.find('.lb8.') != -1:
+            endianness = 'little'
+        else:
+            raise RuntimeError('Unknown endianness for file {}'.format(fileName))
+    else:
+        endianness = ''
 
-    meshInfo = GetMeshInfo(meshId)
-    print(meshInfo)
     compression = ''
-    if meshFile.endswith('.gz'):
+    if fileName.endswith('.gz'):
         compression += 'gz'
-    elif meshFile.endswith('.bz2'):
+    elif fileName.endswith('.bz2'):
         compression += 'bz2'
 
-    fileName = GetMeshFileName(meshInfo['meshName'], meshInfo['meshFormat'],
-                               meshInfo['meshEndianness'], compression)
+    return fmat, endianness, compression
+
+@refreshToken
+def GetRemoteMeshFileName(localMeshFileName=None, meshId=None):
 
-    S3TransferType.VolumeMesh.upload_file(meshId, fileName, meshFile)
+    if localMeshFileName is not None:
+        fmat, endianness, compression = MeshFileNameBreakdown(localMeshFileName)
+        remoteFileName = GetMeshFileName(fmat, endianness, compression)
 
-    CompleteVolumeMeshUpload(meshInfo, fileName)
+        return remoteFileName, fmat, endianness, compression
+    
+    if meshId is not None:
+        remoteFiles = flow360ApiGet(f"volumemeshes/{meshId}/files")
+        remoteFileName = None
+        for file in remoteFiles:
+            try:
+                fmat, endianness, compression = MeshFileNameBreakdown(file['fileName'])
+                return file['fileName'], fmat, endianness, compression
+            except RuntimeError:
+                continue
+
+        if remoteFileName is None:
+            raise RuntimeError(f"No volume mesh file found for id={meshId}")
+        
+    raise ValueError('You need to provide localMeshFileName OR meshId')
+
+
+@refreshToken
+def UploadMesh(meshId, localMeshFileName, remoteMeshFileName):
+    '''
+    UploadMesh(meshId, meshFile)
+    '''
+
+    S3TransferType.VolumeMesh.upload_file(meshId, remoteMeshFileName, localMeshFileName)
+    CompleteVolumeMeshUpload(meshId, remoteMeshFileName)
 
 def DownloadVolumeFile(id, src, target):
     S3TransferType.VolumeMesh.download_file(id, src, target)
 
 @refreshToken
 @deprecated("DownloadMeshGenerationConfigJson()")
 def DownloadMeshConfigJson(id, fileName=None):
@@ -153,43 +195,40 @@
     if fileName is None:
         fileName = os.path.basename(logFileName)
     DownloadVolumeFile(meshId, src=logFileName, target=fileName)
 
 def DownloadMeshingLogs(id, fileName=None):
     DownloadMeshProc(id, fileName)
 
-def GetMeshFileName(meshName, meshFormat, endianness, compression):
+def GetMeshFileName(meshFormat, endianness, compression):
     if meshFormat == 'aflr3':
         if endianness == 'big':
             name = 'mesh.b8.ugrid'
         elif endianness == 'little':
             name = 'mesh.lb8.ugrid'
         else:
             raise RuntimeError("unknown endianness: {}".format(endianness))
     else:
-        name = meshName
-        if not name.endswith('.' + meshFormat):
-            name += '.' + meshFormat
+        name = "volumeMesh" + '.' + meshFormat
 
     if compression is not None and len(compression) > 0:
         name += '.' + compression
     return name
 
 def DownloadVolumeMesh(id, target=None, targetDir=None):
-    meshInfo = GetMeshInfo(id)
-    src = GetMeshFileName(meshInfo['meshName'], meshInfo['meshFormat'],
-                               meshInfo['meshEndianness'], meshInfo['meshCompression'])
+    remoteFileName, _, _, _ = GetRemoteMeshFileName(meshId=id)
+
     if target is None:
-        meshName = os.path.basename(src)
+        meshName = os.path.basename(remoteFileName)
         if targetDir is None:
             target = os.path.join(os.getcwd(), meshName)
         else:
             target = os.path.join(targetDir, meshName)
 
-    DownloadVolumeFile(id, src, target)
+    DownloadVolumeFile(id, remoteFileName, target)
 
 def WaitOnMesh(meshId, timeout=86400, sleepSeconds=10):
     startTime = time.time()
     while time.time() - startTime < timeout:
         try:
             info = GetMeshInfo(meshId)
             if info['meshStatus'] in ['deleted', 'error', 'preerror', 'unknownError', 'processed']:
```

### Comparing `flow360client-22.3.3.0/flow360client/meshUtils.py` & `flow360client-23.2.3.0/flow360client/meshUtils.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,43 +74,63 @@
                 if 'label' not in bcNode.attrs:
                     continue
                 label = bcNode.attrs['label'].decode()
                 if label == 'BC_t':
                     boundaryNamesNoSlash.append(bcName)
     return boundaryNamesNoSlash
 
+def getBase(fh):
+    baseNames = list()
+    for subName in fh.keys():
+        subNode = fh[subName]
+        if 'label' in subNode.attrs.keys() \
+                and subNode.attrs['label'].decode()=='CGNSBase_t':
+            baseNames.append(subName)
+    if len(baseNames) > 1:
+        warnings.warn('The CGNS mesh has more than 1 base node.')
+    return fh[baseNames[0]]
+
 def implGetBoundaryCompoundNamesFromCGNS_v1(meshFile):
     with h5py.File(meshFile, "r") as fh:
-        base = fh['Base']
+        base = getBase(fh)
         zoneNamesRaw = getSubNodeNames(base)
         zoneNames = [zone for zone in zoneNamesRaw 
                      if checkValidZone(base[zone])]
         boundaryCompleteNames = list()
         for zoneName in zoneNames:
             zone = base[zoneName]
             elementSectionNames = getElementsTypeSectionNames(zone)
             for secName in elementSectionNames:
                 section = zone[secName]
                 if Is2DElementSection(section):
                     boundaryCompleteNames.append(zoneName+'/'+secName)
         return boundaryCompleteNames
 
 def implGetBoundaryCompoundNamesFromCGNS_v2(meshFile):
+    zoneBCExist = True
+    zoneInTrouble = None
+    boundaryCompleteNames = list()
     with h5py.File(meshFile, "r") as fh:
-        base = fh['Base']
+        base = getBase(fh)
         zoneNamesRaw = getSubNodeNames(base)
-        zoneNames = [zone for zone in zoneNamesRaw 
+        zoneNames = [zone for zone in zoneNamesRaw
                      if checkValidZone(base[zone])]
-        boundaryCompleteNames = list()
         for zoneName in zoneNames:
             zone = base[zoneName]
             bndNames = getBoundaryNamesFromZoneNoSlash(zone)
+            if len(bndNames) == 0:
+                zoneBCExist = False
+                zoneInTrouble = zoneName
+                break
             for bndName in bndNames:
                 boundaryCompleteNames.append(zoneName+'/'+bndName)
-        return boundaryCompleteNames
+    if not zoneBCExist:
+        warnings.warn(f'No boundary conditions (BCType_t) are defined in the zone: {zoneInTrouble}. Flow360 will treat every 2D element sections in the CGNS mesh as boundaries.')
+        boundaryCompleteNames = implGetBoundaryCompoundNamesFromCGNS_v1(meshFile)
+    return boundaryCompleteNames
 
 def getBoundaryCompoundNamesFromCGNS(meshFile, solverVersion):
     if solverVersion == None:
         return implGetBoundaryCompoundNamesFromCGNS_v2(meshFile)
     elif Flow360Version(solverVersion) < Flow360Version('release-22.2.1.0'):
         return implGetBoundaryCompoundNamesFromCGNS_v1(meshFile)
     else:
@@ -118,15 +138,15 @@
 
 def getNotFoundBoundaries(inputBndNames, availableBndNames):
     return [bnd for bnd in inputBndNames if bnd not in availableBndNames]
 
 def getWallsInCGNSMesh(meshFile):
     walls = list()
     with h5py.File(meshFile, "r") as fh:
-        base = fh['Base']
+        base = getBase(fh)
         zoneNamesRaw = getSubNodeNames(base)
         for zoneName in zoneNamesRaw:
             zone = base[zoneName]
             if 'FamBC_TypeName' in zone:
                 typeNameStr = convertIntDatasetToStr(zone['FamBC_TypeName'][' data'])
                 if typeNameStr == 'Wall' or 'Wall Viscous' in typeNameStr:
                     walls.append(zoneName)
```

### Comparing `flow360client-22.3.3.0/flow360client/s3utils.py` & `flow360client-23.2.3.0/flow360client/s3utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,15 @@
             region_name=Config.AWS_REGION,
             aws_access_key_id=self.user_credential.access_key_id,
             aws_secret_access_key=self.user_credential.secret_access_key,
             aws_session_token=self.user_credential.session_token,
         )
 
     def is_expired(self):
-        return (self.user_credential.expiration - datetime.now(
-            tz=self.user_credential.expiration.tzinfo)).total_seconds() > 300
+        return (self.user_credential.expiration.replace(tzinfo=None) - datetime.utcnow()).total_seconds() > 300
 
 
 class S3TransferType(Enum):
     VolumeMesh = "VolumeMesh"
     SurfaceMesh = "SurfaceMesh"
     Case = "Case"
     Studio = "Studio"
```

### Comparing `flow360client-22.3.3.0/flow360client/studio.py` & `flow360client-23.2.3.0/flow360client/studio.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/surfaceMesh.py` & `flow360client-23.2.3.0/flow360client/surfaceMesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,17 +65,15 @@
     url = f"surfacemeshes/{meshId}/completeUpload?fileName={fileName}"
     resp = flow360ApiPost(url)
     return resp
 
 
 @refreshToken
 def ListSurfaceMeshes(include_deleted=False):
-    resp = flow360ApiGet("surfacemeshes")
-    if not include_deleted:
-        resp = list(filter(lambda i: i['status'] != 'deleted', resp))
+    resp = flow360ApiGet("surfacemeshes", params={"includeDeleted": include_deleted})
     return resp
 
 
 @refreshToken
 def UploadGeometry(surfaceMeshId, geoFile):
     '''
     Upload for files other than surface mesh
```

### Comparing `flow360client-22.3.3.0/flow360client/task.py` & `flow360client-23.2.3.0/flow360client/task.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/validation.py` & `flow360client-23.2.3.0/flow360client/validation.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client/version.py` & `flow360client-23.2.3.0/flow360client/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '22.3.3.0'
+__version__ = '23.2.3.0'
 
 import re
 class Flow360Version:
     def __init__(self, version):
         self.full = version
         ret = re.findall('^([a-zA-Z0-9\-]+)-([0-9\.]+)$', version)
         if len(ret) != 1:
```

### Comparing `flow360client-22.3.3.0/flow360client/versionCheck.py` & `flow360client-23.2.3.0/flow360client/versionCheck.py`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/flow360client.egg-info/SOURCES.txt` & `flow360client-23.2.3.0/flow360client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flow360client-22.3.3.0/setup.py` & `flow360client-23.2.3.0/setup.py`

 * *Files identical despite different names*

