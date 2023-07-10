# Comparing `tmp/cogeo_mosaic-5.1.1.tar.gz` & `tmp/cogeo_mosaic-6.0.0.tar.gz`

## Comparing `cogeo_mosaic-5.1.1.tar` & `cogeo_mosaic-6.0.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/CHANGES.md
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/README.md
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/setup.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/cache.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/errors.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/logger.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/models.py
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/mosaic.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/utils.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/backends/__init__.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/backends/az.py
--rw-r--r--   0        0        0    10689 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/backends/base.py
--rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/backends/dynamodb.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/backends/file.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/backends/gs.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/backends/memory.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/backends/s3.py
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/backends/sqlite.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/backends/stac.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/backends/utils.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/backends/web.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/scripts/__init__.py
--rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/cogeo_mosaic/scripts/cli.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/LICENSE
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/pyproject.toml
--rw-r--r--   0        0        0    14960 2020-02-02 00:00:00.000000 cogeo_mosaic-5.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/CHANGES.md
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/README.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/cache.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/errors.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/logger.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/models.py
+-rw-r--r--   0        0        0    10859 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/mosaic.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/utils.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/az.py
+-rw-r--r--   0        0        0    13571 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/base.py
+-rw-r--r--   0        0        0    11458 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/dynamodb.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/file.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/gs.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/memory.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/s3.py
+-rw-r--r--   0        0        0    14051 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/sqlite.py
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/stac.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/utils.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/backends/web.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/scripts/__init__.py
+-rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/cogeo_mosaic/scripts/cli.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/LICENSE
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0    17221 2020-02-02 00:00:00.000000 cogeo_mosaic-6.0.0/PKG-INFO
```

### Comparing `cogeo_mosaic-5.1.1/CHANGES.md` & `cogeo_mosaic-6.0.0/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,33 @@
 
+## 6.0.0 (2023-07-10)
+
+* update `morecantile>=4.1,<5.0` and `rio-tiler>=5.0,<6.0` requirements
+
+* replace `supermercado` with [`supermorecado`](https://github.com/developmentseed/supermorecado) to burn geometries as tiles for different TMS
+
+* update MosaicJSON models to `0.0.3` specification (adds `tilematrixset`, `asset_type`, `asset_prefix`, `data_type`, `colormap` and `layers` attributes)
+
+* allow Mosaic creation using other TileMatrixSet (default is still `WebMercatorQuad`)
+
+* add `tms` support to MosaicBackend to read tile in other TMS than the mosaic TileMatrixSet
+
+    ```python
+    # Before
+    # Mosaic and output Tile in WebMercatorQuad
+    with MosaicBackend("mosaic.json") as mosaic:
+        img, _ = mosaic.tile(0, 0, 0)
+
+    # Now
+    # Mosaic in WebMercatorQuad (default), output tile in WGS84
+    WGS1984Quad = morecantile.tms.get("WGS1984Quad")
+    with MosaicBackend("mosaic.json", tms=WGS1984Quad) as mosaic:
+        img, _ = mosaic.tile(0, 0, 0)
+    ```
+
 ## 5.1.1 (2023-02-06)
 
 * Clip dataset bounds with of TMS bbox (author @lseelenbinder, https://github.com/developmentseed/cogeo-mosaic/pull/200)
 
 ## 5.1.0 (2023-01-20)
 
 * use `az://` prefix for private Azure Blob Storage Backend.
```

### Comparing `cogeo_mosaic-5.1.1/CONTRIBUTING.md` & `cogeo_mosaic-6.0.0/CONTRIBUTING.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # Development - Contributing
 
 Issues and pull requests are more than welcome.
 
 **Dev install & Pull-Request**
 
 ```
-$ git clone http://github.com/developmentseed/cogeo-mosaic.git
-$ cd cogeo-mosaic
-$ pip install -e .["test,az"]
+git clone http://github.com/developmentseed/cogeo-mosaic.git
+cd cogeo-mosaic
+python -m pip install -e .["test,az"]
 ```
 
 You can then run the tests with the following command:
 
 ```sh
-python -m pytest --cov cogeo_mosaic --cov-report term-missing --benchmark-skip
+python -m pytest --cov cogeo_mosaic --cov-report term-missing
 ```
 
 ### pre-commit
 
 This repo is set to use `pre-commit` to run *isort*, *flake8*, *pydocstring*, *black* ("uncompromising Python code formatter") and mypy when committing new code.
 
 ```bash
-$ pre-commit install
+pre-commit install
 
-$ git add .
+git add .
 
-$ git commit -m'my change'
+git commit -m'my change'
 isort....................................................................Passed
 black....................................................................Passed
 Flake8...................................................................Passed
 Verifying PEP257 Compliance..............................................Passed
 mypy.....................................................................Passed
 
-$ git push origin
+git push origin
 ```
 
 ### Docs
 
 ```bash
-$ git clone https://github.com/developmentseed/cogeo-mosaic.git
-$ cd cogeo-mosaic
-$ pip install -e .["docs"]
+git clone https://github.com/developmentseed/cogeo-mosaic.git
+cd cogeo-mosaic
+python -m pip install -e .["docs"]
 ```
 
 Hot-reloading docs:
 
 ```bash
-$ mkdocs serve
+mkdocs serve
 ```
 
 To manually deploy docs (note you should never need to do this because Github
 Actions deploys automatically for new commits.):
 
 ```bash
-$ mkdocs gh-deploy -f docs/mkdocs.yml
+mkdocs gh-deploy -f docs/mkdocs.yml
 ```
```

### Comparing `cogeo_mosaic-5.1.1/README.md` & `cogeo_mosaic-6.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,20 +33,20 @@
 
 ---
 
 **Read the official announcement https://medium.com/devseed/cog-talk-part-2-mosaics-bbbf474e66df**
 
 ## Install
 ```bash
-$ pip install pip -U
-$ pip install cogeo-mosaic --pre
+python -m pip install pip -U
+python -m pip install cogeo-mosaic --pre
 
 # Or from source
 
-$ pip install git+http://github.com/developmentseed/cogeo-mosaic
+python -m pip install git+http://github.com/developmentseed/cogeo-mosaic
 ```
 
 **Notes**:
 
 - Starting with version 5.0, pygeos has been replaced by shapely and thus makes `libgeos` a requirement.
 Shapely wheels should be available for most environment, if not, you'll need to have libgeos installed.
```

#### html2text {}

```diff
@@ -2,20 +2,20 @@
                                   [rio-tiler]
        Create mosaics of Cloud Optimized GeoTIFF based on the mosaicJSON
                                 specification.
           [Test] [Coverage] [Package_version] [Downloads] [Downloads]
 --- **Documentation**: https://developmentseed.org/cogeo-mosaic/ **Source
 Code**: https://github.com/developmentseed/cogeo-mosaic --- **Read the official
 announcement https://medium.com/devseed/cog-talk-part-2-mosaics-bbbf474e66df**
-## Install ```bash $ pip install pip -U $ pip install cogeo-mosaic --pre # Or
-from source $ pip install git+http://github.com/developmentseed/cogeo-mosaic
-``` **Notes**: - Starting with version 5.0, pygeos has been replaced by shapely
-and thus makes `libgeos` a requirement. Shapely wheels should be available for
-most environment, if not, you'll need to have libgeos installed. ## See it in
-action - [**TiTiler**](http://github.com/developmentseed/titiler): A
-lightweight Cloud Optimized GeoTIFF dynamic tile server (COG, STAC and
-MosaicJSON). ## Contribution & Development See [CONTRIBUTING.md](https://
-github.com/developmentseed/cogeo-mosaic/blob/master/CONTRIBUTING.md) ## License
-See [LICENSE](https://github.com/developmentseed/cogeo-mosaic/blob/master/
-LICENSE) ## Authors Created by [Development Seed](
+## Install ```bash python -m pip install pip -U python -m pip install cogeo-
+mosaic --pre # Or from source python -m pip install git+http://github.com/
+developmentseed/cogeo-mosaic ``` **Notes**: - Starting with version 5.0, pygeos
+has been replaced by shapely and thus makes `libgeos` a requirement. Shapely
+wheels should be available for most environment, if not, you'll need to have
+libgeos installed. ## See it in action - [**TiTiler**](http://github.com/
+developmentseed/titiler): A lightweight Cloud Optimized GeoTIFF dynamic tile
+server (COG, STAC and MosaicJSON). ## Contribution & Development See
+[CONTRIBUTING.md](https://github.com/developmentseed/cogeo-mosaic/blob/master/
+CONTRIBUTING.md) ## License See [LICENSE](https://github.com/developmentseed/
+cogeo-mosaic/blob/master/LICENSE) ## Authors Created by [Development Seed](
 developmentseed.org>) See [contributors](https://github.com/developmentseed/
 cogeo-mosaic/graphs/contributors) for a listing of individual contributors.
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/cache.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/cache.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/errors.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     """MosaicJSON already exists."""
 
 
 class MosaicExistsError(MosaicError):
     """MosaicJSON already exists."""
 
 
+class MultipleDataTypeError(MosaicError):
+    """Can create mosaic will dataset of multiple datatype."""
+
+
 _HTTP_EXCEPTIONS = {
     401: MosaicAuthError,
     403: MosaicAuthError,
     404: MosaicNotFoundError,
 }
 
 _FILE_EXCEPTIONS = {FileNotFoundError: MosaicNotFoundError}
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/mosaic.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/mosaic.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 import sys
 import warnings
 from contextlib import ExitStack
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple
 
 import click
 import morecantile
-from pydantic import BaseModel, Field, root_validator
+from pydantic import BaseModel, Field, root_validator, validator
 from shapely import linearrings, polygons, total_bounds
 from shapely.strtree import STRtree
-from supermercado import burntiles
+from supermorecado import burnTiles
 
-from cogeo_mosaic.errors import MosaicError
+from cogeo_mosaic.errors import MosaicError, MultipleDataTypeError
 from cogeo_mosaic.utils import _intersect_percent, get_footprints
 
-tms = morecantile.tms.get("WebMercatorQuad")
+WEB_MERCATOR_TMS = morecantile.tms.get("WebMercatorQuad")
 
 
-def default_accessor(feature: Dict):
+def default_accessor(feature: Dict) -> str:
     """Return specific feature identifier."""
     return feature["properties"]["path"]
 
 
 def default_filter(
     tile: morecantile.Tile,
     dataset: Sequence[Dict],
@@ -32,15 +32,17 @@
     tile_cover_sort: bool = False,
     maximum_items_per_tile: Optional[int] = None,
 ) -> List:
     """Filter and/or sort dataset per intersection coverage."""
     indices = list(range(len(dataset)))
 
     if minimum_tile_cover or tile_cover_sort:
-        tile_geom = polygons(tms.feature(tile)["geometry"]["coordinates"][0])
+        tile_geom = polygons(
+            WEB_MERCATOR_TMS.feature(tile)["geometry"]["coordinates"][0]
+        )
         int_pcts = _intersect_percent(tile_geom, geoms)
 
         if minimum_tile_cover:
             if minimum_tile_cover > 1.0:
                 raise MosaicError("`minimum_tile_cover` HAS TO be between 0 and 1.")
 
             indices = [ind for ind in indices if int_pcts[ind] > minimum_tile_cover]
@@ -66,23 +68,40 @@
     name: Optional[str]
     description: Optional[str]
     version: str = "1.0.0"
     attribution: Optional[str]
     minzoom: int = Field(0, ge=0, le=30)
     maxzoom: int = Field(30, ge=0, le=30)
     quadkey_zoom: Optional[int]
-    bounds: Tuple[float, float, float, float] = Field((-180, -90, 180, 90))
+    bounds: Tuple[float, float, float, float] = Field(default=(-180, -90, 180, 90))
     center: Optional[Tuple[float, float, int]]
     tiles: Dict[str, List[str]]
+    tilematrixset: Optional[morecantile.TileMatrixSet]
+    asset_type: Optional[str]
+    asset_prefix: Optional[str]
+    data_type: Optional[str]
+    colormap: Optional[Dict[int, Tuple[int, int, int, int]]]
+    layers: Optional[Dict]
 
     class Config:
         """Validate model on update."""
 
         validate_assignment = True
 
+    @validator("tilematrixset", pre=True, always=True)
+    def parse_tms(cls, value) -> Optional[morecantile.TileMatrixSet]:
+        """Parse TMS."""
+        if isinstance(value, dict):
+            value = morecantile.TileMatrixSet(**value)
+
+        if value:
+            assert value._is_quadtree, f"{value.id} TMS does not support quadtree."
+
+        return value
+
     @root_validator
     def compute_center(cls, values):
         """Compute center if it does not exist."""
         bounds = values["bounds"]
         if not values.get("center"):
             values["center"] = (
                 (bounds[0] + bounds[2]) / 2,
@@ -103,15 +122,21 @@
         cls,
         features: Sequence[Dict],
         minzoom: int,
         maxzoom: int,
         quadkey_zoom: Optional[int] = None,
         accessor: Callable[[Dict], str] = default_accessor,
         asset_filter: Callable = default_filter,
-        version: str = "0.0.2",
+        version: str = "0.0.3",
+        tilematrixset: Optional[morecantile.TileMatrixSet] = None,
+        asset_type: Optional[str] = None,
+        asset_prefix: Optional[str] = None,
+        data_type: Optional[str] = None,
+        colormap: Optional[Dict[int, Tuple[int, int, int, int]]] = None,
+        layers: Optional[Dict] = None,
         quiet: bool = True,
         **kwargs,
     ):
         """Create mosaic definition content.
 
         Attributes:
             features (list): List of GeoJSON features.
@@ -127,38 +152,58 @@
         Returns:
             mosaic_definition (MosaicJSON): Mosaic definition.
 
         Examples:
             >>> MosaicJSON._create_mosaic([], 12, 14)
 
         """
+        tms = tilematrixset or WEB_MERCATOR_TMS
+
+        assert tms._is_quadtree, f"{tms.id} TMS does not support quadtree."
+
         quadkey_zoom = quadkey_zoom or minzoom
 
         if not quiet:
             click.echo(f"Get quadkey list for zoom: {quadkey_zoom}", err=True)
 
         dataset_geoms = polygons(
             [linearrings(feat["geometry"]["coordinates"][0]) for feat in features]
         )
 
         bounds = tuple(total_bounds(dataset_geoms))
 
-        tiles = burntiles.burn(features, quadkey_zoom)
-        tiles = [morecantile.Tile(*tile) for tile in tiles]
+        burntiles = burnTiles(tms=tms)
+        tiles = [morecantile.Tile(*t) for t in burntiles.burn(features, quadkey_zoom)]
 
-        mosaic_definition: Dict[str, Any] = dict(
-            mosaicjson=version,
-            minzoom=minzoom,
-            maxzoom=maxzoom,
-            quadkey_zoom=quadkey_zoom,
-            bounds=bounds,
-            center=((bounds[0] + bounds[2]) / 2, (bounds[1] + bounds[3]) / 2, minzoom),
-            tiles={},
-            version="1.0.0",
-        )
+        mosaic_definition: Dict[str, Any] = {
+            "mosaicjson": version,
+            "minzoom": minzoom,
+            "maxzoom": maxzoom,
+            "quadkey_zoom": quadkey_zoom,
+            "bounds": bounds,
+            "center": (
+                (bounds[0] + bounds[2]) / 2,
+                (bounds[1] + bounds[3]) / 2,
+                minzoom,
+            ),
+            "tiles": {},
+            "version": "1.0.0",
+        }
+
+        mosaic_003 = {
+            "tilematrixset": tilematrixset,
+            "asset_type": asset_type,
+            "asset_prefix": asset_prefix,
+            "data_type": data_type,
+            "colormap": colormap,
+            "layers": layers,
+        }
+        for k, v in mosaic_003.items():
+            if v is not None:
+                mosaic_definition[k] = v
 
         if not quiet:
             click.echo("Feed Quadkey index", err=True)
 
         # Create tree and find assets that overlap each tile
         tree = STRtree(dataset_geoms)
 
@@ -225,15 +270,14 @@
         Raises:
             Exception: If COGs don't have the same datatype
 
         Examples:
             >>> MosaicJSON.from_urls(["1.tif", "2.tif"])
 
         """
-
         features = get_footprints(urls, max_threads=max_threads, quiet=quiet)
 
         if minzoom is None:
             data_minzoom = {feat["properties"]["minzoom"] for feat in features}
             if len(data_minzoom) > 1:
                 warnings.warn(
                     "Multiple MinZoom, Assets different minzoom values", UserWarning
@@ -249,15 +293,15 @@
                     UserWarning,
                 )
 
             maxzoom = max(data_maxzoom)
 
         datatype = {feat["properties"]["datatype"] for feat in features}
         if len(datatype) > 1:
-            raise Exception("Dataset should have the same data type")
+            raise MultipleDataTypeError("Dataset should have the same data type")
 
         return cls._create_mosaic(
             features, minzoom=minzoom, maxzoom=maxzoom, quiet=quiet, **kwargs
         )
 
     @classmethod
     def from_features(
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/utils.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import numpy
 from rio_tiler.io import Reader
 from shapely import area, intersection
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 
-tms = morecantile.tms.get("WebMercatorQuad")
+WEB_MERCATOR_TMS = morecantile.tms.get("WebMercatorQuad")
 
 
 def _filter_futures(tasks):
     """
     Filter future task to remove Exceptions.
 
     Attributes
@@ -37,17 +37,24 @@
         try:
             yield future.result()
         except Exception as err:
             logger.warning(str(err))
             pass
 
 
-def get_dataset_info(src_path: str) -> Dict:
+def get_dataset_info(
+    src_path: str,
+    tms: morecantile.TileMatrixSet = WEB_MERCATOR_TMS,
+) -> Dict:
     """Get rasterio dataset meta."""
-    with Reader(src_path) as src:
+    with Reader(
+        src_path,
+        tms=tms,
+        geographic_crs=tms.rasterio_geographic_crs,
+    ) as src:
         bounds = src.geographic_bounds
         return {
             "geometry": {
                 "type": "Polygon",
                 "coordinates": [
                     [
                         tms.truncate_lnglat(bounds[0], bounds[3]),
@@ -66,61 +73,71 @@
                 "datatype": src.dataset.meta["dtype"],
             },
             "type": "Feature",
         }
 
 
 def get_footprints(
-    dataset_list: Sequence[str], max_threads: int = 20, quiet: bool = True
+    dataset_list: Sequence[str],
+    tms: morecantile.TileMatrixSet = WEB_MERCATOR_TMS,
+    max_threads: int = 20,
+    quiet: bool = True,
 ) -> List:
     """
     Create footprint GeoJSON.
 
     Attributes
     ----------
     dataset_listurl : tuple or list, required
         Dataset urls.
+    tms : TileMatrixSet
+        TileMartixSet to use (default WebMercatorQaud
     max_threads : int
         Max threads to use (default: 20).
 
     Returns
     -------
     out : tuple
         tuple of footprint feature.
 
     """
     with ExitStack() as ctx:
         fout = ctx.enter_context(open(os.devnull, "w")) if quiet else sys.stderr
         with futures.ThreadPoolExecutor(max_workers=max_threads) as executor:
             future_work = [
-                executor.submit(get_dataset_info, item) for item in dataset_list
+                executor.submit(get_dataset_info, item, tms) for item in dataset_list
             ]
             with click.progressbar(  # type: ignore
                 futures.as_completed(future_work),
                 file=fout,
                 length=len(future_work),
                 label="Get footprints",
                 show_percent=True,
             ) as future:
                 for _ in future:
                     pass
 
     return list(_filter_futures(future_work))
 
 
-def tiles_to_bounds(tiles: List[morecantile.Tile]) -> Tuple[float, float, float, float]:
+def tiles_to_bounds(
+    tiles: List[morecantile.Tile],
+    tms: morecantile.TileMatrixSet = WEB_MERCATOR_TMS,
+) -> Tuple[float, float, float, float]:
     """Get bounds from a set of mercator tiles."""
     zoom = tiles[0].z
     xyz = numpy.array([[t.x, t.y, t.z] for t in tiles])
     extrema = {
         "x": {"min": xyz[:, 0].min(), "max": xyz[:, 0].max() + 1},
         "y": {"min": xyz[:, 1].min(), "max": xyz[:, 1].max() + 1},
     }
+
     ulx, uly = tms.ul(extrema["x"]["min"], extrema["y"]["min"], zoom)
     lrx, lry = tms.ul(extrema["x"]["max"], extrema["y"]["max"], zoom)
+
     return (ulx, lry, lrx, uly)
 
 
 def _intersect_percent(tile, dataset_geoms):
     """Return the overlap percent."""
     inter_areas = area(intersection(tile, dataset_geoms))
     return [inter_area / area(tile) for inter_area in inter_areas]
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/backends/__init__.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cogeo_mosaic.backends.memory import MemoryBackend
 from cogeo_mosaic.backends.s3 import S3Backend
 from cogeo_mosaic.backends.sqlite import SQLiteBackend
 from cogeo_mosaic.backends.stac import STACBackend
 from cogeo_mosaic.backends.web import HttpBackend
 
 
-def MosaicBackend(input: str, *args: Any, **kwargs: Any) -> BaseBackend:
+def MosaicBackend(input: str, *args: Any, **kwargs: Any) -> BaseBackend:  # noqa: C901
     """Select mosaic backend for input."""
     parsed = urlparse(input)
 
     if not input or input == ":memory:":
         return MemoryBackend(*args, **kwargs)
 
     # `stac+https//{hostname}/{path}`
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/backends/az.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/az.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,23 +53,23 @@
         super().__attrs_post_init__()
 
     def write(self, overwrite: bool = False, **kwargs: Any):
         """Write mosaicjson document to Azure Blob Storage."""
         if not overwrite and self._head_object(self.key, self.container):
             raise MosaicExistsError("Mosaic file already exist, use `overwrite=True`.")
 
-        mosaic_doc = self.mosaic_def.dict(exclude_none=True)
+        mosaic_doc = self.mosaic_def.json(exclude_none=True)
         if self.key.endswith(".gz"):
             body = _compress_gz_json(mosaic_doc)
         else:
-            body = json.dumps(mosaic_doc).encode("utf-8")
+            body = mosaic_doc.encode("utf-8")
 
         self._put_object(self.key, self.container, body, **kwargs)
 
-    @cached(
+    @cached(  # type: ignore
         TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
         key=lambda self: hashkey(self.input),
     )
     def _read(self) -> MosaicJSON:  # type: ignore
         """Get mosaicjson document."""
         body = self._get_object(self.key, self.container)
         self._file_byte_size = len(body)
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/backends/base.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """cogeo_mosaic.backend.base: base Backend class."""
 
 import abc
 import itertools
+import warnings
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Type, Union
 
 import attr
-import morecantile
 from cachetools import TTLCache, cached
 from cachetools.keys import hashkey
-from morecantile import TileMatrixSet
+from morecantile import Tile, TileMatrixSet
 from rasterio.crs import CRS
+from rasterio.warp import transform, transform_bounds
 from rio_tiler.constants import WEB_MERCATOR_TMS, WGS84_CRS
 from rio_tiler.errors import PointOutsideBounds
 from rio_tiler.io import BaseReader, MultiBandReader, MultiBaseReader, Reader
 from rio_tiler.models import ImageData, PointData
 from rio_tiler.mosaic import mosaic_reader
 from rio_tiler.tasks import multi_values
 
@@ -33,58 +34,75 @@
 @attr.s
 class BaseBackend(BaseReader):
     """Base Class for cogeo-mosaic backend storage.
 
     Attributes:
         input (str): mosaic path.
         mosaic_def (MosaicJSON, optional): mosaicJSON document.
+        tms (morecantile.TileMatrixSet, optional): TileMatrixSet grid definition. Defaults to `WebMercatorQuad`.
+        minzoom (int): mosaic Min zoom level. Defaults to tms or mosaic minzoom.
+        maxzoom (int): mosaic Max zoom level. Defaults to tms or mosaic maxzoom.
         reader (rio_tiler.io.BaseReader): Dataset reader. Defaults to `rio_tiler.io.Reader`.
         reader_options (dict): Options to forward to the reader config.
-        geographic_crs (rasterio.crs.CRS, optional): CRS to use as geographic coordinate system. Defaults to WGS84.
-        tms (morecantile.TileMatrixSet, optional): TileMatrixSet grid definition. **READ ONLY attribute**. Defaults to `WebMercatorQuad`.
-        bbox (tuple): mosaic bounds (left, bottom, right, top). **READ ONLY attribute**. Defaults to `(-180, -90, 180, 90)`.
-        minzoom (int): mosaic Min zoom level. **READ ONLY attribute**. Defaults to `0`.
-        maxzoom (int): mosaic Max zoom level. **READ ONLY attribute**. Defaults to `30`
+        bounds (tuple): mosaic bounds (left, bottom, right, top). **READ ONLY attribute**. Defaults to `(-180, -90, 180, 90)`.
+        crs (rasterio.crs.CRS): mosaic crs in which its bounds is defined. **READ ONLY attribute**. Defaults to WGS84.
+        geographic_crs (rasterio.crs.CRS, optional): CRS to use as geographic coordinate system. **READ ONLY attribute**. Defaults to WGS84.
 
     """
 
     input: str = attr.ib()
     mosaic_def: MosaicJSON = attr.ib(default=None, converter=_convert_to_mosaicjson)
 
+    tms: TileMatrixSet = attr.ib(default=WEB_MERCATOR_TMS)
+    minzoom: int = attr.ib(default=None)
+    maxzoom: int = attr.ib(default=None)
+
     reader: Union[
         Type[BaseReader],
         Type[MultiBaseReader],
         Type[MultiBandReader],
     ] = attr.ib(default=Reader)
     reader_options: Dict = attr.ib(factory=dict)
 
-    geographic_crs: CRS = attr.ib(default=WGS84_CRS)
-
-    # TMS is outside the init because mosaicJSON and cogeo-mosaic only
-    # works with WebMercator for now.
-    tms: TileMatrixSet = attr.ib(init=False, default=WEB_MERCATOR_TMS)
-    minzoom: int = attr.ib(init=False)
-    maxzoom: int = attr.ib(init=False)
-
-    # default values for bounds
     bounds: Tuple[float, float, float, float] = attr.ib(
         init=False, default=(-180, -90, 180, 90)
     )
     crs: CRS = attr.ib(init=False, default=WGS84_CRS)
+    geographic_crs: CRS = attr.ib(init=False, default=WGS84_CRS)
 
     _backend_name: str
     _file_byte_size: Optional[int] = 0
 
     def __attrs_post_init__(self):
         """Post Init: if not passed in init, try to read from self.input."""
         self.mosaic_def = self.mosaic_def or self._read()
-        self.minzoom = self.mosaic_def.minzoom
-        self.maxzoom = self.mosaic_def.maxzoom
         self.bounds = self.mosaic_def.bounds
 
+        # in order to keep support for old mosaic document we assume the default TMS to be WebMercatorQuad
+        mosaic_tms = self.mosaic_def.tilematrixset or WEB_MERCATOR_TMS
+
+        # By mosaic definition, its `bounds` is defined using the mosaic's TMS
+        # Geographic CRS so we define both `crs` and `geographic_crs` using the mosaic
+        # TMS geographic_crs.
+        self.crs = mosaic_tms.rasterio_geographic_crs
+        self.geographic_crs = mosaic_tms.rasterio_geographic_crs
+
+        # if we open the Mosaic with a TMS which is not the mosaic TMS
+        # the min/max zoom will default to the TMS (read) zooms
+        # except if min/max zoom are passed by the user
+        if self.minzoom is None:
+            self.minzoom = (
+                self.mosaic_def.minzoom if mosaic_tms == self.tms else self.tms.minzoom
+            )
+
+        if self.maxzoom is None:
+            self.maxzoom = (
+                self.mosaic_def.maxzoom if mosaic_tms == self.tms else self.tms.maxzoom
+            )
+
     @abc.abstractmethod
     def _read(self) -> MosaicJSON:
         """Fetch mosaic definition"""
 
     @abc.abstractmethod
     def write(self, overwrite: bool = True):
         """Upload new MosaicJSON to backend."""
@@ -98,119 +116,178 @@
     ):
         """Update existing MosaicJSON on backend."""
         new_mosaic = MosaicJSON.from_features(
             features,
             self.mosaic_def.minzoom,
             self.mosaic_def.maxzoom,
             quadkey_zoom=self.quadkey_zoom,
+            tilematrixset=self.mosaic_def.tilematrixset,
             quiet=quiet,
             **kwargs,
         )
 
         for quadkey, new_assets in new_mosaic.tiles.items():
-            tile = self.tms.quadkey_to_tile(quadkey)
+            mosaic_tms = self.mosaic_def.tilematrixset or WEB_MERCATOR_TMS
+            tile = mosaic_tms.quadkey_to_tile(quadkey)
             assets = self.assets_for_tile(*tile)
             assets = [*new_assets, *assets] if add_first else [*assets, *new_assets]
 
             # add custom sorting algorithm (e.g based on path name)
             self.mosaic_def.tiles[quadkey] = assets
 
         bounds = bbox_union(new_mosaic.bounds, self.mosaic_def.bounds)
 
+        if self.mosaic_def.mosaicjson != new_mosaic.mosaicjson:
+            warnings.warn(
+                f"Updating `mosaicjson` version from {self.mosaic_def.mosaicjson} to {new_mosaic.mosaicjson}"
+            )
+            self.mosaic_def.mosaicjson = new_mosaic.mosaicjson
+
         self.mosaic_def._increase_version()
         self.mosaic_def.bounds = bounds
         self.mosaic_def.center = (
             (bounds[0] + bounds[2]) / 2,
             (bounds[1] + bounds[3]) / 2,
             self.mosaic_def.minzoom,
         )
         self.bounds = bounds
         self.write(overwrite=True)
 
     def assets_for_tile(self, x: int, y: int, z: int) -> List[str]:
         """Retrieve assets for tile."""
-        return self.get_assets(x, y, z)
+        mosaic_tms = self.mosaic_def.tilematrixset or WEB_MERCATOR_TMS
+        if self.tms == mosaic_tms:
+            return self.get_assets(x, y, z)
+
+        # If TMS are different, then use Tile's geographic coordinates
+        # and `assets_for_bbox` to get the assets
+        xmin, ymin, xmax, ymax = self.tms.bounds(x, y, z)
+        return self.assets_for_bbox(
+            xmin,
+            ymin,
+            xmax,
+            ymax,
+            coord_crs=self.tms.rasterio_geographic_crs,
+        )
 
-    def assets_for_point(self, lng: float, lat: float) -> List[str]:
+    def assets_for_point(
+        self,
+        lng: float,
+        lat: float,
+        coord_crs: CRS = WGS84_CRS,
+    ) -> List[str]:
         """Retrieve assets for point."""
-        tile = self.tms.tile(lng, lat, self.quadkey_zoom)
+        mosaic_tms = self.mosaic_def.tilematrixset or WEB_MERCATOR_TMS
+
+        # If coord_crs is not the same as the mosaic's geographic CRS
+        # we reproject the coordinates
+        if coord_crs != mosaic_tms.rasterio_geographic_crs:
+            xs, ys = transform(
+                coord_crs, mosaic_tms.rasterio_geographic_crs, [lng], [lat]
+            )
+            lng, lat = xs[0], ys[0]
+
+        # Find the tile index using geographic coordinates
+        tile = mosaic_tms.tile(lng, lat, self.quadkey_zoom)
+
         return self.get_assets(tile.x, tile.y, tile.z)
 
     def assets_for_bbox(
-        self, xmin: float, ymin: float, xmax: float, ymax: float
+        self,
+        xmin: float,
+        ymin: float,
+        xmax: float,
+        ymax: float,
+        coord_crs: Optional[CRS] = WGS84_CRS,
     ) -> List[str]:
         """Retrieve assets for bbox."""
-        tl_tile = self.tms.tile(xmin, ymax, self.quadkey_zoom)
-        br_tile = self.tms.tile(xmax, ymin, self.quadkey_zoom)
+        mosaic_tms = self.mosaic_def.tilematrixset or WEB_MERCATOR_TMS
+
+        # If coord_crs is not the same as the mosaic's geographic CRS
+        # we reproject the bounding box
+        if coord_crs != mosaic_tms.rasterio_geographic_crs:
+            xmin, ymin, xmax, ymax = transform_bounds(
+                coord_crs,
+                mosaic_tms.rasterio_geographic_crs,
+                xmin,
+                ymin,
+                xmax,
+                ymax,
+            )
+
+        tl_tile = mosaic_tms.tile(xmin, ymax, self.quadkey_zoom)
+        br_tile = mosaic_tms.tile(xmax, ymin, self.quadkey_zoom)
 
         tiles = [
             (x, y, self.quadkey_zoom)
             for x in range(tl_tile.x, br_tile.x + 1)
             for y in range(tl_tile.y, br_tile.y + 1)
         ]
 
         return list(
             dict.fromkeys(
-                itertools.chain.from_iterable([self.assets_for_tile(*t) for t in tiles])
+                itertools.chain.from_iterable([self.get_assets(*t) for t in tiles])
             )
         )
 
-    @cached(
+    @cached(  # type: ignore
         TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
         key=lambda self, x, y, z: hashkey(self.input, x, y, z, self.mosaicid),
     )
     def get_assets(self, x: int, y: int, z: int) -> List[str]:
         """Find assets."""
-        mercator_tile = morecantile.Tile(x=x, y=y, z=z)
-        quadkeys = self.find_quadkeys(mercator_tile, self.quadkey_zoom)
+        quadkeys = self.find_quadkeys(Tile(x=x, y=y, z=z), self.quadkey_zoom)
         return list(
             dict.fromkeys(
                 itertools.chain.from_iterable(
                     [self.mosaic_def.tiles.get(qk, []) for qk in quadkeys]
                 )
             )
         )
 
-    def find_quadkeys(
-        self, mercator_tile: morecantile.Tile, quadkey_zoom: int
-    ) -> List[str]:
+    def find_quadkeys(self, tile: Tile, quadkey_zoom: int) -> List[str]:
         """
         Find quadkeys at desired zoom for tile
 
         Attributes
         ----------
-        mercator_tile: morecantile.Tile
+        tile: morecantile.Tile
             Input tile to use when searching for quadkeys
         quadkey_zoom: int
             Zoom level
 
         Returns
         -------
         list
             List[str] of quadkeys
 
         """
+        mosaic_tms = self.mosaic_def.tilematrixset or WEB_MERCATOR_TMS
+
         # get parent
-        if mercator_tile.z > quadkey_zoom:
-            depth = mercator_tile.z - quadkey_zoom
+        if tile.z > quadkey_zoom:
+            depth = tile.z - quadkey_zoom
             for _ in range(depth):
-                mercator_tile = self.tms.parent(mercator_tile)[0]
-            return [self.tms.quadkey(*mercator_tile)]
+                tile = mosaic_tms.parent(tile)[0]
+
+            return [mosaic_tms.quadkey(*tile)]
 
         # get child
-        elif mercator_tile.z < quadkey_zoom:
-            depth = quadkey_zoom - mercator_tile.z
-            mercator_tiles = [mercator_tile]
+        elif tile.z < quadkey_zoom:
+            depth = quadkey_zoom - tile.z
+
+            tiles = [tile]
             for _ in range(depth):
-                mercator_tiles = sum([self.tms.children(t) for t in mercator_tiles], [])
+                tiles = sum([mosaic_tms.children(t) for t in tiles], [])
+
+            tiles = list(filter(lambda t: t.z == quadkey_zoom, tiles))
+            return [mosaic_tms.quadkey(*tile) for tile in tiles]
 
-            mercator_tiles = list(filter(lambda t: t.z == quadkey_zoom, mercator_tiles))
-            return [self.tms.quadkey(*tile) for tile in mercator_tiles]
         else:
-            return [self.tms.quadkey(*mercator_tile)]
+            return [mosaic_tms.quadkey(*tile)]
 
     def tile(  # type: ignore
         self,
         x: int,
         y: int,
         z: int,
         reverse: bool = False,
@@ -221,15 +298,15 @@
         if not mosaic_assets:
             raise NoAssetFoundError(f"No assets found for tile {z}-{x}-{y}")
 
         if reverse:
             mosaic_assets = list(reversed(mosaic_assets))
 
         def _reader(asset: str, x: int, y: int, z: int, **kwargs: Any) -> ImageData:
-            with self.reader(asset, **self.reader_options) as src_dst:
+            with self.reader(asset, tms=self.tms, **self.reader_options) as src_dst:
                 return src_dst.tile(x, y, z, **kwargs)
 
         return mosaic_reader(mosaic_assets, _reader, x, y, z, **kwargs)
 
     def point(
         self,
         lon: float,
@@ -253,26 +330,30 @@
             kwargs.update({"allowed_exceptions": (PointOutsideBounds,)})
 
         return list(multi_values(mosaic_assets, _reader, lon, lat, **kwargs).items())
 
     def info(self, quadkeys: bool = False) -> Info:  # type: ignore
         """Mosaic info."""
         return Info(
-            bounds=self.mosaic_def.bounds,
-            center=self.mosaic_def.center,
-            maxzoom=self.mosaic_def.maxzoom,
-            minzoom=self.mosaic_def.minzoom,
+            bounds=self.geographic_bounds,
+            center=self.center,
+            maxzoom=self.maxzoom,
+            minzoom=self.minzoom,
             name=self.mosaic_def.name if self.mosaic_def.name else "mosaic",
             quadkeys=[] if not quadkeys else self._quadkeys,
         )
 
     @property
     def center(self):
         """Return center from the mosaic definition."""
-        return self.mosaic_def.center
+        return (
+            (self.bounds[0] + self.bounds[2]) / 2,
+            (self.bounds[1] + self.bounds[3]) / 2,
+            self.minzoom,
+        )
 
     @property
     def mosaicid(self) -> str:
         """Return sha224 id of the mosaicjson document."""
         return get_hash(**self.mosaic_def.dict(exclude_none=True))
 
     @property
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/backends/dynamodb.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/dynamodb.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 import warnings
 from decimal import Decimal
 from typing import Any, Dict, List, Sequence
 from urllib.parse import urlparse
 
 import attr
 import click
-import morecantile
 from cachetools import TTLCache, cached
 from cachetools.keys import hashkey
+from morecantile import Tile
+from rio_tiler.constants import WEB_MERCATOR_TMS
 
 from cogeo_mosaic.backends.base import BaseBackend
 from cogeo_mosaic.cache import cache_config
 from cogeo_mosaic.errors import (
     _HTTP_EXCEPTIONS,
     MosaicError,
     MosaicExistsError,
@@ -80,15 +81,15 @@
         logger.debug(f"Mosaic: {self.mosaic_name}")
 
         self.region = parsed.netloc or self.region
         self.client = self.client or boto3.resource("dynamodb", region_name=self.region)
         self.table = self.client.Table(self.table_name)
         super().__attrs_post_init__()
 
-    @cached(
+    @cached(  # type: ignore
         TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
         key=lambda self: hashkey(self.input),
     )
     def _read(self) -> MosaicJSON:  # type: ignore
         """Get Mosaic definition info."""
         meta = self._fetch_dynamodb(self._metadata_quadkey)
         if not meta:
@@ -162,20 +163,27 @@
         logger.debug(f"Updating {self.mosaic_name}...")
 
         new_mosaic = MosaicJSON.from_features(
             features,
             self.mosaic_def.minzoom,
             self.mosaic_def.maxzoom,
             quadkey_zoom=self.quadkey_zoom,
+            tilematrixset=self.mosaic_def.tilematrixset,
             quiet=quiet,
             **kwargs,
         )
 
         bounds = bbox_union(new_mosaic.bounds, self.mosaic_def.bounds)
 
+        if self.mosaic_def.mosaicjson != new_mosaic.mosaicjson:
+            warnings.warn(
+                f"Updating `mosaicjson` version from {self.mosaic_def.mosaicjson} to {new_mosaic.mosaicjson}"
+            )
+            self.mosaic_def.mosaicjson = new_mosaic.mosaicjson
+
         self.mosaic_def._increase_version()
         self.mosaic_def.bounds = bounds
         self.mosaic_def.center = (
             (bounds[0] + bounds[2]) / 2,
             (bounds[1] + bounds[3]) / 2,
             self.mosaic_def.minzoom,
         )
@@ -189,31 +197,31 @@
         meta = json.loads(self.mosaic_def.json(exclude={"tiles"}), parse_float=Decimal)
         items.append(
             {"quadkey": self._metadata_quadkey, "mosaicId": self.mosaic_name, **meta}
         )
 
         # Create Tile items
         for quadkey, new_assets in new_mosaic.tiles.items():
-            tile = self.tms.quadkey_to_tile(quadkey)
+            mosaic_tms = self.mosaic_def.tilematrixset or WEB_MERCATOR_TMS
+            tile = mosaic_tms.quadkey_to_tile(quadkey)
             assets = self.assets_for_tile(*tile)
             assets = [*new_assets, *assets] if add_first else [*assets, *new_assets]
             items.append(
                 {"mosaicId": self.mosaic_name, "quadkey": quadkey, "assets": assets}
             )
 
         self._write_items(items)
 
-    @cached(
+    @cached(  # type: ignore
         TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
         key=lambda self, x, y, z: hashkey(self.input, x, y, z, self.mosaicid),
     )
     def get_assets(self, x: int, y: int, z: int) -> List[str]:
         """Find assets."""
-        mercator_tile = morecantile.Tile(x=x, y=y, z=z)
-        quadkeys = self.find_quadkeys(mercator_tile, self.quadkey_zoom)
+        quadkeys = self.find_quadkeys(Tile(x=x, y=y, z=z), self.quadkey_zoom)
         return list(
             dict.fromkeys(
                 itertools.chain.from_iterable(
                     [self._fetch_dynamodb(qk).get("assets", []) for qk in quadkeys]
                 )
             )
         )
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/backends/file.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,26 +21,26 @@
     _backend_name = "File"
 
     def write(self, overwrite: bool = False):
         """Write mosaicjson document to a file."""
         if not overwrite and pathlib.Path(self.input).exists():
             raise MosaicExistsError("Mosaic file already exist, use `overwrite=True`.")
 
-        body = self.mosaic_def.dict(exclude_none=True)
+        body = self.mosaic_def.json(exclude_none=True)
         with open(self.input, "wb") as f:
             try:
                 if self.input.endswith(".gz"):
                     f.write(_compress_gz_json(body))
                 else:
-                    f.write(json.dumps(body).encode("utf-8"))
+                    f.write(body.encode("utf-8"))
             except Exception as e:
                 exc = _FILE_EXCEPTIONS.get(e, MosaicError)  # type: ignore
                 raise exc(str(e)) from e
 
-    @cached(
+    @cached(  # type: ignore
         TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
         key=lambda self: hashkey(self.input),
     )
     def _read(self) -> MosaicJSON:  # type: ignore
         """Get mosaicjson document."""
         try:
             with open(self.input, "rb") as f:
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/backends/gs.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/gs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,23 +45,23 @@
         super().__attrs_post_init__()
 
     def write(self, overwrite: bool = False, **kwargs: Any):
         """Write mosaicjson document to Google Cloud Storage."""
         if not overwrite and self._head_object(self.key, self.bucket):
             raise MosaicExistsError("Mosaic file already exist, use `overwrite=True`.")
 
-        mosaic_doc = self.mosaic_def.dict(exclude_none=True)
+        mosaic_doc = self.mosaic_def.json(exclude_none=True)
         if self.key.endswith(".gz"):
             body = _compress_gz_json(mosaic_doc)
         else:
-            body = json.dumps(mosaic_doc).encode("utf-8")
+            body = mosaic_doc.encode("utf-8")
 
         self._put_object(self.key, self.bucket, body, **kwargs)
 
-    @cached(
+    @cached(  # type: ignore
         TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
         key=lambda self: hashkey(self.input),
     )
     def _read(self) -> MosaicJSON:  # type: ignore
         """Get mosaicjson document."""
         body = self._get_object(self.key, self.bucket)
         self._file_byte_size = len(body)
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/backends/s3.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,23 +43,23 @@
         super().__attrs_post_init__()
 
     def write(self, overwrite: bool = False, **kwargs: Any):
         """Write mosaicjson document to AWS S3."""
         if not overwrite and self._head_object(self.key, self.bucket):
             raise MosaicExistsError("Mosaic file already exist, use `overwrite=True`.")
 
-        mosaic_doc = self.mosaic_def.dict(exclude_none=True)
+        mosaic_doc = self.mosaic_def.json(exclude_none=True)
         if self.key.endswith(".gz"):
             body = _compress_gz_json(mosaic_doc)
         else:
-            body = json.dumps(mosaic_doc).encode("utf-8")
+            body = mosaic_doc.encode("utf-8")
 
         self._put_object(self.key, self.bucket, body, **kwargs)
 
-    @cached(
+    @cached(  # type: ignore
         TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
         key=lambda self: hashkey(self.input),
     )
     def _read(self) -> MosaicJSON:  # type: ignore
         """Get mosaicjson document."""
         body = self._get_object(self.key, self.bucket)
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/backends/sqlite.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/sqlite.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,27 +10,31 @@
 from urllib.parse import urlparse
 
 import attr
 import morecantile
 from cachetools import TTLCache, cached
 from cachetools.keys import hashkey
 
+from cogeo_mosaic import __version__ as cogeo_mosaic_version
 from cogeo_mosaic.backends.base import BaseBackend
 from cogeo_mosaic.cache import cache_config
 from cogeo_mosaic.errors import MosaicExistsError, MosaicNotFoundError
 from cogeo_mosaic.logger import logger
 from cogeo_mosaic.mosaic import MosaicJSON
 from cogeo_mosaic.utils import bbox_union
 
 sqlite3.register_adapter(dict, json.dumps)
 sqlite3.register_adapter(tuple, json.dumps)
 sqlite3.register_adapter(list, json.dumps)
 sqlite3.register_converter("JSON", json.loads)
 
 
+MOSAIC_JSON_VERSION = 3
+
+
 @attr.s
 class SQLiteBackend(BaseBackend):
     """SQLite Backend Adapter."""
 
     db_path: str = attr.ib(init=False)
     mosaic_name: str = attr.ib(init=False)
     db: sqlite3.Connection = attr.ib(init=False)
@@ -83,15 +87,15 @@
         """Close SQLite connection."""
         self.db.close()
 
     def __exit__(self, exc_type, exc_value, traceback):
         """Support using with Context Managers."""
         self.close()
 
-    @cached(
+    @cached(  # type: ignore
         TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
         key=lambda self: hashkey(self.input),
     )
     def _read(self) -> MosaicJSON:  # type: ignore
         """Get Mosaic definition info."""
         meta = self._fetch_metadata()
         if not meta:
@@ -114,29 +118,40 @@
             if not overwrite:
                 raise MosaicExistsError(
                     f"'{self.mosaic_name}' Table already exists in {self.db_path}, use `overwrite=True`."
                 )
             self.delete()
 
         with self.db:
+            logger.debug(
+                f"Setting user_version to '{MOSAIC_JSON_VERSION}' in {self.db_path}."
+            )
+            self.db.execute(f"PRAGMA user_version = {MOSAIC_JSON_VERSION};")
+
             logger.debug(f"Creating '{self.mosaic_name}' Table in {self.db_path}.")
             self.db.execute(
                 f"""
                     CREATE TABLE IF NOT EXISTS {self._metadata_table}
                     (
                         mosaicjson TEXT NOT NULL,
                         name TEXT NOT NULL,
                         description TEXT,
                         version TEXT NOT NULL,
                         attribution TEXT,
                         minzoom INTEGER NOT NULL,
                         maxzoom INTEGER NOT NULL,
                         quadkey_zoom INTEGER,
                         bounds JSON NOT NULL,
-                        center JSON
+                        center JSON,
+                        tilematrixset JSON,
+                        asset_type TEXT,
+                        asset_prefix TEXT,
+                        data_type TEXT,
+                        colormap JSON,
+                        layers JSON
                     );
                 """
             )
             self.db.execute(
                 f"""
                     CREATE TABLE "{self.mosaic_name}"
                     (
@@ -156,31 +171,43 @@
                         description,
                         version,
                         attribution,
                         minzoom,
                         maxzoom,
                         quadkey_zoom,
                         bounds,
-                        center
+                        center,
+                        tilematrixset,
+                        asset_type,
+                        asset_prefix,
+                        data_type,
+                        colormap,
+                        layers
                     )
                     VALUES
                     (
                         :mosaicjson,
                         :name,
                         :description,
                         :version,
                         :attribution,
                         :minzoom,
                         :maxzoom,
                         :quadkey_zoom,
                         :bounds,
-                        :center
+                        :center,
+                        :tilematrixset,
+                        :asset_type,
+                        :asset_prefix,
+                        :data_type,
+                        :colormap,
+                        :layers
                     );
                 """,
-                self.mosaic_def.dict(),
+                self.mosaic_def.dict(exclude={"tiles"}),
             )
 
             self.db.executemany(
                 f'INSERT INTO "{self.mosaic_name}" (quadkey, assets) VALUES (?, ?);',
                 self.mosaic_def.tiles.items(),
             )
 
@@ -188,21 +215,29 @@
         self,
         features: Sequence[Dict],
         add_first: bool = True,
         quiet: bool = False,
         **kwargs,
     ):
         """Update existing MosaicJSON on backend."""
+        logger.debug(f"Checking {self.db_path} version ...")
+        with self.db:
+            r = self.db.execute("PRAGMA user_version;").fetchone()
+            assert (
+                r[0] == MOSAIC_JSON_VERSION
+            ), f"{self.db_path} is not compatible with this Backend version ({cogeo_mosaic_version})"
+
         logger.debug(f"Updating {self.mosaic_name}...")
 
         new_mosaic = MosaicJSON.from_features(
             features,
             self.mosaic_def.minzoom,
             self.mosaic_def.maxzoom,
             quadkey_zoom=self.quadkey_zoom,
+            tilematrixset=self.mosaic_def.tilematrixset,
             quiet=quiet,
             **kwargs,
         )
 
         bounds = bbox_union(new_mosaic.bounds, self.mosaic_def.bounds)
 
         self.mosaic_def._increase_version()
@@ -223,18 +258,24 @@
                         description = :description,
                         version = :version,
                         attribution = :attribution,
                         minzoom = :minzoom,
                         maxzoom = :maxzoom,
                         quadkey_zoom = :quadkey_zoom,
                         bounds = :bounds,
-                        center = :center
+                        center = :center,
+                        tilematrixset = :tilematrixset,
+                        asset_type = :asset_type,
+                        asset_prefix = :asset_prefix,
+                        data_type = :data_type,
+                        colormap = :colormap,
+                        layers = :layers
                     WHERE name=:name
                 """,
-                self.mosaic_def.dict(),
+                self.mosaic_def.dict(exclude={"tiles"}),
             )
 
             if add_first:
                 self.db.executemany(
                     f"""
                         UPDATE "{self.mosaic_name}"
                         SET assets = (
@@ -263,15 +304,15 @@
                             )
                         )
                         WHERE quadkey=?;
                     """,
                     [(assets, qk) for qk, assets in new_mosaic.tiles.items()],
                 )
 
-    @cached(
+    @cached(  # type: ignore
         TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
         key=lambda self, x, y, z: hashkey(self.input, x, y, z, self.mosaicid),
     )
     def get_assets(self, x: int, y: int, z: int) -> List[str]:
         """Find assets."""
         mercator_tile = morecantile.Tile(x=x, y=y, z=z)
         quadkeys = self.find_quadkeys(mercator_tile, self.quadkey_zoom)
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/backends/stac.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/stac.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """cogeo-mosaic STAC backend."""
 
 import json
 import os
-from typing import Dict, List, Optional, Sequence, Type
+from typing import Dict, List, Optional, Sequence, Tuple, Type
 
 import attr
 import httpx
 from cachetools import TTLCache, cached
 from cachetools.keys import hashkey
+from morecantile import TileMatrixSet
 from rasterio.crs import CRS
-from rio_tiler.constants import WGS84_CRS
+from rio_tiler.constants import WEB_MERCATOR_TMS, WGS84_CRS
 from rio_tiler.io import STACReader
 
 from cogeo_mosaic.backends.base import BaseBackend
 from cogeo_mosaic.cache import cache_config
 from cogeo_mosaic.errors import _HTTP_EXCEPTIONS, MosaicError
 from cogeo_mosaic.logger import logger
 from cogeo_mosaic.mosaic import MosaicJSON
@@ -56,38 +57,39 @@
 
     input: str = attr.ib()
     query: Dict = attr.ib()
 
     minzoom: int = attr.ib()
     maxzoom: int = attr.ib()
 
+    tms: TileMatrixSet = attr.ib(default=WEB_MERCATOR_TMS)
+
     reader: Type[STACReader] = attr.ib(default=STACReader)
     reader_options: Dict = attr.ib(factory=dict)
 
+    bounds: Tuple[float, float, float, float] = attr.ib(
+        init=False, default=(-180, -90, 180, 90)
+    )
+    crs: CRS = attr.ib(init=False, default=WGS84_CRS)
+    geographic_crs: CRS = attr.ib(init=False, default=WGS84_CRS)
+
     # STAC API related options
     # max_items |  next_link_key | limit
     stac_api_options: Dict = attr.ib(factory=dict)
 
     # Mosaic Creation options
     # e.g `accessor`
     mosaic_options: Dict = attr.ib(factory=dict)
 
-    geographic_crs: CRS = attr.ib(default=WGS84_CRS)
-
     # Because the STACBackend is a Read-Only backend, there is no need for
     # mosaic_def to be in the init method.
-    mosaic_def: MosaicJSON = attr.ib(init=False)
+    mosaic_def: MosaicJSON = attr.ib(init=False, default=None)
 
     _backend_name = "STAC"
 
-    def __attrs_post_init__(self):
-        """Post Init: if not passed in init, try to read from self.input."""
-        self.mosaic_def = self._read()
-        self.bounds = self.mosaic_def.bounds
-
     def _read(self) -> MosaicJSON:
         """
         Fetch STAC API and construct the mosaicjson.
 
         Returns:
             MosaicJSON: Mosaic definition.
 
@@ -102,15 +104,26 @@
         logger.debug(f"Creating mosaic from {len(features)} features")
 
         # We need a specific accessor for STAC
         options = self.mosaic_options.copy()
         if "accessor" not in options:
             options["accessor"] = default_stac_accessor
 
-        return MosaicJSON.from_features(features, self.minzoom, self.maxzoom, **options)
+        minzoom = options.pop("minzoom", None)
+        maxzoom = options.pop("maxzoom", None)
+        mosaic_tms = options.get("tilematrixset", WEB_MERCATOR_TMS)
+        if mosaic_tms == self.tms:
+            minzoom, maxzoom = self.minzoom, self.maxzoom
+        else:
+            if minzoom is None or maxzoom is None:
+                raise MosaicError(
+                    "Min/Max zoom HAVE TO be provided through `mosaic_options` when using different TMS for Read and Mosaic creation"
+                )
+
+        return MosaicJSON.from_features(features, minzoom, maxzoom, **options)
 
     def write(self, overwrite: bool = True):
         """Write mosaicjson document."""
         raise NotImplementedError
 
     def update(
         self,
@@ -133,19 +146,19 @@
         q.update(link.get("body", {}))
     else:
         q = link.get("body", {})
 
     return q
 
 
-@cached(
+@cached(  # type: ignore
     TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
     key=lambda url, query, **kwargs: hashkey(url, json.dumps(query), **kwargs),
 )
-def _fetch(
+def _fetch(  # noqa: C901
     stac_url: str,
     query: Dict,
     max_items: Optional[int] = None,
     next_link_key: Optional[str] = None,
     limit: int = 500,
 ) -> List[Dict]:
     """Call STAC API."""
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/backends/utils.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """cogeo-mosaic.backends utility functions."""
 
 import hashlib
 import json
 import zlib
-from typing import Any, Dict
+from typing import Any
 
 
-def _compress_gz_json(data: Dict) -> bytes:
+def _compress_gz_json(data: str) -> bytes:
     gzip_compress = zlib.compressobj(9, zlib.DEFLATED, zlib.MAX_WBITS | 16)
 
-    return (
-        gzip_compress.compress(json.dumps(data).encode("utf-8")) + gzip_compress.flush()
-    )
+    return gzip_compress.compress(data.encode("utf-8")) + gzip_compress.flush()
 
 
 def _decompress_gz(gzip_buffer: bytes):
     return zlib.decompress(gzip_buffer, zlib.MAX_WBITS | 16).decode()
 
 
 def get_hash(**kwargs: Any) -> str:
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/backends/web.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/backends/web.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __attrs_post_init__(self):
         """Post Init."""
         self.mosaic_def = self._read()
         self.minzoom = self.mosaic_def.minzoom
         self.maxzoom = self.mosaic_def.maxzoom
         self.bounds = self.mosaic_def.bounds
 
-    @cached(
+    @cached(  # type: ignore
         TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
         key=lambda self: hashkey(self.input),
     )
     def _read(self) -> MosaicJSON:  # type: ignore
         """Get mosaicjson document."""
         try:
             r = httpx.get(self.input)
```

### Comparing `cogeo_mosaic-5.1.1/cogeo_mosaic/scripts/cli.py` & `cogeo_mosaic-6.0.0/cogeo_mosaic/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-5.1.1/.gitignore` & `cogeo_mosaic-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-5.1.1/LICENSE` & `cogeo_mosaic-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cogeo_mosaic-5.1.1/pyproject.toml` & `cogeo_mosaic-6.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "cogeo-mosaic"
 description = 'CLI and Backends to work with MosaicJSON.'
 requires-python = ">=3.8"
-license = "MIT"
+license = {file = "LICENSE"}
 authors = [
   { name = "Vincent Sarago", email = "vincent@developmentseed.com" },
 ]
 keywords = ["COG", "MosaicJSON"]
 classifiers = [
   "Intended Audience :: Information Technology",
   "Intended Audience :: Science/Research",
@@ -18,36 +18,36 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = ["version", "readme"]
 dependencies = [
   "attrs",
-  "morecantile>=3.1,<4.0",
-  "shapely>=2.0b2,<3.0",
-  "pydantic",
+  "morecantile>=4.1,<5.0",
+  "shapely>=2.0,<3.0",
+  "pydantic~=1.0",
   "httpx",
   "rasterio",
-  "rio-tiler>=4.0.0a0,<5.0",
+  "rio-tiler>=5.0,<6.0",
+  "supermorecado",
   "cachetools",
-  "supermercado",
 ]
 
 [project.optional-dependencies]
 aws = [
   "boto3",
 ]
 az = [
   "azure-identity", "azure-storage-blob",
 ]
 gcp = [
   "google-cloud-storage"
 ]
 test = [
-  "pytest", "pytest-cov"
+  "pytest", "pytest-cov", "boto3",
 ]
 dev = [
   "pytest", "pytest-cov", "pre-commit"
 ]
 docs = [
   "mkdocs", "mkdocs-material", "pygments", "mkdocs-jupyter"
 ]
@@ -55,14 +55,16 @@
 [project.urls]
 Homepage = 'https://github.com/developmentseed/cogeo-mosaic'
 Documentation = "https://developmentseed.org/cogeo-mosaic/"
 Issues = "https://github.com/developmentseed/cogeo-mosaic/issues"
 Source = "https://github.com/developmentseed/cogeo-mosaic"
 Changelog = "https://developmentseed.org/cogeo-mosaic/release-notes/"
 
+[project.scripts]
+cogeo-mosaic = "cogeo_mosaic.scripts.cli:cogeo_cli"
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = 'text/markdown'
 # construct the PyPI readme from README.md and HISTORY.md
 fragments = [
     {path = "README.md"},
     {text = "\n## Changelog\n\n"},
@@ -107,21 +109,33 @@
 [tool.isort]
 profile = "black"
 known_first_party = ["cogeo_mosaic"]
 known_third_party = [
     "rasterio",
     "rio_tiler",
     "morecantile",
-    "supermercatdo",
+    "supermorecado",
     "shapely",
 ]
 default_section = "THIRDPARTY"
 
 [tool.mypy]
 no_strict_optional = "True"
 
-[tool.pydocstyle]
-select = "D1"
-match = "(?!test).*.py"
+[tool.ruff]
+select = [
+    "D1",  # pydocstyle errors
+    "E",  # pycodestyle errors
+    "W",  # pycodestyle warnings
+    "F",  # flake8
+    "C",  # flake8-comprehensions
+    "B",  # flake8-bugbear
+]
+ignore = [
+    "E501",  # line too long, handled by black
+    "B008",  # do not perform function calls in argument defaults
+    "B905",  # ignore zip() without an explicit strict= parameter, only support with python >3.10
+    "B028",  # ignore No explicit stacklevel keyword argument found
+]
 
-[project.scripts]
-cogeo-mosaic = "cogeo_mosaic.scripts.cli:cogeo_cli"
+[tool.ruff.extend-per-file-ignores]
+"tests/*.py" = ["D1"]
```

### Comparing `cogeo_mosaic-5.1.1/PKG-INFO` & `cogeo_mosaic-6.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,38 @@
 Metadata-Version: 2.1
 Name: cogeo-mosaic
-Version: 5.1.1
+Version: 6.0.0
 Summary: CLI and Backends to work with MosaicJSON.
 Project-URL: Homepage, https://github.com/developmentseed/cogeo-mosaic
 Project-URL: Documentation, https://developmentseed.org/cogeo-mosaic/
 Project-URL: Issues, https://github.com/developmentseed/cogeo-mosaic/issues
 Project-URL: Source, https://github.com/developmentseed/cogeo-mosaic
 Project-URL: Changelog, https://developmentseed.org/cogeo-mosaic/release-notes/
 Author-email: Vincent Sarago <vincent@developmentseed.com>
-License-Expression: MIT
+License: MIT License
+        
+        Copyright (c) 2019 Development Seed
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 License-File: LICENSE
 Keywords: COG,MosaicJSON
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,20 +41,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Requires-Dist: attrs
 Requires-Dist: cachetools
 Requires-Dist: httpx
-Requires-Dist: morecantile<4.0,>=3.1
-Requires-Dist: pydantic
+Requires-Dist: morecantile<5.0,>=4.1
+Requires-Dist: pydantic~=1.0
 Requires-Dist: rasterio
-Requires-Dist: rio-tiler<5.0,>=4.0.0a0
-Requires-Dist: shapely<3.0,>=2.0b2
-Requires-Dist: supermercado
+Requires-Dist: rio-tiler<6.0,>=5.0
+Requires-Dist: shapely<3.0,>=2.0
+Requires-Dist: supermorecado
 Provides-Extra: aws
 Requires-Dist: boto3; extra == 'aws'
 Provides-Extra: az
 Requires-Dist: azure-identity; extra == 'az'
 Requires-Dist: azure-storage-blob; extra == 'az'
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
@@ -44,14 +64,15 @@
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-jupyter; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: pygments; extra == 'docs'
 Provides-Extra: gcp
 Requires-Dist: google-cloud-storage; extra == 'gcp'
 Provides-Extra: test
+Requires-Dist: boto3; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 # cogeo-mosaic
 
 <p align="center">
@@ -87,20 +108,20 @@
 
 ---
 
 **Read the official announcement https://medium.com/devseed/cog-talk-part-2-mosaics-bbbf474e66df**
 
 ## Install
 ```bash
-$ pip install pip -U
-$ pip install cogeo-mosaic --pre
+python -m pip install pip -U
+python -m pip install cogeo-mosaic --pre
 
 # Or from source
 
-$ pip install git+http://github.com/developmentseed/cogeo-mosaic
+python -m pip install git+http://github.com/developmentseed/cogeo-mosaic
 ```
 
 **Notes**:
 
 - Starting with version 5.0, pygeos has been replaced by shapely and thus makes `libgeos` a requirement.
 Shapely wheels should be available for most environment, if not, you'll need to have libgeos installed.
 
@@ -121,14 +142,39 @@
 Created by [Development Seed](<http://developmentseed.org>)
 
 See [contributors](https://github.com/developmentseed/cogeo-mosaic/graphs/contributors) for a listing of individual contributors.
 
 ## Changelog
 
 
+## 6.0.0 (2023-07-10)
+
+* update `morecantile>=4.1,<5.0` and `rio-tiler>=5.0,<6.0` requirements
+
+* replace `supermercado` with [`supermorecado`](https://github.com/developmentseed/supermorecado) to burn geometries as tiles for different TMS
+
+* update MosaicJSON models to `0.0.3` specification (adds `tilematrixset`, `asset_type`, `asset_prefix`, `data_type`, `colormap` and `layers` attributes)
+
+* allow Mosaic creation using other TileMatrixSet (default is still `WebMercatorQuad`)
+
+* add `tms` support to MosaicBackend to read tile in other TMS than the mosaic TileMatrixSet
+
+    ```python
+    # Before
+    # Mosaic and output Tile in WebMercatorQuad
+    with MosaicBackend("mosaic.json") as mosaic:
+        img, _ = mosaic.tile(0, 0, 0)
+
+    # Now
+    # Mosaic in WebMercatorQuad (default), output tile in WGS84
+    WGS1984Quad = morecantile.tms.get("WGS1984Quad")
+    with MosaicBackend("mosaic.json", tms=WGS1984Quad) as mosaic:
+        img, _ = mosaic.tile(0, 0, 0)
+    ```
+
 ## 5.1.1 (2023-02-06)
 
 * Clip dataset bounds with of TMS bbox (author [@lseelenbinder](https://github.com/lseelenbinder), https://github.com/developmentseed/cogeo-mosaic/pull/200)
 
 ## 5.1.0 (2023-01-20)
 
 * use `az://` prefix for private Azure Blob Storage Backend.
```

#### html2text {}

```diff
@@ -1,58 +1,84 @@
-Metadata-Version: 2.1 Name: cogeo-mosaic Version: 5.1.1 Summary: CLI and
+Metadata-Version: 2.1 Name: cogeo-mosaic Version: 6.0.0 Summary: CLI and
 Backends to work with MosaicJSON. Project-URL: Homepage, https://github.com/
 developmentseed/cogeo-mosaic Project-URL: Documentation, https://
 developmentseed.org/cogeo-mosaic/ Project-URL: Issues, https://github.com/
 developmentseed/cogeo-mosaic/issues Project-URL: Source, https://github.com/
 developmentseed/cogeo-mosaic Project-URL: Changelog, https://
 developmentseed.org/cogeo-mosaic/release-notes/ Author-email: Vincent Sarago
-developmentseed.com> License-Expression: MIT License-File: LICENSE Keywords:
-COG,MosaicJSON Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.8 Requires-Dist: attrs Requires-Dist: cachetools Requires-
-Dist: httpx Requires-Dist: morecantile<4.0,>=3.1 Requires-Dist: pydantic
-Requires-Dist: rasterio Requires-Dist: rio-tiler<5.0,>=4.0.0a0 Requires-Dist:
-shapely<3.0,>=2.0b2 Requires-Dist: supermercado Provides-Extra: aws Requires-
-Dist: boto3; extra == 'aws' Provides-Extra: az Requires-Dist: azure-identity;
-extra == 'az' Requires-Dist: azure-storage-blob; extra == 'az' Provides-Extra:
-dev Requires-Dist: pre-commit; extra == 'dev' Requires-Dist: pytest; extra ==
-'dev' Requires-Dist: pytest-cov; extra == 'dev' Provides-Extra: docs Requires-
-Dist: mkdocs; extra == 'docs' Requires-Dist: mkdocs-jupyter; extra == 'docs'
-Requires-Dist: mkdocs-material; extra == 'docs' Requires-Dist: pygments; extra
-== 'docs' Provides-Extra: gcp Requires-Dist: google-cloud-storage; extra ==
-'gcp' Provides-Extra: test Requires-Dist: pytest; extra == 'test' Requires-
-Dist: pytest-cov; extra == 'test' Description-Content-Type: text/markdown #
-cogeo-mosaic
+developmentseed.com> License: MIT License Copyright (c) 2019 Development Seed
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions: The above copyright notice and this
+permission notice shall be included in all copies or substantial portions of
+the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
+EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
+OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE. License-File: LICENSE Keywords: COG,MosaicJSON
+Classifier: Intended Audience :: Information Technology Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: GIS Requires-Python: >=3.8
+Requires-Dist: attrs Requires-Dist: cachetools Requires-Dist: httpx Requires-
+Dist: morecantile<5.0,>=4.1 Requires-Dist: pydantic~=1.0 Requires-Dist:
+rasterio Requires-Dist: rio-tiler<6.0,>=5.0 Requires-Dist: shapely<3.0,>=2.0
+Requires-Dist: supermorecado Provides-Extra: aws Requires-Dist: boto3; extra ==
+'aws' Provides-Extra: az Requires-Dist: azure-identity; extra == 'az' Requires-
+Dist: azure-storage-blob; extra == 'az' Provides-Extra: dev Requires-Dist: pre-
+commit; extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist:
+pytest-cov; extra == 'dev' Provides-Extra: docs Requires-Dist: mkdocs; extra ==
+'docs' Requires-Dist: mkdocs-jupyter; extra == 'docs' Requires-Dist: mkdocs-
+material; extra == 'docs' Requires-Dist: pygments; extra == 'docs' Provides-
+Extra: gcp Requires-Dist: google-cloud-storage; extra == 'gcp' Provides-Extra:
+test Requires-Dist: boto3; extra == 'test' Requires-Dist: pytest; extra ==
+'test' Requires-Dist: pytest-cov; extra == 'test' Description-Content-Type:
+text/markdown # cogeo-mosaic
                                   [rio-tiler]
        Create mosaics of Cloud Optimized GeoTIFF based on the mosaicJSON
                                 specification.
           [Test] [Coverage] [Package_version] [Downloads] [Downloads]
 --- **Documentation**: https://developmentseed.org/cogeo-mosaic/ **Source
 Code**: https://github.com/developmentseed/cogeo-mosaic --- **Read the official
 announcement https://medium.com/devseed/cog-talk-part-2-mosaics-bbbf474e66df**
-## Install ```bash $ pip install pip -U $ pip install cogeo-mosaic --pre # Or
-from source $ pip install git+http://github.com/developmentseed/cogeo-mosaic
-``` **Notes**: - Starting with version 5.0, pygeos has been replaced by shapely
-and thus makes `libgeos` a requirement. Shapely wheels should be available for
-most environment, if not, you'll need to have libgeos installed. ## See it in
-action - [**TiTiler**](http://github.com/developmentseed/titiler): A
-lightweight Cloud Optimized GeoTIFF dynamic tile server (COG, STAC and
-MosaicJSON). ## Contribution & Development See [CONTRIBUTING.md](https://
-github.com/developmentseed/cogeo-mosaic/blob/master/CONTRIBUTING.md) ## License
-See [LICENSE](https://github.com/developmentseed/cogeo-mosaic/blob/master/
-LICENSE) ## Authors Created by [Development Seed](
+## Install ```bash python -m pip install pip -U python -m pip install cogeo-
+mosaic --pre # Or from source python -m pip install git+http://github.com/
+developmentseed/cogeo-mosaic ``` **Notes**: - Starting with version 5.0, pygeos
+has been replaced by shapely and thus makes `libgeos` a requirement. Shapely
+wheels should be available for most environment, if not, you'll need to have
+libgeos installed. ## See it in action - [**TiTiler**](http://github.com/
+developmentseed/titiler): A lightweight Cloud Optimized GeoTIFF dynamic tile
+server (COG, STAC and MosaicJSON). ## Contribution & Development See
+[CONTRIBUTING.md](https://github.com/developmentseed/cogeo-mosaic/blob/master/
+CONTRIBUTING.md) ## License See [LICENSE](https://github.com/developmentseed/
+cogeo-mosaic/blob/master/LICENSE) ## Authors Created by [Development Seed](
 developmentseed.org>) See [contributors](https://github.com/developmentseed/
 cogeo-mosaic/graphs/contributors) for a listing of individual contributors. ##
-Changelog ## 5.1.1 (2023-02-06) * Clip dataset bounds with of TMS bbox (author
-[@lseelenbinder](https://github.com/lseelenbinder), https://github.com/
+Changelog ## 6.0.0 (2023-07-10) * update `morecantile>=4.1,<5.0` and `rio-
+tiler>=5.0,<6.0` requirements * replace `supermercado` with [`supermorecado`]
+(https://github.com/developmentseed/supermorecado) to burn geometries as tiles
+for different TMS * update MosaicJSON models to `0.0.3` specification (adds
+`tilematrixset`, `asset_type`, `asset_prefix`, `data_type`, `colormap` and
+`layers` attributes) * allow Mosaic creation using other TileMatrixSet (default
+is still `WebMercatorQuad`) * add `tms` support to MosaicBackend to read tile
+in other TMS than the mosaic TileMatrixSet ```python # Before # Mosaic and
+output Tile in WebMercatorQuad with MosaicBackend("mosaic.json") as mosaic:
+img, _ = mosaic.tile(0, 0, 0) # Now # Mosaic in WebMercatorQuad (default),
+output tile in WGS84 WGS1984Quad = morecantile.tms.get("WGS1984Quad") with
+MosaicBackend("mosaic.json", tms=WGS1984Quad) as mosaic: img, _ = mosaic.tile
+(0, 0, 0) ``` ## 5.1.1 (2023-02-06) * Clip dataset bounds with of TMS bbox
+(author [@lseelenbinder](https://github.com/lseelenbinder), https://github.com/
 developmentseed/cogeo-mosaic/pull/200) ## 5.1.0 (2023-01-20) * use `az://
 ` prefix for private Azure Blob Storage Backend. ## 5.0.0 (2022-11-21) * switch
 from pygeos to shapely>=2.0 ## 4.2.2 (2022-11-19) * remove useless file in
 package ## 4.2.1 (2022-11-15) * add python 3.11 support ## 4.2.0 (2022-10-24) *
 remove python 3.7 support * add python 3.10 support * switch to hatch build-
 system * update rio-tiler dependency to >=4.0.0a0 ## 4.1.1 (2022-10-21) * Add
 Azure Blob Storage backend (author [@christoe](https://github.com/christoe),
```

