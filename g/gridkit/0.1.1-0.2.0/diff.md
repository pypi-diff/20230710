# Comparing `tmp/gridkit-0.1.1.tar.gz` & `tmp/gridkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridkit-0.1.1.tar", last modified: Fri Mar 17 19:26:42 2023, max compression
+gzip compressed data, was "gridkit-0.2.0.tar", last modified: Sun Jul  9 22:22:54 2023, max compression
```

## Comparing `gridkit-0.1.1.tar` & `gridkit-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:26:42.363365 gridkit-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-17 19:26:29.000000 gridkit-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-17 19:26:42.363365 gridkit-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-17 19:26:29.000000 gridkit-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:26:42.359365 gridkit-0.1.1/gridkit/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-17 19:26:29.000000 gridkit-0.1.1/gridkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-03-17 19:26:29.000000 gridkit-0.1.1/gridkit/_statistical_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-03-17 19:26:29.000000 gridkit-0.1.1/gridkit/base_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-03-17 19:26:29.000000 gridkit-0.1.1/gridkit/bounded_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-17 19:26:29.000000 gridkit-0.1.1/gridkit/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-17 19:26:29.000000 gridkit-0.1.1/gridkit/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    26504 2023-03-17 19:26:29.000000 gridkit-0.1.1/gridkit/rect_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-17 19:26:41.000000 gridkit-0.1.1/gridkit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:26:42.359365 gridkit-0.1.1/gridkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-17 19:26:42.000000 gridkit-0.1.1/gridkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-17 19:26:42.000000 gridkit-0.1.1/gridkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 19:26:42.000000 gridkit-0.1.1/gridkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-17 19:26:42.000000 gridkit-0.1.1/gridkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-17 19:26:42.000000 gridkit-0.1.1/gridkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 19:26:42.363365 gridkit-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-17 19:26:29.000000 gridkit-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:22:54.888889 gridkit-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-09 22:22:46.000000 gridkit-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-09 22:22:54.888889 gridkit-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-09 22:22:46.000000 gridkit-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:22:54.888889 gridkit-0.2.0/gridkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/_statistical_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/base_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/bounded_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27996 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/hex_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27382 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/rect_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 22:22:54.000000 gridkit-0.2.0/gridkit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:22:54.888889 gridkit-0.2.0/gridkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-09 22:22:54.000000 gridkit-0.2.0/gridkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-09 22:22:54.000000 gridkit-0.2.0/gridkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:22:54.000000 gridkit-0.2.0/gridkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-09 22:22:54.000000 gridkit-0.2.0/gridkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 22:22:54.000000 gridkit-0.2.0/gridkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:22:54.888889 gridkit-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-09 22:22:46.000000 gridkit-0.2.0/setup.py
```

### Comparing `gridkit-0.1.1/LICENSE.txt` & `gridkit-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gridkit-0.1.1/README.md` & `gridkit-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 GridKit
 =======
 
 GridKit is a tool to work with grids on a high abstraction level.
 
+[![Downloads](https://static.pepy.tech/personalized-badge/gridkit?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/gridkit)
+[![Downloads](https://badge.fury.io/py/gridkit.svg)](https://pypi.org/project/gridkit/)
+
 Documentation
 =============
 Find the docs on [GitHub Pages](https://tmillenaar.github.io/GridKit).
 
 Examples
 ========
 Find the examples in the [Example Gallery](https://tmillenaar.github.io/GridKit/example_gallery/index.html) section of the documentation.
```

### Comparing `gridkit-0.1.1/gridkit/_statistical_functions.py` & `gridkit-0.2.0/gridkit/_statistical_functions.py`

 * *Files identical despite different names*

### Comparing `gridkit-0.1.1/gridkit/bounded_grid.py` & `gridkit-0.2.0/gridkit/bounded_grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import operator
 import abc
 import warnings
 import functools
 
 import gridkit
 from gridkit.base_grid import BaseGrid
-from gridkit.errors import AlignmentError
+from gridkit.errors import IntersectionError, AlignmentError
 
 class _BoundedGridMeta(type):
     """metaclass of the Raster class"""
 
     def __new__(cls, name, bases, namespace):
 
         # operators with a nan-base
@@ -359,22 +359,33 @@
         if not self._data.shape == mask.shape:
             raise ValueError(f"Mask shape {mask.shape} does not match data shape {self._data.shape}")
 
         ids, shape = self.cells_in_bounds(self.bounds)
         ids = ids.reshape([*shape, 2])
         return ids[mask]
 
-
-    @abc.abstractmethod
     def shared_bounds(self, other):
-        pass
-        
-    @abc.abstractmethod
+        other_bounds = other.bounds if isinstance(other, BaseGrid) else other
+        if not self.intersects(other):
+            raise IntersectionError(f"Grid with bounds {self.bounds} does not intersect with grid with bounds {other_bounds}.")
+        return (
+            max(self.bounds[0], other_bounds[0]),
+            max(self.bounds[1], other_bounds[1]),
+            min(self.bounds[2], other_bounds[2]),
+            min(self.bounds[3], other_bounds[3]),
+        )
+
     def combined_bounds(self, other):
-        pass
+        other_bounds = other.bounds if isinstance(other, BaseGrid) else other
+        return (
+            min(self.bounds[0], other_bounds[0]),
+            min(self.bounds[1], other_bounds[1]),
+            max(self.bounds[2], other_bounds[2]),
+            max(self.bounds[3], other_bounds[3]),
+        )
 
     @abc.abstractmethod
     def crop(self, new_bounds, bounds_crs=None):
         pass
 
     @abc.abstractmethod
     def intersecting_cells(self, other):
@@ -384,14 +395,19 @@
     def numpy_id_to_grid_id(self, index):
         pass
 
     @abc.abstractmethod
     def grid_id_to_numpy_id(self, index):
         pass
 
+    @property
+    def indices(self):
+        """Return the indices within the bounds of the data"""       
+        return self.cells_in_bounds(self.bounds)[0]
+
     def assign(self, data, *, anchor=None, bounds=None, in_place=True, assign_nodata=True):
         if not any([anchor, bounds]):
             raise ValueError("Please supply either an 'anchor' or 'bounds' keyword to position the data in the grid.")
         new_data = self.data if in_place else self.data.copy()
 
         if bounds:
             slice_y, slice_x = self._data_slice_from_bounds(bounds)
```

### Comparing `gridkit-0.1.1/gridkit/io.py` & `gridkit-0.2.0/gridkit/io.py`

 * *Files identical despite different names*

### Comparing `gridkit-0.1.1/gridkit/rect_grid.py` & `gridkit-0.2.0/gridkit/rect_grid.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,41 +23,125 @@
 
     @property
     def dy(self) -> float:
         """The cellsize in y-direction
         """
         return self.__dy
 
-    def neighbours(self, index, connect_corners=False, include_selected=False):
-        """
+    def relative_neighbours(self, depth=1, connect_corners=False, include_selected=False, index=None):
+        """The relative indices of the neighbouring cells.
+
+        Parameters
+        ----------
+        depth: :class:`int` Default: 1
+            Determines the number of neighbours that are returned.
+            If `depth=1` the direct neighbours are returned.
+            If `depth=2` the direct neighbours are returned, as well as the neighbours of these neighbours.
+            `depth=3` returns yet another layer of neighbours, and so forth.
+        include_selected: :class:`bool` Default: False
+            Whether to include the specified cell in the return array.
+            Even though the specified cell can never be a neighbour of itself,
+            this can be useful when for example a weighted average of the neighbours is desired
+            in which case the cell itself often should also be included.
+        connect_corners: :class:`bool` Default: False
+            Whether to consider cells that touch corners but not sides as neighbours.
+            If `connect_corners` is True, the 4 cells directly touching the cell are considered neighbours.
+            If `connect_corners` is True, the 8 cells surrounding the cell are considered neighbours.
+            This escalates in combination with `depth` where indices in a square shape around the cell are returned
+            when `connect_corners` is True, and indices in a diamond shape around the cell are returned when `connect_corners` is False.
+        index: :class:`numpy.ndarray`
+            The index is mostly relevant for hexagonal grids.
+            For a square grid the relative neighbours are independent on the location on the grid.
+            Here it is only used for the return length.
+            If 10 cells are supplied to `index`, the relative neighbours are returned 10 times.
+            This is to keep a consistent api between the two classes.
+
+
+        Examples
+        --------
+        The direct neighbours of a cell can be returned by using depth=1, which is the default.
+        For square grids, the number of returned neighbours depends on whether `connect_corners` is True or False:
+        
+        .. code-block:: python
+
+            >>> from gridkit.rect_grid import RectGrid
+            >>> grid = RectGrid(dx=2, dy=3)
+            >>> grid.relative_neighbours()
+            array([[ 0,  1],
+                   [-1,  0],
+                   [ 1,  0],
+                   [ 0, -1]])
+            >>> grid.relative_neighbours(connect_corners=True)
+            array([[-1,  1],
+                   [ 0,  1],
+                   [ 1,  1],
+                   [-1,  0],
+                   [ 1,  0],
+                   [-1, -1],
+                   [ 0, -1],
+                   [ 1, -1]])
+
+        ..
+
+        By specifying `depth` we can include indirect neighbours from further away.
+        The number of neighbours increases with depth by a factor of `depth*4` or `depth*8` depending on `connect_corners` being True or False.
+        So the 3rd element in the list will be `1*4 + 2*4 + 3*4 = 24` if `connect_corners` is False.
+        And it will be `1*8 + 2*8 + 3*8 = 48` if `connect_corners` is True.
+
+        .. code-block:: python
+
+            >>> [len(grid.relative_neighbours(depth=depth)) for depth in range(1,5)]
+            [4, 12, 24, 36]
+            >>> [len(grid.relative_neighbours(depth=depth, connect_corners=True)) for depth in range(1,5)]
+            [8, 24, 48, 80]
+
+        ..
+
+        The specified cell can be included if `include_selected` is set to True:
+
+        .. code-block:: python
+
+            >>> grid.relative_neighbours(include_selected=True)
+            array([[ 0,  1],
+                   [-1,  0],
+                   [ 0,  0],
+                   [ 1,  0],
+                   [ 0, -1]])
+
+        ..
+
+        See also
+        --------
+        :py:meth:`.BaseGrid.neighbours`
+        :py:meth:`.HexGrid.relative_neighbours`
         """
-        if not isinstance(index, numpy.ndarray):
-            index = numpy.array(index)
 
-        relative_neighbours = numpy.vstack([
-            numpy.array([[-1,0,1]] * 3).ravel(),
-            numpy.array([[1,0,-1]] * 3).T.ravel()
-        ]).T
-
-        relative_neighbor_indices = {1,3,5,7}
-        if connect_corners:
-            relative_neighbor_indices.update({0,2,6,8})
-        if include_selected:
-            center_id = int(numpy.mean(list(relative_neighbor_indices)))
-            relative_neighbor_indices.add(center_id)
-        relative_neighbours = relative_neighbours[list(relative_neighbor_indices)]
-    
-        neighbours = numpy.expand_dims(index, 1)
-        neighbours = numpy.repeat(neighbours, len(relative_neighbours), axis=1)
+        if depth < 1:
+            raise ValueError("'depth' cannot be lower than 1")
 
-        if index.ndim == 1: # make sure 'neighbours' is in the desired shape if index contains only one ID
-            neighbours = neighbours.T
+        neighbours = numpy.empty(((2*depth+1)**2, 2), dtype=int)
 
-        return neighbours + relative_neighbours
+        relative_ids_1d = numpy.arange(-depth, depth+1)
+        relative_x, relative_y = numpy.meshgrid(relative_ids_1d, relative_ids_1d[::-1])
+        neighbours[:,0], neighbours[:,1] = numpy.ravel(relative_x), numpy.ravel(relative_y)
+
+        if not connect_corners:
+            mask = abs(numpy.multiply(*neighbours.T)) < depth
+            neighbours = neighbours[mask]
+
+        if include_selected is False:
+            center_cell = int(numpy.floor(len(neighbours)/2))
+            neighbours = numpy.delete(neighbours, center_cell, 0)
+
+        if index is not None:
+            index = numpy.array(index)
+            if len(index.shape) == 2:
+                neighbours = numpy.repeat(neighbours[numpy.newaxis], len(index), axis=0)
 
+        return neighbours
 
     def centroid(self, index=None):
         """Coordinates at the center of the cell(s) specified by `index`.
 
         .. Warning ::
             The two values that make up an `index` are expected to be integers, and will be cast as such.
 
@@ -339,53 +423,14 @@
             aligned = False
             reasons.append("offset")
 
         reason = f"The following attributes are not the same: {reasons}" if reasons else reason
         return aligned, reason
 
 
-    def are_bounds_aligned(self, bounds, separate=False):
-        is_aligned = lambda val, cellsize: numpy.isclose(val, 0) or numpy.isclose(val, cellsize)
-        per_axis = (
-            is_aligned((bounds[0] - self.offset[0]) % self.dx, self.dx), # left
-            is_aligned((bounds[1] - self.offset[1]) % self.dy, self.dy), # bottom
-            is_aligned((bounds[2] - self.offset[0]) % self.dx, self.dx), # right
-            is_aligned((bounds[3] - self.offset[1]) % self.dy, self.dy)  # top
-        )
-        return per_axis if separate else numpy.all(per_axis)
-
-
-    def align_bounds(self, bounds, mode="expand"):
-        
-        if self.are_bounds_aligned(bounds):
-            return bounds
-
-        if mode == "expand":
-            return (
-                numpy.floor((bounds[0] - self.offset[0]) / self.dx) * self.dx + self.offset[0],
-                numpy.floor((bounds[1] - self.offset[1]) / self.dy) * self.dy + self.offset[1],
-                numpy.ceil((bounds[2] - self.offset[0]) / self.dx) * self.dx + self.offset[0],
-                numpy.ceil((bounds[3] - self.offset[1]) / self.dy) * self.dy + self.offset[1],
-            )
-        if mode == "contract":
-            return (
-                numpy.ceil((bounds[0] - self.offset[0]) / self.dx) * self.dx + self.offset[0],
-                numpy.ceil((bounds[1] - self.offset[1]) / self.dy) * self.dy + self.offset[1],
-                numpy.floor((bounds[2] - self.offset[0]) / self.dx) * self.dx + self.offset[0],
-                numpy.floor((bounds[3] - self.offset[1]) / self.dy) * self.dy + self.offset[1],
-            )
-        if mode == "nearest":
-            return (
-                round((bounds[0] - self.offset[0]) / self.dx) * self.dx + self.offset[0],
-                round((bounds[1] - self.offset[1]) / self.dy) * self.dy + self.offset[1],
-                round((bounds[2] - self.offset[0]) / self.dx) * self.dx + self.offset[0],
-                round((bounds[3] - self.offset[1]) / self.dy) * self.dy + self.offset[1],
-            )
-        raise ValueError(f"mode = '{mode}' is not supported. Supported modes: ('expand', 'contract', 'nearest')")
-
     def cells_in_bounds(self, bounds):
         """
         Parameters
         ----------
         bounds: :class:`tuple`
         align_mode: :class:`str`
             Specifies when to consider a cell included in the bounds. Options:
@@ -481,42 +526,22 @@
         :class:`numpy.ndarray`
             Multidimensional array containing the longitude and latitude of the center of each cell respectively,
             in (width, height, lonlat)
         """
         if index is not None:
             return super(BoundedRectGrid, self).centroid(index=index)
         # get grid in shape (latlon, width, height)
-        latlon = numpy.array(numpy.meshgrid(self.lon, self.lat, sparse=False, indexing="xy"))
+        latlon = numpy.meshgrid(self.lon, self.lat, sparse=False, indexing="xy")
 
         # return grid in shape (width, height, lonlat)
         return numpy.array([latlon[0].ravel(),latlon[1].ravel()]).T
 
     def intersecting_cells(self, other):
         raise NotImplementedError()
 
-    def shared_bounds(self, other):
-        other_bounds = other.bounds if isinstance(other, BaseGrid) else other
-        if not self.intersects(other):
-            raise IntersectionError(f"Grid with bounds {self.bounds} does not intersect with grid with bounds {other_bounds}.")
-        return (
-            max(self.bounds[0], other_bounds[0]),
-            max(self.bounds[1], other_bounds[1]),
-            min(self.bounds[2], other_bounds[2]),
-            min(self.bounds[3], other_bounds[3]),
-        )
-
-    def combined_bounds(self, other):
-        other_bounds = other.bounds if isinstance(other, BaseGrid) else other
-        return (
-            min(self.bounds[0], other_bounds[0]),
-            min(self.bounds[1], other_bounds[1]),
-            max(self.bounds[2], other_bounds[2]),
-            max(self.bounds[3], other_bounds[3]),
-        )
-
     def crop(self, new_bounds, bounds_crs=None, buffer_cells=0):
 
         if bounds_crs is not None:
             bounds_crs = CRS.from_user_input(bounds_crs)
             transformer = Transformer.from_crs(bounds_crs, self.crs, always_xy=True)
             new_bounds = transformer.transform_bounds(*new_bounds)
 
@@ -561,41 +586,42 @@
 
         return slice_y, slice_x
 
     def cell_corners(self, index: numpy.ndarray = None) -> numpy.ndarray:
         if index is None:
             index = self.indices()
         return super(BoundedRectGrid, self).cell_corners(index=index)
+    
+    def to_shapely(self, index=None, as_multipolygon: bool = False):
+        """Refer to parent method :meth:`.BaseGrid.to_shapely`
 
-    def indices(self, index: numpy.ndarray = None):
-        """Return the indices"""
-        # I guess this only makes sense for data grids, maybe remove the index argument?
+        Difference with parent method:
+            `index` is optional. 
+            If `index` is None (default) the cells containing data are used as the `index` argument.
+        
+        See also
+        --------
+        :meth:`.BaseGrid.to_shapely`
+        :meth:`.BoundedHexGrid.to_shapely`
+        """
         if index is None:
-            return self.cells_in_bounds(self.bounds)
-        cell_centers = self.centroid(index=index)
-        return self.cell_at_point(cell_centers)
+            index = self.indices
+        return super().to_shapely(index, as_multipolygon)
 
     def resample(self, alignment_grid, method="nearest"):
-
         if self.crs is None or alignment_grid.crs is None:
             warnings.warn("`crs` not set for one or both grids. Assuming both grids have an identical CRS.")
             different_crs = False
         else:
             different_crs = not self.crs.is_exact_same(alignment_grid.crs)
 
         # make sure the bounds align with the grid
         if different_crs:
             transformer = Transformer.from_crs(self.crs, alignment_grid.crs, always_xy=True)
-            transformed_corners = numpy.vstack(transformer.transform(*self.corners.T)).T
-            bounds = (
-                min(transformed_corners[0, 0], transformed_corners[3, 0]),
-                min(transformed_corners[2, 1], transformed_corners[3, 1]),
-                max(transformed_corners[1, 0], transformed_corners[2, 0]),
-                max(transformed_corners[0, 1], transformed_corners[1, 1])
-            )
+            bounds = transformer.transform_bounds(*self.bounds)
         else:
             bounds = self.bounds
 
         # Align using "contract" for we cannot sample outside of the original bounds
         new_bounds = alignment_grid.align_bounds(bounds, mode="contract")
 
         new_ids, new_shape = alignment_grid.cells_in_bounds(bounds=new_bounds)
@@ -629,15 +655,22 @@
             value = bot_val + (top_val - bot_val) * y_diff
 
             # TODO: remove rows and cols with nans around the edge after bilinear
         else:
             raise ValueError(f"Resampling method '{method}' is not supported.")
 
         value = value.reshape(new_shape)
-        new_grid = BoundedRectGrid(value, bounds=new_bounds, crs=alignment_grid.crs, nodata_value=nodata_value)
+
+        grid_kwargs = dict(
+            data=value, bounds=new_bounds, crs=alignment_grid.crs, nodata_value=nodata_value
+        )
+        if hasattr(alignment_grid, "_shape"):
+            grid_kwargs["shape"] = alignment_grid._shape
+
+        new_grid = alignment_grid.bounded_cls(**grid_kwargs)
 
         return new_grid
 
     def to_crs(self, crs, resample_method="nearest"):
         new_inf_grid = super(BoundedRectGrid, self).to_crs(crs, resample_method=resample_method)
         return self.resample(new_inf_grid, method=resample_method)
```

### Comparing `gridkit-0.1.1/setup.py` & `gridkit-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "geopandas",
 ]
 
 setup(
     name="gridkit",
     version=version_info["__version__"],
     author="Timo Millenaar",
-    description="Operations on, and tessellation of, regular grids",
+    description="Powerful abstractions of infinite grids for grid-vector interactions, tesselation, resampling and interactions between related grids.",
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     packages=find_packages(),
```

