# Comparing `tmp/hyperx-0.1.1.tar.gz` & `tmp/hyperx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperx-0.1.1.tar", last modified: Thu Jul  6 15:54:45 2023, max compression
+gzip compressed data, was "hyperx-0.1.2.tar", last modified: Mon Jul 10 15:33:58 2023, max compression
```

## Comparing `hyperx-0.1.1.tar` & `hyperx-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.803233 hyperx-0.1.1/
--rw-rw-rw-   0        0        0      535 2023-07-06 15:54:45.802233 hyperx-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.767609 hyperx-0.1.1/hyperx/
--rw-rw-rw-   0        0        0      747 2023-06-29 20:58:54.000000 hyperx-0.1.1/hyperx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.789003 hyperx-0.1.1/hyperx/api/
--rw-rw-rw-   0        0        0   145708 2023-07-06 15:54:30.000000 hyperx-0.1.1/hyperx/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.791234 hyperx-0.1.1/hyperx/api/types/
--rw-rw-rw-   0        0        0    24178 2023-06-29 20:33:40.000000 hyperx-0.1.1/hyperx/api/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.797234 hyperx-0.1.1/hyperx/library/
--rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-0.1.1/hyperx/library/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-0.1.1/hyperx/library/find.py
--rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-0.1.1/hyperx/library/library.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.800233 hyperx-0.1.1/hyperx/utils/
--rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-0.1.1/hyperx/utils/__init__.py
--rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-0.1.1/hyperx/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.786194 hyperx-0.1.1/hyperx.egg-info/
--rw-rw-rw-   0        0        0      535 2023-07-06 15:54:45.000000 hyperx-0.1.1/hyperx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-07-06 15:54:45.000000 hyperx-0.1.1/hyperx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 15:54:45.000000 hyperx-0.1.1/hyperx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-06 15:54:45.000000 hyperx-0.1.1/hyperx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 15:54:45.000000 hyperx-0.1.1/hyperx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      660 2023-07-06 15:19:27.000000 hyperx-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 15:54:45.803233 hyperx-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.428981 hyperx-0.1.2/
+-rw-rw-rw-   0        0        0      535 2023-07-10 15:33:58.428036 hyperx-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.352293 hyperx-0.1.2/hyperx/
+-rw-rw-rw-   0        0        0      747 2023-06-29 20:58:54.000000 hyperx-0.1.2/hyperx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.401576 hyperx-0.1.2/hyperx/api/
+-rw-rw-rw-   0        0        0   145840 2023-07-10 15:31:55.000000 hyperx-0.1.2/hyperx/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.405943 hyperx-0.1.2/hyperx/api/types/
+-rw-rw-rw-   0        0        0    24178 2023-07-10 15:31:23.000000 hyperx-0.1.2/hyperx/api/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.417962 hyperx-0.1.2/hyperx/library/
+-rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-0.1.2/hyperx/library/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-0.1.2/hyperx/library/find.py
+-rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-0.1.2/hyperx/library/library.py
+drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.424990 hyperx-0.1.2/hyperx/utils/
+-rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-0.1.2/hyperx/utils/__init__.py
+-rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-0.1.2/hyperx/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.397573 hyperx-0.1.2/hyperx.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-07-10 15:33:58.000000 hyperx-0.1.2/hyperx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-07-10 15:33:58.000000 hyperx-0.1.2/hyperx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 15:33:58.000000 hyperx-0.1.2/hyperx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-10 15:33:58.000000 hyperx-0.1.2/hyperx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 15:33:58.000000 hyperx-0.1.2/hyperx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      660 2023-07-10 15:30:01.000000 hyperx-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 15:33:58.429983 hyperx-0.1.2/setup.cfg
```

### Comparing `hyperx-0.1.1/PKG-INFO` & `hyperx-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 0.1.1
+Version: 0.1.2
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `hyperx-0.1.1/hyperx/__init__.py` & `hyperx-0.1.2/hyperx/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.1/hyperx/api/__init__.py` & `hyperx-0.1.2/hyperx/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4860,23 +4860,14 @@
 	def SetToRange(self, min: float, max: float) -> None:
 		return self._Entity.SetToRange(min, max)
 
 	def SetToValue(self, value: float) -> None:
 		return self._Entity.SetToValue(value)
 
 
-class DesignVariableMaterial:
-	def __init__(self, designVariableMaterial: _api.DesignVariableMaterial):
-		self._Entity = designVariableMaterial
-
-	@property
-	def MaterialId(self) -> int:
-		return self._Entity.MaterialId
-
-
 class DesignVariable(IdEntity):
 	def __init__(self, designVariable: _api.DesignVariable):
 		self._Entity = designVariable
 
 	@property
 	def AllowMaterials(self) -> bool:
 		return self._Entity.AllowMaterials
@@ -4917,19 +4908,27 @@
 	def UseAnalysis(self, value: bool) -> None:
 		self._Entity.UseAnalysis = value
 
 	def AddMaterials(self, materialIds: list[int]) -> None:
 		materialIdsList = MakeCSharpIntList(materialIds)
 		return self._Entity.AddMaterials(materialIdsList)
 
-	def GetMaterials(self) -> list[DesignVariableMaterial]:
-		return list[DesignVariableMaterial](self._Entity.GetMaterials())
+	def GetSizingMaterials(self) -> list[int]:
+		return list[int](self._Entity.GetSizingMaterials())
+
+	def GetAnalysisMaterial(self) -> int:
+		return self._Entity.GetAnalysisMaterial()
+
+	def RemoveSizingMaterials(self, materialIds: tuple[int] = None) -> None:
+		materialIdsList = MakeCSharpIntList(materialIds)
+		materialIdsEnumerable = IEnumerable(materialIdsList)
+		return self._Entity.RemoveSizingMaterials(materialIds if materialIds is None else materialIdsEnumerable)
 
-	def RemoveAllMaterials(self) -> None:
-		return self._Entity.RemoveAllMaterials()
+	def RemoveAnalysisMaterial(self) -> None:
+		return self._Entity.RemoveAnalysisMaterial()
 
 
 class ToolingConstraintCol(IdNameEntityCol[ToolingConstraint]):
 	def __init__(self, toolingConstraintCol: _api.ToolingConstraintCol):
 		self._Entity = toolingConstraintCol
 		self._CollectedClass = ToolingConstraint
```

### Comparing `hyperx-0.1.1/hyperx/api/types/__init__.py` & `hyperx-0.1.2/hyperx/api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.1/hyperx/library/find.py` & `hyperx-0.1.2/hyperx/library/find.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.1/hyperx/library/library.py` & `hyperx-0.1.2/hyperx/library/library.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.1/hyperx/utils/utils.py` & `hyperx-0.1.2/hyperx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.1/hyperx.egg-info/PKG-INFO` & `hyperx-0.1.2/hyperx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 0.1.1
+Version: 0.1.2
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `hyperx-0.1.1/pyproject.toml` & `hyperx-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hyperx"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Kelly Ann Smith", email="kellyann.smith@collieraerospace.com" },
   { name="Noah Prezant", email="noah.prezant@collieraerospace.com" },
 ]
 description = "HyperX scripting for Python"
 readme = "README.md"
 requires-python = ">=3.10"
```

