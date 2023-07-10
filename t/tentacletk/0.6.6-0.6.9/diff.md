# Comparing `tmp/tentacletk-0.6.6.tar.gz` & `tmp/tentacletk-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tentacletk-0.6.6.tar", last modified: Fri Apr  7 13:24:07 2023, max compression
+gzip compressed data, was "tentacletk-0.6.9.tar", last modified: Mon Jul 10 18:21:57 2023, max compression
```

## Comparing `tentacletk-0.6.6.tar` & `tentacletk-0.6.9.tar`

### file list

```diff
@@ -1,159 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 13:24:07.000767 tentacletk-0.6.6/
--rw-rw-rw-   0        0        0       24 2023-03-28 23:37:53.000000 tentacletk-0.6.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2460 2023-04-07 13:24:07.000767 tentacletk-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-07 13:24:07.001786 tentacletk-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0     2186 2023-04-06 23:23:20.000000 tentacletk-0.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 13:24:06.140186 tentacletk-0.6.6/tentacle/
--rw-rw-rw-   0        0        0     1740 2023-04-07 13:24:03.000000 tentacletk-0.6.6/tentacle/__init__.py
--rw-rw-rw-   0        0        0    12360 2023-04-06 23:12:50.000000 tentacletk-0.6.6/tentacle/overlay.py
-drwxrwxrwx   0        0        0        0 2023-04-07 13:24:06.332619 tentacletk-0.6.6/tentacle/slots/
--rw-rw-rw-   0        0        0     3836 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/__init__.py
--rw-rw-rw-   0        0        0     1822 2023-04-06 00:58:24.000000 tentacletk-0.6.6/tentacle/slots/animation.py
-drwxrwxrwx   0        0        0        0 2023-04-07 13:24:06.545625 tentacletk-0.6.6/tentacle/slots/blender/
--rw-rw-rw-   0        0        0     1162 2023-04-06 00:58:24.000000 tentacletk-0.6.6/tentacle/slots/blender/__init__.py
--rw-rw-rw-   0        0        0     2869 2023-04-06 00:58:24.000000 tentacletk-0.6.6/tentacle/slots/blender/animation_blender.py
--rw-rw-rw-   0        0        0    17195 2023-04-06 00:58:24.000000 tentacletk-0.6.6/tentacle/slots/blender/cameras_blender.py
--rw-rw-rw-   0        0        0     3043 2023-04-06 00:58:24.000000 tentacletk-0.6.6/tentacle/slots/blender/convert_blender.py
--rw-rw-rw-   0        0        0     4142 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/blender/crease_blender.py
--rw-rw-rw-   0        0        0    11953 2023-04-06 00:58:24.000000 tentacletk-0.6.6/tentacle/slots/blender/create_blender.py
--rw-rw-rw-   0        0        0      936 2023-04-06 00:58:24.000000 tentacletk-0.6.6/tentacle/slots/blender/deformation_blender.py
--rw-rw-rw-   0        0        0     4399 2023-04-06 00:58:24.000000 tentacletk-0.6.6/tentacle/slots/blender/display_blender.py
--rw-rw-rw-   0        0        0    14112 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/blender/duplicate_blender.py
--rw-rw-rw-   0        0        0      878 2023-04-06 00:58:24.000000 tentacletk-0.6.6/tentacle/slots/blender/dynLayout_blender.py
--rw-rw-rw-   0        0        0    21181 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/blender/edit_blender.py
--rw-rw-rw-   0        0        0     9522 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/editors_blender.py
--rw-rw-rw-   0        0        0    15533 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/file_blender.py
--rw-rw-rw-   0        0        0     4578 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/init_blender.py
--rw-rw-rw-   0        0        0      985 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/lighting_blender.py
--rw-rw-rw-   0        0        0     1982 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/blender/main_blender.py
--rw-rw-rw-   0        0        0    16190 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/blender/materials_blender.py
--rw-rw-rw-   0        0        0     6423 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/mirror_blender.py
--rw-rw-rw-   0        0        0     9786 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/normals_blender.py
--rw-rw-rw-   0        0        0    21551 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/blender/nurbs_blender.py
--rw-rw-rw-   0        0        0     2963 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/pivot_blender.py
--rw-rw-rw-   0        0        0    15693 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/polygons_blender.py
--rw-rw-rw-   0        0        0     3913 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/preferences_blender.py
--rw-rw-rw-   0        0        0     2860 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/rendering_blender.py
--rw-rw-rw-   0        0        0    18300 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/blender/rigging_blender.py
--rw-rw-rw-   0        0        0     4775 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/blender/scene_blender.py
--rw-rw-rw-   0        0        0     1644 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/scripting_blender.py
--rw-rw-rw-   0        0        0    13684 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/blender/selection_blender.py
--rw-rw-rw-   0        0        0     5658 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/blender/subdivision_blender.py
--rw-rw-rw-   0        0        0     2267 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/symmetry_blender.py
--rw-rw-rw-   0        0        0    33457 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/blender/transform_blender.py
--rw-rw-rw-   0        0        0     1187 2023-04-06 00:58:25.000000 tentacletk-0.6.6/tentacle/slots/blender/utilities_blender.py
--rw-rw-rw-   0        0        0    19062 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/blender/uv_blender.py
--rw-rw-rw-   0        0        0      838 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/blender/vfx_blender.py
--rw-rw-rw-   0        0        0      390 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/cameras.py
--rw-rw-rw-   0        0        0      795 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/convert.py
--rw-rw-rw-   0        0        0     5652 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/crease.py
--rw-rw-rw-   0        0        0     2086 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/create.py
--rw-rw-rw-   0        0        0      478 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/deformation.py
--rw-rw-rw-   0        0        0      466 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/display.py
--rw-rw-rw-   0        0        0     3592 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/duplicate.py
--rw-rw-rw-   0        0        0      638 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/dynLayout.py
--rw-rw-rw-   0        0        0     2723 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/edit.py
--rw-rw-rw-   0        0        0      201 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/editors.py
--rw-rw-rw-   0        0        0     4265 2023-04-06 23:27:47.000000 tentacletk-0.6.6/tentacle/slots/file.py
--rw-rw-rw-   0        0        0      200 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/init.py
--rw-rw-rw-   0        0        0      355 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/lighting.py
--rw-rw-rw-   0        0        0     1241 2023-04-06 00:58:26.000000 tentacletk-0.6.6/tentacle/slots/main.py
--rw-rw-rw-   0        0        0     3648 2023-04-06 00:58:27.000000 tentacletk-0.6.6/tentacle/slots/materials.py
-drwxrwxrwx   0        0        0        0 2023-04-07 13:24:06.764654 tentacletk-0.6.6/tentacle/slots/max/
--rw-rw-rw-   0        0        0    16091 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/max/__init__.py
--rw-rw-rw-   0        0        0     5936 2023-04-06 00:58:27.000000 tentacletk-0.6.6/tentacle/slots/max/animation_max.py
--rw-rw-rw-   0        0        0     9528 2023-04-06 00:58:27.000000 tentacletk-0.6.6/tentacle/slots/max/cameras_max.py
--rw-rw-rw-   0        0        0     2976 2023-04-06 00:58:27.000000 tentacletk-0.6.6/tentacle/slots/max/convert_max.py
--rw-rw-rw-   0        0        0     3858 2023-04-06 00:58:27.000000 tentacletk-0.6.6/tentacle/slots/max/crease_max.py
--rw-rw-rw-   0        0        0     9368 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/max/create_max.py
--rw-rw-rw-   0        0        0      865 2023-04-06 00:58:27.000000 tentacletk-0.6.6/tentacle/slots/max/deformation_max.py
--rw-rw-rw-   0        0        0     4491 2023-04-06 00:58:27.000000 tentacletk-0.6.6/tentacle/slots/max/display_max.py
--rw-rw-rw-   0        0        0    12865 2023-04-06 00:58:27.000000 tentacletk-0.6.6/tentacle/slots/max/duplicate_max.py
--rw-rw-rw-   0        0        0      809 2023-04-06 00:58:27.000000 tentacletk-0.6.6/tentacle/slots/max/dynLayout_max.py
--rw-rw-rw-   0        0        0    11599 2023-04-06 00:58:28.000000 tentacletk-0.6.6/tentacle/slots/max/edit_max.py
--rw-rw-rw-   0        0        0    11315 2023-04-06 00:58:28.000000 tentacletk-0.6.6/tentacle/slots/max/editors_max.py
--rw-rw-rw-   0        0        0    13244 2023-04-06 00:58:28.000000 tentacletk-0.6.6/tentacle/slots/max/file_max.py
--rw-rw-rw-   0        0        0     4077 2023-04-06 00:58:28.000000 tentacletk-0.6.6/tentacle/slots/max/init_max.py
--rw-rw-rw-   0        0        0      919 2023-04-06 00:58:28.000000 tentacletk-0.6.6/tentacle/slots/max/lighting_max.py
--rw-rw-rw-   0        0        0      481 2023-04-06 00:58:28.000000 tentacletk-0.6.6/tentacle/slots/max/main_max.py
--rw-rw-rw-   0        0        0    23407 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/max/materials_max.py
--rw-rw-rw-   0        0        0     6869 2023-04-06 00:58:28.000000 tentacletk-0.6.6/tentacle/slots/max/mirror_max.py
--rw-rw-rw-   0        0        0     6732 2023-04-06 00:58:29.000000 tentacletk-0.6.6/tentacle/slots/max/normals_max.py
--rw-rw-rw-   0        0        0     6478 2023-04-06 00:58:29.000000 tentacletk-0.6.6/tentacle/slots/max/nurbs_max.py
--rw-rw-rw-   0        0        0     6257 2023-04-06 00:58:29.000000 tentacletk-0.6.6/tentacle/slots/max/pivot_max.py
--rw-rw-rw-   0        0        0    12140 2023-04-06 00:58:29.000000 tentacletk-0.6.6/tentacle/slots/max/polygons_max.py
--rw-rw-rw-   0        0        0     3410 2023-04-06 00:58:30.000000 tentacletk-0.6.6/tentacle/slots/max/preferences_max.py
--rw-rw-rw-   0        0        0     2418 2023-04-06 00:58:30.000000 tentacletk-0.6.6/tentacle/slots/max/rendering_max.py
--rw-rw-rw-   0        0        0    13735 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/max/rigging_max.py
--rw-rw-rw-   0        0        0     4184 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/max/scene_max.py
--rw-rw-rw-   0        0        0     1586 2023-04-06 00:58:31.000000 tentacletk-0.6.6/tentacle/slots/max/scripting_max.py
--rw-rw-rw-   0        0        0    18110 2023-04-06 00:58:31.000000 tentacletk-0.6.6/tentacle/slots/max/selection_max.py
--rw-rw-rw-   0        0        0     4980 2023-04-06 00:58:31.000000 tentacletk-0.6.6/tentacle/slots/max/subdivision_max.py
--rw-rw-rw-   0        0        0     2536 2023-04-06 00:58:31.000000 tentacletk-0.6.6/tentacle/slots/max/symmetry_max.py
--rw-rw-rw-   0        0        0    21275 2023-04-06 00:58:32.000000 tentacletk-0.6.6/tentacle/slots/max/transform_max.py
--rw-rw-rw-   0        0        0     1143 2023-04-06 00:58:32.000000 tentacletk-0.6.6/tentacle/slots/max/utilities_max.py
--rw-rw-rw-   0        0        0    11929 2023-04-06 00:58:32.000000 tentacletk-0.6.6/tentacle/slots/max/uv_max.py
--rw-rw-rw-   0        0        0      775 2023-04-06 00:58:32.000000 tentacletk-0.6.6/tentacle/slots/max/vfx_max.py
-drwxrwxrwx   0        0        0        0 2023-04-07 13:24:06.978659 tentacletk-0.6.6/tentacle/slots/maya/
--rw-rw-rw-   0        0        0     3463 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/maya/__init__.py
--rw-rw-rw-   0        0        0     2788 2023-04-06 00:58:33.000000 tentacletk-0.6.6/tentacle/slots/maya/animation_maya.py
--rw-rw-rw-   0        0        0    17443 2023-04-06 00:58:33.000000 tentacletk-0.6.6/tentacle/slots/maya/cameras_maya.py
--rw-rw-rw-   0        0        0     3544 2023-04-06 00:58:34.000000 tentacletk-0.6.6/tentacle/slots/maya/convert_maya.py
--rw-rw-rw-   0        0        0     4084 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/maya/crease_maya.py
--rw-rw-rw-   0        0        0    11656 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/maya/create_maya.py
--rw-rw-rw-   0        0        0      868 2023-04-06 00:58:34.000000 tentacletk-0.6.6/tentacle/slots/maya/deformation_maya.py
--rw-rw-rw-   0        0        0     4421 2023-04-06 00:58:35.000000 tentacletk-0.6.6/tentacle/slots/maya/display_maya.py
--rw-rw-rw-   0        0        0    17523 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/maya/duplicate_maya.py
--rw-rw-rw-   0        0        0      812 2023-04-06 00:58:35.000000 tentacletk-0.6.6/tentacle/slots/maya/dynLayout_maya.py
--rw-rw-rw-   0        0        0    13364 2023-04-06 00:58:35.000000 tentacletk-0.6.6/tentacle/slots/maya/edit_maya.py
--rw-rw-rw-   0        0        0    10694 2023-04-06 00:58:36.000000 tentacletk-0.6.6/tentacle/slots/maya/editors_maya.py
--rw-rw-rw-   0        0        0    17501 2023-04-06 00:58:36.000000 tentacletk-0.6.6/tentacle/slots/maya/file_maya.py
--rw-rw-rw-   0        0        0     5043 2023-04-06 00:58:36.000000 tentacletk-0.6.6/tentacle/slots/maya/init_maya.py
--rw-rw-rw-   0        0        0      920 2023-04-06 00:58:36.000000 tentacletk-0.6.6/tentacle/slots/maya/lighting_maya.py
--rw-rw-rw-   0        0        0     1924 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/maya/main_maya.py
--rw-rw-rw-   0        0        0    16392 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/maya/materials_maya.py
--rw-rw-rw-   0        0        0     8087 2023-04-06 00:58:37.000000 tentacletk-0.6.6/tentacle/slots/maya/mirror_maya.py
--rw-rw-rw-   0        0        0    11979 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/maya/normals_maya.py
--rw-rw-rw-   0        0        0    21461 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/maya/nurbs_maya.py
--rw-rw-rw-   0        0        0     3123 2023-04-06 00:58:38.000000 tentacletk-0.6.6/tentacle/slots/maya/pivot_maya.py
--rw-rw-rw-   0        0        0    15152 2023-04-06 00:58:38.000000 tentacletk-0.6.6/tentacle/slots/maya/polygons_maya.py
--rw-rw-rw-   0        0        0     3664 2023-04-06 00:58:39.000000 tentacletk-0.6.6/tentacle/slots/maya/preferences_maya.py
--rw-rw-rw-   0        0        0     3229 2023-04-06 00:58:39.000000 tentacletk-0.6.6/tentacle/slots/maya/rendering_maya.py
--rw-rw-rw-   0        0        0    12606 2023-04-06 00:58:39.000000 tentacletk-0.6.6/tentacle/slots/maya/rigging_maya.py
--rw-rw-rw-   0        0        0     2774 2023-04-06 00:58:39.000000 tentacletk-0.6.6/tentacle/slots/maya/scene_maya.py
--rw-rw-rw-   0        0        0     1582 2023-04-06 00:58:40.000000 tentacletk-0.6.6/tentacle/slots/maya/scripting_maya.py
--rw-rw-rw-   0        0        0    15315 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/maya/selection_maya.py
--rw-rw-rw-   0        0        0     6208 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/maya/subdivision_maya.py
--rw-rw-rw-   0        0        0     2249 2023-04-06 00:58:41.000000 tentacletk-0.6.6/tentacle/slots/maya/symmetry_maya.py
--rw-rw-rw-   0        0        0    20821 2023-04-06 00:58:41.000000 tentacletk-0.6.6/tentacle/slots/maya/transform_maya.py
--rw-rw-rw-   0        0        0     1131 2023-04-06 00:58:41.000000 tentacletk-0.6.6/tentacle/slots/maya/utilities_maya.py
--rw-rw-rw-   0        0        0    23371 2023-04-06 23:28:21.000000 tentacletk-0.6.6/tentacle/slots/maya/uv_maya.py
--rw-rw-rw-   0        0        0      778 2023-04-06 00:58:42.000000 tentacletk-0.6.6/tentacle/slots/maya/vfx_maya.py
--rw-rw-rw-   0        0        0     3331 2023-04-06 00:58:43.000000 tentacletk-0.6.6/tentacle/slots/mirror.py
--rw-rw-rw-   0        0        0     2212 2023-04-06 00:58:43.000000 tentacletk-0.6.6/tentacle/slots/normals.py
--rw-rw-rw-   0        0        0     4161 2023-04-06 00:58:43.000000 tentacletk-0.6.6/tentacle/slots/nurbs.py
--rw-rw-rw-   0        0        0      876 2023-04-06 00:58:44.000000 tentacletk-0.6.6/tentacle/slots/pivot.py
--rw-rw-rw-   0        0        0     4778 2023-04-06 23:06:49.000000 tentacletk-0.6.6/tentacle/slots/polygons.py
--rw-rw-rw-   0        0        0      726 2023-04-06 00:58:44.000000 tentacletk-0.6.6/tentacle/slots/preferences.py
--rw-rw-rw-   0        0        0      475 2023-04-06 00:58:44.000000 tentacletk-0.6.6/tentacle/slots/rendering.py
--rw-rw-rw-   0        0        0     4546 2023-04-06 00:58:45.000000 tentacletk-0.6.6/tentacle/slots/rigging.py
--rw-rw-rw-   0        0        0     2092 2023-04-06 00:58:45.000000 tentacletk-0.6.6/tentacle/slots/scene.py
--rw-rw-rw-   0        0        0      686 2023-04-06 00:58:45.000000 tentacletk-0.6.6/tentacle/slots/scripting.py
--rw-rw-rw-   0        0        0     8294 2023-04-06 00:58:45.000000 tentacletk-0.6.6/tentacle/slots/selection.py
--rw-rw-rw-   0        0        0      325 2023-04-06 00:58:45.000000 tentacletk-0.6.6/tentacle/slots/subdivision.py
--rw-rw-rw-   0        0        0     1617 2023-04-06 00:58:46.000000 tentacletk-0.6.6/tentacle/slots/symmetry.py
--rw-rw-rw-   0        0        0     6229 2023-04-06 00:58:46.000000 tentacletk-0.6.6/tentacle/slots/transform.py
--rw-rw-rw-   0        0        0      477 2023-04-06 00:58:46.000000 tentacletk-0.6.6/tentacle/slots/utilities.py
--rw-rw-rw-   0        0        0     7517 2023-04-06 00:58:46.000000 tentacletk-0.6.6/tentacle/slots/uv.py
--rw-rw-rw-   0        0        0      456 2023-04-06 00:58:47.000000 tentacletk-0.6.6/tentacle/slots/vfx.py
--rw-rw-rw-   0        0        0    22310 2023-04-07 13:22:05.000000 tentacletk-0.6.6/tentacle/tcl.py
--rw-rw-rw-   0        0        0     3525 2023-04-06 00:58:54.000000 tentacletk-0.6.6/tentacle/tcl_blender.py
--rw-rw-rw-   0        0        0     5108 2023-04-06 00:58:54.000000 tentacletk-0.6.6/tentacle/tcl_max.py
--rw-rw-rw-   0        0        0     5200 2023-04-06 00:58:54.000000 tentacletk-0.6.6/tentacle/tcl_maya.py
-drwxrwxrwx   0        0        0        0 2023-04-07 13:24:06.984254 tentacletk-0.6.6/tentacle/ui/
--rw-rw-rw-   0        0        0      839 2023-04-06 23:28:45.000000 tentacletk-0.6.6/tentacle/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 13:24:06.999267 tentacletk-0.6.6/tentacletk.egg-info/
--rw-rw-rw-   0        0        0     2460 2023-04-07 13:24:05.000000 tentacletk-0.6.6/tentacletk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4993 2023-04-07 13:24:06.000000 tentacletk-0.6.6/tentacletk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 13:24:05.000000 tentacletk-0.6.6/tentacletk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-07 13:24:05.000000 tentacletk-0.6.6/tentacletk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 18:21:57.464597 tentacletk-0.6.9/
+-rw-rw-rw-   0        0        0     7815 2023-06-22 17:46:01.000000 tentacletk-0.6.9/COPYING.LESSER
+-rw-rw-rw-   0        0        0       24 2023-03-28 23:37:53.000000 tentacletk-0.6.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2951 2023-07-10 18:21:57.464597 tentacletk-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-10 18:21:57.465599 tentacletk-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1447 2023-07-10 18:21:48.000000 tentacletk-0.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:21:57.408599 tentacletk-0.6.9/tentacle/
+-rw-rw-rw-   0        0        0     1581 2023-07-10 18:21:54.000000 tentacletk-0.6.9/tentacle/__init__.py
+-rw-rw-rw-   0        0        0    14113 2023-07-02 22:35:29.000000 tentacletk-0.6.9/tentacle/overlay.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:21:57.409597 tentacletk-0.6.9/tentacle/slots/
+-rw-rw-rw-   0        0        0     1535 2023-07-02 22:34:48.000000 tentacletk-0.6.9/tentacle/slots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:21:57.442597 tentacletk-0.6.9/tentacle/slots/maya/
+-rw-rw-rw-   0        0        0      758 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/__init__.py
+-rw-rw-rw-   0        0        0     4877 2023-07-01 23:43:08.000000 tentacletk-0.6.9/tentacle/slots/maya/animation_maya.py
+-rw-rw-rw-   0        0        0    13291 2023-07-07 13:31:21.000000 tentacletk-0.6.9/tentacle/slots/maya/cameras_maya.py
+-rw-rw-rw-   0        0        0     4554 2023-07-07 14:07:28.000000 tentacletk-0.6.9/tentacle/slots/maya/convert_maya.py
+-rw-rw-rw-   0        0        0    10767 2023-07-01 23:43:08.000000 tentacletk-0.6.9/tentacle/slots/maya/crease_maya.py
+-rw-rw-rw-   0        0        0    13166 2023-07-07 14:11:56.000000 tentacletk-0.6.9/tentacle/slots/maya/create_maya.py
+-rw-rw-rw-   0        0        0      534 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/deformation_maya.py
+-rw-rw-rw-   0        0        0     4939 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/display_maya.py
+-rw-rw-rw-   0        0        0    25512 2023-07-07 13:33:24.000000 tentacletk-0.6.9/tentacle/slots/maya/duplicate_maya.py
+-rw-rw-rw-   0        0        0    18624 2023-07-07 17:35:30.000000 tentacletk-0.6.9/tentacle/slots/maya/edit_maya.py
+-rw-rw-rw-   0        0        0    12380 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/editors_maya.py
+-rw-rw-rw-   0        0        0    12553 2023-07-07 14:05:51.000000 tentacletk-0.6.9/tentacle/slots/maya/file_maya.py
+-rw-rw-rw-   0        0        0     6919 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/init_maya.py
+-rw-rw-rw-   0        0        0      629 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/lighting_maya.py
+-rw-rw-rw-   0        0        0     3265 2023-06-23 21:19:10.000000 tentacletk-0.6.9/tentacle/slots/maya/main_maya.py
+-rw-rw-rw-   0        0        0    10735 2023-07-10 16:59:48.000000 tentacletk-0.6.9/tentacle/slots/maya/materials_maya.py
+-rw-rw-rw-   0        0        0    12955 2023-07-01 23:43:08.000000 tentacletk-0.6.9/tentacle/slots/maya/mirror_maya.py
+-rw-rw-rw-   0        0        0     9340 2023-07-01 23:43:08.000000 tentacletk-0.6.9/tentacle/slots/maya/normals_maya.py
+-rw-rw-rw-   0        0        0    30767 2023-07-07 14:11:04.000000 tentacletk-0.6.9/tentacle/slots/maya/nurbs_maya.py
+-rw-rw-rw-   0        0        0     3918 2023-07-01 23:43:08.000000 tentacletk-0.6.9/tentacle/slots/maya/pivot_maya.py
+-rw-rw-rw-   0        0        0    23332 2023-07-03 03:10:09.000000 tentacletk-0.6.9/tentacle/slots/maya/polygons_maya.py
+-rw-rw-rw-   0        0        0     3153 2023-07-07 13:31:33.000000 tentacletk-0.6.9/tentacle/slots/maya/preferences_maya.py
+-rw-rw-rw-   0        0        0     3415 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/rendering_maya.py
+-rw-rw-rw-   0        0        0    23526 2023-07-07 17:35:30.000000 tentacletk-0.6.9/tentacle/slots/maya/rigging_maya.py
+-rw-rw-rw-   0        0        0     4076 2023-07-01 23:43:08.000000 tentacletk-0.6.9/tentacle/slots/maya/scene_maya.py
+-rw-rw-rw-   0        0        0    27172 2023-07-07 19:04:50.000000 tentacletk-0.6.9/tentacle/slots/maya/selection_maya.py
+-rw-rw-rw-   0        0        0     5853 2023-06-23 21:19:10.000000 tentacletk-0.6.9/tentacle/slots/maya/subdivision_maya.py
+-rw-rw-rw-   0        0        0     2927 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/symmetry_maya.py
+-rw-rw-rw-   0        0        0    25170 2023-07-07 14:13:18.000000 tentacletk-0.6.9/tentacle/slots/maya/transform_maya.py
+-rw-rw-rw-   0        0        0      957 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/utilities_maya.py
+-rw-rw-rw-   0        0        0    22998 2023-07-07 14:11:36.000000 tentacletk-0.6.9/tentacle/slots/maya/uv_maya.py
+-rw-rw-rw-   0        0        0      624 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/vfx_maya.py
+-rw-rw-rw-   0        0        0    21461 2023-07-03 14:35:57.000000 tentacletk-0.6.9/tentacle/tcl.py
+-rw-rw-rw-   0        0        0    25342 2023-06-06 00:33:56.000000 tentacletk-0.6.9/tentacle/tcl.py.bak
+-rw-rw-rw-   0        0        0     3561 2023-07-02 22:31:43.000000 tentacletk-0.6.9/tentacle/tcl_blender.py
+-rw-rw-rw-   0        0        0     4885 2023-07-02 22:30:32.000000 tentacletk-0.6.9/tentacle/tcl_max.py
+-rw-rw-rw-   0        0        0     2930 2023-07-02 22:33:24.000000 tentacletk-0.6.9/tentacle/tcl_maya.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:21:57.443596 tentacletk-0.6.9/tentacle/ui/
+-rw-rw-rw-   0        0        0      511 2023-07-02 22:34:35.000000 tentacletk-0.6.9/tentacle/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:21:57.462597 tentacletk-0.6.9/tentacletk.egg-info/
+-rw-rw-rw-   0        0        0     2951 2023-07-10 18:21:57.000000 tentacletk-0.6.9/tentacletk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1511 2023-07-10 18:21:57.000000 tentacletk-0.6.9/tentacletk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 18:21:57.000000 tentacletk-0.6.9/tentacletk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 18:21:57.000000 tentacletk-0.6.9/tentacletk.egg-info/top_level.txt
```

### Comparing `tentacletk-0.6.6/PKG-INFO` & `tentacletk-0.6.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 Metadata-Version: 2.1
 Name: tentacletk
-Version: 0.6.6
-Summary: Tentacle is a marking menu style UI and toolkit derived from a QStackedWidget and constructed using the uitk backend. It aims to bring a similar UI experience across multiple DCC modeling applications that support the PySide2 GUI framework.
+Version: 0.6.9
+Summary: A Python3/PySide2 marking menu style toolkit for Maya, 3ds Max, and Blender.
 Home-page: https://github.com/m3trik/tentacle
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
+License: LGPLv3
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: COPYING.LESSER
 
-## Tentacle
+[![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.en.html)
 
-\*\*personal project. work in progress ..\*\*
+# Tentacle: A Python3/PySide2 Marking Menu and UI Toolkit
 
+Tentacle is a Python3/PySide2 marking menu and UI toolkit designed for Maya, 3ds Max, Blender, and any other DCC app that supports the PySide2 framework. It is a personal project and is currently a work in progress.
 
-##### 
----
-<!-- short_description_start -->
-Tentacle is a marking menu style UI and toolkit derived from a QStackedWidget and constructed using the uitk backend. It aims to bring a similar UI experience across multiple DCC modeling applications that support the PySide2 GUI framework.
-<!-- short_description_end -->
+## Design
 
-![alt text](https://raw.githubusercontent.com/m3trik/tentacle/master/docs/toolkit_demo.gif) \*Example re-opening the last scene, renaming a material, and selecting geometry by that material.
+Tentacle is a dynamic UI toolkit with a marking menu style UI derived from a QStackedWidget. The switchboard module, derived from QUiLoader, provides properties and convenience methods that allow quick and easy getting/setting of relevant UI and widget data across modules.
 
-##
+## Example
 
+The following example demonstrates re-opening the last scene, renaming a material, and selecting geometry by that material.
 
-## Design:
+![Example](https://raw.githubusercontent.com/m3trik/tentacle/master/docs/toolkit_demo.gif)
 
-![alt text](https://raw.githubusercontent.com/m3trik/tentacle/master/docs/dependancy_graph.jpg)
+## Structure
 
+The structure of the project is as follows:
 
-Module | Description
-------- | -------
-[tcl](https://github.com/m3trik/tentacle/blob/main/tentacle/tcl.py) | *A Custom QStackedWidget that handles UI hierarchy navigation.*
-[overlay](https://github.com/m3trik/tentacle/blob/main/tentacle/overlay.py) | *Tracks cursor position and UI hierarchy to generate paint events that overlay the parent widget.*
-[slots](https://github.com/m3trik/tentacle/blob/main/tentacle/slots) | *The source directory for the various slot connection modules.*
-[ui](https://github.com/m3trik/tentacle/blob/main/tentacle/slots) | *The source directory for dynamic UI files.*
+![Structure](https://raw.githubusercontent.com/m3trik/tentacle/master/docs/dependancy_graph.jpg)
 
----
+| Module | Description |
+| ------- | ----------- |
+| [tcl](https://github.com/m3trik/uitk/blob/main/tentacle/tcl.py) | Handles main GUI construction for the marking menu. |
+| [overlay](https://github.com/m3trik/uitk/blob/main/tentacle/overlay.py) | Tracks cursor position and UI hierarchy to generate paint events that overlay its parent widget. |
+| [ui](https://github.com/m3trik/uitk/blob/main/tentacle/events.py) | Location of the dynamic UI files. |
+| [slots](https://github.com/m3trik/uitk/blob/main/tentacle/slots) | Location of the various slot modules. |
 
-## Installation:
+## Installation
 
-#####
+Add the `tentacle` folder to a directory on your Python path, or install via pip in a command line window using:
 
-To install:
-install via pip in a command line window using:
-```
+```bash
 python -m pip install tentacletk
 ```
-
+## Usage
 To launch the marking menu:
-For Maya:
-Add a macro to a hotkey similar to the following:
+
+For Maya, add a macro to a hotkey similar to the following:
 ```python
-from tentacle import tcl_maya
+from uitk import tcl_maya
 tcl_maya.show(key_show='Key_F12')
 ```
 
-For 3ds Max:
-Add a macro to a hotkey similar to the following:
-```python
+For 3ds Max, add a macro to a hotkey similar to the following:
+```maxscript
 macroScript main_max
 category: "_macros.ui"
 silentErrors: false
 autoUndoEnabled: false
 (
-	python.Execute "from tentacle import tcl_max"
+	python.Execute "from uitk import tcl_max"
 	python.Execute "tcl_max.show(key_show='Key_F12')"
 )
 ```
+Again, please note that this is a personal project and is currently a work in progress. Contributions are welcome.
```

### Comparing `tentacletk-0.6.6/tentacle/__init__.py` & `tentacletk-0.6.9/tentacle/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,49 @@
 # !/usr/bin/python
 # coding=utf-8
 import sys
 
-
-__package__ = 'tentacle'
-__version__ = '0.6.6'
+__package__ = "tentacle"
+__version__ = '0.6.9'
 
 
 def greeting(string, outputToConsole=True):
-	'''Format a string using preset variables.
-
-	Parameters:
-		string (str): The greeting to format as a string with placeholders using the below keywords. 
-			ex. 'Good {hr}! You are using {modver} with {pyver}.'
-			{hr} - Gives the current time of day (morning, afternoon, evening)
-			{pyver} - The python interpreter version.
-			{modver} - This modules version.
-		outputToConsole = Print the greeting.
-
-	Return:
-		(str)
-
-	Example: greeting('Good {hr}! You are using {modver} with {pyver}.')
-	'''
-	import datetime
-	h = datetime.datetime.now().hour
-	hr = 'morning' if 5<=h<12 else 'afternoon' if h<18 else 'evening'
-
-	pyver = 'python v{}.{}.{}'.format(sys.version_info[0], sys.version_info[1], sys.version_info[2])
-
-	modver = 'tentacle v{}'.format(__version__)
-
-	result = string.format(hr=hr, pyver=pyver, modver=modver)
-
-	if outputToConsole:
-		print (result)
-	return result
+    """Format a string using preset variables.
 
-# --------------------------------------------------------------------------------------------
+    Parameters:
+            string (str): The greeting to format as a string with placeholders using the below keywords.
+                    ex. 'Good {hr}! You are using {modver} with {pyver}.'
+                    {hr} - Gives the current time of day (morning, afternoon, evening)
+                    {pyver} - The python interpreter version.
+                    {modver} - This modules version.
+            outputToConsole = Print the greeting.
 
+    Returns:
+            (str)
 
+    Example: greeting('Good {hr}! You are using {modver} with {pyver}.')
+    """
+    import datetime
 
+    h = datetime.datetime.now().hour
+    hr = "morning" if 5 <= h < 12 else "afternoon" if h < 18 else "evening"
 
+    pyver = "python v{}.{}.{}".format(
+        sys.version_info[0], sys.version_info[1], sys.version_info[2]
+    )
 
+    modver = "tentacle v{}".format(__version__)
 
+    result = string.format(hr=hr, pyver=pyver, modver=modver)
 
+    if outputToConsole:
+        print(result)
+    return result
 
 
 # --------------------------------------------------------------------------------------------
 
-greeting('Good {hr}! You are using {modver} with {pyver}.')
+greeting("Good {hr}! You are using {modver} with {pyver}.")
 
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
-
-
-# --------------------------------------------------------------------------------------------
-# deprecated:
-# --------------------------------------------------------------------------------------------
```

### Comparing `tentacletk-0.6.6/tentacle/slots/blender/subdivision_blender.py` & `tentacletk-0.6.9/tentacle/slots/maya/subdivision_maya.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,176 +1,155 @@
 # !/usr/bin/python
 # coding=utf-8
-from tentacle.slots.blender import *
-from tentacle.slots.subdivision import Subdivision
-
-
-
-class Subdivision_blender(Subdivision, Slots_blender):
-	def __init__(self, *args, **kwargs):
-		Slots_blender.__init__(self, *args, **kwargs)
-		Subdivision.__init__(self, *args, **kwargs)
-
-		ctx = self.sb.subdivision.draggable_header.ctxMenu
-		if not ctx.containsMenuItems:
-			ctx.add(self.sb.ComboBox, setObjectName='cmb000', setToolTip='Subdivision Editiors.')
-			ctx.add(self.sb.ComboBox, setObjectName='cmb001', setToolTip='Smooth Proxy.')
-			ctx.add(self.sb.ComboBox, setObjectName='cmb002', setToolTip='Maya Subdivision Operations.')
-
-		cmb = self.sb.subdivision.draggable_header.ctxMenu.cmb000
-		items = ['Polygon Display Options']
-		cmb.addItems_(items, 'Subdivision Editiors')
-
-		cmb = self.sb.subdivision.draggable_header.ctxMenu.cmb001
-		items = ['Create Subdiv Proxy','Remove Subdiv Proxy Mirror','Crease Tool','Toggle Subdiv Proxy Display', 'Both Proxy and Subdiv Display']
-		cmb.addItems_(items, 'Smooth Proxy')
-
-		cmb = self.sb.subdivision.draggable_header.ctxMenu.cmb002
-		items = ['Reduce Polygons','Add Divisions','Smooth']
-		cmb.addItems_(items, 'Maya Subdivision Operations')
-
-
-	def cmb000(self, index=-1):
-		'''Editors
-		'''
-		cmb = self.sb.subdivision.draggable_header.ctxMenu.cmb000
-
-		if index>0:
-			text = cmb.items[index]
-			if text=='Polygon Display Options':
-				pm.mel.CustomPolygonDisplayOptions() #Polygon Display Options #mel.eval("polysDisplaySetup 1;")
-			cmb.setCurrentIndex(0)
-
-
-	def cmb001(self, index=-1):
-		'''Smooth Proxy
-		'''
-		cmb = self.sb.subdivision.draggable_header.ctxMenu.cmb001
-
-		if index>0:
-			text = cmb.items[index]
-			if text=='Create Subdiv Proxy':
-				pm.mel.SmoothProxyOptions() #'Add polygons to the selected proxy objects.' #performSmoothProxy 1;
-			elif text=='Remove Subdiv Proxy Mirror':
-				pm.mel.UnmirrorSmoothProxyOptions() #'Create a single low resolution mesh for a mirrored proxy setup.' #performUnmirrorSmoothProxy 1;
-			elif text=='Crease Tool':
-				pm.mel.polyCreaseProperties() #'Harden or soften the edges of a smooth mesh preview.' #polyCreaseValues polyCreaseContext;
-			elif text=='Toggle Subdiv Proxy Display':
-				pm.mel.SmoothingDisplayToggle()	#'Toggle the display of smooth shapes.' #smoothingDisplayToggle 1;
-			elif text=='Both Proxy and Subdiv Display':
-				pm.mel.SmoothingDisplayShowBoth() #'Display both smooth shapes' #smoothingDisplayToggle 0;
-			cmb.setCurrentIndex(0)
-
-
-	def cmb002(self, index=-1):
-		'''Maya Subdivision Operations
-		'''
-		cmb = self.sb.subdivision.draggable_header.ctxMenu.cmb002
-
-		if index>0:
-			if index is cmb.items.index('Reduce Polygons'):
-				pm.mel.ReducePolygonOptions()
-			elif index is cmb.items.index('Add Divisions'):
-				pm.mel.SubdividePolygonOptions()
-			elif index is cmb.items.index('Smooth'):
-				pm.mel.performPolySmooth(1)
-			cmb.setCurrentIndex(0)
-
-
-	def s000(self, value=None):
-		'''Division Level
-		'''
-		value = self.sb.subdivision.s000.value()
-
-		shapes = pm.ls(sl=1, dag=1, leaf=1)
-		transforms = pm.listRelatives(shapes, p=True)
-		for obj in transforms:
-			if hasattr(obj, 'smoothLevel'):
-				self.setNodeAttributes(obj, {'smoothLevel':value})
-				pm.optionVar(intValue=['proxyDivisions', 1]) #subDiv proxy options: 'divisions'
-				print(obj+': Division Level: <hl>'+str(value)+'</hl>')
-
-
-	def s001(self, value=None):
-		'''Tesselation Level
-		'''
-		value = self.sb.subdivision.s001.value()
-
-		shapes = pm.ls(sl=1, dag=1, leaf=1)
-		transforms = pm.listRelatives(shapes, p=True)
-		for obj in transforms:
-			if hasattr(obj, 'smoothLevel'):
-				self.setNodeAttributes(obj, {'smoothTessLevel':value})
-				print(obj+': Tesselation Level: <hl>'+str(value)+'</hl>')
-
-
-	def b005(self):
-		'''Reduce
-		'''
-		pm.mel.polyReduce(version=1, keepCreaseEdgeWeight=1)
-		# pm.mel.ReducePolygon()
-
-
-	def b008(self):
-		'''Add Divisions - Subdivide Mesh
-		'''
-		pm.mel.SubdividePolygon()
-
-
-	def b009(self):
-		'''Smooth
-		'''
-		pm.mel.SmoothPolygon()
-
-
-	def b011(self):
-		'''Apply Smooth Preview
-		'''
-		pm.mel.performSmoothMeshPreviewToPolygon() #convert smooth mesh preview to polygons
-
-
-	@staticmethod
-	def smoothProxy():
-		'''Subdiv Proxy
-		'''
-		global polySmoothBaseMesh
-		polySmoothBaseMesh=[]
-		#disable creating seperate layers for subdiv proxy
-		pm.optionVar (intValue=["polySmoothLoInLayer",0])
-		pm.optionVar (intValue=["polySmoothHiInLayer",0])
-		#query smooth proxy state.
-		sel = pm.mel.polyCheckSelection("polySmoothProxy", "o", 0) #mel.eval("polyCheckSelection \"polySmoothProxy\" \"o\" 0")
-		
-		if len(sel)==0 and len(polySmoothBaseMesh)==0:
-			return 'Error: Nothing selected.'
-
-		if len(sel)!=0:
-			del polySmoothBaseMesh[:]
-			for object_ in sel:
-				polySmoothBaseMesh.append(object_)
-		elif len(polySmoothBaseMesh) != 0:
-			sel = polySmoothBaseMesh
-
-		transform = pm.listRelatives (sel[0], fullPath=1, parent=1)
-		shape = pm.listRelatives (transform[0], pa=1, shapes=1)
-
-		#check shape for an existing output to a smoothProxy
-		attachedSmoothProxies = pm.listConnections(shape[0], type="polySmoothProxy", s=0, d=1)
-		if len(attachedSmoothProxies) != 0: #subdiv off
-			pm.mel.smoothingDisplayToggle(0)
-
-		#toggle performSmoothProxy
-		pm.mel.performSmoothProxy(0) #toggle SubDiv Proxy;
-
-
-
-
-
+try:
+    import pymel.core as pm
+except ImportError as error:
+    print(__file__, error)
+import mayatk as mtk
+from tentacle.slots.maya import SlotsMaya
+
+
+class Subdivision_maya(SlotsMaya):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def cmb001(self, index, widget):
+        """Smooth Proxy"""
+        if index > 0:
+            text = widget.items[index]
+            if text == "Create Subdiv Proxy":
+                pm.mel.SmoothProxyOptions()  # Add polygons to the selected proxy objects #performSmoothProxy 1;
+            elif text == "Remove Subdiv Proxy Mirror":
+                pm.mel.UnmirrorSmoothProxyOptions()  # Create a single low resolution mesh for a mirrored proxy setup #performUnmirrorSmoothProxy 1;
+            elif text == "Crease Tool":
+                pm.mel.polyCreaseProperties()  # Harden or soften the edges of a smooth mesh preview #polyCreaseValues polyCreaseContext;
+            elif text == "Toggle Subdiv Proxy Display":
+                pm.mel.SmoothingDisplayToggle()  # Toggle the display of smooth shapes #smoothingDisplayToggle 1;
+            elif text == "Both Proxy and Subdiv Display":
+                pm.mel.SmoothingDisplayShowBoth()  # Display both smooth shapes #smoothingDisplayToggle 0;
+            widget.setCurrentIndex(0)
+
+    def cmb002(self, index, widget):
+        """Maya Subdivision Operations"""
+        if index > 0:
+            if index is widget.items.index("Reduce Polygons"):
+                pm.mel.ReducePolygonOptions()
+            elif index is widget.items.index("Add Divisions"):
+                pm.mel.SubdividePolygonOptions()
+            elif index is widget.items.index("Smooth"):
+                pm.mel.performPolySmooth(1)
+            widget.setCurrentIndex(0)
+
+    def s000(self, value, widget):
+        """Division Level"""
+        shapes = pm.ls(sl=1, dag=1, leaf=1)
+        transforms = pm.listRelatives(shapes, p=True)
+        for obj in transforms:
+            if hasattr(obj, "smoothLevel"):
+                mtk.set_node_attributes(obj, {"smoothLevel": value})
+                # subDiv proxy options: 'divisions'
+                pm.optionVar(intValue=["proxyDivisions", 1])
+                mtk.viewport_message(f"{obj}: Division Level: <hl>{value}</hl>")
+
+    def s001(self, value, widget):
+        """Tesselation Level"""
+        shapes = pm.ls(sl=1, dag=1, leaf=1)
+        transforms = pm.listRelatives(shapes, p=True)
+        for obj in transforms:
+            if hasattr(obj, "smoothLevel"):
+                mtk.set_node_attributes(obj, {"smoothTessLevel": value})
+                mtk.viewport_message(f"{obj}: Tesselation Level: <hl>{value}</hl>")
+
+    def b005(self):
+        """Reduce"""
+        selection = pm.ls(sl=1, objectsOnly=1, type="transform")
+
+        pm.polyReduce(
+            selection,
+            ver=1,
+            trm=0,
+            shp=0,
+            keepBorder=1,
+            keepMapBorder=1,
+            keepColorBorder=1,
+            keepFaceGroupBorder=1,
+            keepHardEdge=1,
+            keepCreaseEdge=1,
+            keepBorderWeight=0.5,
+            keepMapBorderWeight=0.5,
+            keepColorBorderWeight=0.5,
+            keepFaceGroupBorderWeight=0.5,
+            keepHardEdgeWeight=0.5,
+            keepCreaseEdgeWeight=0.5,
+            useVirtualSymmetry=0,
+            symmetryTolerance=0.01,
+            sx=0,
+            sy=1,
+            sz=0,
+            sw=0,
+            preserveTopology=1,
+            keepQuadsWeight=1,
+            vertexMapName="",
+            cachingReduce=1,
+            ch=1,
+            p=50,
+            vct=0,
+            tct=0,
+            replaceOriginal=1,
+        )
+
+    def b008(self):
+        """Add Divisions - Subdivide Mesh"""
+        pm.mel.SubdividePolygon()
+
+    def b009(self):
+        """Smooth"""
+        pm.mel.SmoothPolygon()
+
+    def b011(self):
+        """Apply Smooth Preview"""
+        pm.mel.performSmoothMeshPreviewToPolygon()  # convert smooth mesh preview to polygons
+
+    @staticmethod
+    def smoothProxy():
+        """Subdiv Proxy"""
+        global polySmoothBaseMesh
+        polySmoothBaseMesh = []
+        # disable creating seperate layers for subdiv proxy
+        pm.optionVar(intValue=["polySmoothLoInLayer", 0])
+        pm.optionVar(intValue=["polySmoothHiInLayer", 0])
+        # query smooth proxy state.
+        sel = pm.mel.polyCheckSelection(
+            "polySmoothProxy", "o", 0
+        )  # pm.mel.eval("polyCheckSelection \"polySmoothProxy\" \"o\" 0")
+
+        if len(sel) == 0 and len(polySmoothBaseMesh) == 0:
+            return "Error: Nothing selected."
+
+        if len(sel) != 0:
+            del polySmoothBaseMesh[:]
+            for object_ in sel:
+                polySmoothBaseMesh.append(object_)
+        elif len(polySmoothBaseMesh) != 0:
+            sel = polySmoothBaseMesh
+
+        transform = pm.listRelatives(sel[0], fullPath=1, parent=1)
+        shape = pm.listRelatives(transform[0], pa=1, shapes=1)
+
+        # check shape for an existing output to a smoothProxy
+        attachedSmoothProxies = pm.listConnections(
+            shape[0], type="polySmoothProxy", s=0, d=1
+        )
+        if len(attachedSmoothProxies) != 0:  # subdiv off
+            pm.mel.smoothingDisplayToggle(0)
 
+        # toggle performSmoothProxy
+        pm.mel.performSmoothProxy(0)  # toggle SubDiv Proxy;
 
 
+# --------------------------------------------------------------------------------------------
 
-#module name
-print (__name__)
+# module name
+print(__name__)
 # --------------------------------------------------------------------------------------------
 # Notes
-# --------------------------------------------------------------------------------------------
+# --------------------------------------------------------------------------------------------
```

### Comparing `tentacletk-0.6.6/tentacle/slots/maya/create_maya.py` & `tentacletk-0.6.9/tentacle/slots/maya/create_maya.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,337 +1,347 @@
 # !/usr/bin/python
 # coding=utf-8
-from tentacle.slots.maya import *
-from tentacle.slots.create import Create
-
-
-class Create_maya(Create, Slots_maya):
-	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
-
-		ctx = self.sb.create.draggable_header.ctxMenu
-		if not ctx.containsMenuItems:
-			ctx.add(self.sb.ComboBox, setObjectName='cmb000', setToolTip='')
-
-		cmb = self.sb.create.draggable_header.ctxMenu.cmb000
-		items = ['']
-		cmb.addItems_(items, '')
-
-		cmb = self.sb.create.cmb001
-		items = ['Polygon', 'NURBS', 'Light']
-		cmb.addItems_(items)
-
-		cmb = self.sb.create.cmb002
-		items = ["Cube", "Sphere", "Cylinder", "Plane", "Circle", "Cone", "Pyramid", "Torus", "Tube", "GeoSphere", "Platonic Solids", "Text"]
-		cmb.addItems_(items)
-
-		ctx = self.sb.create.tb000.ctxMenu
-		if not ctx.containsMenuItems:
-			ctx.add('QCheckBox', setText='Translate', setObjectName='chk000', setChecked=True, setToolTip='Move the created object to the center point of any selected object(s).')
-			ctx.add('QCheckBox', setText='Scale', setObjectName='chk001', setChecked=True, setToolTip='Uniformly scale the created object to match the averaged scale of any selected object(s).')
-
-
-	def cmb000(self, index=-1):
-		'''Editors
-		'''
-		cmb = self.sb.create.draggable_header.ctxMenu.cmb000
-
-		if index>0:
-			text = cmb.items[index]
-			if text=='':
-				pass
-			cmb.setCurrentIndex(0)
-
-
-	def cmb001(self, index=-1):
-		'''
-		'''
-		cmb = self.sb.create.cmb001
-
-		if index>=0:
-			self.cmb002(index)
-
-
-	def cmb002(self, index=-1):
-		'''
-		'''
-		cmb = self.sb.create.cmb002
-
-		polygons = ["Cube", "Sphere", "Cylinder", "Plane", "Circle", "Cone", "Pyramid", "Torus", "Tube", "GeoSphere", "Platonic Solids", "Text"]
-		nurbs = ["Cube", "Sphere", "Cylinder", "Cone", "Plane", "Torus", "Circle", "Square"]
-		lights = ["Ambient", "Directional", "Point", "Spot", "Area", "Volume"]
-
-		if index==0: #shared menu. later converted to the specified type.
-			cmb.addItems_(polygons, clear=True)
-
-		if index==1:
-			cmb.addItems_(nurbs, clear=True)
-
-		if index==2:
-			cmb.addItems_(lights, clear=True)
-
-
-	@Slots_maya.attr
-	def tb000(self, state=None):
-		'''Create Primitive
-		'''
-		tb = self.sb.create.tb000
-
-		baseType = self.sb.create.cmb001.currentText()
-		subType = self.sb.create.cmb002.currentText()
-		scale = tb.ctxMenu.chk001.isChecked()
-		translate = tb.ctxMenu.chk000.isChecked()
-
-		return self.createDefaultPrimitive(baseType, subType, scale, translate)
-
-
-	def createDefaultPrimitive(self, baseType, subType, scale=False, translate=False, axis=[0,90,0]):
-		'''
-		'''
-		baseType = baseType.lower()
-		subType = subType.lower()
-
-		selection = pm.ls(selection=1, transforms=1)
-
-		primitives = {	
-			'polygon': {
-				'cube': 'pm.polyCube(axis=axis, width=5, height=5, depth=5, subdivisionsX=1, subdivisionsY=1, subdivisionsZ=1)',
-				'sphere': 'pm.polySphere(axis=axis, radius=5, subdivisionsX=12, subdivisionsY=12)',
-				'cylinder': 'pm.polyCylinder(axis=axis, radius=5, height=10, subdivisionsX=12, subdivisionsY=1, subdivisionsZ=1)',
-				'plane': 'pm.polyPlane(axis=axis, width=5, height=5, subdivisionsX=1, subdivisionsY=1)',
-				'circle': 'self.createCircle(axis=axis, numPoints=12, radius=5, mode=0)',
-				'cone': 'pm.polyCone(axis=axis, radius=5, height=5, subdivisionsX=1, subdivisionsY=1, subdivisionsZ=1)',
-				'pyramid': 'pm.polyPyramid(axis=axis, sideLength=5, numberOfSides=5, subdivisionsHeight=1, subdivisionsCaps=1)',
-				'torus': 'pm.polyTorus(axis=axis, radius=10, sectionRadius=5, twist=0, subdivisionsX=5, subdivisionsY=5)',
-				'pipe': 'pm.polyPipe(axis=axis, radius=5, height=5, thickness=2, subdivisionsHeight=1, subdivisionsCaps=1)',
-				'geosphere': 'pm.polyPrimitive(axis=axis, radius=5, sideLength=5, polyType=0)',
-				'platonic solids': 'pm.mel.eval("performPolyPrimitive PlatonicSolid 0;")',
-			},
-
-			'nurbs': {
-				'cube': 'pm.nurbsCube(ch=1, d=3, hr=1, p=(0, 0, 0), lr=1, w=1, v=1, ax=(0, 1, 0), u=1)',
-				'sphere': 'pm.sphere(esw=360, ch=1, d=3, ut=0, ssw=0, p=(0, 0, 0), s=8, r=1, tol=0.01, nsp=4, ax=(0, 1, 0))',
-				'cylinder': 'pm.cylinder(esw=360, ch=1, d=3, hr=2, ut=0, ssw=0, p=(0, 0, 0), s=8, r=1, tol=0.01, nsp=1, ax=(0, 1, 0))',
-				'cone': 'pm.cone(esw=360, ch=1, d=3, hr=2, ut=0, ssw=0, p=(0, 0, 0), s=8, r=1, tol=0.01, nsp=1, ax=(0, 1, 0))',
-				'plane': 'pm.nurbsPlane(ch=1, d=3, v=1, p=(0, 0, 0), u=1, w=1, ax=(0, 1, 0), lr=1)',
-				'torus': 'pm.torus(esw=360, ch=1, d=3, msw=360, ut=0, ssw=0, hr=0.5, p=(0, 0, 0), s=8, r=1, tol=0.01, nsp=4, ax=(0, 1, 0))',
-				'circle': 'pm.circle(c=(0, 0, 0), ch=1, d=3, ut=0, sw=360, s=8, r=1, tol=0.01, nr=(0, 1, 0))',
-				'square': 'pm.nurbsSquare(c=(0, 0, 0), ch=1, d=3, sps=1, sl1=1, sl2=1, nr=(0, 1, 0))',
-			},
-
-			'light': {
-				'ambient': 'pm.ambientLight()', #defaults: 1, 0.45, 1,1,1, "0", 0,0,0, "1"
-				'directional': 'pm.directionalLight()', #1, 1,1,1, "0", 0,0,0, 0
-				'point': 'pm.pointLight()', #1, 1,1,1, 0, 0, 0,0,0, 1
-				'spot': 'pm.spotLight()', #1, 1,1,1, 0, 40, 0, 0, 0, 0,0,0, 1, 0
-				'area': 'pm.shadingNode("areaLight", asLight=True)', #1, 1,1,1, 0, 0, 0,0,0, 1, 0
-				'volume': 'pm.shadingNode("volumeLight", asLight=True)', #1, 1,1,1, 0, 0, 0,0,0, 1
-			},
-		}
-
-		node = eval(primitives[baseType][subType])
-
-		if selection: #if originally there was a selected object, move the object to that objects's bounding box center.
-			if translate:
-				mtk.Xform.moveTo(node, selection)
-				# center_pos = mtk.Xform.getCenterPoint(selection)
-				# pm.xform(node, translation=center_pos, worldSpace=1, absolute=1)
-			if scale:
-				mtk.Xform.matchScale(node[0], selection, average=True)
-
-		pm.selectMode(object=1) #place scene select type in object mode.
-		pm.select(node) #select the transform node so that you can see any edits
-
-		return mtk.Node.getHistoryNode(node)
-
-
-	def b005(self):
-		'''Create 6 sided poly cylinder
-		'''
-		obj = self.createPrimitive('Polygon', 'Cylinder')
-		mtk.Node.setNodeAttributes(obj, verbose=True, subdivisionsAxis=6)
-
-
-	@mtk.undo
-	def createCircle(self, axis='y', numPoints=5, radius=5, center=[0,0,0], mode=0, name='pCircle'):
-		'''Create a circular polygon plane.
-
-		Parameters:
-			axis (str): 'x','y','z' 
-			numPoints(int): number of outer points
-			radius=int
-			center=[float3 list] - point location of circle center
-			mode(int): 0 -no subdivisions, 1 -subdivide tris, 2 -subdivide quads
-
-		Return:
-			(list) [transform node, history node] ex. [nt.Transform('polySurface1'), nt.PolyCreateFace('polyCreateFace1')]
-
-		Example: self.createCircle(axis='x', numPoints=20, radius=8, mode='tri')
-		'''
-		import math
-
-		degree = 360/float(numPoints)
-		radian = math.radians(degree) #or math.pi*degree/180 (pi * degrees / 180)
-
-		vertexPoints=[]
-		for _ in range(numPoints):
-			# print("deg:", degree,"\n", "cos:",math.cos(radian),"\n", "sin:",math.sin(radian),"\n", "rad:",radian)
-			if axis =='x': #x axis
-				y = center[2] + (math.cos(radian) *radius)
-				z = center[1] + (math.sin(radian) *radius)
-				vertexPoints.append([0,y,z])
-			if axis =='y': #y axis
-				x = center[2] + (math.cos(radian) *radius)
-				z = center[0] + (math.sin(radian) *radius)
-				vertexPoints.append([x,0,z])
-			else: # z axis
-				x = center[0] + (math.cos(radian) *radius)
-				y = center[1] + (math.sin(radian) *radius)
-				vertexPoints.append([x,y,0]) #not working.
-
-			radian = radian+math.radians(degree) #increment by original radian value that was converted from degrees
-			#print(x,y,"\n")
-
-		# pm.undoInfo (openChunk=True)
-		node = pm.ls(pm.polyCreateFacet(point=vertexPoints, name=name)) #returns: ['Object name', 'node name']. pymel 'ls' converts those to objects.
-		pm.polyNormal(node, normalMode=4) #4=reverse and propagate
-		if mode==1:
-			pm.polySubdivideFacet(divisions=1, mode=1)
-		if mode==2:
-			pm.polySubdivideFacet(divisions=1, mode=0)
-		# pm.undoInfo (closeChunk=True)
-
-		return node
-
-
-
-
+try:
+    import pymel.core as pm
+except ImportError as error:
+    print(__file__, error)
+import mayatk as mtk
+from tentacle.slots.maya import SlotsMaya
+
+
+class Create_maya(SlotsMaya):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def cmb001_init(self, widget):
+        """ """
+        items = ["Polygon", "NURBS", "Light"]
+        widget.add(items)
+
+        widget.currentIndexChanged.connect(
+            lambda i, w=widget: self.cmb002_init(w.ui.cmb002)
+        )
+
+    def cmb002_init(self, widget):
+        """ """
+        index = widget.ui.cmb001.currentIndex()
+
+        if index == 1:
+            items = [
+                "Cube",
+                "Sphere",
+                "Cylinder",
+                "Cone",
+                "Plane",
+                "Torus",
+                "Circle",
+                "Square",
+            ]
+
+        elif index == 2:
+            items = ["Ambient", "Directional", "Point", "Spot", "Area", "Volume"]
+
+        else:  # Default to polygon  primitives.
+            items = [
+                "Cube",
+                "Sphere",
+                "Cylinder",
+                "Plane",
+                "Circle",
+                "Cone",
+                "Pyramid",
+                "Torus",
+                "Tube",
+                "GeoSphere",
+                "Platonic Solids",
+                "Text",
+            ]
+
+        widget.add(items, clear=True)
+
+    def tb000_init(self, widget):
+        """ """
+        widget.menu.add(
+            "QCheckBox",
+            setText="Translate",
+            setObjectName="chk000",
+            setChecked=True,
+            setToolTip="Move the created object to the center point of any selected object(s).",
+        )
+        widget.menu.add(
+            "QCheckBox",
+            setText="Scale",
+            setObjectName="chk001",
+            setChecked=True,
+            setToolTip="Uniformly scale the created object to match the averaged scale of any selected object(s).",
+        )
+
+    def tb000(self, widget):
+        """Create Primitive"""
+        baseType = self.sb.create.cmb001.currentText()
+        subType = self.sb.create.cmb002.currentText()
+        scale = widget.menu.chk001.isChecked()
+        translate = widget.menu.chk000.isChecked()
+
+        hist_node = self.createDefaultPrimitive(baseType, subType, scale, translate)
+        pm.selectMode(object=True)  # place scene select type in object mode.
+        pm.select(hist_node)  # select the transform node so that you can see any edits
+
+    def b001(self):
+        """Create poly cube"""
+        self.createDefaultPrimitive("Polygon", "Cube")
+
+    def b002(self):
+        """Create poly sphere"""
+        self.createDefaultPrimitive("Polygon", "Sphere")
+
+    def b003(self):
+        """Create poly cylinder"""
+        self.createDefaultPrimitive("Polygon", "Cylinder")
+
+    def b004(self):
+        """Create poly plane"""
+        self.createDefaultPrimitive("Polygon", "Plane")
+
+    def b005(self):
+        """Create 6 sided poly cylinder"""
+        cyl = self.createDefaultPrimitive("Polygon", "Cylinder")
+        mtk.set_node_attributes(cyl, subdivisionsAxis=6)
+
+    def createDefaultPrimitive(
+        self, baseType, subType, scale=False, translate=False, axis=[0, 90, 0]
+    ):
+        """ """
+        baseType = baseType.lower()
+        subType = subType.lower()
+
+        selection = pm.ls(sl=True, transforms=1)
+
+        primitives = {
+            "polygon": {
+                "cube": "pm.polyCube(axis=axis, width=5, height=5, depth=5, subdivisionsX=1, subdivisionsY=1, subdivisionsZ=1)",
+                "sphere": "pm.polySphere(axis=axis, radius=5, subdivisionsX=12, subdivisionsY=12)",
+                "cylinder": "pm.polyCylinder(axis=axis, radius=5, height=10, subdivisionsX=12, subdivisionsY=1, subdivisionsZ=1)",
+                "plane": "pm.polyPlane(axis=axis, width=5, height=5, subdivisionsX=1, subdivisionsY=1)",
+                "circle": "self.createCircle(axis=axis, numPoints=12, radius=5, mode=0)",
+                "cone": "pm.polyCone(axis=axis, radius=5, height=5, subdivisionsX=1, subdivisionsY=1, subdivisionsZ=1)",
+                "pyramid": "pm.polyPyramid(axis=axis, sideLength=5, numberOfSides=5, subdivisionsHeight=1, subdivisionsCaps=1)",
+                "torus": "pm.polyTorus(axis=axis, radius=10, sectionRadius=5, twist=0, subdivisionsX=5, subdivisionsY=5)",
+                "pipe": "pm.polyPipe(axis=axis, radius=5, height=5, thickness=2, subdivisionsHeight=1, subdivisionsCaps=1)",
+                "geosphere": "pm.polyPrimitive(axis=axis, radius=5, sideLength=5, polyType=0)",
+                "platonic solids": 'pm.mel.eval("performPolyPrimitive PlatonicSolid 0;")',
+            },
+            "nurbs": {
+                "cube": "pm.nurbsCube(ch=1, d=3, hr=1, p=(0, 0, 0), lr=1, w=1, v=1, ax=(0, 1, 0), u=1)",
+                "sphere": "pm.sphere(esw=360, ch=1, d=3, ut=0, ssw=0, p=(0, 0, 0), s=8, r=1, tolerance=0.01, nsp=4, ax=(0, 1, 0))",
+                "cylinder": "pm.cylinder(esw=360, ch=1, d=3, hr=2, ut=0, ssw=0, p=(0, 0, 0), s=8, r=1, tolerance=0.01, nsp=1, ax=(0, 1, 0))",
+                "cone": "pm.cone(esw=360, ch=1, d=3, hr=2, ut=0, ssw=0, p=(0, 0, 0), s=8, r=1, tolerance=0.01, nsp=1, ax=(0, 1, 0))",
+                "plane": "pm.nurbsPlane(ch=1, d=3, v=1, p=(0, 0, 0), u=1, w=1, ax=(0, 1, 0), lr=1)",
+                "torus": "pm.torus(esw=360, ch=1, d=3, msw=360, ut=0, ssw=0, hr=0.5, p=(0, 0, 0), s=8, r=1, tolerance=0.01, nsp=4, ax=(0, 1, 0))",
+                "circle": "pm.circle(c=(0, 0, 0), ch=1, d=3, ut=0, sw=360, s=8, r=1, tolerance=0.01, nr=(0, 1, 0))",
+                "square": "pm.nurbsSquare(c=(0, 0, 0), ch=1, d=3, sps=1, sl1=1, sl2=1, nr=(0, 1, 0))",
+            },
+            "light": {
+                "ambient": "pm.ambientLight()",  # defaults: 1, 0.45, 1,1,1, "0", 0,0,0, "1"
+                "directional": "pm.directionalLight()",  # 1, 1,1,1, "0", 0,0,0, 0
+                "point": "pm.pointLight()",  # 1, 1,1,1, 0, 0, 0,0,0, 1
+                "spot": "pm.spotLight()",  # 1, 1,1,1, 0, 40, 0, 0, 0, 0,0,0, 1, 0
+                "area": 'pm.shadingNode("areaLight", asLight=True)',  # 1, 1,1,1, 0, 0, 0,0,0, 1, 0
+                "volume": 'pm.shadingNode("volumeLight", asLight=True)',  # 1, 1,1,1, 0, 0, 0,0,0, 1
+            },
+        }
+
+        node = eval(primitives[baseType][subType])
+        # if originally there was a selected object, move the object to that objects's bounding box center.
+        if selection:
+            if translate:
+                mtk.move_to(node, selection)
+                # center_pos = mtk.get_center_point(selection)
+                # pm.xform(node, translation=center_pos, worldSpace=1, absolute=1)
+            if scale:
+                mtk.match_scale(node[0], selection, average=True)
+
+        return mtk.get_history_node(node[0])
+
+    @mtk.undo
+    def createCircle(
+        self, axis="y", numPoints=5, radius=5, center=[0, 0, 0], mode=0, name="pCircle"
+    ):
+        """Create a circular polygon plane.
+
+        Parameters:
+            axis (str): 'x','y','z'
+            numPoints(int): number of outer points
+            radius=int
+            center=[float3 list] - point location of circle center
+            mode(int): 0 -no subdivisions, 1 -subdivide tris, 2 -subdivide quads
+
+        Returns:
+            (list) [transform node, history node] ex. [nt.Transform('polySurface1'), nt.PolyCreateFace('polyCreateFace1')]
+
+        Example: self.createCircle(axis='x', numPoints=20, radius=8, mode='tri')
+        """
+        import math
+
+        degree = 360 / float(numPoints)
+        radian = math.radians(degree)  # or math.pi*degree/180 (pi * degrees / 180)
+
+        vertexPoints = []
+        for _ in range(numPoints):
+            # print("deg:", degree,"\n", "cos:",math.cos(radian),"\n", "sin:",math.sin(radian),"\n", "rad:",radian)
+            if axis == "x":  # x axis
+                y = center[2] + (math.cos(radian) * radius)
+                z = center[1] + (math.sin(radian) * radius)
+                vertexPoints.append([0, y, z])
+            if axis == "y":  # y axis
+                x = center[2] + (math.cos(radian) * radius)
+                z = center[0] + (math.sin(radian) * radius)
+                vertexPoints.append([x, 0, z])
+            else:  # z axis
+                x = center[0] + (math.cos(radian) * radius)
+                y = center[1] + (math.sin(radian) * radius)
+                vertexPoints.append([x, y, 0])  # not working.
+
+            # increment by original radian value that was converted from degrees
+            radian = radian + math.radians(degree)
+            # print(x,y,"\n")
+
+        # pm.undoInfo (openChunk=True)
+        node = pm.ls(pm.polyCreateFacet(point=vertexPoints, name=name))
+        # returns: ['Object name', 'node name']. pymel 'ls' converts those to objects.
+        pm.polyNormal(node, normalMode=4)  # 4=reverse and propagate
+        if mode == 1:
+            pm.polySubdivideFacet(divisions=1, mode=1)
+        if mode == 2:
+            pm.polySubdivideFacet(divisions=1, mode=0)
+        # pm.undoInfo (closeChunk=True)
 
+        return node
 
 
+# --------------------------------------------------------------------------------------------
 
 
-#module name
-print (__name__)
+# module name
+print(__name__)
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
 
 
-
 # deprecated:
 
-	# self.rotation = {'x':[90,0,0], 'y':[0,90,0], 'z':[0,0,90], '-x':[-90,0,0], '-y':[0,-90,0], '-z':[0,0,-90], 'last':[]}
-	# self.point=[0,0,0]
+# self.rotation = {'x':[90,0,0], 'y':[0,90,0], 'z':[0,0,90], '-x':[-90,0,0], '-y':[0,-90,0], '-z':[0,0,-90], 'last':[]}
+# self.point=[0,0,0]
 
-	# @property
-	# def node(self):
-	# 	'''Get the Transform Node
-	# 	'''
-	# 	transform = mtk.Node.getTransformNode()
-	# 	if transform:
-	# 		if not self.sb.create.txt003.text()==transform[0].name(): #make sure the same field reflects the current working node.
-	# 			self.sb.create.txt003.setText(transform[0].name())
-
-	# 	return transform
-
-	# def rotateAbsolute(self, axis, node):
-	# 	'''undo previous rotation and rotate on the specified axis.
-	# 	uses an external rotation dictionary.
-
-	# 	Parameters:
-	# 		axis (str): axis to rotate on. ie. '-x'
-	# 		node (obj): transform node.
-	# 	'''
-	# 	axis = self.rotation[axis]
-
-	# 	rotateOrder = pm.xform(node, query=1, rotateOrder=1)
-	# 	pm.xform(node, preserve=1, rotation=axis, rotateOrder=rotateOrder, absolute=1)
-	# 	self.rotation['last'] = axis
-
-	# def txt003(self):
-	# 	'''Set Name
-	# 	'''
-	# 	if self.node:
-	# 		pm.rename(self.node.name(), self.sb.create.txt003.text())
-
-	# def getAxis(self):
-	# 	''''''
-	# 	if self.sb.create.chk000.isChecked():
-	# 		axis = 'x'
-	# 	elif self.sb.create.chk001.isChecked():
-	# 		axis = 'y'
-	# 	elif self.sb.create.chk002.isChecked():
-	# 		axis = 'z'
-	# 	if self.sb.create.chk003.isChecked(): #negative
-	# 		axis = '-'+axis
-	# 	return axis
-
-
-	# def chk000(self, state=None):
-	# 	'''Rotate X Axis
-	# 	'''
-	# 	self.sb.toggleWidgets(setChecked='chk000', setUnChecked='chk001, chk002')
-	# 	if self.node:
-	# 		self.rotateAbsolute(self.getAxis(), self.node)
-
-
-	# def chk001(self, state=None):
-	# 	'''Rotate Y Axis
-	# 	'''
-	# 	self.sb.toggleWidgets(setChecked='chk001', setUnChecked='chk000, chk002')
-	# 	if self.node:
-	# 		self.rotateAbsolute(self.getAxis(), self.node)
-
-
-	# def chk002(self, state=None):
-	# 	'''Rotate Z Axis
-	# 	'''
-	# 	self.sb.toggleWidgets(setChecked='chk002', setUnChecked='chk000, chk001')
-	# 	if self.node:
-	# 		self.rotateAbsolute(self.getAxis(), self.node)
-
-
-	# def chk003(self, state=None):
-	# 	'''Rotate Negative Axis
-	# 	'''
-	# 	if self.node:
-	# 		self.rotateAbsolute(self.getAxis(), self.node)
-
-		# def chk005(self, state=None):
-		# '''Set Point
-		# '''
-		# #add support for averaging multiple components.
-		# selection = pm.ls(selection=1, flatten=1)
-		# try:
-		# 	self.point = pm.xform(selection, query=1, translation=1, worldSpace=1, absolute=1)
-		# except:
-		# 	self.point = [0,0,0]
-		# 	print('Warning: Nothing selected. Point set to origin [0,0,0].')
-
-		# self.sb.create.s000.setValue(self.point[0])
-		# self.sb.create.s001.setValue(self.point[1])
-		# self.sb.create.s002.setValue(self.point[2])
-
-
-	# def s000(self, value=None):
-	# 	'''Set Translate X
-	# 	'''
-	# 	if self.node:
-	# 		self.point[0] = self.sb.create.s000.value()
-	# 		pm.xform(self.node, translation=self.point, worldSpace=1, absolute=1)
-
-
-	# def s001(self, value=None):
-	# 	'''Set Translate Y
-	# 	'''
-	# 	if self.node:
-	# 		self.point[1] = self.sb.create.s001.value()
-	# 		pm.xform(self.node, translation=self.point, worldSpace=1, absolute=1)
-
-
-	# def s002(self, value=None):
-	# 	'''Set Translate Z
-	# 	'''
-	# 	if self.node:
-	# 		self.point[2] = self.sb.create.s002.value()
-	# 		pm.xform (self.node, translation=self.point, worldSpace=1, absolute=1)
+# @property
+# def node(self):
+#   '''Get the Transform Node
+#   '''
+#   transform = mtk.get_transform_node()
+#   if transform:
+#       if not self.sb.create.txt003.text()==transform[0].name(): #make sure the same field reflects the current working node.
+#           self.sb.create.txt003.setText(transform[0].name())
+
+#   return transform
+
+# def rotateAbsolute(self, axis, node):
+#   '''undo previous rotation and rotate on the specified axis.
+#   uses an external rotation dictionary.
+
+#   Parameters:
+#       axis (str): axis to rotate on. ie. '-x'
+#       node (obj): transform node.
+#   '''
+#   axis = self.rotation[axis]
+
+#   rotateOrder = pm.xform(node, q=True, rotateOrder=1)
+#   pm.xform(node, preserve=1, rotation=axis, rotateOrder=rotateOrder, absolute=1)
+#   self.rotation['last'] = axis
+
+# def txt003(self):
+#   '''Set Name
+#   '''
+#   if self.node:
+#       pm.rename(self.node.name(), self.sb.create.txt003.text())
+
+# def getAxis(self):
+#   ''''''
+#   if self.sb.create.chk000.isChecked():
+#       axis = 'x'
+#   elif self.sb.create.chk001.isChecked():
+#       axis = 'y'
+#   elif self.sb.create.chk002.isChecked():
+#       axis = 'z'
+#   if self.sb.create.chk003.isChecked(): #negative
+#       axis = '-'+axis
+#   return axis
+
+
+# def chk000(self, *args, **kwargs):
+#   '''Rotate X Axis
+#   '''
+#   self.sb.toggle_widgets(setChecked='chk000', setUnChecked='chk001, chk002')
+#   if self.node:
+#       self.rotateAbsolute(self.getAxis(), self.node)
+
+
+# def chk001(self, *args, **kwargs):
+#   '''Rotate Y Axis
+#   '''
+#   self.sb.toggle_widgets(setChecked='chk001', setUnChecked='chk000, chk002')
+#   if self.node:
+#       self.rotateAbsolute(self.getAxis(), self.node)
+
+
+# def chk002(self, *args, **kwargs):
+#   '''Rotate Z Axis
+#   '''
+#   self.sb.toggle_widgets(setChecked='chk002', setUnChecked='chk000, chk001')
+#   if self.node:
+#       self.rotateAbsolute(self.getAxis(), self.node)
+
+
+# def chk003(self, *args, **kwargs):
+#   '''Rotate Negative Axis
+#   '''
+#   if self.node:
+#       self.rotateAbsolute(self.getAxis(), self.node)
+
+# def chk005(self, *args, **kwargs):
+# '''Set Point
+# '''
+# #add support for averaging multiple components.
+# selection = pm.ls(sl=True, flatten=1)
+# try:
+#   self.point = pm.xform(selection, q=True, translation=1, worldSpace=1, absolute=1)
+# except:
+#   self.point = [0,0,0]
+#   print('Warning: Nothing selected. Point set to origin [0,0,0].')
+
+# self.sb.create.s000.setValue(self.point[0])
+# self.sb.create.s001.setValue(self.point[1])
+# self.sb.create.s002.setValue(self.point[2])
+
+
+# def s000(self, *args, **kwargs):
+#   '''Set Translate X
+#   '''
+#   if self.node:
+#       self.point[0] = self.sb.create.s000.value()
+#       pm.xform(self.node, translation=self.point, worldSpace=1, absolute=1)
+
+
+# def s001(self, *args, **kwargs):
+#   '''Set Translate Y
+#   '''
+#   if self.node:
+#       self.point[1] = self.sb.create.s001.value()
+#       pm.xform(self.node, translation=self.point, worldSpace=1, absolute=1)
+
+
+# def s002(self, *args, **kwargs):
+#   '''Set Translate Z
+#   '''
+#   if self.node:
+#       self.point[2] = self.sb.create.s002.value()
+#       pm.xform (self.node, translation=self.point, worldSpace=1, absolute=1)
```

### Comparing `tentacletk-0.6.6/tentacletk.egg-info/PKG-INFO` & `tentacletk-0.6.9/tentacletk.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 Metadata-Version: 2.1
 Name: tentacletk
-Version: 0.6.6
-Summary: Tentacle is a marking menu style UI and toolkit derived from a QStackedWidget and constructed using the uitk backend. It aims to bring a similar UI experience across multiple DCC modeling applications that support the PySide2 GUI framework.
+Version: 0.6.9
+Summary: A Python3/PySide2 marking menu style toolkit for Maya, 3ds Max, and Blender.
 Home-page: https://github.com/m3trik/tentacle
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
+License: LGPLv3
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: COPYING.LESSER
 
-## Tentacle
+[![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.en.html)
 
-\*\*personal project. work in progress ..\*\*
+# Tentacle: A Python3/PySide2 Marking Menu and UI Toolkit
 
+Tentacle is a Python3/PySide2 marking menu and UI toolkit designed for Maya, 3ds Max, Blender, and any other DCC app that supports the PySide2 framework. It is a personal project and is currently a work in progress.
 
-##### 
----
-<!-- short_description_start -->
-Tentacle is a marking menu style UI and toolkit derived from a QStackedWidget and constructed using the uitk backend. It aims to bring a similar UI experience across multiple DCC modeling applications that support the PySide2 GUI framework.
-<!-- short_description_end -->
+## Design
 
-![alt text](https://raw.githubusercontent.com/m3trik/tentacle/master/docs/toolkit_demo.gif) \*Example re-opening the last scene, renaming a material, and selecting geometry by that material.
+Tentacle is a dynamic UI toolkit with a marking menu style UI derived from a QStackedWidget. The switchboard module, derived from QUiLoader, provides properties and convenience methods that allow quick and easy getting/setting of relevant UI and widget data across modules.
 
-##
+## Example
 
+The following example demonstrates re-opening the last scene, renaming a material, and selecting geometry by that material.
 
-## Design:
+![Example](https://raw.githubusercontent.com/m3trik/tentacle/master/docs/toolkit_demo.gif)
 
-![alt text](https://raw.githubusercontent.com/m3trik/tentacle/master/docs/dependancy_graph.jpg)
+## Structure
 
+The structure of the project is as follows:
 
-Module | Description
-------- | -------
-[tcl](https://github.com/m3trik/tentacle/blob/main/tentacle/tcl.py) | *A Custom QStackedWidget that handles UI hierarchy navigation.*
-[overlay](https://github.com/m3trik/tentacle/blob/main/tentacle/overlay.py) | *Tracks cursor position and UI hierarchy to generate paint events that overlay the parent widget.*
-[slots](https://github.com/m3trik/tentacle/blob/main/tentacle/slots) | *The source directory for the various slot connection modules.*
-[ui](https://github.com/m3trik/tentacle/blob/main/tentacle/slots) | *The source directory for dynamic UI files.*
+![Structure](https://raw.githubusercontent.com/m3trik/tentacle/master/docs/dependancy_graph.jpg)
 
----
+| Module | Description |
+| ------- | ----------- |
+| [tcl](https://github.com/m3trik/uitk/blob/main/tentacle/tcl.py) | Handles main GUI construction for the marking menu. |
+| [overlay](https://github.com/m3trik/uitk/blob/main/tentacle/overlay.py) | Tracks cursor position and UI hierarchy to generate paint events that overlay its parent widget. |
+| [ui](https://github.com/m3trik/uitk/blob/main/tentacle/events.py) | Location of the dynamic UI files. |
+| [slots](https://github.com/m3trik/uitk/blob/main/tentacle/slots) | Location of the various slot modules. |
 
-## Installation:
+## Installation
 
-#####
+Add the `tentacle` folder to a directory on your Python path, or install via pip in a command line window using:
 
-To install:
-install via pip in a command line window using:
-```
+```bash
 python -m pip install tentacletk
 ```
-
+## Usage
 To launch the marking menu:
-For Maya:
-Add a macro to a hotkey similar to the following:
+
+For Maya, add a macro to a hotkey similar to the following:
 ```python
-from tentacle import tcl_maya
+from uitk import tcl_maya
 tcl_maya.show(key_show='Key_F12')
 ```
 
-For 3ds Max:
-Add a macro to a hotkey similar to the following:
-```python
+For 3ds Max, add a macro to a hotkey similar to the following:
+```maxscript
 macroScript main_max
 category: "_macros.ui"
 silentErrors: false
 autoUndoEnabled: false
 (
-	python.Execute "from tentacle import tcl_max"
+	python.Execute "from uitk import tcl_max"
 	python.Execute "tcl_max.show(key_show='Key_F12')"
 )
 ```
+Again, please note that this is a personal project and is currently a work in progress. Contributions are welcome.
```

