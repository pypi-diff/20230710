# Comparing `tmp/katalytic_images-0.9.0.tar.gz` & `tmp/katalytic_images-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic_images-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "katalytic_images-0.9.1.tar", last modified: Mon Jul 10 20:59:20 2023, max compression
```

## Comparing `katalytic_images-0.9.0.tar` & `katalytic_images-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,6 @@
--rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic_images-0.9.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_images-0.9.0/.gitignore
--rw-r--r--   0        0        0     3308 2023-05-05 03:58:55.053635 katalytic_images-0.9.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     4677 2023-07-02 19:13:45.536276 katalytic_images-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     2218 2023-05-31 06:28:52.615620 katalytic_images-0.9.0/README.md
--rw-r--r--   0        0        0     1549 2023-07-02 19:13:45.536276 katalytic_images-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    25454 2023-07-02 16:16:38.305751 katalytic_images-0.9.0/src/katalytic/images.py
--rw-r--r--   0        0        0    20897 2023-07-02 16:07:05.753628 katalytic_images-0.9.0/tests/test_images.py
--rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 katalytic_images-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     2212 2023-07-10 04:57:46.112850 katalytic_images-0.9.1/README.md
+-rw-r--r--   0        0        0     1598 2023-07-10 20:59:20.576380 katalytic_images-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    25507 2023-07-10 20:57:45.604107 katalytic_images-0.9.1/src/katalytic/images/__init__.py
+-rw-r--r--   0        0        0    20549 2023-07-02 19:24:10.781971 katalytic_images-0.9.1/tests/test_images.py
+-rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 katalytic_images-0.9.1/PKG-INFO
```

### Comparing `katalytic_images-0.9.0/LICENSE.txt` & `katalytic_images-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.9.0/pyproject.toml` & `katalytic_images-0.9.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 [build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
+[tool.pdm.build]
+includes = [
+    "src/katalytic/",
+]
+
+[tool.pytest.ini_options]
+addopts = [
+    "--import-mode=importlib",
+]
 
 [project]
 name = "katalytic-images"
-version = "0.9.0"
+version = "0.9.1"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
-license = {file = "LICENSE.txt"}
 readme = "README.md"
-
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
@@ -20,36 +30,33 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
-authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
-
+authors = [
+    { name = "Valentin Neagu", email = "vali19th@protonmail.com" },
+]
 requires-python = ">=3.6"
 dependencies = [
-    "katalytic-data>=0.8.0",
-    "katalytic-files>=0.3.0",
-    "katalytic-pkg>=0.2.0",
+    "katalytic>=0.2.2",
     "numpy>=1.14",
     "opencv-python>=4.0.0",
     "pillow>=8.4.0",
 ]
 
+[project.license]
+file = "LICENSE.txt"
+
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
     "pytest-clarity",
     "pytest-randomly",
 ]
 
 [project.urls]
-homepage = "https://gitlab.com/katalytic/katalytic-images.git"
-repository = "https://gitlab.com/katalytic/katalytic-images.git"
-
-[tool.pytest.ini_options]
-addopts = ["--import-mode=importlib"]
-
-[tool.flit.module]
-name = "katalytic.images"
+Changelog = "https://gitlab.com/katalytic/katalytic-images/-/blob/main/CHANGELOG.md"
+Homepage = "https://gitlab.com/katalytic/katalytic-images.git"
+Repository = "https://gitlab.com/katalytic/katalytic-images.git"
```

### Comparing `katalytic_images-0.9.0/src/katalytic/images.py` & `katalytic_images-0.9.1/src/katalytic/images/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,17 @@
     ndarray as __np_ndarray
 )
 
 import PIL.Image
 __PIL_Image_open = PIL.Image.open
 __PIL_Image_Image = PIL.Image.Image
 
-# noinspection PyProtectedMember
-from katalytic.data import _UNDEFINED
 from katalytic.data.checks import is_iterable, is_number, is_sequence
-from katalytic.pkg import get_version, mark, KatalyticInterrupt
+# noinspection PyProtectedMember
+from katalytic._pkg import get_version, mark, KatalyticInterrupt, _UNDEFINED
 
 __version__, __version_info__ = get_version(__name__)
 
 
 def bhwc(arr):
     """
     Returns a tuple representing the shape of the input array in the BHWC format: batch, height, width, and channels. The missing dimensions are filled with 1s.
@@ -480,14 +479,15 @@
         TypeError: If the 'image' parameter has an unsupported type.
 
     """
     if not(mode is None or isinstance(mode, str)):
         raise TypeError(f'mode expected None or str. Got {type(mode)!r}')
 
     if isinstance(image, (str, Path)):
+        # noinspection PyProtectedMember
         from katalytic.files import _warn_if_another_function_should_be_used, _load_funcs
         _warn_if_another_function_should_be_used(str(image), _load_funcs)
         if not Path(image).exists() and default is not _UNDEFINED:
             return default
         else:
             return __np_array(__PIL_Image_open(image))
     elif isinstance(image, __PIL_Image_Image):
@@ -590,14 +590,15 @@
 
     """
     if not isinstance(mode, str):
         raise TypeError(f'type(mode) = {type(mode)!r}')
     elif exists not in ('error', 'skip', 'replace'):
         raise ValueError(f'exists must be one of \'error\', \'skip\', \'replace\'. Got {exists!r}')
 
+    # noinspection PyProtectedMember
     from katalytic.files import _warn_if_another_function_should_be_used, _save_funcs
     _warn_if_another_function_should_be_used(str(path), _save_funcs)
     if Path(path).exists():
         if exists == 'error':
             raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
         elif exists == 'replace':
             pass  # continue executing
```

### Comparing `katalytic_images-0.9.0/tests/test_images.py` & `katalytic_images-0.9.1/tests/test_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,86 +323,74 @@
 
 
 class Test_load_and_save:
     def test_atomicity_interrupt(self):
         path = get_unique_path('{}.png')
         data = _create_RGB()
 
-        try:
-            save_image.__katalytic_test_atomicity_interrupt__ = True
-            save_image(data, path)
-            assert not Path(path).exists()
-
-            # make sure it's still working after the test
-            # the atomicity flag is set back to False inside the function
-            save_image(data, path)
-            assert are_arrays_equal(load(path), data)
-        except:
-            raise
+        save_image.__katalytic_test_atomicity_interrupt__ = True
+        save_image(data, path)
+        assert not Path(path).exists()
+
+        # make sure it's still working after the test
+        # the atomicity flag is set back to False inside the function
+        save_image(data, path)
+        assert are_arrays_equal(load(path), data)
 
     def test_atomicity_race_condition_error(self):
         path = get_unique_path('{}.png')
         data = _create_RGB()
 
-        try:
-            save_image.__katalytic_test_atomicity_race_condition__ = True
-            assert not Path(path).exists()
-            with pytest.raises(FileExistsError):
-                save_image(data, path, exists='error')
-
-            expected = np.array([[[0,255,0]]], dtype=np.uint8)
-            assert are_arrays_equal(load(path), expected)
-
-            # make sure it's still working after the test
-            # the atomicity flag is set back to False inside the function
-            delete_file(path)
-            assert not Path(path).exists()
+        save_image.__katalytic_test_atomicity_race_condition__ = True
+        assert not Path(path).exists()
+        with pytest.raises(FileExistsError):
             save_image(data, path, exists='error')
-            assert are_arrays_equal(load(path), data)
-        except:
-            raise
+
+        expected = np.array([[[0,255,0]]], dtype=np.uint8)
+        assert are_arrays_equal(load(path), expected)
+
+        # make sure it's still working after the test
+        # the atomicity flag is set back to False inside the function
+        delete_file(path)
+        assert not Path(path).exists()
+        save_image(data, path, exists='error')
+        assert are_arrays_equal(load(path), data)
 
     def test_atomicity_race_condition_replace(self):
         path = get_unique_path('{}.png')
         data = _create_RGB()
 
-        try:
-            save_image.__katalytic_test_atomicity_race_condition__ = True
-            assert not Path(path).exists()
-            save_image(data, path, exists='replace')
-            assert are_arrays_equal(load(path), data)
-
-            # make sure it's still working after the test
-            # the atomicity flag is set back to False inside the function
-            delete_file(path)
-            assert not Path(path).exists()
-            save_image(data, path, exists='replace')
-            assert are_arrays_equal(load(path), data)
-        except:
-            raise
+        save_image.__katalytic_test_atomicity_race_condition__ = True
+        assert not Path(path).exists()
+        save_image(data, path, exists='replace')
+        assert are_arrays_equal(load(path), data)
+
+        # make sure it's still working after the test
+        # the atomicity flag is set back to False inside the function
+        delete_file(path)
+        assert not Path(path).exists()
+        save_image(data, path, exists='replace')
+        assert are_arrays_equal(load(path), data)
 
     def test_atomicity_race_condition_skip(self):
         path = get_unique_path('{}.png')
         data = _create_RGB()
 
-        try:
-            save_image.__katalytic_test_atomicity_race_condition__ = True
-            assert not Path(path).exists()
-            save_image(data, path, exists='skip')
-            expected = np.array([[[0,255,0]]], dtype=np.uint8)
-            assert are_arrays_equal(load(path), expected)
-
-            # make sure it's still working after the test
-            # the atomicity flag is set back to False inside the function
-            delete_file(path)
-            assert not Path(path).exists()
-            save_image(data, path, exists='skip')
-            assert are_arrays_equal(load(path), data)
-        except:
-            raise
+        save_image.__katalytic_test_atomicity_race_condition__ = True
+        assert not Path(path).exists()
+        save_image(data, path, exists='skip')
+        expected = np.array([[[0,255,0]]], dtype=np.uint8)
+        assert are_arrays_equal(load(path), expected)
+
+        # make sure it's still working after the test
+        # the atomicity flag is set back to False inside the function
+        delete_file(path)
+        assert not Path(path).exists()
+        save_image(data, path, exists='skip')
+        assert are_arrays_equal(load(path), data)
 
     # noinspection PyBroadException
     @pytest.mark.parametrize('ext, wrong_load, correct_load', [
         ('jpeg', load_csv, 'load_image'),
         ('jpg', load_json, 'load_image'),
         ('png', load_text, 'load_image'),
     ])
```

