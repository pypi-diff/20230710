# Comparing `tmp/pydra_ants-0.0.1.tar.gz` & `tmp/pydra_ants-0.0.2.tar.gz`

## Comparing `pydra_ants-0.0.1.tar` & `pydra_ants-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/.editorconfig
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/.github/dependabot.yaml
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/src/pydra/tasks/ants/__init__.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/src/pydra/tasks/ants/apply_transforms.py
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/src/pydra/tasks/ants/bias_correction.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/src/pydra/tasks/ants/registration.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/LICENSE
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/README.md
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/hatch.toml
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pydra_ants-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/.editorconfig
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/.github/dependabot.yaml
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/src/pydra/tasks/ants/__init__.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/src/pydra/tasks/ants/apply_transforms.py
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/src/pydra/tasks/ants/bias_correction.py
+-rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/src/pydra/tasks/ants/registration.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/README.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/hatch.toml
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pydra_ants-0.0.2/PKG-INFO
```

### Comparing `pydra_ants-0.0.1/.github/workflows/publish.yaml` & `pydra_ants-0.0.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.1/.github/workflows/test.yaml` & `pydra_ants-0.0.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.1/src/pydra/tasks/ants/apply_transforms.py` & `pydra_ants-0.0.2/src/pydra/tasks/ants/apply_transforms.py`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.1/src/pydra/tasks/ants/bias_correction.py` & `pydra_ants-0.0.2/src/pydra/tasks/ants/bias_correction.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,68 +49,68 @@
             },
         )
 
         weight_image: PathLike = field(metadata={"help_string": "weight image", "argstr": "--weight-image"})
 
         shrink_factor: int = field(default=4, metadata={"help_string": "shrink factor", "argstr": "--shrink-factor"})
 
-        _bspline_fitting = field(
+        bspline_fitting_parameters: str = field(
             metadata={
                 "help_string": "b-spline fitting parameters",
                 "argstr": "--bspline-fitting [{spline_distance}, {spline_order}]",
                 "readonly": True,
             }
         )
 
         spline_distance: float = field(default=200, metadata={"help_string": "spline distance"})
 
         spline_order: int = field(default=3, metadata={"help_string": "spline order"})
 
-        _convergence = field(
+        convergence_parameters: str = field(
             metadata={
-                "help_string": "convergence",
+                "help_string": "convergence parameters",
                 "readonly": True,
                 "formatter": lambda num_iterations, convergence_threshold: (
                     "--convergence [{}, {}]".format("x".join(str(i) for i in num_iterations), convergence_threshold)
                 ),
             }
         )
 
         num_iterations: Sequence[int] = field(
             default=(50, 50, 50, 50), metadata={"help_string": "number of iterations"}
         )
 
         convergence_threshold: float = field(default=0.0, metadata={"help_string": "convergence threshold"})
 
-        _histogram_sharpening = field(
+        histogram_sharpening_parameters: str = field(
             metadata={
-                "help_string": "histogram sharpening",
+                "help_string": "histogram sharpening parameters",
                 "argstr": "--histogram-sharpening [{bias_field_fwhm}, {wiener_filter_noise}, {num_histogram_bins}]",
                 "readonly": True,
             }
         )
 
         bias_field_fwhm: float = field(default=0.15, metadata={"help_string": "Bias field FWHM"})
 
         wiener_filter_noise: float = field(default=0.01, metadata={"help_string": "Wiener filter noise"})
 
         num_histogram_bins: int = field(default=200, metadata={"help_string": "number of histogram bins"})
 
-        _output_images = field(
+        output_parameters = field(
             metadata={
-                "help_string": "output images",
-                "argstr": "--output [{output_corrected_image}, {output_bias_field}]",
+                "help_string": "output parameters",
+                "argstr": "--output [{output_image}, {output_bias_field}]",
                 "readonly": True,
             }
         )
 
-        output_corrected_image: str = field(
-            metadata={"help_string": "output corrected image", "output_file_template": "{input_image}_corrected"}
+        output_image: str = field(
+            metadata={"help_string": "output image", "output_file_template": "{input_image}_corrected"}
         )
 
         output_bias_field: str = field(
-            metadata={"help_string": "output bias field image", "output_file_template": "{input_image}_biasfield"}
+            metadata={"help_string": "output bias field", "output_file_template": "{input_image}_biasfield"}
         )
 
     input_spec = SpecInfo(name="Input", bases=(InputSpec,))
 
     executable = "N4BiasFieldCorrection"
```

### Comparing `pydra_ants-0.0.1/src/pydra/tasks/ants/registration.py` & `pydra_ants-0.0.2/src/pydra/tasks/ants/registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,30 @@
 >>> task.cmdline    # doctest: +ELLIPSIS
 'antsRegistrationSyNQuick.sh -d 3 -f reference.nii -m structural.nii ...'
 
 >>> task = RegistrationSyNQuick(
 ...     dimensionality=3,
 ...     fixed_image="reference.nii",
 ...     moving_image="structural.nii", 
-...     output_prefix="output",
 ...     transform_type="b",
 ...     spline_distance=32,
 ...     gradient_step_size=0.2,
 ...     random_seed=42,
 ... )
 >>> task.cmdline    # doctest: +ELLIPSIS
 'antsRegistrationSyNQuick.sh ... -t b -s 32 -g 0.2 ... -e 42'
+
+>>> task = RegistrationSyNQuick(
+...     dimensionality=3,
+...     fixed_image="reference.nii",
+...     moving_image="structural.nii",
+...     fixed_mask="mask.nii",
+... )
+>>> task.cmdline    # doctest: +ELLIPSIS
+'antsRegistrationSyNQuick.sh ... -x mask.nii ...'
 """
 
 __all__ = ["RegistrationSyNQuick"]
 
 from os import PathLike
 from typing import Sequence
 
@@ -108,25 +116,23 @@
                 "help_string": "gradient step size for SyN and B-spline SyN",
                 "formatter": lambda transform_type, gradient_step_size: (
                     f"-g {gradient_step_size}" if any(c in transform_type for c in ("s", "b")) else ""
                 ),
             },
         )
 
-        _masks = field(
+        fixed_mask: PathLike = field(
             metadata={
-                "help_string": "masks parameter",
+                "help_string": "mask applied to the fixed image",
                 "formatter": lambda fixed_mask, moving_mask: (
                     "" if not fixed_mask else f"-x {fixed_mask},{moving_mask}" if moving_mask else f"-x {fixed_mask}"
                 ),
             }
         )
 
-        fixed_mask: PathLike = field(metadata={"help_string": "mask applied to the fixed image"})
-
         moving_mask: PathLike = field(
             metadata={"help_string": "mask applied to the moving image", "requires": {"fixed_mask"}}
         )
 
         precision: str = field(
             default="double",
             metadata={
```

### Comparing `pydra_ants-0.0.1/.gitignore` & `pydra_ants-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.1/LICENSE` & `pydra_ants-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.1/pyproject.toml` & `pydra_ants-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pydra-ants"
-version = "0.0.1"
+version = "0.0.2"
 description = "Pydra tasks for ANTs"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = [
   "ants",
   "neuroimaging",
```

### Comparing `pydra_ants-0.0.1/PKG-INFO` & `pydra_ants-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydra-ants
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pydra tasks for ANTs
 Project-URL: Documentation, https://github.com/ghisvail/pydra-ants#readme
 Project-URL: Issues, https://github.com/ghisvail/pydra-ants/issues
 Project-URL: Source, https://github.com/ghisvail/pydra-ants
 Author-email: Ghislain Vaillant <ghislain.vaillant@icm-institute.org>
 License-Expression: MIT
 License-File: LICENSE
@@ -24,14 +24,19 @@
 Requires-Python: >=3.7
 Requires-Dist: attrs>=22.1.0
 Requires-Dist: pydra>=0.22
 Description-Content-Type: text/markdown
 
 # pydra-ants
 
+[![PyPI - Version][pypi-version]][pypi-project]
+[![PyPI - Python Version][pypi-pyversions]][pypi-project]
+[![PyPI - Downloads][pypi-downloads]][pypi-project]
+![][status-test]
+
 -----
 
 Pydra tasks for ANTs
 
 [Pydra][pydra] is a dataflow engine which provides
 a set of lightweight abstractions for DAG
 construction, manipulation, and distributed execution.
@@ -86,14 +91,24 @@
 hatch run lint:fix
 ```
 
 ## License
 
 This project is distributed under the terms of the [Apache License, Version 2.0][license].
 
-[pydra]: https://pydra.readthedocs.io/
-
 [ants]: https://github.com/ANTsX/ANTs
 
 [hatch]: https://hatch.pypa.io/
 
 [license]: https://spdx.org/licenses/Apache-2.0.html
+
+[pydra]: https://pydra.readthedocs.io/
+
+[pypi-downloads]: https://static.pepy.tech/badge/pydra-ants
+
+[pypi-project]: https://pypi.org/project/pydra-ants
+
+[pypi-pyversions]: https://img.shields.io/pypi/pyversions/pydra-ants.svg
+
+[pypi-version]: https://img.shields.io/pypi/v/pydra-ants.svg
+
+[status-test]: https://github.com/aramis-lab/pydra-ants/actions/workflows/test.yaml/badge.svg
```

