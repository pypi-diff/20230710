# Comparing `tmp/spatial_transform-1.2.8.tar.gz` & `tmp/spatial_transform-1.2.9.tar.gz`

## Comparing `spatial_transform-1.2.8.tar` & `spatial_transform-1.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/.flake8
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/changelog.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/requirements.txt
--rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/test.ipynb
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/.github/workflows/publish_main.yml
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/.github/workflows/publish_preview.yml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/SpatialTransform/__init__.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/SpatialTransform/lib/euler.py
--rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/SpatialTransform/lib/pose.py
--rw-r--r--   0        0        0    17990 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/SpatialTransform/lib/transform.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/SpatialTransform/tests/test_euler.py
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/SpatialTransform/tests/test_hierarchy.py
--rw-r--r--   0        0        0     8601 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/SpatialTransform/tests/test_methods.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/SpatialTransform/tests/test_properties.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/SpatialTransform/tests/utils.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/LICENSE
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     8008 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/readme.md
--rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 spatial_transform-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/.flake8
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/changelog.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/requirements.txt
+-rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/test.ipynb
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/.github/workflows/publish_main.yml
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/.github/workflows/publish_preview.yml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/SpatialTransform/__init__.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/SpatialTransform/lib/euler.py
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/SpatialTransform/lib/pose.py
+-rw-r--r--   0        0        0    17352 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/SpatialTransform/lib/transform.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/SpatialTransform/tests/test_euler.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/SpatialTransform/tests/test_hierarchy.py
+-rw-r--r--   0        0        0     8601 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/SpatialTransform/tests/test_methods.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/SpatialTransform/tests/test_properties.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/SpatialTransform/tests/utils.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/LICENSE
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     8008 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/readme.md
+-rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 spatial_transform-1.2.9/PKG-INFO
```

### Comparing `spatial_transform-1.2.8/test.ipynb` & `spatial_transform-1.2.9/test.ipynb`

 * *Files identical despite different names*

### Comparing `spatial_transform-1.2.8/.github/workflows/publish_main.yml` & `spatial_transform-1.2.9/.github/workflows/publish_main.yml`

 * *Files identical despite different names*

### Comparing `spatial_transform-1.2.8/.github/workflows/publish_preview.yml` & `spatial_transform-1.2.9/.github/workflows/publish_preview.yml`

 * *Files identical despite different names*

### Comparing `spatial_transform-1.2.8/SpatialTransform/lib/euler.py` & `spatial_transform-1.2.9/SpatialTransform/lib/euler.py`

 * *Files identical despite different names*

### Comparing `spatial_transform-1.2.8/SpatialTransform/lib/pose.py` & `spatial_transform-1.2.9/SpatialTransform/lib/pose.py`

 * *Files identical despite different names*

### Comparing `spatial_transform-1.2.8/SpatialTransform/lib/transform.py` & `spatial_transform-1.2.9/SpatialTransform/lib/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -221,102 +221,86 @@
         - If keep contains properties -> the property is modified to keep its spatial algiment in world space.
         - If keep is None or empty -> Local space propteries do not change.
         Returns itself."""
         if (len(self.Children) > 0):
             self.detach(*self.Children, keep=keep)
         return self
 
-    def applyPosition(self, position: glm.vec3 = None, recursive: bool = False, includeParentChange: list[Pose] = [], includeChildrenChange: list[Pose] = []) -> "Transform":
-        """Changes the position of this transform and updates its children to keep them spatial unchanged.
-        - If position is None -> the transform resets its position to (0, 0, 0).
-        - If position IS set -> the given position is added to the current position.
-        - If includeParentChange contains poses -> Those poses recieve the same change as this transfrom.
-        - If includeChildChange contains poses -> Those poses recieve the same change as the children.
-        Returns itself."""
-        # define positional change
+    def __applyPositionChange(self, position: glm.vec3 = None) -> tuple[glm.vec3, glm.vec3]:
         change = -self.Position if position is None else position
         changeInverse = glm.inverse(self.Rotation) * ((1.0 / self.Scale) * -change)
+        return (change, changeInverse)
 
-        # apply changes to itself
+    def __applyPositionSelf(self, change: glm.vec3, changeInverse: glm.vec3):
         self.Position = self.Position + change
-
-        # apply changes to children
         for child in self.Children:
             child.Position = child.Position + changeInverse
 
-            # may do it recursively
-            if recursive: child.applyPosition(position, recursive=True)
+    def applyPosition(self, position: glm.vec3 = None, recursive: bool = False) -> "Transform":
+        """Changes the position of this transform and updates its children to keep them spatial unchanged.
+        - If position is None -> the transform resets its position to (0, 0, 0).
+        - If position IS set -> the given position is added to the current position.
+        Returns itself."""
+        self.__applyPositionSelf(*self.__applyPositionChange(position))
 
-        # apply to additionals
-        for item in includeParentChange:
-            item.Position = item.Position + change
-        for item in includeChildrenChange:
-            item.Position = item.Position + changeInverse
+        if recursive:
+            for child in self.Children:
+                child.applyPosition(position=position, recursive=True)
 
         return self
 
-    def applyRotation(self, rotation: glm.quat = None, recursive: bool = False, includeParentChange: list[Pose] = [], includeChildrenChange: list[Pose] = []) -> "Transform":
-        """Changes the rotation of this transform and updates its children to keep them spatial unchanged.
-        - If rotation is None -> the transform resets its rotation to (1, 0, 0, 0).
-        - If rotation IS set -> the given rotation is added to the current rotation.
-        - If includeParentChange contains poses -> Those poses recieve the same change as this transfrom.
-        - If includeChildChange contains poses -> Those poses recieve the same change as the children.
-        Returns itself."""
-        # define rotational change
+    def __applyRotationChange(self, rotation: glm.quat = None) -> tuple[glm.quat, glm.quat]:
         change = glm.inverse(self.Rotation) if rotation is None else rotation
         changeInverse = glm.inverse(change)
+        return (change, changeInverse)
 
-        # apply changes to itself
+    def __applyRotationSelf(self, change: glm.quat, changeInverse: glm.quat, bake: bool = False):
         self.Rotation = self.Rotation * change
-
-        # apply changes to children
         for child in self.Children:
             child.Position = changeInverse * child.Position
-            child.Rotation = changeInverse * child.Rotation
+            if not bake:
+                child.Rotation = changeInverse * child.Rotation
 
-            # may do it recursively
-            if recursive: child.applyRotation(rotation, recursive=True)
+    def applyRotation(self, rotation: glm.quat = None, recursive: bool = False, bake: bool = False) -> "Transform":
+        """Changes the rotation of this transform and updates its children to keep them spatial unchanged.
+        - If rotation is None -> the transform resets its rotation to (1, 0, 0, 0).
+        - If rotation IS set -> the given rotation is added to the current rotation.
+        - If bake Is True -> The rotation correction is NOT passed to the children, only positions will be modified.
+        Returns itself."""
+        self.__applyRotationSelf(*self.__applyRotationChange(rotation), bake=bake)
 
-        # apply to additionals
-        for item in includeParentChange:
-            item.Rotation = item.Rotation * change
-        for item in includeChildrenChange:
-            item.Position = changeInverse * item.Position
-            item.Rotation = changeInverse * item.Rotation
+        if recursive:
+            for child in self.Children:
+                child.applyRotation(rotation=rotation, recursive=True, bake=bake)
 
         return self
 
-    def applyScale(self, scale: glm.vec3 = None, recursive: bool = False, includeParentChange: list[Pose] = [], includeChildrenChange: list[Pose] = []) -> "Transform":
-        """Changes the scale of the transform and updates its children to keep them spatial unchanged.
-        - If scale is NOT set -> the transform resets its scale to (1, 1, 1).
-        - If scale IS set -> the given scale is added to the current scale.
-        - If includeParentChange contains poses -> Those poses recieve the same change as this transfrom.
-        - If includeChildChange contains poses -> Those poses recieve the same change as the children.
-        Returns itself."""
-        # define change in scale
+    def __applyScaleChange(self, scale: glm.vec3 = None) -> tuple[glm.vec3, glm.vec3]:
         change = (1.0 / self.Scale) if scale is None else scale
         changeInverse = (1.0 / change)
+        return (change, changeInverse)
 
-        # apply changes to itself
+    def __applyScaleSelf(self, change: glm.vec3, changeInverse: glm.vec3, bake: bool = False):
         self.Scale = self.Scale * change
-
-        # keep space for children
         for child in self.Children:
             child.Position = changeInverse * child.Position
-            child.Scale = changeInverse * child.Scale
+            if not bake:
+                child.Scale = changeInverse * child.Scale
 
-            # may do it recursively
-            if recursive: child.applyScale(scale, recursive=True)
+    def applyScale(self, scale: glm.vec3 = None, recursive: bool = False, bake: bool = False) -> "Transform":
+        """Changes the scale of the transform and updates its children to keep them spatial unchanged.
+        - If scale is NOT set -> The transform resets its scale to (1, 1, 1).
+        - If scale IS set -> The given scale is added to the current scale.
+        - If bake Is True -> The scale correction is NOT passed to the children, only positions will be modified.
+        Returns itself."""
+        self.__applyScaleSelf(*self.__applyScaleChange(scale), bake=bake)
 
-        # apply to additionals
-        for item in includeParentChange:
-            item.Scale = item.Scale * change
-        for item in includeChildrenChange:
-            item.Position = changeInverse * item.Position
-            item.Scale = changeInverse * item.Scale
+        if recursive:
+            for child in self.Children:
+                child.applyScale(scale=scale, recursive=True, bake=bake)
 
         return self
 
     def layout(self, index: int = 0, depth: int = 0) -> list[tuple["Transform", int, int]]:
         """Returns the hierarchy, inclunding this transform, in order of 'depth first' with their index and depth.
         - Order of the tuple -> [transform, index, depth]"""
         result = [[self, index, depth]]
```

### Comparing `spatial_transform-1.2.8/SpatialTransform/tests/test_euler.py` & `spatial_transform-1.2.9/SpatialTransform/tests/test_euler.py`

 * *Files identical despite different names*

### Comparing `spatial_transform-1.2.8/SpatialTransform/tests/test_hierarchy.py` & `spatial_transform-1.2.9/SpatialTransform/tests/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `spatial_transform-1.2.8/SpatialTransform/tests/test_methods.py` & `spatial_transform-1.2.9/SpatialTransform/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `spatial_transform-1.2.8/SpatialTransform/tests/test_properties.py` & `spatial_transform-1.2.9/SpatialTransform/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `spatial_transform-1.2.8/SpatialTransform/tests/utils.py` & `spatial_transform-1.2.9/SpatialTransform/tests/utils.py`

 * *Files identical despite different names*

### Comparing `spatial_transform-1.2.8/LICENSE` & `spatial_transform-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial_transform-1.2.8/pyproject.toml` & `spatial_transform-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 dynamic = ["dependencies"]
 name = "spatial-transform"
-version = "1.2.8"
+version = "1.2.9"
 authors = [ { name="Wasserwecken", email="author@example.com" }, ]
 description = "Libary for creating spatial space hierarchies"
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `spatial_transform-1.2.8/readme.md` & `spatial_transform-1.2.9/readme.md`

 * *Files identical despite different names*

### Comparing `spatial_transform-1.2.8/PKG-INFO` & `spatial_transform-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatial-transform
-Version: 1.2.8
+Version: 1.2.9
 Summary: Libary for creating spatial space hierarchies
 Project-URL: Homepage, https://github.com/Wasserwecken/spatial-transform
 Project-URL: Bug Tracker, https://github.com/Wasserwecken/spatial-transform/issues
 Author-email: Wasserwecken <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spatial-transform Version: 1.2.8 Summary: Libary
+Metadata-Version: 2.1 Name: spatial-transform Version: 1.2.9 Summary: Libary
 for creating spatial space hierarchies Project-URL: Homepage, https://
 github.com/Wasserwecken/spatial-transform Project-URL: Bug Tracker, https://
 github.com/Wasserwecken/spatial-transform/issues Author-email: Wasserwecken
 example.com> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-Type: text/
 markdown [![PyPI version](https://badge.fury.io/py/spatial-transform.svg)]
```

