# Comparing `tmp/nitransforms-23.0.0.tar.gz` & `tmp/nitransforms-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitransforms-23.0.0.tar", last modified: Tue Jun 13 16:06:29 2023, max compression
+gzip compressed data, was "nitransforms-23.0.1.tar", last modified: Mon Jul 10 19:05:30 2023, max compression
```

## Comparing `nitransforms-23.0.0.tar` & `nitransforms-23.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:06:29.527976 nitransforms-23.0.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1057 2023-06-13 16:06:18.000000 nitransforms-23.0.0/.dockerignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1808 2023-06-13 16:06:18.000000 nitransforms-23.0.0/.zenodo.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5617 2023-06-13 16:06:18.000000 nitransforms-23.0.0/CHANGES.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5352 2023-06-13 16:06:18.000000 nitransforms-23.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      687 2023-06-13 16:06:18.000000 nitransforms-23.0.0/CONTRIBUTING.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-06-13 16:06:18.000000 nitransforms-23.0.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      261 2023-06-13 16:06:18.000000 nitransforms-23.0.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-06-13 16:06:29.527976 nitransforms-23.0.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3187 2023-06-13 16:06:18.000000 nitransforms-23.0.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:06:29.527976 nitransforms-23.0.0/nitransforms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1315 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11833 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3978 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2919 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:06:29.527976 nitransforms-23.0.0/nitransforms/interp/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/interp/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/interp/bspline.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:06:29.527976 nitransforms-23.0.0/nitransforms/io/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/io/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11098 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/io/afni.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4485 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/io/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6676 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/io/fsl.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13871 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/io/itk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13802 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/io/lta.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16718 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/linear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6049 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/manip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/nonlinear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2241 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/patched.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:06:29.527976 nitransforms-23.0.0/nitransforms.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      775 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       56 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-06-13 16:06:18.000000 nitransforms-23.0.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-06-13 16:06:29.531977 nitransforms-23.0.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      143 2023-06-13 16:06:18.000000 nitransforms-23.0.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 19:05:30.988662 nitransforms-23.0.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1057 2023-07-10 19:05:19.000000 nitransforms-23.0.1/.dockerignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1808 2023-07-10 19:05:19.000000 nitransforms-23.0.1/.zenodo.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5837 2023-07-10 19:05:19.000000 nitransforms-23.0.1/CHANGES.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5352 2023-07-10 19:05:19.000000 nitransforms-23.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      687 2023-07-10 19:05:19.000000 nitransforms-23.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-07-10 19:05:19.000000 nitransforms-23.0.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      261 2023-07-10 19:05:19.000000 nitransforms-23.0.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-07-10 19:05:30.992662 nitransforms-23.0.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3187 2023-07-10 19:05:19.000000 nitransforms-23.0.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 19:05:30.988662 nitransforms-23.0.1/nitransforms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1315 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-07-10 19:05:30.000000 nitransforms-23.0.1/nitransforms/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11833 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3978 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2919 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 19:05:30.988662 nitransforms-23.0.1/nitransforms/interp/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/interp/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/interp/bspline.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 19:05:30.988662 nitransforms-23.0.1/nitransforms/io/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/io/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11098 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/io/afni.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4485 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/io/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6623 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/io/fsl.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14147 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/io/itk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13802 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/io/lta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17292 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/linear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6049 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/manip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13863 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/nonlinear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2241 2023-07-10 19:05:19.000000 nitransforms-23.0.1/nitransforms/patched.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 19:05:30.988662 nitransforms-23.0.1/nitransforms.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-07-10 19:05:30.000000 nitransforms-23.0.1/nitransforms.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      775 2023-07-10 19:05:30.000000 nitransforms-23.0.1/nitransforms.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-10 19:05:30.000000 nitransforms-23.0.1/nitransforms.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       56 2023-07-10 19:05:30.000000 nitransforms-23.0.1/nitransforms.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-07-10 19:05:30.000000 nitransforms-23.0.1/nitransforms.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-10 19:05:30.000000 nitransforms-23.0.1/nitransforms.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-07-10 19:05:19.000000 nitransforms-23.0.1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-07-10 19:05:30.992662 nitransforms-23.0.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      143 2023-07-10 19:05:19.000000 nitransforms-23.0.1/setup.py
```

### Comparing `nitransforms-23.0.0/.dockerignore` & `nitransforms-23.0.1/.dockerignore`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/.zenodo.json` & `nitransforms-23.0.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/CHANGES.rst` & `nitransforms-23.0.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+23.0.1 (July 10, 2023)
+======================
+Hotfix release addressing two issues.
+
+CHANGES
+-------
+
+* FIX: Load ITK's ``.mat`` files with ``Affine``'s loaders (#179)
+* FIX: numpy deprecation errors after 1.22 (#180)
+
+
 23.0.0 (June 13, 2023)
 ======================
 A new major release preparing for the finalization of the package and migration into
 NiBabel, mostly addressing bugfixes and scheduled added new features.
 
 CHANGES
 -------
```

### Comparing `nitransforms-23.0.0/CODE_OF_CONDUCT.md` & `nitransforms-23.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/CONTRIBUTING.rst` & `nitransforms-23.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/LICENSE` & `nitransforms-23.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/PKG-INFO` & `nitransforms-23.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitransforms
-Version: 23.0.0
+Version: 23.0.1
 Summary: NiTransforms -- Neuroimaging spatial transforms in Python.
 Home-page: https://github.com/nipy/nitransforms
 Author: The NiPy developers
 Author-email: nipreps@gmail.com
 License: MIT License
 Project-URL: Manuscript, https://doi.org/10.31219/osf.io/8aq7b
 Project-URL: NiBabel, https://github.com/nipy/nibabel/pull/656
```

### Comparing `nitransforms-23.0.0/README.md` & `nitransforms-23.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/nitransforms/__init__.py` & `nitransforms-23.0.1/nitransforms/__init__.py`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/nitransforms/base.py` & `nitransforms-23.0.1/nitransforms/base.py`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/nitransforms/cli.py` & `nitransforms-23.0.1/nitransforms/cli.py`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/nitransforms/conftest.py` & `nitransforms-23.0.1/nitransforms/conftest.py`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/nitransforms/interp/bspline.py` & `nitransforms-23.0.1/nitransforms/interp/bspline.py`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/nitransforms/io/__init__.py` & `nitransforms-23.0.1/nitransforms/io/__init__.py`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/nitransforms/io/afni.py` & `nitransforms-23.0.1/nitransforms/io/afni.py`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/nitransforms/io/base.py` & `nitransforms-23.0.1/nitransforms/io/base.py`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/nitransforms/io/fsl.py` & `nitransforms-23.0.1/nitransforms/io/fsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,15 @@
     _inner_type = FSLLinearTransform
 
     def to_filename(self, filename):
         """Store this transform to a file with the appropriate format."""
         output_dir = Path(filename).parent
         output_dir.mkdir(exist_ok=True, parents=True)
         for i, xfm in enumerate(self.xforms):
-            (output_dir / ".".join((str(filename), "%03d" % i))).write_text(
-                xfm.to_string()
-            )
+            (output_dir / f"{filename}.{i:03d}").write_text(str(xfm))
 
     def to_ras(self, moving=None, reference=None):
         """Return a nitransforms' internal RAS matrix."""
         return np.stack(
             [xfm.to_ras(moving=moving, reference=reference) for xfm in self.xforms]
         )
```

### Comparing `nitransforms-23.0.0/nitransforms/io/itk.py` & `nitransforms-23.0.1/nitransforms/io/itk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Read/write ITK transforms."""
 import warnings
 import numpy as np
 from scipy.io import loadmat as _read_mat, savemat as _save_mat
 from h5py import File as H5File
 from nibabel import Nifti1Header, Nifti1Image
 from nibabel.affines import from_matvec
-from .base import (
+from nitransforms.io.base import (
     BaseLinearTransformList,
     DisplacementsField,
     LinearParameters,
     TransformIOError,
     TransformFileError,
 )
 
@@ -200,15 +200,22 @@
         sa["offset"] = np.genfromtxt(
             [lines[3].split(":")[-1].encode()], dtype=cls.dtype["offset"]
         )
         vals = np.genfromtxt([lines[2].split(":")[-1].encode()], dtype="f4")
         parameters[:3, :3] = vals[:-3].reshape((3, 3))
         parameters[:3, 3] = vals[-3:]
         sa["parameters"] = parameters
-        return tf
+
+        # Try to double-dip and see if there are more transforms
+        try:
+            cls.from_string("\n".join(lines[4:8]))
+        except TransformFileError:
+            return tf
+        else:
+            raise TransformFileError("More than one linear transform found.")
 
 
 class ITKLinearTransformArray(BaseLinearTransformList):
     """A string-based structure for series of ITK linear transforms."""
 
     _inner_type = ITKLinearTransform
```

### Comparing `nitransforms-23.0.0/nitransforms/io/lta.py` & `nitransforms-23.0.1/nitransforms/io/lta.py`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/nitransforms/linear.py` & `nitransforms-23.0.1/nitransforms/linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,26 +199,43 @@
         return filename
 
     @classmethod
     def from_filename(cls, filename, fmt=None, reference=None, moving=None):
         """Create an affine from a transform file."""
         fmtlist = [fmt] if fmt is not None else ("itk", "lta", "afni", "fsl")
 
+        if fmt is not None and not Path(filename).exists():
+            if fmt != "fsl":
+                raise FileNotFoundError(
+                    f"[Errno 2] No such file or directory: '{filename}'"
+                )
+            elif not Path(f"{filename}.000").exists():
+                raise FileNotFoundError(
+                    f"[Errno 2] No such file or directory: '{filename}[.000]'"
+                )
+
+        is_array = cls != Affine
+        errors = []
         for potential_fmt in fmtlist:
+            if (potential_fmt == "itk" and Path(filename).suffix == ".mat"):
+                is_array = False
+                cls = Affine
+
             try:
-                struct = get_linear_factory(potential_fmt).from_filename(filename)
-                matrix = struct.to_ras(reference=reference, moving=moving)
-                if cls == Affine:
-                    if np.shape(matrix)[0] != 1:
-                        raise TypeError("Cannot load transform array '%s'" % filename)
-                    matrix = matrix[0]
-                return cls(matrix, reference=reference)
-            except (TransformFileError, FileNotFoundError):
+                struct = get_linear_factory(
+                    potential_fmt,
+                    is_array=is_array
+                ).from_filename(filename)
+            except (TransformFileError, FileNotFoundError) as err:
+                errors.append((potential_fmt, err))
                 continue
 
+            matrix = struct.to_ras(reference=reference, moving=moving)
+            return cls(matrix, reference=reference)
+
         raise TransformFileError(
             f"Could not open <{filename}> (formats tried: {', '.join(fmtlist)})."
         )
 
     @classmethod
     def from_matvec(cls, mat=None, vec=None, reference=None):
         """
@@ -495,10 +512,12 @@
     >>> isinstance(xfm, LinearTransformsMapping)
     True
 
     """
     xfm = LinearTransformsMapping.from_filename(
         filename, fmt=fmt, reference=reference, moving=moving
     )
-    if len(xfm) == 1:
-        return xfm[0]
+
+    if isinstance(xfm, LinearTransformsMapping) and len(xfm) == 1:
+        xfm = xfm[0]
+
     return xfm
```

### Comparing `nitransforms-23.0.0/nitransforms/manip.py` & `nitransforms-23.0.1/nitransforms/manip.py`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/nitransforms/nonlinear.py` & `nitransforms-23.0.1/nitransforms/nonlinear.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         ijk = self.reference.index(x)
         indexes = np.round(ijk).astype("int")
 
         if np.all(np.abs(ijk - indexes) < 1e-3):
             indexes = tuple(tuple(i) for i in indexes.T)
             return self._field[indexes]
 
-        return np.vstack((
+        return np.vstack(tuple(
             map_coordinates(
                 self._field[..., i],
                 ijk.T,
                 order=3,
                 mode="constant",
                 cval=0,
                 prefilter=True,
```

### Comparing `nitransforms-23.0.0/nitransforms/patched.py` & `nitransforms-23.0.1/nitransforms/patched.py`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/nitransforms.egg-info/PKG-INFO` & `nitransforms-23.0.1/nitransforms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitransforms
-Version: 23.0.0
+Version: 23.0.1
 Summary: NiTransforms -- Neuroimaging spatial transforms in Python.
 Home-page: https://github.com/nipy/nitransforms
 Author: The NiPy developers
 Author-email: nipreps@gmail.com
 License: MIT License
 Project-URL: Manuscript, https://doi.org/10.31219/osf.io/8aq7b
 Project-URL: NiBabel, https://github.com/nipy/nibabel/pull/656
```

### Comparing `nitransforms-23.0.0/nitransforms.egg-info/SOURCES.txt` & `nitransforms-23.0.1/nitransforms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nitransforms-23.0.0/setup.cfg` & `nitransforms-23.0.1/setup.cfg`

 * *Files identical despite different names*

