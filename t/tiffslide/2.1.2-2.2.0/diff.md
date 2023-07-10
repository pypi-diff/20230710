# Comparing `tmp/tiffslide-2.1.2.tar.gz` & `tmp/tiffslide-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiffslide-2.1.2.tar", last modified: Tue Apr  4 21:47:36 2023, max compression
+gzip compressed data, was "tiffslide-2.2.0.tar", last modified: Mon Jul 10 19:37:30 2023, max compression
```

## Comparing `tiffslide-2.1.2.tar` & `tiffslide-2.2.0.tar`

### file list

```diff
@@ -1,103 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.071622 tiffslide-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-04 21:47:26.000000 tiffslide-2.1.2/.bandit
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-04 21:47:26.000000 tiffslide-2.1.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-04 21:47:26.000000 tiffslide-2.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-04-04 21:47:26.000000 tiffslide-2.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-04 21:47:26.000000 tiffslide-2.1.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-04 21:47:26.000000 tiffslide-2.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-04 21:47:26.000000 tiffslide-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-04 21:47:26.000000 tiffslide-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-04-04 21:47:36.071622 tiffslide-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-04-04 21:47:26.000000 tiffslide-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.043622 tiffslide-2.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-04 21:47:26.000000 tiffslide-2.1.2/docs/generate_benchmark_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.043622 tiffslide-2.1.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-04-04 21:47:26.000000 tiffslide-2.1.2/docs/images/benchmark_read_tiles_as_numpy.png
--rw-r--r--   0 runner    (1001) docker     (123)    23219 2023-04-04 21:47:26.000000 tiffslide-2.1.2/docs/images/benchmark_read_tiles_as_pil.png
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-04 21:47:26.000000 tiffslide-2.1.2/environment.devenv.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.039622 tiffslide-2.1.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.043622 tiffslide-2.1.2/examples/compare/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/compare/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/compare/compare_smallest_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/compare/compare_tiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.043622 tiffslide-2.1.2/examples/deepzoom/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/deepzoom_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.039622 tiffslide-2.1.2/examples/deepzoom/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.051622 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36115 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/changelog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.063622 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/button_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/button_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/button_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/button_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/flip_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/flip_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/flip_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/flip_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/home_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/home_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/home_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/home_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/next_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/next_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/next_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/next_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/previous_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/previous_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/previous_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/previous_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)   872924 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.js
--rw-r--r--   0 runner    (1001) docker     (123)  2254078 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   226423 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   280828 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.063622 tiffslide-2.1.2/examples/deepzoom/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-04 21:47:26.000000 tiffslide-2.1.2/examples/deepzoom/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-04 21:47:26.000000 tiffslide-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-04 21:47:36.071622 tiffslide-2.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.067622 tiffslide-2.1.2/tiffslide/
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/_kerchunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/_pycompat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 21:47:35.000000 tiffslide-2.1.2/tiffslide/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/_zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/deepzoom.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/repair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.071622 tiffslide-2.1.2/tiffslide/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/tests/test_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/tests/test_kerchunk.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/tests/test_pycompat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/tests/test_tiffslide.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/tests/test_zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)    36842 2023-04-04 21:47:26.000000 tiffslide-2.1.2/tiffslide/tiffslide.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:47:36.067622 tiffslide-2.1.2/tiffslide.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-04-04 21:47:35.000000 tiffslide-2.1.2/tiffslide.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-04 21:47:36.000000 tiffslide-2.1.2/tiffslide.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 21:47:35.000000 tiffslide-2.1.2/tiffslide.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-04 21:47:35.000000 tiffslide-2.1.2/tiffslide.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-04 21:47:35.000000 tiffslide-2.1.2/tiffslide.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:30.021469 tiffslide-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 19:37:15.000000 tiffslide-2.2.0/.bandit
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 19:37:15.000000 tiffslide-2.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-10 19:37:15.000000 tiffslide-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-10 19:37:15.000000 tiffslide-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 19:37:15.000000 tiffslide-2.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-10 19:37:15.000000 tiffslide-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-10 19:37:15.000000 tiffslide-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 19:37:15.000000 tiffslide-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-10 19:37:30.021469 tiffslide-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-07-10 19:37:15.000000 tiffslide-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:29.997469 tiffslide-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-10 19:37:15.000000 tiffslide-2.2.0/docs/generate_benchmark_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:30.001469 tiffslide-2.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-07-10 19:37:15.000000 tiffslide-2.2.0/docs/images/benchmark_read_tiles_as_numpy.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23219 2023-07-10 19:37:15.000000 tiffslide-2.2.0/docs/images/benchmark_read_tiles_as_pil.png
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-10 19:37:15.000000 tiffslide-2.2.0/environment.devenv.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:29.997469 tiffslide-2.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:30.001469 tiffslide-2.2.0/examples/compare/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/compare/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/compare/compare_smallest_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/compare/compare_tiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:30.001469 tiffslide-2.2.0/examples/deepzoom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/deepzoom_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:29.997469 tiffslide-2.2.0/examples/deepzoom/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:30.005469 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    36115 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/changelog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:30.013469 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/button_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/button_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/button_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/button_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/flip_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/flip_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/flip_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/flip_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/home_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/home_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/home_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/home_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/next_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/next_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/next_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/next_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/previous_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/previous_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/previous_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/previous_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)   872924 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2254078 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   226423 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   280828 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:30.013469 tiffslide-2.2.0/examples/deepzoom/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-10 19:37:15.000000 tiffslide-2.2.0/examples/deepzoom/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-10 19:37:15.000000 tiffslide-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-10 19:37:30.021469 tiffslide-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:30.017469 tiffslide-2.2.0/tiffslide/
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/_kerchunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 19:37:29.000000 tiffslide-2.2.0/tiffslide/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/deepzoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/repair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:30.021469 tiffslide-2.2.0/tiffslide/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/tests/test_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/tests/test_kerchunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/tests/test_tiffslide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/tests/test_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36696 2023-07-10 19:37:15.000000 tiffslide-2.2.0/tiffslide/tiffslide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:37:30.017469 tiffslide-2.2.0/tiffslide.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-10 19:37:29.000000 tiffslide-2.2.0/tiffslide.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-10 19:37:29.000000 tiffslide-2.2.0/tiffslide.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:37:29.000000 tiffslide-2.2.0/tiffslide.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-10 19:37:29.000000 tiffslide-2.2.0/tiffslide.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 19:37:29.000000 tiffslide-2.2.0/tiffslide.egg-info/top_level.txt
```

### Comparing `tiffslide-2.1.2/.pre-commit-config.yaml` & `tiffslide-2.2.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-added-large-files
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
+  rev: v3.9.0
   hooks:
   - id: pyupgrade
-    args: [--py37-plus]
+    args: [--py38-plus]
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
   - id: isort
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 23.3.0
   hooks:
   - id: black
     language_version: python3
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: 'v1.0.1'
+  rev: 'v1.4.1'
   hooks:
   - id: mypy
     additional_dependencies: ["numpy"]
-    exclude: ^examples/
+    exclude: ^examples/|^tiffslide/tests/
 - repo: https://github.com/PyCQA/flake8
   rev: '6.0.0'
   hooks:
   - id: flake8
     additional_dependencies:
     - flake8-typing-imports==1.12.0
     language_version: python3
     exclude: "^(build|docs|setup.py)|tests[/]"
 - repo: https://github.com/PyCQA/bandit
-  rev: '1.7.4'
+  rev: '1.7.5'
   hooks:
   - id: bandit
     args: ["--ini", ".bandit", "-lll"]
```

### Comparing `tiffslide-2.1.2/CHANGELOG.md` & `tiffslide-2.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased] - ...
 
+## [2.2.0] - 2023-06-10
+## Changed
+- `tiffslide`: drop support for Python 3.7
+
+## Fixed
+- `tiffslide._zarr`: speedup tile access by preventing double decode #72
+
 ## [2.1.2] - 2023-04-04
 ## Fixed
 - `tiffslide`: add bounds when parsing leica metadata #68
 
 ## [2.1.1] - 2023-03-13
 ## Fixed
 - `tiffslide`: Provide fallback support for broken images with non-ascii ImageDescription tags
@@ -173,15 +180,16 @@
 ### Changed
 - removed `TiffSlide.ts_filename` attribute
 
 ## [0.0.1] - 2021-03-18
 ### Added
 - initial release of tiffslide and
 
-[Unreleased]: https://github.com/bayer-science-for-a-better-life/tiffslide/compare/v2.1.2...HEAD
+[Unreleased]: https://github.com/bayer-science-for-a-better-life/tiffslide/compare/v2.2.0...HEAD
+[2.2.0]: https://github.com/bayer-science-for-a-better-life/tiffslide/compare/v2.1.2...v2.2.0
 [2.1.2]: https://github.com/bayer-science-for-a-better-life/tiffslide/compare/v2.1.1...v2.1.2
 [2.1.1]: https://github.com/bayer-science-for-a-better-life/tiffslide/compare/v2.1.0...v2.1.1
 [2.1.0]: https://github.com/bayer-science-for-a-better-life/tiffslide/compare/v2.0.1...v2.1.0
 [2.0.1]: https://github.com/bayer-science-for-a-better-life/tiffslide/compare/v2.0.0...v2.0.1
 [2.0.0]: https://github.com/bayer-science-for-a-better-life/tiffslide/compare/v1.10.1...v2.0.0
 [1.10.1]: https://github.com/bayer-science-for-a-better-life/tiffslide/compare/v1.10.0...v1.10.1
 [1.10.0]: https://github.com/bayer-science-for-a-better-life/tiffslide/compare/v1.9.0...v1.10.0
```

### Comparing `tiffslide-2.1.2/CONTRIBUTING.md` & `tiffslide-2.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/LICENSE` & `tiffslide-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/PKG-INFO` & `tiffslide-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: tiffslide
-Version: 2.1.2
+Version: 2.2.0
 Summary: tifffile-based drop-in replacement for openslide-python
 Home-page: https://github.com/bayer-science-for-a-better-life/tiffslide
 Download-URL: https://github.com/bayer-science-for-a-better-life/tiffslide
 Author: Andreas Poehlmann
 Author-email: andreas.poehlmann@bayer.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Utilities
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # tiffslide: a drop-in replacement for openslide-python
 
 [![PyPI Version](https://img.shields.io/pypi/v/tiffslide)](https://pypi.org/project/tiffslide/)
```

### Comparing `tiffslide-2.1.2/README.md` & `tiffslide-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/docs/generate_benchmark_plots.py` & `tiffslide-2.2.0/docs/generate_benchmark_plots.py`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/docs/images/benchmark_read_tiles_as_numpy.png` & `tiffslide-2.2.0/docs/images/benchmark_read_tiles_as_numpy.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/docs/images/benchmark_read_tiles_as_pil.png` & `tiffslide-2.2.0/docs/images/benchmark_read_tiles_as_pil.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/environment.devenv.yml` & `tiffslide-2.2.0/environment.devenv.yml`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/compare/compare_smallest_zoom.py` & `tiffslide-2.2.0/examples/compare/compare_smallest_zoom.py`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/compare/compare_tiles.py` & `tiffslide-2.2.0/examples/compare/compare_tiles.py`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/deepzoom_server.py` & `tiffslide-2.2.0/examples/deepzoom/deepzoom_server.py`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/LICENSE.txt` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/changelog.txt` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/changelog.txt`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/button_grouphover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/button_grouphover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/button_hover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/button_hover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/button_pressed.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/button_pressed.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/button_rest.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/button_rest.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/flip_grouphover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/flip_grouphover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/flip_hover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/flip_hover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/flip_pressed.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/flip_pressed.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/flip_rest.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/flip_rest.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_grouphover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_grouphover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_hover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_hover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_pressed.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_pressed.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_rest.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/fullpage_rest.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/home_grouphover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/home_grouphover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/home_hover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/home_hover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/home_pressed.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/home_pressed.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/home_rest.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/home_rest.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/next_grouphover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/next_grouphover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/next_hover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/next_hover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/next_pressed.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/next_pressed.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/next_rest.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/next_rest.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/previous_grouphover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/previous_grouphover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/previous_hover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/previous_hover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/previous_pressed.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/previous_pressed.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/previous_rest.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/previous_rest.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_grouphover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_grouphover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_hover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_hover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_pressed.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_pressed.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_rest.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateleft_rest.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_grouphover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_grouphover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_hover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_hover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_pressed.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_pressed.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_rest.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/rotateright_rest.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_grouphover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_grouphover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_hover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_hover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_pressed.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_pressed.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_rest.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomin_rest.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_grouphover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_grouphover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_hover.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_hover.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_pressed.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_pressed.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_rest.png` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_rest.png`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.js` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.js`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.js.map` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.js.map`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.min.js` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.min.js`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.min.js.map` & `tiffslide-2.2.0/examples/deepzoom/static/openseadragon-2.4.2/openseadragon.min.js.map`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/examples/deepzoom/templates/index.html` & `tiffslide-2.2.0/examples/deepzoom/templates/index.html`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/pyproject.toml` & `tiffslide-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/setup.cfg` & `tiffslide-2.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 author_email = andreas.poehlmann@bayer.com
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Information Analysis
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Utilities
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Operating System :: Unix
 	Operating System :: MacOS
 
 [options]
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	imagecodecs
 	fsspec!=2022.11.0,!=2023.1.0
 	pillow
 	tifffile>=2021.6.14
-	zarr
+	zarr>=2.11.0
 	typing_extensions>=4.0
 
 [options.packages.find]
 exclude = 
 	tests/*
 
 [options.package_data]
```

### Comparing `tiffslide-2.1.2/tiffslide/__init__.py` & `tiffslide-2.2.0/tiffslide/__init__.py`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/tiffslide/_compat.py` & `tiffslide-2.2.0/tiffslide/_compat.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,18 @@
 import os.path
 import sys
 from pathlib import PurePath
 from types import MappingProxyType
 from types import TracebackType
 from typing import TYPE_CHECKING
 from typing import Any
+from typing import Literal
 from typing import Mapping
 from typing import Sequence
 
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
 import numpy as np
 import zarr
 from imagecodecs import __version__ as _imagecodecs_version
 from imagecodecs import imread
 
 try:
     from tiffslide._version import version as _tiffslide_version
```

### Comparing `tiffslide-2.1.2/tiffslide/_kerchunk.py` & `tiffslide-2.2.0/tiffslide/_kerchunk.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,15 @@
 import json
 import os
 import sys
 from collections import ChainMap
 from io import StringIO
 from typing import TYPE_CHECKING
 from typing import Any
-
-if sys.version_info >= (3, 8):
-    from typing import TypedDict
-else:
-    from typing_extensions import TypedDict
+from typing import TypedDict
 
 import fsspec
 from imagecodecs.numcodecs import register_codecs
 
 from tiffslide.tiffslide import TiffSlide
 
 if TYPE_CHECKING:
```

### Comparing `tiffslide-2.1.2/tiffslide/_types.py` & `tiffslide-2.2.0/tiffslide/_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,18 @@
 
 import os
 import sys
 import warnings
 from typing import IO
 from typing import TYPE_CHECKING
 from typing import Any
+from typing import Protocol
+from typing import TypedDict
 from typing import Union
-
-if sys.version_info >= (3, 8):
-    from typing import Protocol
-    from typing import TypedDict
-    from typing import runtime_checkable
-
-else:
-    from typing_extensions import Protocol
-    from typing_extensions import TypedDict
-    from typing_extensions import runtime_checkable
+from typing import runtime_checkable
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 if TYPE_CHECKING:
```

### Comparing `tiffslide-2.1.2/tiffslide/_zarr.py` & `tiffslide-2.2.0/tiffslide/_zarr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 """
 provides helpers for handling and compositing arrays and zarr-like groups
 """
 from __future__ import annotations
 
 import json
-import sys
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Iterator
 from typing import Mapping
-from warnings import warn
 
 import numpy as np
 import zarr
 from fsspec.implementations.reference import ReferenceFileSystem
 from tifffile import TiffFile
 from tifffile import ZarrTiffStore
+from zarr.storage import BaseStore
 from zarr.storage import FSStore
+from zarr.storage import KVStore as _KVStore
 
 from tiffslide._compat import NotTiffFile
-from tiffslide._pycompat import REQUIRES_STORE_FIX
-from tiffslide._pycompat import py37_fix_store
 from tiffslide._types import Point3D
 from tiffslide._types import SeriesCompositionInfo
 from tiffslide._types import Size3D
 from tiffslide._types import Slice3D
 
 if TYPE_CHECKING:
     from numpy.typing import DTypeLike
     from numpy.typing import NDArray
 
-try:
-    from zarr.storage import KVStore
-except ImportError:
-    KVStore = lambda x: x  # noqa
-
 
 __all__ = [
     "get_zarr_store",
     "get_zarr_depth_and_dtype",
     "get_zarr_selection",
 ]
 
-if REQUIRES_STORE_FIX and sys.version_info >= (3, 8):
-    warn(
-        "detected outdated tifffile version on `python>=3.8` with `zarr>=2.11.0`: "
-        "updating tifffile is recommended!"
-    )
-
 
 # --- zarr storage classes --------------------------------------------
 
+if "__contains__" not in _KVStore.__dict__:
+    # fix missing contains caused double decode:
+    # https://github.com/bayer-science-for-a-better-life/tiffslide/issues/72#issuecomment-1627918238
+    class KVStore(_KVStore):
+        def __contains__(self, item: str) -> bool:
+            return item in self._mutable_mapping
+
+else:
+    KVStore = _KVStore  # type: ignore
+
 
 class _CompositedStore(Mapping[str, Any]):
     """prefix zarr stores to allow mounting them in groups"""
 
     def __init__(
         self,
         prefixed_stores: Mapping[str, Mapping[str, Any]],
@@ -116,25 +113,23 @@
     """return a zarr store from the object"""
     if isinstance(obj, (TiffFile, NotTiffFile)):
         zstore = obj.series[series_idx].aszarr(maxworkers=num_decode_threads)  # type: ignore
     elif isinstance(obj, ReferenceFileSystem):
         zstore = FSStore(f"s{series_idx}", fs=obj)
     else:
         raise NotImplementedError(f"{type(obj).__name__} unsupported")
-    if REQUIRES_STORE_FIX:
-        zstore = py37_fix_store(zstore)
     return zstore  # type: ignore
 
 
 def get_zarr_store(
     properties: Mapping[str, Any],
     tf: TiffFile | ReferenceFileSystem | None,
     *,
     num_decode_threads: int | None = None,
-) -> Mapping[str, Any]:
+) -> BaseStore:
     """return a zarr store
 
     Parameters
     ----------
     properties:
         the TiffSlide().properties mapping
     tf:
@@ -150,37 +145,41 @@
     if tf is None:
         raise NotImplementedError("support in future versions")
 
     # the tiff might contain multiple series that require composition
     composition: SeriesCompositionInfo | None = properties.get(
         "tiffslide.series-composition"
     )
-    store: Mapping[str, Any]
+    store: BaseStore
     if composition:
         prefixed_stores = {}
         for series_idx in composition["located_series"].keys():
             _store = _get_series_zarr(
                 tf, series_idx, num_decode_threads=num_decode_threads
             )
             # encapsulate store as group if tifffile returns a zarr array
             if ".zarray" in _store:
                 _store = _CompositedStore({"0": _store})
             prefixed_stores[str(series_idx)] = _store
 
-        store = _CompositedStore(prefixed_stores, zattrs=composition)
-        store = KVStore(store)
+        _store = _CompositedStore(prefixed_stores, zattrs=composition)
+        store = KVStore(_store)
 
     else:
         series_idx = properties.get("tiffslide.series-index", 0)
-        store = _get_series_zarr(tf, series_idx, num_decode_threads=num_decode_threads)
+        _store = _get_series_zarr(tf, series_idx, num_decode_threads=num_decode_threads)
 
         # encapsulate store as group if tifffile returns a zarr array
-        if ".zarray" in store:
-            store = _CompositedStore({"0": store})
-            store = KVStore(store)
+        if ".zarray" in _store:
+            _store = _CompositedStore({"0": _store})
+            store = KVStore(_store)
+        elif isinstance(_store, BaseStore):
+            store = _store
+        else:
+            store = KVStore(_store)
 
     return store
 
 
 def get_zarr_selection(
     grp: zarr.Group,
     level: int,
@@ -298,15 +297,15 @@
         # noinspection PyProtectedMember
         chunkmode = store._chunkmode
         # noinspection PyProtectedMember
         parse_key = store._parse_key
     except AttributeError:
         raise RuntimeError("probably not supported with your tifffile version")
 
-    chunk_sizes = np.full(chunked, dtype=np.int64, fill_value=-1)
+    chunk_sizes: NDArray[np.int64] = np.full(chunked, dtype=np.int64, fill_value=-1)
 
     # _index = ""
     for indices in np.ndindex(*chunked):
         chunkindex = ".".join(str(index) for index in indices)
         key = levelstr + chunkindex
         keyframe, page, _, offset, bytecount = parse_key(key)
         # key = levelstr + _index + chunkindex
```

### Comparing `tiffslide-2.1.2/tiffslide/deepzoom.py` & `tiffslide-2.2.0/tiffslide/deepzoom.py`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/tiffslide/repair.py` & `tiffslide-2.2.0/tiffslide/repair.py`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/tiffslide/tests/conftest.py` & `tiffslide-2.2.0/tiffslide/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,21 +175,18 @@
 
     tile_hw = (512, 512)
     # multi resolution
     multi_hw = [(10240, 10240), (5120, 5120), (2560, 2560)]
     mpp = 0.25
     mag = 40
     filename = "ASD"
-    if sys.version_info >= (3, 8):
-        resolution_kw = {
-            "resolution": (10000 / mpp, 10000 / mpp),
-            "resolutionunit": "CENTIMETER",
-        }
-    else:
-        resolution_kw = {"resolution": (10000 / mpp, 10000 / mpp, "CENTIMETER")}
+    resolution_kw = {
+        "resolution": (10000 / mpp, 10000 / mpp),
+        "resolutionunit": "CENTIMETER",
+    }
 
     # write to svs format
     with tifffile.TiffWriter(pth, bigtiff=True) as tif:
         kwargs = {
             "subifds": 0,
             "photometric": "MINISBLACK",
             "compression": APERIO_JP2000_RGB,
```

### Comparing `tiffslide-2.1.2/tiffslide/tests/test_benchmark.py` & `tiffslide-2.2.0/tiffslide/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/tiffslide/tests/test_compatibility.py` & `tiffslide-2.2.0/tiffslide/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/tiffslide/tests/test_kerchunk.py` & `tiffslide-2.2.0/tiffslide/tests/test_kerchunk.py`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/tiffslide/tests/test_tiffslide.py` & `tiffslide-2.2.0/tiffslide/tests/test_tiffslide.py`

 * *Files identical despite different names*

### Comparing `tiffslide-2.1.2/tiffslide/tiffslide.py` & `tiffslide-2.2.0/tiffslide/tiffslide.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,52 +1,45 @@
 from __future__ import annotations
 
 import math
 import os.path
 import sys
 from collections import defaultdict
 from fractions import Fraction
+from functools import cached_property
 from itertools import count
 from types import TracebackType
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Iterator
+from typing import Literal
 from typing import Mapping
 from typing import TypeVar
 from typing import overload
 from warnings import warn
 from xml.etree import ElementTree
 
-from tifffile import TiffPage
-
-from tiffslide._types import Slice3D
-
-if sys.version_info[:2] >= (3, 8):
-    from functools import cached_property
-    from typing import Literal
-else:
-    from tiffslide._pycompat import cached_property
-    from typing_extensions import Literal
-
 import numpy as np
 import tifffile
 import zarr
 from fsspec.core import url_to_fs
 from fsspec.implementations.local import LocalFileSystem
 from fsspec.implementations.reference import ReferenceFileSystem
 from PIL import Image
 from tifffile import TiffFile
 from tifffile import TiffFileError as TiffFileError
+from tifffile import TiffPage
 from tifffile import TiffPageSeries
 from tifffile.tifffile import svs_description_metadata
 
 from tiffslide._compat import NotTiffFile
 from tiffslide._types import OpenFileLike
 from tiffslide._types import PathOrFileOrBufferLike
 from tiffslide._types import SeriesCompositionInfo
+from tiffslide._types import Slice3D
 from tiffslide._types import TiffFileIO
 from tiffslide._zarr import get_zarr_depth_and_dtype
 from tiffslide._zarr import get_zarr_selection
 from tiffslide._zarr import get_zarr_store
 
 if TYPE_CHECKING:
     import numpy.typing as npt
```

### Comparing `tiffslide-2.1.2/tiffslide.egg-info/PKG-INFO` & `tiffslide-2.2.0/tiffslide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: tiffslide
-Version: 2.1.2
+Version: 2.2.0
 Summary: tifffile-based drop-in replacement for openslide-python
 Home-page: https://github.com/bayer-science-for-a-better-life/tiffslide
 Download-URL: https://github.com/bayer-science-for-a-better-life/tiffslide
 Author: Andreas Poehlmann
 Author-email: andreas.poehlmann@bayer.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Utilities
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # tiffslide: a drop-in replacement for openslide-python
 
 [![PyPI Version](https://img.shields.io/pypi/v/tiffslide)](https://pypi.org/project/tiffslide/)
```

### Comparing `tiffslide-2.1.2/tiffslide.egg-info/SOURCES.txt` & `tiffslide-2.2.0/tiffslide.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_hover.png
 examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_pressed.png
 examples/deepzoom/static/openseadragon-2.4.2/images/zoomout_rest.png
 examples/deepzoom/templates/index.html
 tiffslide/__init__.py
 tiffslide/_compat.py
 tiffslide/_kerchunk.py
-tiffslide/_pycompat.py
 tiffslide/_types.py
 tiffslide/_version.py
 tiffslide/_zarr.py
 tiffslide/deepzoom.py
 tiffslide/py.typed
 tiffslide/repair.py
 tiffslide/tiffslide.py
@@ -80,10 +79,9 @@
 tiffslide.egg-info/dependency_links.txt
 tiffslide.egg-info/requires.txt
 tiffslide.egg-info/top_level.txt
 tiffslide/tests/conftest.py
 tiffslide/tests/test_benchmark.py
 tiffslide/tests/test_compatibility.py
 tiffslide/tests/test_kerchunk.py
-tiffslide/tests/test_pycompat.py
 tiffslide/tests/test_tiffslide.py
 tiffslide/tests/test_zarr.py
```

