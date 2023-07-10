# Comparing `tmp/pytint-1.0.0.tar.gz` & `tmp/pytint-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytint-1.0.0.tar", max compression
+gzip compressed data, was "pytint-1.0.1.tar", max compression
```

## Comparing `pytint-1.0.0.tar` & `pytint-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35123 2023-06-21 17:12:40.000000 pytint-1.0.0/LICENSE
--rw-r--r--   0        0        0     8906 2023-07-09 13:10:50.462666 pytint-1.0.0/README.md
--rw-r--r--   0        0        0      491 2023-06-22 20:54:30.000000 pytint-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1526 2023-07-08 21:49:59.618008 pytint-1.0.0/pytint/__init__.py
--rw-r--r--   0        0        0      239 2023-07-09 15:05:39.527460 pytint-1.0.0/pytint/__init__.pyi
--rw-r--r--   0        0        0     2923 2023-07-09 12:11:22.921225 pytint-1.0.0/pytint/colors.py
--rw-r--r--   0        0        0      459 2023-07-09 15:05:39.527460 pytint-1.0.0/pytint/colors.pyi
--rw-r--r--   0        0        0     2015 2023-07-09 11:58:43.817701 pytint-1.0.0/pytint/pytint.py
--rw-r--r--   0        0        0      394 2023-07-09 15:06:45.953919 pytint-1.0.0/pytint/pytint.pyi
--rw-r--r--   0        0        0     2292 2023-07-08 23:35:45.269535 pytint-1.0.0/pytint/svg_tool.py
--rw-r--r--   0        0        0      406 2023-07-09 15:07:29.203785 pytint-1.0.0/pytint/svg_tool.pyi
--rw-r--r--   0        0        0     2305 2023-07-07 21:45:05.696406 pytint-1.0.0/pytint/tint.py
--rw-r--r--   0        0        0      670 2023-07-09 15:08:32.560257 pytint-1.0.0/pytint/tint.pyi
--rw-r--r--   0        0        0     9503 1970-01-01 00:00:00.000000 pytint-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35123 2023-06-21 17:12:40.000000 pytint-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5362 2023-07-10 21:32:02.718642 pytint-1.0.1/README.md
+-rw-r--r--   0        0        0      491 2023-07-10 21:42:32.220751 pytint-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1526 2023-07-08 21:49:59.618008 pytint-1.0.1/pytint/__init__.py
+-rw-r--r--   0        0        0      239 2023-07-09 15:05:39.527460 pytint-1.0.1/pytint/__init__.pyi
+-rw-r--r--   0        0        0     2923 2023-07-09 12:11:22.921225 pytint-1.0.1/pytint/colors.py
+-rw-r--r--   0        0        0      459 2023-07-09 15:05:39.527460 pytint-1.0.1/pytint/colors.pyi
+-rw-r--r--   0        0        0     2015 2023-07-09 11:58:43.817701 pytint-1.0.1/pytint/pytint.py
+-rw-r--r--   0        0        0      394 2023-07-09 15:06:45.953919 pytint-1.0.1/pytint/pytint.pyi
+-rw-r--r--   0        0        0     2292 2023-07-08 23:35:45.269535 pytint-1.0.1/pytint/svg_tool.py
+-rw-r--r--   0        0        0      406 2023-07-09 15:07:29.203785 pytint-1.0.1/pytint/svg_tool.pyi
+-rw-r--r--   0        0        0     2519 2023-07-10 21:40:22.874337 pytint-1.0.1/pytint/tint.py
+-rw-r--r--   0        0        0      670 2023-07-09 15:08:32.560257 pytint-1.0.1/pytint/tint.pyi
+-rw-r--r--   0        0        0     5959 1970-01-01 00:00:00.000000 pytint-1.0.1/PKG-INFO
```

### Comparing `pytint-1.0.0/LICENSE` & `pytint-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytint-1.0.0/pytint/__init__.py` & `pytint-1.0.1/pytint/__init__.py`

 * *Files identical despite different names*

### Comparing `pytint-1.0.0/pytint/colors.py` & `pytint-1.0.1/pytint/colors.py`

 * *Files identical despite different names*

### Comparing `pytint-1.0.0/pytint/pytint.py` & `pytint-1.0.1/pytint/pytint.py`

 * *Files identical despite different names*

### Comparing `pytint-1.0.0/pytint/svg_tool.py` & `pytint-1.0.1/pytint/svg_tool.py`

 * *Files identical despite different names*

### Comparing `pytint-1.0.0/pytint/tint.py` & `pytint-1.0.1/pytint/tint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from . import PRIMARY, SECONDARY, BACKGROUND, DETAIL, INVERSE_BG
 
 
 class Tint:
+    """this is only here to make the process more modular
+    use `PyTint().tint_svg()` instead.
+    """
+
     def __init__(self, svg_in: str) -> None:
         self.__primary = PRIMARY
         self.__secondary = SECONDARY
         self.__background = BACKGROUND
         self.__detail = DETAIL
         self.__inverse_background = INVERSE_BG
         self.__svg_in = svg_in
@@ -25,14 +29,18 @@
         for scheme in self.__detail:
             self.__svg_in = self.__svg_in.replace(scheme, alt)
         for scheme in self.__inverse_background:
             self.__svg_in = self.__svg_in.replace(scheme, difference)
 
 
 class BatchTint:
+    """this is only here to make the process more modular
+    use `PyTint().tint_batch()` instead.
+    """
+
     def __init__(self, svg_dict: dict[str, str]) -> None:
         self.__svg_dict = svg_dict
 
     def get_svg_dict(self) -> dict[str, str]:
         return self.__svg_dict
 
     def tint_colors(self, default: str, accent: str):
```

### Comparing `pytint-1.0.0/pytint/tint.pyi` & `pytint-1.0.1/pytint/tint.pyi`

 * *Files identical despite different names*

