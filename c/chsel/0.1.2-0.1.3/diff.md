# Comparing `tmp/chsel-0.1.2.tar.gz` & `tmp/chsel-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chsel-0.1.2.tar", last modified: Sun May 14 01:53:11 2023, max compression
+gzip compressed data, was "chsel-0.1.3.tar", last modified: Mon Jul 10 14:23:21 2023, max compression
```

## Comparing `chsel-0.1.2.tar` & `chsel-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-14 01:53:11.619197 chsel-0.1.2/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1075 2023-02-10 04:07:46.000000 chsel-0.1.2/LICENSE.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    13733 2023-05-14 01:53:11.619197 chsel-0.1.2/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    11668 2023-05-14 01:48:03.000000 chsel-0.1.2/README.md
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4184 2023-03-09 21:26:50.000000 chsel-0.1.2/pyproject.toml
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       38 2023-05-14 01:53:11.619197 chsel-0.1.2/setup.cfg
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-14 01:53:11.619197 chsel-0.1.2/src/
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-14 01:53:11.619197 chsel-0.1.2/src/chsel/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      595 2023-04-07 17:56:33.000000 chsel-0.1.2/src/chsel/__init__.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      492 2023-03-09 00:26:40.000000 chsel-0.1.2/src/chsel/conversion.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    31816 2023-04-11 23:23:26.000000 chsel-0.1.2/src/chsel/costs.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3783 2023-03-09 00:26:40.000000 chsel-0.1.2/src/chsel/initialization.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    12625 2023-04-26 04:02:46.000000 chsel-0.1.2/src/chsel/quality_diversity.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     5692 2023-04-26 04:19:45.000000 chsel-0.1.2/src/chsel/registration_util.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     9561 2023-03-09 00:26:40.000000 chsel-0.1.2/src/chsel/sgd.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      628 2023-03-09 00:26:40.000000 chsel-0.1.2/src/chsel/types.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    14488 2023-05-13 00:11:33.000000 chsel-0.1.2/src/chsel/wrapper.py
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-14 01:53:11.619197 chsel-0.1.2/src/chsel.egg-info/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    13733 2023-05-14 01:53:11.000000 chsel-0.1.2/src/chsel.egg-info/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      434 2023-05-14 01:53:11.000000 chsel-0.1.2/src/chsel.egg-info/SOURCES.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        1 2023-05-14 01:53:11.000000 chsel-0.1.2/src/chsel.egg-info/dependency_links.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       89 2023-05-14 01:53:11.000000 chsel-0.1.2/src/chsel.egg-info/requires.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        6 2023-05-14 01:53:11.000000 chsel-0.1.2/src/chsel.egg-info/top_level.txt
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-14 01:53:11.619197 chsel-0.1.2/tests/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    11325 2023-05-13 00:16:43.000000 chsel-0.1.2/tests/test_wrapper.py
+drwxr-xr-x   0 johnsonzhong   (501) staff       (20)        0 2023-07-10 14:23:21.297149 chsel-0.1.3/
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)     1075 2023-07-10 09:19:03.000000 chsel-0.1.3/LICENSE.txt
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)    13829 2023-07-10 14:23:21.296721 chsel-0.1.3/PKG-INFO
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)    11764 2023-07-10 09:19:03.000000 chsel-0.1.3/README.md
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)     4222 2023-07-10 09:20:13.000000 chsel-0.1.3/pyproject.toml
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)       38 2023-07-10 14:23:21.297265 chsel-0.1.3/setup.cfg
+drwxr-xr-x   0 johnsonzhong   (501) staff       (20)        0 2023-07-10 14:23:21.286989 chsel-0.1.3/src/
+drwxr-xr-x   0 johnsonzhong   (501) staff       (20)        0 2023-07-10 14:23:21.293816 chsel-0.1.3/src/chsel/
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)      595 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/__init__.py
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)      492 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/conversion.py
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)    31816 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/costs.py
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)     3783 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/initialization.py
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)    12625 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/quality_diversity.py
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)     5692 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/registration_util.py
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)     9561 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/sgd.py
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)      628 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/types.py
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)    14488 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/wrapper.py
+drwxr-xr-x   0 johnsonzhong   (501) staff       (20)        0 2023-07-10 14:23:21.295866 chsel-0.1.3/src/chsel.egg-info/
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)    13829 2023-07-10 14:23:21.000000 chsel-0.1.3/src/chsel.egg-info/PKG-INFO
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)      434 2023-07-10 14:23:21.000000 chsel-0.1.3/src/chsel.egg-info/SOURCES.txt
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)        1 2023-07-10 14:23:21.000000 chsel-0.1.3/src/chsel.egg-info/dependency_links.txt
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)      112 2023-07-10 14:23:21.000000 chsel-0.1.3/src/chsel.egg-info/requires.txt
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)        6 2023-07-10 14:23:21.000000 chsel-0.1.3/src/chsel.egg-info/top_level.txt
+drwxr-xr-x   0 johnsonzhong   (501) staff       (20)        0 2023-07-10 14:23:21.296181 chsel-0.1.3/tests/
+-rw-r--r--   0 johnsonzhong   (501) staff       (20)    12205 2023-07-10 14:16:24.000000 chsel-0.1.3/tests/test_wrapper.py
```

### Comparing `chsel-0.1.2/LICENSE.txt` & `chsel-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chsel-0.1.2/PKG-INFO` & `chsel-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chsel
-Version: 0.1.2
+Version: 0.1.3
 Summary: Constrained pose Hypothesis Set Elimination official code for pose estimation
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -42,18 +42,24 @@
 ## CHSEL: Producing Diverse Plausible Pose Estimates from Contact and Free Space Data
 
 ![combined demo](https://i.imgur.com/T4DnKDu.gif)
 
 Demo CHSEL results on drill with sparse contact data (top) and mug with dense vision data (bottom).
 
 ## Installation
-TODO PyPI after making repository public
+```bash
+pip install chsel
+```
 
 For development, clone repository somewhere, then `pip3 install -e .` to install in editable mode.
 
+## Links
+- [arxiv](https://arxiv.org/abs/2305.08042)
+- [website](https://johnsonzhong.me/projects/chsel/)
+
 ## Citation
 If you use it, please cite
 
 ```bibtex
 @inproceedings{zhong2023chsel,
   title={CHSEL: Producing Diverse Plausible Pose Estimates from Contact and Free Space Data},
   author={Zhong, Sheng and Fazeli, Nima and Berenson, Dmitry},
```

### Comparing `chsel-0.1.2/README.md` & `chsel-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 ## CHSEL: Producing Diverse Plausible Pose Estimates from Contact and Free Space Data
 
 ![combined demo](https://i.imgur.com/T4DnKDu.gif)
 
 Demo CHSEL results on drill with sparse contact data (top) and mug with dense vision data (bottom).
 
 ## Installation
-TODO PyPI after making repository public
+```bash
+pip install chsel
+```
 
 For development, clone repository somewhere, then `pip3 install -e .` to install in editable mode.
 
+## Links
+- [arxiv](https://arxiv.org/abs/2305.08042)
+- [website](https://johnsonzhong.me/projects/chsel/)
+
 ## Citation
 If you use it, please cite
 
 ```bibtex
 @inproceedings{zhong2023chsel,
   title={CHSEL: Producing Diverse Plausible Pose Estimates from Contact and Free Space Data},
   author={Zhong, Sheng and Fazeli, Nima and Berenson, Dmitry},
```

### Comparing `chsel-0.1.2/pyproject.toml` & `chsel-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chsel"
-version = "0.1.2"
+version = "0.1.3"
 description = "Constrained pose Hypothesis Set Elimination official code for pose estimation"
 readme = "README.md" # Optional
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
@@ -53,14 +53,16 @@
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [# Optional
     'torch',
     'numpy',
     'matplotlib',
     'arm-pytorch-utilities',
     'pytorch-kinematics',
+    'pytorch-volumetric',
+    'cma',
     'ribs[all]'
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
@@ -97,8 +99,8 @@
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
```

### Comparing `chsel-0.1.2/src/chsel/__init__.py` & `chsel-0.1.3/src/chsel/__init__.py`

 * *Files identical despite different names*

### Comparing `chsel-0.1.2/src/chsel/costs.py` & `chsel-0.1.3/src/chsel/costs.py`

 * *Files identical despite different names*

### Comparing `chsel-0.1.2/src/chsel/initialization.py` & `chsel-0.1.3/src/chsel/initialization.py`

 * *Files identical despite different names*

### Comparing `chsel-0.1.2/src/chsel/quality_diversity.py` & `chsel-0.1.3/src/chsel/quality_diversity.py`

 * *Files identical despite different names*

### Comparing `chsel-0.1.2/src/chsel/registration_util.py` & `chsel-0.1.3/src/chsel/registration_util.py`

 * *Files identical despite different names*

### Comparing `chsel-0.1.2/src/chsel/sgd.py` & `chsel-0.1.3/src/chsel/sgd.py`

 * *Files identical despite different names*

### Comparing `chsel-0.1.2/src/chsel/types.py` & `chsel-0.1.3/src/chsel/types.py`

 * *Files identical despite different names*

### Comparing `chsel-0.1.2/src/chsel/wrapper.py` & `chsel-0.1.3/src/chsel/wrapper.py`

 * *Files identical despite different names*

### Comparing `chsel-0.1.2/src/chsel.egg-info/PKG-INFO` & `chsel-0.1.3/src/chsel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chsel
-Version: 0.1.2
+Version: 0.1.3
 Summary: Constrained pose Hypothesis Set Elimination official code for pose estimation
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -42,18 +42,24 @@
 ## CHSEL: Producing Diverse Plausible Pose Estimates from Contact and Free Space Data
 
 ![combined demo](https://i.imgur.com/T4DnKDu.gif)
 
 Demo CHSEL results on drill with sparse contact data (top) and mug with dense vision data (bottom).
 
 ## Installation
-TODO PyPI after making repository public
+```bash
+pip install chsel
+```
 
 For development, clone repository somewhere, then `pip3 install -e .` to install in editable mode.
 
+## Links
+- [arxiv](https://arxiv.org/abs/2305.08042)
+- [website](https://johnsonzhong.me/projects/chsel/)
+
 ## Citation
 If you use it, please cite
 
 ```bibtex
 @inproceedings{zhong2023chsel,
   title={CHSEL: Producing Diverse Plausible Pose Estimates from Contact and Free Space Data},
   author={Zhong, Sheng and Fazeli, Nima and Berenson, Dmitry},
```

### Comparing `chsel-0.1.2/tests/test_wrapper.py` & `chsel-0.1.3/tests/test_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import copy
 import os
+import sys
 import numpy as np
 import torch
 import open3d as o3d
 
 import chsel
+import pytorch_kinematics as pk
 import pytorch_volumetric as pv
 from pytorch_seed import seed
 
 import subprocess
 import logging
 
 from chsel.types import SimilarityTransform
@@ -21,15 +23,18 @@
 logger = logging.getLogger(__file__)
 
 logging.basicConfig(level=logging.INFO, force=True,
                     format='[%(levelname)s %(asctime)s %(pathname)s:%(lineno)d] %(message)s',
                     datefmt='%m-%d %H:%M:%S')
 
 visualize = True
+visualize_after_each_iteration = True
 compare_against_icp = True
+# number of transforms to estimate at one time
+B = 30
 # if record video is true then the visualization will always rotate one rotation to allow for looping gifs
 # if it's false then it will be interactable and you can rotate it yourself or close the window
 record_video = False
 d = "cuda" if torch.cuda.is_available() else "cpu"
 
 # for rotating the visualization the first time we enter to get a better angle
 first_rotate = False
@@ -74,15 +79,14 @@
                 break
         first_rotate = False
         recorder.wait()
         logger.info("recording finished")
 
 
 def test_chsel_on_obj(obj, sdf, positions_obj_frame, semantics):
-    B = 30
     _free = torch.tensor([s == chsel.SemanticsClass.FREE for s in semantics])
     _occupied = torch.tensor([s == chsel.SemanticsClass.OCCUPIED for s in semantics])
     _known = ~_free & ~_occupied
 
     if visualize:
         pts_free = positions_obj_frame[_free]
         pts_occupied = positions_obj_frame[_occupied]
@@ -97,31 +101,32 @@
         pc_occupied.points = o3d.utility.Vector3dVector(pts_occupied.cpu().numpy())
         pc_occupied.paint_uniform_color([0, 0.706, 0])
 
         pc_sdf = o3d.geometry.PointCloud()
         pc_sdf.points = o3d.utility.Vector3dVector(pts_sdf.cpu().numpy())
         pc_sdf.paint_uniform_color([0, 0.706, 1])
 
+        print(f"visualize object mesh, free space points (orange), and known SDF points (blue) (press Q or the close window button to move on)")
         draw_geometries_one_rotation([obj._mesh, pc_free, pc_occupied, pc_sdf])
 
-    import pytorch_kinematics as pk
 
     gt_tf = pk.Transform3d(pos=torch.randn(3, device=d), rot=pk.random_rotation(device=d), device=d)
     positions = gt_tf.transform_points(positions_obj_frame)
 
     # visualize the transformed mesh and points
     if visualize:
         link_to_world_gt = gt_tf.get_matrix()[0]
         tf_mesh = copy.deepcopy(obj._mesh).transform(link_to_world_gt.cpu().numpy())
         pts_free = positions[_free]
         pts_sdf = positions[_known]
 
         # only plotting the transformed known SDF points for clarity
         pc_free.points = o3d.utility.Vector3dVector(pts_free.cpu())
         pc_sdf.points = o3d.utility.Vector3dVector(pts_sdf.cpu())
+        print(f"visualize the transformed object mesh, free space points, and known SDF points (press Q or the close window button to move on)")
         draw_geometries_one_rotation([tf_mesh, pc_free, pc_sdf])
 
     def visualize_transforms(link_to_world):
         # visualize the transformed mesh and points
         if visualize:
             # est_tf = pk.Transform3d(matrix=world_to_link.inverse())
             geo = [tf_mesh, pc_free, pc_sdf]
@@ -138,25 +143,48 @@
     # we want a set of 30 transforms
     random_init_tsf = pk.Transform3d(pos=torch.randn((B, 3), device=d), rot=pk.random_rotations(B, device=d), device=d)
     random_init_tsf = random_init_tsf.get_matrix()
 
     # try to use the ground truth transform as the initial guess
     # gt_init = chsel.reinitialize_transform_estimates(B, gt_tf.inverse().get_matrix()[0])
     # res, all_solutions = registration.register(iterations=15, batch=B, initial_tsf=gt_init)
-    res, all_solutions = registration.register(iterations=15, batch=B, initial_tsf=random_init_tsf)
-    print("Showing each iteration of the registration result")
-    for i in range(len(registration.res_history)):
-        # print the sorted RMSE for each iteration
-        print(torch.sort(registration.res_history[i].rmse).values)
-
-        # res.RTs.R, res.RTs.T, res.RTs.s are the similarity transform parameters
-        # get 30 4x4 transform matrix for homogeneous coordinates
-        world_to_link = chsel.solution_to_world_to_link_matrix(registration.res_history[i])
-        link_to_world = world_to_link.inverse()
-        visualize_transforms(link_to_world)
+    iterations = 15
+    if visualize_after_each_iteration:
+        world_to_link = random_init_tsf
+        all_solutions = None
+        # refine the solutions
+        for i in range(iterations):
+            print(f"iteration {i}")
+            start = timer()
+            # assuming the object hasn't moved, use the output of the previous iteration as the initial estimate
+            res, all_solutions = registration.register(initial_tsf=world_to_link, batch=B,
+                                                       low_cost_transform_set=all_solutions)
+            print(f"registration took {timer() - start} seconds")
+
+            world_to_link = chsel.solution_to_world_to_link_matrix(res)
+            link_to_world = world_to_link.inverse()
+            # print sorted rmse
+            print(torch.sort(res.rmse))
+            visualize_transforms(link_to_world)
+
+            # reinitialize world_to_link around elites
+            world_to_link = chsel.reinitialize_transform_around_elites(world_to_link, res.rmse)
+    else:
+        res, all_solutions = registration.register(iterations=iterations, batch=B, initial_tsf=random_init_tsf)
+        print("Showing each iteration of the registration result (press Q or the close window button to move on)")
+        for i in range(len(registration.res_history)):
+            # print the sorted RMSE for each iteration
+            print(f"iteration {i}")
+            print(torch.sort(registration.res_history[i].rmse).values)
+
+            # res.RTs.R, res.RTs.T, res.RTs.s are the similarity transform parameters
+            # get 30 4x4 transform matrix for homogeneous coordinates
+            world_to_link = chsel.solution_to_world_to_link_matrix(registration.res_history[i])
+            link_to_world = world_to_link.inverse()
+            visualize_transforms(link_to_world)
 
     # try ICP on this problem for comparison
     try:
         if compare_against_icp:
             from pytorch3d.ops.points_alignment import iterative_closest_point
 
             print("Compare against ICP")
@@ -187,41 +215,19 @@
                 initial_tsf = SimilarityTransform(initial_tsf[:, :3, :3],
                                                   initial_tsf[:, :3, 3],
                                                   torch.ones(B, device=d, dtype=model_points_register.dtype))
     except ImportError:
         print("Install pytorch3d to run ICP")
 
     # manually do single step registrations (iterations=1 essentially)
-    """
-    world_to_link = chsel.solution_to_world_to_link_matrix(res)
-    link_to_world = world_to_link.inverse()
-    # can evaluate the cost of each transform
-    print(res.rmse)
-    visualize_transforms(link_to_world)
-
-    # refine the solutions
-    iterations = 10
-    for i in range(iterations):
-        # reinitialize world_to_link around elites
-        world_to_link = chsel.reinitialize_transform_around_elites(world_to_link, res.rmse)
-
-        # assuming the object hasn't moved, use the output of the previous iteration as the initial estimate
-        res, all_solutions = registration.register(initial_tsf=world_to_link, batch=B,
-                                                   low_cost_transform_set=all_solutions)
-
-        world_to_link = chsel.solution_to_world_to_link_matrix(res)
-        link_to_world = world_to_link.inverse()
-        # print sorted rmse
-        print(torch.sort(res.rmse))
-        visualize_transforms(link_to_world)
-    """
 
 
-def test_chsel_on_drill():
-    seed(2)
+
+def test_chsel_on_drill(rng_seed=3):
+    seed(rng_seed)
     # supposing we have an object mesh (most formats supported) - from https://github.com/eleramp/pybullet-object-models
     obj = pv.MeshObjectFactory(os.path.join(TEST_DIR, "YcbPowerDrill/textured_simple_reoriented.obj"))
     sdf = pv.MeshSDF(obj)
 
     # get some points in a grid in the object frame (can get points through other means)
     # this is only around one part of the object to simulate the local nature of contacts
     query_range = np.array([
@@ -240,16 +246,14 @@
     # note that this is the most common case, but you can know non-zero (non-surface) SDF values
     known_free = sdf_val > 0.005
     known_occupied = sdf_val < -0.005
     known_sdf = ~known_free & ~known_occupied
 
     # randomly downsample (we randomly permutated before) to simulate getting partial observations
     N = 100
-    # retrieve batch of 30 transforms
-    B = 30
 
     # group and stack the points together
     # note that it will still work even if you don't have all 3 or even 2 classes
     # for example with only known surface points, it degenerates to a form of ICP
     # we also don't need balanced data from each class
     pts_free = pts[known_free][:N]
     pts_occupied = pts[known_occupied][:N]
@@ -261,8 +265,12 @@
 
     positions = torch.cat((pts_free, pts_occupied, pts_sdf))
     semantics = sem_free + sem_occupied + sem_sdf.tolist()
     test_chsel_on_obj(obj, sdf, positions, semantics)
 
 
 if __name__ == "__main__":
-    test_chsel_on_drill()
+    rng_seed = int(sys.argv[1]) if len(sys.argv) > 1 else 3
+    print(f"Using random seed {rng_seed}; try running with different seeds to see different results with\npython tests/test_wrapper.py <seed>")
+    if not torch.cuda.is_available():
+        print("Warning: CUDA not available, running on CPU which may be much slower")
+    test_chsel_on_drill(rng_seed)
```

