# Comparing `tmp/femwell-0.1.3.tar.gz` & `tmp/femwell-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femwell-0.1.3.tar", max compression
+gzip compressed data, was "femwell-0.1.4.tar", max compression
```

## Comparing `femwell-0.1.3.tar` & `femwell-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-06-27 11:49:31.818492 femwell-0.1.3/LICENSE
--rw-r--r--   0        0        0     2480 2023-06-27 11:49:31.818492 femwell-0.1.3/README.md
--rw-r--r--   0        0        0      255 2023-06-27 11:49:31.822492 femwell-0.1.3/femwell/__init__.py
--rw-r--r--   0        0        0     3080 2023-06-27 11:49:31.822492 femwell-0.1.3/femwell/culomb.py
--rw-r--r--   0        0        0    10175 2023-06-27 11:49:31.822492 femwell-0.1.3/femwell/eme.py.bak
--rw-r--r--   0        0        0        0 2023-06-27 11:49:31.822492 femwell-0.1.3/femwell/examples/__init__.py
--rw-r--r--   0        0        0     4820 2023-06-27 11:49:31.822492 femwell-0.1.3/femwell/examples/coplanar_waveguide.py
--rw-r--r--   0        0        0     5762 2023-06-27 11:49:31.822492 femwell-0.1.3/femwell/fefd.py
--rw-r--r--   0        0        0     1304 2023-06-27 11:49:31.822492 femwell-0.1.3/femwell/fiber.py
--rw-r--r--   0        0        0     1782 2023-06-27 11:49:31.822492 femwell-0.1.3/femwell/laplace.py
--rw-r--r--   0        0        0    17333 2023-06-27 11:49:31.822492 femwell-0.1.3/femwell/maxwell/waveguide.py
--rw-r--r--   0        0        0      224 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/mesh/__init__.py
--rw-r--r--   0        0        0    26893 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/mesh/mesh.py
--rw-r--r--   0        0        0     7713 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/mesh/meshtracker.py
--rw-r--r--   0        0        0     9318 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/mesh/slice.py
--rw-r--r--   0        0        0    21359 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/mesh.py
--rw-r--r--   0        0        0     1033 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/mode_solver_1d.py
--rw-r--r--   0        0        0     2922 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/mode_solver_2d_periodic.py
--rw-r--r--   0        0        0     6950 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/mode_solver_2d_periodic_quadratic.py
--rw-r--r--   0        0        0     4224 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/mode_solver_inplane.py
--rw-r--r--   0        0        0     1243 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/mode_solver_schrodinger.py
--rw-r--r--   0        0        0     8799 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/pn_analytical.py
--rw-r--r--   0        0        0     6453 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/solver.py
--rw-r--r--   0        0        0     5897 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/tcad.py
--rw-r--r--   0        0        0     2820 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/tests/test_mesh.py
--rw-r--r--   0        0        0     5880 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/thermal.py
--rw-r--r--   0        0        0     8803 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/thermal_transient.py
--rw-r--r--   0        0        0     2655 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/utils.py
--rw-r--r--   0        0        0     1123 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/visualization.py
--rw-r--r--   0        0        0     2089 2023-06-27 11:49:31.826492 femwell-0.1.3/femwell/waveguide.py
--rw-r--r--   0        0        0      974 2023-06-27 11:49:47.046522 femwell-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 femwell-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-10 14:54:59.990798 femwell-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2480 2023-07-10 14:54:59.990798 femwell-0.1.4/README.md
+-rw-r--r--   0        0        0      255 2023-07-10 14:54:59.990798 femwell-0.1.4/femwell/__init__.py
+-rw-r--r--   0        0        0     3080 2023-07-10 14:54:59.990798 femwell-0.1.4/femwell/culomb.py
+-rw-r--r--   0        0        0    10175 2023-07-10 14:54:59.990798 femwell-0.1.4/femwell/eme.py.bak
+-rw-r--r--   0        0        0        0 2023-07-10 14:54:59.990798 femwell-0.1.4/femwell/examples/__init__.py
+-rw-r--r--   0        0        0     4820 2023-07-10 14:54:59.990798 femwell-0.1.4/femwell/examples/coplanar_waveguide.py
+-rw-r--r--   0        0        0     5762 2023-07-10 14:54:59.990798 femwell-0.1.4/femwell/fefd.py
+-rw-r--r--   0        0        0     3173 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/fefd_2d.py
+-rw-r--r--   0        0        0     1304 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/fiber.py
+-rw-r--r--   0        0        0     1782 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/laplace.py
+-rw-r--r--   0        0        0    17333 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/maxwell/waveguide.py
+-rw-r--r--   0        0        0      224 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mesh/__init__.py
+-rw-r--r--   0        0        0    26893 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mesh/mesh.py
+-rw-r--r--   0        0        0     7900 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mesh/meshtracker.py
+-rw-r--r--   0        0        0     9318 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mesh/slice.py
+-rw-r--r--   0        0        0    21359 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mesh.py
+-rw-r--r--   0        0        0     1033 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mode_solver_1d.py
+-rw-r--r--   0        0        0     2922 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mode_solver_2d_periodic.py
+-rw-r--r--   0        0        0     6950 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mode_solver_2d_periodic_quadratic.py
+-rw-r--r--   0        0        0     4224 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mode_solver_inplane.py
+-rw-r--r--   0        0        0     1243 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/mode_solver_schrodinger.py
+-rw-r--r--   0        0        0     8799 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/pn_analytical.py
+-rw-r--r--   0        0        0     6453 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/solver.py
+-rw-r--r--   0        0        0     5897 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/tcad.py
+-rw-r--r--   0        0        0     2820 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/tests/test_mesh.py
+-rw-r--r--   0        0        0     5880 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/thermal.py
+-rw-r--r--   0        0        0     8803 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/thermal_transient.py
+-rw-r--r--   0        0        0     2655 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/utils.py
+-rw-r--r--   0        0        0     1123 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/visualization.py
+-rw-r--r--   0        0        0     2089 2023-07-10 14:54:59.994798 femwell-0.1.4/femwell/waveguide.py
+-rw-r--r--   0        0        0      974 2023-07-10 14:55:11.575044 femwell-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 femwell-0.1.4/PKG-INFO
```

### Comparing `femwell-0.1.3/LICENSE` & `femwell-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/README.md` & `femwell-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/culomb.py` & `femwell-0.1.4/femwell/culomb.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/eme.py.bak` & `femwell-0.1.4/femwell/eme.py.bak`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/examples/coplanar_waveguide.py` & `femwell-0.1.4/femwell/examples/coplanar_waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/fefd.py` & `femwell-0.1.4/femwell/fefd.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/fiber.py` & `femwell-0.1.4/femwell/fiber.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/laplace.py` & `femwell-0.1.4/femwell/laplace.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/maxwell/waveguide.py` & `femwell-0.1.4/femwell/maxwell/waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/mesh/mesh.py` & `femwell-0.1.4/femwell/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/mesh/meshtracker.py` & `femwell-0.1.4/femwell/mesh/meshtracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,32 +126,35 @@
                 shapely.geometry.LineString([shapely_xy_point1, shapely_xy_point2])
             )
             self.gmsh_xy_segments.append(gmsh_segment)
             self.xy_segments_main_labels.append(label)
             self.xy_segments_secondary_labels.append(None)
         return gmsh_segment, orientation
 
-    def add_get_xy_line(self, shapely_xy_curve, label):
+    def add_get_xy_line(self, shapely_xy_curves, label):
         """
         Add a shapely line (multi-point line) to the gmsh model in the xy plane, or retrieve the existing gmsh segment with equivalent coordinates (within tol.)
 
         Args:
-            shapely_xy_curve (shapely.geometry.LineString): curve
+            shapely_xy_curves (shapely.geometry.LineString): curve
         """
         segments = []
-        for shapely_xy_point1, shapely_xy_point2 in zip(
-            shapely_xy_curve.coords[:-1], shapely_xy_curve.coords[1:]
+        for shapely_xy_curve in (
+            shapely_xy_curves.geoms if hasattr(shapely_xy_curves, "geoms") else [shapely_xy_curves]
         ):
-            gmsh_segment, orientation = self.add_get_xy_segment(
-                Point(shapely_xy_point1), Point(shapely_xy_point2), label
-            )
-            if orientation:
-                segments.append(gmsh_segment)
-            else:
-                segments.append(-gmsh_segment)
+            for shapely_xy_point1, shapely_xy_point2 in zip(
+                shapely_xy_curve.coords[:-1], shapely_xy_curve.coords[1:]
+            ):
+                gmsh_segment, orientation = self.add_get_xy_segment(
+                    Point(shapely_xy_point1), Point(shapely_xy_point2), label
+                )
+                if orientation:
+                    segments.append(gmsh_segment)
+                else:
+                    segments.append(-gmsh_segment)
         self.model.add_physical(segments, f"{label}")
 
     def add_xy_surface(self, shapely_xy_polygons, label=None, physical=True):
         """
         Add a xy surface corresponding to shapely_xy_polygon, or retrieve the existing gmsh model surface with equivalent coordinates (within tol.)
 
         Args:
```

### Comparing `femwell-0.1.3/femwell/mesh/slice.py` & `femwell-0.1.4/femwell/mesh/slice.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/mesh.py` & `femwell-0.1.4/femwell/mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/mode_solver_1d.py` & `femwell-0.1.4/femwell/mode_solver_1d.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/mode_solver_2d_periodic.py` & `femwell-0.1.4/femwell/mode_solver_2d_periodic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/mode_solver_2d_periodic_quadratic.py` & `femwell-0.1.4/femwell/mode_solver_2d_periodic_quadratic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/mode_solver_inplane.py` & `femwell-0.1.4/femwell/mode_solver_inplane.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/mode_solver_schrodinger.py` & `femwell-0.1.4/femwell/mode_solver_schrodinger.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/pn_analytical.py` & `femwell-0.1.4/femwell/pn_analytical.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/solver.py` & `femwell-0.1.4/femwell/solver.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/tcad.py` & `femwell-0.1.4/femwell/tcad.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/tests/test_mesh.py` & `femwell-0.1.4/femwell/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/thermal.py` & `femwell-0.1.4/femwell/thermal.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/thermal_transient.py` & `femwell-0.1.4/femwell/thermal_transient.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/utils.py` & `femwell-0.1.4/femwell/utils.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/visualization.py` & `femwell-0.1.4/femwell/visualization.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/femwell/waveguide.py` & `femwell-0.1.4/femwell/waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.3/pyproject.toml` & `femwell-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "femwell"
-version = "0.1.3"
+version = "0.1.4"
 authors = ["Helge Gehring"]
 description = "Mode solver for photonic and electric waveguides based on FEM"
 homepage = "https://github.com/HelgeGehring/femwell"
 keywords = [
     "integrated photonics",
     "silicon photonics",
     "mode solving",
```

### Comparing `femwell-0.1.3/PKG-INFO` & `femwell-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femwell
-Version: 0.1.3
+Version: 0.1.4
 Summary: Mode solver for photonic and electric waveguides based on FEM
 Home-page: https://github.com/HelgeGehring/femwell
 License: GPLv3
 Keywords: integrated photonics,silicon photonics,mode solving,finite element analysis
 Author: Helge Gehring
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
```

