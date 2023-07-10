# Comparing `tmp/jaxip-0.6.1.tar.gz` & `tmp/jaxip-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxip-0.6.1.tar", last modified: Sat Jun 24 19:26:59 2023, max compression
+gzip compressed data, was "jaxip-0.7.0.tar", last modified: Mon Jul 10 18:19:33 2023, max compression
```

## Comparing `jaxip-0.6.1.tar` & `jaxip-0.7.0.tar`

### file list

```diff
@@ -1,151 +1,149 @@
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.908974 jaxip-0.6.1/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.6.1/AUTHORS.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.6.1/CONTRIBUTING.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      669 2023-06-24 19:26:34.000000 jaxip-0.6.1/HISTORY.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.6.1/LICENSE
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.6.1/MANIFEST.in
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5332 2023-06-24 19:26:59.908974 jaxip-0.6.1/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4745 2023-05-17 19:30:18.000000 jaxip-0.6.1/README.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.864973 jaxip-0.6.1/docs/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.6.1/docs/Makefile
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.856973 jaxip-0.6.1/docs/_build/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.856973 jaxip-0.6.1/docs/_build/doctrees/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.864973 jaxip-0.6.1/docs/_build/doctrees/nbsphinx/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-06-18 09:34:19.000000 jaxip-0.6.1/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:34:19.000000 jaxip-0.6.1/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:34:19.000000 jaxip-0.6.1/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.856973 jaxip-0.6.1/docs/_build/html/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.868973 jaxip-0.6.1/docs/_build/html/_images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-06-18 09:20:05.000000 jaxip-0.6.1/docs/_build/html/_images/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:20:05.000000 jaxip-0.6.1/docs/_build/html/_images/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:20:05.000000 jaxip-0.6.1/docs/_build/html/_images/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.872973 jaxip-0.6.1/docs/_build/html/_static/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.6.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.6.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.6.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.6.1/docs/authors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6406 2023-06-18 10:02:01.000000 jaxip-0.6.1/docs/conf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.6.1/docs/contributing.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       71 2023-05-17 19:30:18.000000 jaxip-0.6.1/docs/examples.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.6.1/docs/history.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.880973 jaxip-0.6.1/docs/images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.6.1/docs/images/flowchart.drawio.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.6.1/docs/images/water.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.6.1/docs/index.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.6.1/docs/installation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-10 20:36:05.000000 jaxip-0.6.1/docs/jaxip.atoms.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      662 2023-05-17 19:30:18.000000 jaxip-0.6.1/docs/jaxip.datasets.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-10 20:36:05.000000 jaxip-0.6.1/docs/jaxip.descriptors.acsf.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      613 2023-05-17 19:30:18.000000 jaxip-0.6.1/docs/jaxip.descriptors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-05-10 20:36:05.000000 jaxip-0.6.1/docs/jaxip.models.nn.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      400 2023-05-17 19:30:18.000000 jaxip-0.6.1/docs/jaxip.models.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1290 2023-05-17 19:30:18.000000 jaxip-0.6.1/docs/jaxip.potentials.nnp.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-05-10 20:36:05.000000 jaxip-0.6.1/docs/jaxip.potentials.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      961 2023-06-18 10:02:01.000000 jaxip-0.6.1/docs/jaxip.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      560 2023-06-18 10:02:01.000000 jaxip-0.6.1/docs/jaxip.simulation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-10 20:36:05.000000 jaxip-0.6.1/docs/jaxip.utils.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.6.1/docs/make.bat
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-06-18 09:19:55.000000 jaxip-0.6.1/docs/modules.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.6.1/docs/readme.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.6.1/docs/theory.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.6.1/docs/usage.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.884973 jaxip-0.6.1/jaxip/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.6.1/jaxip/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/_version.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.888973 jaxip-0.6.1/jaxip/atoms/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/atoms/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/atoms/_box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/atoms/_neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1471 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/atoms/_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3918 2023-06-18 10:02:01.000000 jaxip-0.6.1/jaxip/atoms/box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6639 2023-06-18 10:02:01.000000 jaxip-0.6.1/jaxip/atoms/element.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3015 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/atoms/neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    17266 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/atoms/structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/config.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.888973 jaxip-0.6.1/jaxip/datasets/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/datasets/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      408 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/datasets/dataset.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6445 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/datasets/runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1039 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/datasets/transformer.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.892974 jaxip-0.6.1/jaxip/descriptors/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/descriptors/__init__.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.892974 jaxip-0.6.1/jaxip/descriptors/acsf/
--rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.6.1/jaxip/descriptors/acsf/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5275 2023-05-06 13:11:44.000000 jaxip-0.6.1/jaxip/descriptors/acsf/_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7767 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/descriptors/acsf/acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2236 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/descriptors/acsf/angular.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2627 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/descriptors/acsf/cutoff.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1495 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/descriptors/acsf/radial.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1015 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/descriptors/acsf/symmetry.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/descriptors/descriptor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/descriptors/scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/logger.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.892974 jaxip-0.6.1/jaxip/models/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.6.1/jaxip/models/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      389 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/models/model.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.892974 jaxip-0.6.1/jaxip/models/nn/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.6.1/jaxip/models/nn/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.6.1/jaxip/models/nn/activation.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.6.1/jaxip/models/nn/initializer.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2911 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/models/nn/network.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.892974 jaxip-0.6.1/jaxip/potentials/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      212 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/potentials/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1973 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/potentials/_energy.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/potentials/_force.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1831 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/potentials/atomic_potential.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.892974 jaxip-0.6.1/jaxip/potentials/nnp/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      238 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/potentials/nnp/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9149 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/potentials/nnp/gradient_descent.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9358 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/potentials/nnp/kalman_filter.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/potentials/nnp/metrics.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      542 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/potentials/nnp/nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    18963 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/potentials/nnp/potential.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11352 2023-06-22 07:40:24.000000 jaxip-0.6.1/jaxip/potentials/nnp/settings.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3585 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/pytree.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.896973 jaxip-0.6.1/jaxip/simulation/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      296 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/simulation/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4289 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/simulation/mc.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     8395 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/simulation/md.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1756 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/simulation/run.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      834 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/simulation/thermostat.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-05-07 09:13:07.000000 jaxip-0.6.1/jaxip/types.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2573 2023-06-18 10:02:01.000000 jaxip-0.6.1/jaxip/units.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.896973 jaxip-0.6.1/jaxip/utils/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/utils/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.6.1/jaxip/utils/attribute.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/utils/batch.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.6.1/jaxip/utils/compare.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/utils/profiler.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.6.1/jaxip/utils/tokenize.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.888973 jaxip-0.6.1/jaxip.egg-info/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5332 2023-06-24 19:26:59.000000 jaxip-0.6.1/jaxip.egg-info/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3296 2023-06-24 19:26:59.000000 jaxip-0.6.1/jaxip.egg-info/SOURCES.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-06-24 19:26:59.000000 jaxip-0.6.1/jaxip.egg-info/dependency_links.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-06-24 19:26:59.000000 jaxip-0.6.1/jaxip.egg-info/entry_points.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-06-22 10:45:16.000000 jaxip-0.6.1/jaxip.egg-info/not-zip-safe
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-06-24 19:26:59.000000 jaxip-0.6.1/jaxip.egg-info/requires.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-06-24 19:26:59.000000 jaxip-0.6.1/jaxip.egg-info/top_level.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-06-24 19:26:59.908974 jaxip-0.6.1/setup.cfg
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.6.1/setup.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.900973 jaxip-0.6.1/tests/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.904974 jaxip-0.6.1/tests/.ipynb_checkpoints/
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.6.1/tests/.ipynb_checkpoints/h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.6.1/tests/.ipynb_checkpoints/h2o-checkpoint.json
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.6.1/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.6.1/tests/.ipynb_checkpoints/test-checkpoint.ipynb
--rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.6.1/tests/__init__.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.6.1/tests/h2o.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.6.1/tests/h2o.json
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1681 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/ljpot.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-06-24 19:18:13.000000 jaxip-0.6.1/tests/scaling.001.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-06-24 19:18:13.000000 jaxip-0.6.1/tests/scaling.008.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5116 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/test_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2536 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/test_mc.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3242 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/test_md.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4115 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/test_nn.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3469 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/test_nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.6.1/tests/test_runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.6.1/tests/test_scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5465 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/test_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-06-24 19:18:13.000000 jaxip-0.6.1/tests/weights.001.pkl
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-06-24 19:18:13.000000 jaxip-0.6.1/tests/weights.008.pkl
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.939054 jaxip-0.7.0/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.7.0/AUTHORS.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.7.0/CONTRIBUTING.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      801 2023-07-10 18:19:00.000000 jaxip-0.7.0/HISTORY.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.7.0/LICENSE
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.7.0/MANIFEST.in
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5649 2023-07-10 18:19:33.939054 jaxip-0.7.0/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5062 2023-07-10 18:19:00.000000 jaxip-0.7.0/README.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.863057 jaxip-0.7.0/docs/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.7.0/docs/Makefile
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.847057 jaxip-0.7.0/docs/_build/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.847057 jaxip-0.7.0/docs/_build/doctrees/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.863057 jaxip-0.7.0/docs/_build/doctrees/nbsphinx/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-07-10 18:10:15.000000 jaxip-0.7.0/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-10 18:10:15.000000 jaxip-0.7.0/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-10 18:10:15.000000 jaxip-0.7.0/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.847057 jaxip-0.7.0/docs/_build/html/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.867056 jaxip-0.7.0/docs/_build/html/_images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-07-10 18:10:15.000000 jaxip-0.7.0/docs/_build/html/_images/notebooks_getting_started_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-10 18:10:15.000000 jaxip-0.7.0/docs/_build/html/_images/notebooks_getting_started_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-10 18:10:15.000000 jaxip-0.7.0/docs/_build/html/_images/notebooks_getting_started_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.867056 jaxip-0.7.0/docs/_build/html/_static/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.7.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.7.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.7.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.7.0/docs/authors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6412 2023-07-10 18:19:00.000000 jaxip-0.7.0/docs/conf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.7.0/docs/contributing.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       77 2023-07-10 18:19:00.000000 jaxip-0.7.0/docs/examples.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.7.0/docs/history.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.871056 jaxip-0.7.0/docs/images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.7.0/docs/images/flowchart.drawio.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.7.0/docs/images/water.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.7.0/docs/index.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.7.0/docs/installation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-10 20:36:05.000000 jaxip-0.7.0/docs/jaxip.atoms.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      662 2023-05-17 19:30:18.000000 jaxip-0.7.0/docs/jaxip.datasets.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-10 20:36:05.000000 jaxip-0.7.0/docs/jaxip.descriptors.acsf.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      613 2023-05-17 19:30:18.000000 jaxip-0.7.0/docs/jaxip.descriptors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-05-10 20:36:05.000000 jaxip-0.7.0/docs/jaxip.models.nn.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      400 2023-05-17 19:30:18.000000 jaxip-0.7.0/docs/jaxip.models.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1290 2023-05-17 19:30:18.000000 jaxip-0.7.0/docs/jaxip.potentials.nnp.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-05-10 20:36:05.000000 jaxip-0.7.0/docs/jaxip.potentials.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      961 2023-07-10 18:10:04.000000 jaxip-0.7.0/docs/jaxip.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      951 2023-07-10 18:19:00.000000 jaxip-0.7.0/docs/jaxip.simulation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-10 20:36:05.000000 jaxip-0.7.0/docs/jaxip.utils.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.7.0/docs/make.bat
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-07-10 18:10:04.000000 jaxip-0.7.0/docs/modules.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.7.0/docs/readme.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.7.0/docs/theory.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.7.0/docs/usage.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.875056 jaxip-0.7.0/jaxip/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.7.0/jaxip/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/_version.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.891055 jaxip-0.7.0/jaxip/atoms/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      232 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/atoms/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1486 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/atoms/_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3683 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/atoms/box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6639 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/atoms/element.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3354 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/atoms/neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    17756 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/atoms/structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1124 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/config.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.891055 jaxip-0.7.0/jaxip/datasets/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/datasets/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      408 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/datasets/dataset.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6451 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/datasets/runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      929 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/datasets/transformer.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.895055 jaxip-0.7.0/jaxip/descriptors/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/descriptors/__init__.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.899055 jaxip-0.7.0/jaxip/descriptors/acsf/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.7.0/jaxip/descriptors/acsf/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5312 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/descriptors/acsf/_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7828 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/descriptors/acsf/acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2236 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/descriptors/acsf/angular.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2627 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/descriptors/acsf/cutoff.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1495 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/descriptors/acsf/radial.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1015 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/descriptors/acsf/symmetry.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/descriptors/descriptor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7467 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/descriptors/scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/logger.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.899055 jaxip-0.7.0/jaxip/models/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.7.0/jaxip/models/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      389 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/models/model.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.903055 jaxip-0.7.0/jaxip/models/nn/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.7.0/jaxip/models/nn/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.7.0/jaxip/models/nn/activation.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.7.0/jaxip/models/nn/initializer.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2902 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/models/nn/network.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.907055 jaxip-0.7.0/jaxip/potentials/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      212 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/potentials/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1979 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/potentials/_energy.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/potentials/_force.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1844 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/potentials/atomic_potential.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.919055 jaxip-0.7.0/jaxip/potentials/nnp/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      238 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/potentials/nnp/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9217 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/potentials/nnp/gradient_descent.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9374 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/potentials/nnp/kalman_filter.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/potentials/nnp/metrics.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      542 2023-06-24 19:26:34.000000 jaxip-0.7.0/jaxip/potentials/nnp/nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    19007 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/potentials/nnp/potential.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11345 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/potentials/nnp/settings.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3627 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/pytree.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.919055 jaxip-0.7.0/jaxip/simulation/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      296 2023-06-24 19:26:34.000000 jaxip-0.7.0/jaxip/simulation/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2143 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/simulation/lj.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4331 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/simulation/mc.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     8523 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/simulation/md.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2515 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/simulation/run.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      840 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/simulation/thermostat.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      766 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/types.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2573 2023-06-18 10:02:01.000000 jaxip-0.7.0/jaxip/units.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.923055 jaxip-0.7.0/jaxip/utils/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/utils/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1418 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/utils/attribute.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/utils/batch.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2012 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/utils/compare.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/utils/profiler.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.7.0/jaxip/utils/tokenize.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.887056 jaxip-0.7.0/jaxip.egg-info/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5649 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3295 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/SOURCES.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/dependency_links.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/entry_points.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/not-zip-safe
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/requires.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/top_level.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-07-10 18:19:33.939054 jaxip-0.7.0/setup.cfg
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.7.0/setup.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.927054 jaxip-0.7.0/tests/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.935054 jaxip-0.7.0/tests/.ipynb_checkpoints/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.7.0/tests/.ipynb_checkpoints/h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.7.0/tests/.ipynb_checkpoints/h2o-checkpoint.json
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.7.0/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.7.0/tests/.ipynb_checkpoints/test-checkpoint.ipynb
+-rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.7.0/tests/__init__.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.7.0/tests/h2o.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.7.0/tests/h2o.json
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-07-10 18:04:56.000000 jaxip-0.7.0/tests/scaling.001.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-07-10 18:04:56.000000 jaxip-0.7.0/tests/scaling.008.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5108 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2569 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_mc.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3137 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_md.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4106 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_nn.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3445 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4825 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2850 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5897 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-07-10 18:04:56.000000 jaxip-0.7.0/tests/weights.001.pkl
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-07-10 18:04:56.000000 jaxip-0.7.0/tests/weights.008.pkl
```

### Comparing `jaxip-0.6.1/CONTRIBUTING.rst` & `jaxip-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/HISTORY.rst` & `jaxip-0.7.0/HISTORY.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 =======
 History
 =======
 
-0.6.x (2023-06-18)
+0.7.x (2023-07-10)
 -------------------
-* molecular dynamics (MD) and Monte-Carlo (MC) simulators
+* Refactored structure including design, documentation, and performance (JIT kernels)
 
+0.6.x (2023-06-18)
+-------------------
+* Implemented Molecular dynamics (MD) and Monte-Carlo (MC) simulators
 
-0.5.0 (2023-03-02)
+0.5.x (2023-03-02)
 -------------------
 * Implemented Kalman filter trainer 
 
-
-0.4.0 (2023-01-03)
+0.4.x (2023-01-03)
 -------------------
 * Applied extensive refactoring
 * Replaced `PyTorch` main dependency with `JAX`
 * First release on PyPI.
 
-
-0.3.0 (2022-12-07)
+0.3.x (2022-12-07)
 -------------------
 * `JAX` optimizations applied to the `ACSF` descriptor
 
-
-0.2.0 (2022-11-11)
+0.2.x (2022-11-11)
 -------------------
 * Some optimizations using `torch.jit.script`
 
-
-0.1.0 (2022-10-28)
+0.1.x (2022-10-28)
 -------------------
 * Primary implementation and validation
 
-
 .. v0.0.1 (2022-01-01)
 .. -------------------
 .. * Start
```

### Comparing `jaxip-0.6.1/LICENSE` & `jaxip-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/PKG-INFO` & `jaxip-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.6.1
+Version: 0.7.0
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -88,14 +88,15 @@
 This script demonstrates the process of evaluating an array of atomic-centered symmetry functions (`ACSF`_) 
 for a specific element, which can be utilized to evaluate the descriptor values for any structure. 
 The resulting values can then be used to construct a machine learning potential.
 
 .. _ACSF: https://aip.scitation.org/doi/10.1063/1.3553717
 
 
+
 .. code-block:: python
 
         from jaxip.datasets import RunnerDataset
         from jaxip.descriptors import ACSF
         from jaxip.descriptors.acsf import CutoffFunction, G2, G3
 
         # Read atomic structure dataset (e.g. water molecules)
@@ -103,22 +104,23 @@
         structure = structures[0]
 
         # Define ACSF descriptor for hydrogen element
         descriptor = ACSF(element='H')
 
         # Add radial and angular symmetry functions
         cfn = CutoffFunction(r_cutoff=12.0, cutoff_type='tanh')
-        descriptor.add( G2(cfn, eta=0.5, r_shift=0.0), 'H')
-        descriptor.add( G3(cfn, eta=0.001, zeta=2.0, lambda0=1.0, r_shift=12.0), 'H', 'O')
+        descriptor.add(G2(cfn, eta=0.5, r_shift=0.0), 'H')
+        descriptor.add(G3(cfn, eta=0.001, zeta=2.0, lambda0=1.0, r_shift=12.0), 'H', 'O')
+        print(descriptor)
 
-        # Compute descriptor values
-        descriptor(structure)
+        values = descriptor(structure)
+        print("Descriptor values:\n", values)
 
-        # Compute gradient
-        descriptor.grad(structure, atom_index=0)
+        gradient = descriptor.grad(structure, atom_index=0)
+        print("Descriptor gradient:\n", gradient)
 
 
 -------------------------------------
 Training a machine learning potential
 -------------------------------------
 This example illustrates how to quickly create a `high-dimensional neural network 
 potential` (`HDNNP`_) instance from an in input setting files and train it on input structures. 
@@ -133,15 +135,15 @@
         from jaxip.potentials import NeuralNetworkPotential
 
         # Read atomic data
         structures = RunnerDataset("input.data")
         structure = structures[0]
 
         # Instantiate potential from input settings file
-        nnp = NeuralNetworkPotential.create_from_file("input.nn")
+        nnp = NeuralNetworkPotential.from_file("input.nn")
 
         # Fit descriptor scaler and model weights
         nnp.fit_scaler(structures)
         nnp.fit_model(structures)
         nnp.save()
 
         # Or loading from files
@@ -150,12 +152,20 @@
         # Total energy
         nnp(structure)
 
         # Force components
         nnp.compute_force(structure)
 
 
+
+Example files: `input.data`_ and `input.nn`_
+
+.. _input.data: https://drive.google.com/file/d/1VMckgIv_OUvCOXQ0pYzaF5yl9AwR0rBy/view?usp=sharing
+.. _input.nn: https://drive.google.com/file/d/15Oq9gAJ2xXVMcHyWXlRukfJFevyVO7lI/view?usp=sharing
+
+
+
 License
 -------
 
 This project is licensed under the GNU General Public License (GPL) version 3 - 
 see the `LICENSE <https://github.com/hghcomphys/jaxip/blob/main/LICENSE>`_ file for details.
```

### Comparing `jaxip-0.6.1/README.rst` & `jaxip-0.7.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 This script demonstrates the process of evaluating an array of atomic-centered symmetry functions (`ACSF`_) 
 for a specific element, which can be utilized to evaluate the descriptor values for any structure. 
 The resulting values can then be used to construct a machine learning potential.
 
 .. _ACSF: https://aip.scitation.org/doi/10.1063/1.3553717
 
 
+
 .. code-block:: python
 
         from jaxip.datasets import RunnerDataset
         from jaxip.descriptors import ACSF
         from jaxip.descriptors.acsf import CutoffFunction, G2, G3
 
         # Read atomic structure dataset (e.g. water molecules)
@@ -85,22 +86,23 @@
         structure = structures[0]
 
         # Define ACSF descriptor for hydrogen element
         descriptor = ACSF(element='H')
 
         # Add radial and angular symmetry functions
         cfn = CutoffFunction(r_cutoff=12.0, cutoff_type='tanh')
-        descriptor.add( G2(cfn, eta=0.5, r_shift=0.0), 'H')
-        descriptor.add( G3(cfn, eta=0.001, zeta=2.0, lambda0=1.0, r_shift=12.0), 'H', 'O')
+        descriptor.add(G2(cfn, eta=0.5, r_shift=0.0), 'H')
+        descriptor.add(G3(cfn, eta=0.001, zeta=2.0, lambda0=1.0, r_shift=12.0), 'H', 'O')
+        print(descriptor)
 
-        # Compute descriptor values
-        descriptor(structure)
+        values = descriptor(structure)
+        print("Descriptor values:\n", values)
 
-        # Compute gradient
-        descriptor.grad(structure, atom_index=0)
+        gradient = descriptor.grad(structure, atom_index=0)
+        print("Descriptor gradient:\n", gradient)
 
 
 -------------------------------------
 Training a machine learning potential
 -------------------------------------
 This example illustrates how to quickly create a `high-dimensional neural network 
 potential` (`HDNNP`_) instance from an in input setting files and train it on input structures. 
@@ -115,15 +117,15 @@
         from jaxip.potentials import NeuralNetworkPotential
 
         # Read atomic data
         structures = RunnerDataset("input.data")
         structure = structures[0]
 
         # Instantiate potential from input settings file
-        nnp = NeuralNetworkPotential.create_from_file("input.nn")
+        nnp = NeuralNetworkPotential.from_file("input.nn")
 
         # Fit descriptor scaler and model weights
         nnp.fit_scaler(structures)
         nnp.fit_model(structures)
         nnp.save()
 
         # Or loading from files
@@ -132,12 +134,20 @@
         # Total energy
         nnp(structure)
 
         # Force components
         nnp.compute_force(structure)
 
 
+
+Example files: `input.data`_ and `input.nn`_
+
+.. _input.data: https://drive.google.com/file/d/1VMckgIv_OUvCOXQ0pYzaF5yl9AwR0rBy/view?usp=sharing
+.. _input.nn: https://drive.google.com/file/d/15Oq9gAJ2xXVMcHyWXlRukfJFevyVO7lI/view?usp=sharing
+
+
+
 License
 -------
 
 This project is licensed under the GNU General Public License (GPL) version 3 - 
 see the `LICENSE <https://github.com/hghcomphys/jaxip/blob/main/LICENSE>`_ file for details.
```

### Comparing `jaxip-0.6.1/docs/Makefile` & `jaxip-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png` & `jaxip-0.7.0/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png` & `jaxip-0.7.0/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png` & `jaxip-0.7.0/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/_build/html/_images/notebooks_tutorials_38_0.png` & `jaxip-0.7.0/docs/_build/html/_images/notebooks_getting_started_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/_build/html/_images/notebooks_tutorials_45_0.png` & `jaxip-0.7.0/docs/_build/html/_images/notebooks_getting_started_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/_build/html/_images/notebooks_tutorials_51_0.png` & `jaxip-0.7.0/docs/_build/html/_images/notebooks_getting_started_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/conf.py` & `jaxip-0.7.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,12 +217,12 @@
 
 curdir = os.path.dirname(os.path.abspath(__file__))
 notebooks_dir = os.path.join(curdir, "notebooks")
 if os.path.exists(notebooks_dir):
     shutil.rmtree(notebooks_dir)
 os.makedirs(notebooks_dir, exist_ok=True)
 
-for filename in ("tutorials.ipynb", "training.ipynb"):
+for filename in ("getting_started.ipynb", "training.ipynb"):
     shutil.copyfile(  # copytree(
         os.path.join(curdir, "..", "examples", filename),
         os.path.join(curdir, "notebooks", filename),
     )
```

### Comparing `jaxip-0.6.1/docs/images/flowchart.drawio.png` & `jaxip-0.7.0/docs/images/flowchart.drawio.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/images/water.png` & `jaxip-0.7.0/docs/images/water.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/installation.rst` & `jaxip-0.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/jaxip.atoms.rst` & `jaxip-0.7.0/docs/jaxip.atoms.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/jaxip.datasets.rst` & `jaxip-0.7.0/docs/jaxip.datasets.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/jaxip.descriptors.acsf.rst` & `jaxip-0.7.0/docs/jaxip.descriptors.acsf.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/jaxip.descriptors.rst` & `jaxip-0.7.0/docs/jaxip.descriptors.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/jaxip.models.nn.rst` & `jaxip-0.7.0/docs/jaxip.models.nn.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/jaxip.potentials.nnp.rst` & `jaxip-0.7.0/docs/jaxip.potentials.nnp.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/jaxip.rst` & `jaxip-0.7.0/docs/jaxip.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/jaxip.simulation.rst` & `jaxip-0.7.0/docs/jaxip.simulation.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,41 @@
 jaxip.simulation package
 ========================
 
 Submodules
 ----------
 
-jaxip.simulation.molecular\_dynamics module
--------------------------------------------
+jaxip.simulation.lj module
+--------------------------
 
-.. automodule:: jaxip.simulation.molecular_dynamics
+.. automodule:: jaxip.simulation.lj
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+jaxip.simulation.mc module
+--------------------------
+
+.. automodule:: jaxip.simulation.mc
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+jaxip.simulation.md module
+--------------------------
+
+.. automodule:: jaxip.simulation.md
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+jaxip.simulation.run module
+---------------------------
+
+.. automodule:: jaxip.simulation.run
    :members:
    :undoc-members:
    :show-inheritance:
 
 jaxip.simulation.thermostat module
 ----------------------------------
```

### Comparing `jaxip-0.6.1/docs/jaxip.utils.rst` & `jaxip-0.7.0/docs/jaxip.utils.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/make.bat` & `jaxip-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/theory.rst` & `jaxip-0.7.0/docs/theory.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/docs/usage.rst` & `jaxip-0.7.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/__init__.py` & `jaxip-0.7.0/jaxip/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/atoms/_structure.py` & `jaxip-0.7.0/jaxip/atoms/_structure.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,47 +5,48 @@
 import jax
 import jax.numpy as jnp
 
 from jaxip.atoms.box import _apply_pbc
 from jaxip.types import Array
 
 
-@jax.jit
-def _calculate_distance_per_atom(
-    atom_position: Array,
-    neighbor_position: Array,
+# @jax.jit
+def _calculate_distances_per_atom(
+    atom_positions: Array,
+    neighbor_positions: Array,
     lattice: Optional[Array] = None,
 ) -> Tuple[Array, Array]:
-    """Calculate an array of distances between a single atom and neighboring atoms."""
-    dx: Array = atom_position - neighbor_position
+    """Calculate distances between a single atom and neighboring atoms."""
+    dx: Array = atom_positions - neighbor_positions
     if lattice is not None:
         dx = _apply_pbc(dx, lattice)
-
     # Fix NaN in gradient of np.linalg.norm
     # see https://github.com/google/jax/issues/3058
     is_zero = dx.sum(axis=1, keepdims=True) == 0.0
     dx_ = jnp.where(is_zero, jnp.ones_like(dx), dx)
     dist = jnp.linalg.norm(dx_, ord=2, axis=1)
     dist = jnp.where(jnp.squeeze(is_zero), 0.0, dist)
-
-    return dist, dx  # type: ignore
+    return dist, dx
 
 
-_vmap_calculate_distance: Callable = jax.vmap(
-    _calculate_distance_per_atom,
+_vmap_calculate_distances: Callable = jax.vmap(
+    _calculate_distances_per_atom,
     in_axes=(0, None, None),
 )
 
 
 @jax.jit
-def _calculate_distance(
-    atom_position: Array,
-    neighbor_position: Array,
+def _calculate_distances(
+    atom_positions: Array,
+    neighbor_positions: Array,
     lattice: Optional[Array] = None,
 ) -> Tuple[Array, Array]:
-    """Calculate an array of distances between multiple atoms and the neighbors (using `jax.vmap`)."""
-    return _vmap_calculate_distance(atom_position, neighbor_position, lattice)
+    """Calculate an array of distances between multiple atoms
+    and the neighbors (using `jax.vmap`)."""
+    return _vmap_calculate_distances(
+        atom_positions, neighbor_positions, lattice
+    )
 
 
 @jax.jit
-def _get_center_of_mass(array: Array, mass: Array) -> Array:
-    return jnp.sum(mass * array, axis=0) / jnp.sum(mass)
+def _calculate_center_of_mass(array: Array, masses: Array) -> Array:
+    return jnp.sum(masses * array, axis=0) / jnp.sum(masses)
```

### Comparing `jaxip-0.6.1/jaxip/atoms/element.py` & `jaxip-0.7.0/jaxip/atoms/element.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,57 +67,56 @@
     efficient array processing (e.g. applying conditions) using
     the arrays of integer (i.e. atom types) instead of strings.
     """
 
     def __init__(self, elements: List[Element]) -> None:
         """Initialize element map."""
         self.unique_elements: Set[Element] = set(elements)
-        self._elem_to_atomic_num: Dict[Element, int] = dict()
-        self._elem_to_atom_type: Dict[Element, int] = dict()
-        self._atom_type_to_elem: Dict[int, Element] = dict()
+        self._element_to_atomic_number: Dict[Element, int] = dict()
+        self._element_to_atom_type: Dict[Element, int] = dict()
+        self._atom_type_to_element: Dict[int, Element] = dict()
         self._create_mapping_dicts()
+        logger.debug(f"Initialized {self.__class__.__name__}")
 
-        logger.debug(f"Initializing {self.__class__.__name__}()")
+    def __call__(self, item: Union[Element, int]) -> Union[int, Element]:
+        """Map an element to the atom type and vice versa."""
+        result: Union[int, Element]
+        if isinstance(item, int):
+            return self._atom_type_to_element[item]
+        elif isinstance(item, Element):
+            return self._element_to_atom_type[item]
+        else:
+            logger.error(
+                f"Unknown item type '{type(item)}'", exception=TypeError
+            )
+            return  # type: ignore
 
     def _create_mapping_dicts(self) -> None:
         """
         Create dictionary to map elements, atom types, and atomic numbers.
-        The given atom types are given and sorted based on elements' atomic number.
+        The atom types are sorted based on elements' atomic number.
         """
-        self._elem_to_atomic_num = {
+        self._element_to_atomic_number = {
             elem: _KNOWN_ELEMENTS_DICT[elem] for elem in self.unique_elements
         }
-        self._elem_to_atom_type = {
+        self._element_to_atom_type = {
             elem: atom_type
             for atom_type, elem in enumerate(
                 sorted(
-                    self._elem_to_atomic_num,
-                    key=self._elem_to_atomic_num.get,  # type: ignore
+                    self._element_to_atomic_number,
+                    key=self._element_to_atomic_number.get,  # type: ignore
                 ),
                 start=1,
             )
         }
-        self._atom_type_to_elem = {
-            atom_type: elem for elem, atom_type in self._elem_to_atom_type.items()
+        self._atom_type_to_element = {
+            atom_type: elem
+            for elem, atom_type in self._element_to_atom_type.items()
         }
 
-    def __getitem__(self, item: Union[Element, int]) -> Union[int, Element]:
-        """Map an element to the atom type and vice versa."""
-        result: Union[int, Element]
-        if isinstance(item, int):
-            result = self._atom_type_to_elem[item]
-        elif isinstance(item, Element):
-            result = self._elem_to_atom_type[item]
-        else:
-            logger.error(f"Unknown item type '{type(item)}'", exception=TypeError)
-        return result  # type: ignore
-
-    def __call__(self, item: Union[Element, int]) -> Union[int, Element]:
-        return self[item]
-
     @classmethod
     def get_atomic_number(cls, element: Element) -> int:
         """
         Return atomic number of the input element.
 
         :param element: element name
         :return: atomic number
@@ -134,29 +133,35 @@
         """
         return _KNOWN_ELEMENTS_LIST[atomic_number - 1]
 
     @property
     def atom_type_to_element(self) -> Dict[int, Element]:
         """
         Return a dictionary mapping of atom type to element.
-        This property is defined due to a serialization issue of the ElementMap class during parallelization.
 
-        :return: a dictionary of mapping an atom type (integer) to the corresponding element (string)
+        This property is defined due to a serialization issue
+        of the ElementMap class during parallelization.
+
+        :return: a dictionary of mapping an atom type (integer)
+        to the corresponding element (string)
         """
-        return self._atom_type_to_elem
+        return self._atom_type_to_element
 
     @property
-    def element_to_atype(self) -> Dict[Element, int]:
+    def element_to_atom_type(self) -> Dict[Element, int]:
         """
         Return a mapping dictionary of element to atom type.
-        This property is defined due to a serialization issue of the ElementMap class during parallelization.
 
-        :return: a dictionary of mapping an element (string) to the corresponding atom type (integer)
+        This property is defined due to a serialization issue of
+        the ElementMap class during parallelization.
+
+        :return: a dictionary of mapping an element (string) to
+        the corresponding atom type (integer)
         """
-        return self._elem_to_atom_type
+        return self._element_to_atom_type
 
     @classmethod
     def atomic_number_to_element(cls, atomic_number: int) -> Element:
         return _KNOWN_ELEMENTS_LIST[atomic_number - 1]
 
     @classmethod
     def element_to_atomic_number(cls, element: Element) -> int:
```

### Comparing `jaxip-0.6.1/jaxip/atoms/structure.py` & `jaxip-0.7.0/jaxip/atoms/structure.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,478 +1,502 @@
 from __future__ import annotations
 
 from collections import defaultdict
-from dataclasses import dataclass, field
-from typing import Any, DefaultDict, Dict, Generator, List, NamedTuple, Optional, Tuple
+from dataclasses import dataclass
+from typing import (
+    Any,
+    DefaultDict,
+    Dict,
+    Iterator,
+    List,
+    NamedTuple,
+    Optional,
+    Tuple,
+)
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 from ase import Atoms as AseAtoms
 from jax import tree_util
 
-from jaxip.atoms._structure import _calculate_distance, _get_center_of_mass
+from jaxip.atoms._structure import (
+    _calculate_center_of_mass,
+    _calculate_distances,
+)
 from jaxip.atoms.box import Box
 from jaxip.atoms.element import ElementMap
 from jaxip.atoms.neighbor import Neighbor
 from jaxip.logger import logger
 from jaxip.pytree import BaseJaxPytreeDataClass, register_jax_pytree_node
-from jaxip.types import Array, Dtype, Element
-from jaxip.types import dtype as _dtype
+from jaxip.types import Array, Dtype, Element, _dtype
 from jaxip.units import units
 
 
-class Inputs(NamedTuple):
-    """
-    Represents array data types of Structure.
-    """
-
-    atom_position: Array
-    position: Array
-    atype: Array
-    lattice: Array
-    emap: Dict[Element, Array]
-
-
 @dataclass
 class Structure(BaseJaxPytreeDataClass):
     """
-    A structure contains arrays of atomic attributes
-    for a collection of atoms in the simulation box.
+    A structure in the context of simulation box consists of
+    arrays that store atomic attributes for a collection of atoms.
 
-    Atomic attributes:
+    The attributes of atoms within a structure can be described as follows:
 
-    * `position`: per-atom position x, y, and z
-    * `force`: per-atom force components x, y, and z
-    * `energy`:  per-atom energy
-    * `total_energy`: total energy of atoms in simulation box
-    * `charge`:  per-atom electric charge
-    * `total_charge`: total charge of atoms in simulation box
-    * `atom_type`: per-atom type (unique integer) corresponding to each element
-
-    An instance structure can be seen as unit of data.
-    list of structures will be used to train a potential,
-    or new energy and forces components can be computed for a given structure.
+    * `positions`: position of atoms
+    * `forces`: force components
+    * `energies`: associated atom energies
+    * `total_energy`: the total energy of atoms
+    * `charges`:  electric charges
+    * `total_charge`: the total charge of atoms
+
+    The structure serves as a fundamental data unit for the atoms in the simulation box.
+    Multiple structures can be gathered into a list to train a potential, or alternatively,
+    the total energy and force components can be computed for a specific structure.
 
     Each structure has three additional instances:
 
-    * `Box`: applying periodic boundary conditions (PBC)
-    * `ElementMap`: determines how to extract atom types (integer) from the element (string)
-    * `Neighbor`: computes the list of neighboring atoms inside a given cutoff radius
+    * `Box`: applying periodic boundary condition (PBC) along x, y, and z directions
+    * `ElementMap`: determines how to extract assigned atom types from the element and vice versa
+    * `Neighbor`: computes the list of neighboring atoms inside a specified cutoff radius
 
     .. note::
-        `Structure` can be considered as one domain
-        in the domain decomposition method for the MPI implementation (see `miniMD`_).
+        The structure can be viewed as a separate domain for implementing MPI in large-scale
+        molecular dynamics (MD) simulations, as demonstrated in the `miniMD`_ program.
 
     .. _miniMD: https://github.com/Mantevo/miniMD
     """
 
-    position: Array
-    force: Array
-    energy: Array
+    positions: Array
+    forces: Array
+    energies: Array
     total_energy: Array
-    charge: Array
+    charges: Array
     total_charge: Array
-    atom_type: Array
-    box: Box
+    atom_types: Array
     element_map: ElementMap
-    neighbor: Neighbor
-    requires_neighbor_update: bool = field(default=True)
+    box: Optional[Box] = None
+    neighbor: Optional[Neighbor] = None
 
-    # --------------------------------------------------------------------------------------
+    def __post_init__(self) -> None:
+        logger.debug(f"Initializing {self.__class__.__name__}()")
+        self._assert_jit_dynamic_attributes(
+            expected=(
+                "positions",
+                "forces",
+                "energies",
+                "total_energy",
+                "charges",
+                "total_charge",
+                "atom_types",
+            )
+        )
+        self._assert_jit_static_attributes(
+            expected=(
+                "element_map",
+                "box",
+                "neighbor",
+            )
+        )
+        if self.box is not None:
+            self.positions = self.box.shift_inside_box(self.positions)
 
     @classmethod
-    def create_from_dict(
+    def from_dict(
         cls,
         data: Dict[str, Any],
-        r_cutoff: Optional[float] = None,
         dtype: Optional[Dtype] = None,
     ) -> Structure:
         """
-        Create a new instance of structure from a dictionary of data including
-        positions, forces, box, neighbor, etc.
+        Instantiate a structure object using an input data dictionary that contains
+        distinct lists of positions, forces, elements, lattice, etc.
 
         :param data: input data
-        :param r_cutoff: neighbor atom cutoff radius, defaults to None
-        :param dtype: data type of arrays, defaults to None
-        :return: an initialized instance
+        :param r_cutoff: neighbor atoms cutoff radius, defaults to None
+        :param dtype: data type for arrays, defaults to None
+        :return: the initialized Structure
         """
         if dtype is None:
             dtype = _dtype.FLOATX
 
-        kwargs: Dict[str, Any] = dict()
-        data_: DefaultDict[str, List] = defaultdict(list, data)
+        input_data: DefaultDict[str, List] = defaultdict(list, data)
+        inputs: Dict[str, Any] = dict()
         try:
-            element_map: ElementMap = ElementMap(data_["element"])
-            kwargs.update(
-                cls._init_arrays(data_, element_map=element_map, dtype=dtype),
+            element_map: ElementMap = ElementMap(input_data["elements"])
+            inputs.update(
+                cls._init_arrays(
+                    input_data,
+                    element_map=element_map,
+                    dtype=dtype,
+                ),
             )
-            kwargs["box"] = cls._init_box(data_["lattice"], dtype=dtype)
-            kwargs["element_map"] = element_map
-            kwargs["neighbor"] = Neighbor(r_cutoff=r_cutoff)
-
+            inputs["element_map"] = element_map
+            inputs["box"] = cls._init_box(input_data["lattice"], dtype=dtype)
         except KeyError:
             logger.error(
                 "Cannot find at least one of the expected keyword in the input data.",
                 exception=KeyError,
             )
-        return cls(**kwargs)
+        return cls(**inputs)
 
     @classmethod
-    def create_from_ase(
+    def from_ase(
         cls,
         atoms: AseAtoms,
-        r_cutoff: Optional[float] = None,
         dtype: Optional[Dtype] = None,
     ) -> Structure:
         """
-        Create a new instance of structure from the ASE atoms.
+        Create an instance of the structure based on the input `ASE`_ atoms.
 
-        :param atoms: input ASE atoms instance
-        :param r_cutoff: neighbor atom cutoff radius, defaults to None
-        :param dtype: data type of arrays, defaults to None
-        :return: an initialized instance
+        :param atoms: input `ASE`_ atoms instance
+        :param r_cutoff: neighbor atoms cutoff radius, defaults to None
+        :param dtype: data type for arrays, defaults to None
+        :return: the initialized structure
+
+        .. _ASE: https://wiki.fysik.dtu.dk/ase/index.html
         """
         if dtype is None:
             dtype = _dtype.FLOATX
 
-        kwargs: Dict[str, Any] = dict()
-
-        # Extract atom info from the ASE atoms instance
+        inputs: Dict[str, Any] = dict()
         data = {
-            "element": [
+            "elements": [
                 ElementMap.atomic_number_to_element(n)
                 for n in atoms.get_atomic_numbers()
             ],
-            "lattice": np.asarray(atoms.get_cell() * units.FROM_ANGSTROM),
-            "position": atoms.get_positions() * units.FROM_ANGSTROM,
+            "lattice": np.array(
+                atoms.get_cell() * units.FROM_ANGSTROM, dtype=dtype
+            ),
+            "positions": atoms.get_positions() * units.FROM_ANGSTROM,
         }
-        for key, attr in zip(
-            ("charge", "energy"),
+        for attr, ase_attr in zip(
+            ("charges", "energies"),
             ("charges", "potential_energies"),
         ):
             try:
-                data[key] = getattr(atoms, f"get_{attr}")()
+                data[attr] = getattr(atoms, f"get_{ase_attr}")()
             except RuntimeError:
                 continue
-        for attr in ("energy", "charge"):
+        for attr in ("energies", "charges"):
             if attr in data:
                 data[f"total_{attr}"] = sum(data[attr])
 
-        data_: DefaultDict[str, List] = defaultdict(list, data)
+        input_data: DefaultDict[str, List] = defaultdict(list, data)
         try:
-            element_map: ElementMap = ElementMap(data_["element"])
-            kwargs.update(
-                cls._init_arrays(data_, element_map=element_map, dtype=dtype),
+            element_map: ElementMap = ElementMap(input_data["elements"])
+            inputs.update(
+                cls._init_arrays(
+                    input_data, element_map=element_map, dtype=dtype
+                ),
             )
-            kwargs["box"] = cls._init_box(data_["lattice"], dtype=dtype)
-            kwargs["element_map"] = element_map
-            kwargs["neighbor"] = Neighbor(r_cutoff=r_cutoff)
-
+            inputs["element_map"] = element_map
+            inputs["box"] = cls._init_box(input_data["lattice"], dtype=dtype)
         except KeyError:
             logger.error(
-                "Cannot find at least one of the expected keyword in the input data.",
+                "Can not find at least one of the expected keyword in the input data.",
                 exception=KeyError,
             )
-        return cls(**kwargs)
+        return cls(**inputs)
 
-    @staticmethod
+    @classmethod
     def _init_arrays(
-        data: Dict, element_map: ElementMap, dtype: Dtype
+        cls,
+        data: Dict[str, Any],
+        element_map: ElementMap,
+        dtype: Dtype,
     ) -> Dict[str, Array]:
-        """Initialize a dictionary of arrays of atomic attributes from the input data."""
-        logger.debug("Allocating arrays for a structure as follows:")
+        """Initialize array atomic attributes from the input data dictionary."""
+        logger.debug(f"{cls.__name__} is allocating arrays as follows:")
         arrays: Dict[str, Array] = dict()
         for atom_attr in Structure._get_atom_attributes():
             try:
                 array: Array
-                if atom_attr == "atom_type":
-                    array = jnp.asarray(
-                        [element_map(atom) for atom in data["element"]],
+                if atom_attr == "atom_types":
+                    array = jnp.array(
+                        [element_map(atom) for atom in data["elements"]],
                         dtype=_dtype.INDEX,
                     )
                 else:
-                    array = jnp.asarray(data[atom_attr], dtype=dtype)
+                    array = jnp.array(data[atom_attr], dtype=dtype)
                 arrays[atom_attr] = array
                 logger.debug(
                     f"{atom_attr:12} -> Array(shape={array.shape}, dtype='{array.dtype}')"
                 )
             except KeyError:
                 logger.error(
                     f"Cannot find atom attribute {atom_attr} in the input data",
-                    exception=KeyError,  # type:ignore
+                    exception=KeyError,
                 )
         return arrays
 
-    @staticmethod
-    def _init_box(lattice: List[List[float]], dtype: Dtype) -> Box:
-        """Initialize a simulation box from the input lattice matrix."""
-        box: Box
+    @classmethod
+    def _init_box(
+        cls,
+        lattice: List[List[float]],
+        dtype: Dtype,
+    ) -> Optional[Box]:
+        """Initialize simulation box from input lattice matrix."""
         if len(lattice) > 0:
-            box = Box(jnp.asarray(lattice, dtype=dtype))
+            return Box(lattice, dtype=dtype)
         else:
-            logger.debug("No lattice info were found in structure")
-            box = Box()
-        return box
+            logger.debug("No lattice info were found")
 
-    @classmethod
-    def _get_atom_attributes(cls) -> Tuple[str, ...]:
-        """Get atom attributes which are basically array values."""
-        return cls._get_jit_dynamic_attributes()
-
-    def __post_init__(self) -> None:
-        """Post initializations."""
-        self.position = self.box.shift_inside_box(self.position)
-        logger.debug(f"Initializing {self.__class__.__name__}()")
-        self._assert_jit_dynamic_attributes(
-            expected=(
-                "position",
-                "force",
-                "energy",
-                "total_energy",
-                "charge",
-                "total_charge",
-                "atom_type",
-            )
-        )
-        self._assert_jit_static_attributes(
-            expected=(
-                "box",
-                "element_map",
-                "neighbor",
-                "requires_neighbor_update",
-            )
-        )
-
-    def __hash__(self) -> int:
-        """Enforce to use the parent class's hash method (JIT)."""
-        return super().__hash__()
-
-    # --------------------------------------------------------------------------------------
-
-    def set_cutoff_radius(self, r_cutoff: float) -> None:
+    def update_neighbor(self, r_cutoff: Optional[float] = None) -> None:
         """
-        Set cutoff radius of neighbor atoms in the structure.
-        This method is useful when having a potential with different cutoff radius.
+        Update the neighbor list, building it if required.
 
-        Updating of the neighbor list for a new cutoff radius is skipped if it is the same the previous one.
-        It's important to note that the Neighbor object in Structure is considered as a buffer and not
-        part of the atomic structure data, and it is used for calculating descriptors, potential, etc.
-        It is the task of calling classes to prepare the buffer neighbor before using it.
 
-        :param r_cutoff: a new values for the cutoff radius
-        :type r_cutoff: float
-        """
-        if self.r_cutoff == r_cutoff:
-            logger.info(
-                f"Skipping updating the neighbor list (cutoff radius): "
-                f"{self.r_cutoff} vs. {r_cutoff} (new)"
-            )
-            return
+        This is useful for efficiently determining the neighboring atoms within
+        a specified cutoff radius. The neighbor list allows for faster calculations
+        properties that depend on nearby atoms, such as computing forces, energies,
+        or evaluating interatomic distances.
 
-        self.neighbor.set_cutoff_radius(r_cutoff)
-        self.requires_neighbor_update = True
-
-    def update_neighbor(self) -> None:
-        """
-        Update the neighbor list of the structure.
-        This task can be computationally expensive.
+        There are various scenarios that may necessitate updating the neighbor list,
+        including changes in the positions of atoms within the structure,
+        modifications to the cutoff radius, or both.
         """
-        self.neighbor.update(self)
+        if self.neighbor is not None:
+            self.neighbor.update(self, r_cutoff)
+        elif r_cutoff is not None:
+            self.neighbor = Neighbor.from_structure(self, r_cutoff)
+        else:
+            logger.error(
+                "No cutoff radius was found",
+                exception=ValueError,
+            )
 
-    @property
-    def r_cutoff(self) -> Optional[float]:
-        """Return cutoff radius of neighboring atoms."""
-        return self.neighbor.r_cutoff
+    @classmethod
+    def _get_atom_attributes(cls) -> Tuple[str, ...]:
+        return cls._get_jit_dynamic_attributes()
 
-    # --------------------------------------------------------------------------------------
+    def __hash__(self) -> int:
+        """Use parent class's hash method because of JIT."""
+        return super().__hash__()
 
     @property
     def natoms(self) -> int:
-        """Number of atoms in the structure"""
-        return self.position.shape[0]
+        """Return number of atoms in the structure"""
+        return self.positions.shape[0]
 
     @property
     def dtype(self) -> Dtype:
-        """Datatype of the arrays in the structure (e.g. float32)."""
-        return self.position.dtype
+        """Return data type of the arrays in the structure (e.g., float64)."""
+        return self.positions.dtype
+
+    @property
+    def r_cutoff(self) -> Optional[float]:
+        """Return cutoff radius for neighboring atoms."""
+        if self.neighbor is not None:
+            return self.neighbor.r_cutoff
 
     @property
     def lattice(self) -> Optional[Array]:
         """Cell 3x3 matrix."""
-        return self.box.lattice
+        if self.box is not None:
+            return self.box.lattice
 
-    @property
-    def elements(self) -> tuple[Element, ...]:
-        atom_type_host = jax.device_get(self.atom_type)
-        return tuple(sorted({str(self.element_map(int(at))) for at in atom_type_host}))
+    def get_unique_elements(self) -> Tuple[Element, ...]:
+        return tuple(sorted(set(self.get_elements())))
 
-    @property
-    def mass(self) -> Array:
-        """Return an array of atomic masses."""
+    def get_elements(self) -> Tuple[Element, ...]:
+        """Get array of elements."""
         to_element = self.element_map.atom_type_to_element
-        elements = (to_element[int(at)] for at in self.atom_type)
+        atom_types_host = jax.device_get(self.atom_types)
+        return tuple(str(to_element[int(at)]) for at in atom_types_host)
+
+    def get_masses(self) -> Array:
+        """Get array of atomic masses."""
+        to_element = self.element_map.atom_type_to_element
+        elements = (to_element[int(at)] for at in self.atom_types)
         return jnp.array(
-            tuple(ElementMap.element_to_atomic_mass(element) for element in elements)
+            tuple(
+                ElementMap.element_to_atomic_mass(element)
+                for element in elements
+            )
         )
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}"
-            f"(natoms={self.natoms}, elements={self.elements}, dtype={self.dtype})"
+            f"(natoms={self.natoms}, "
+            f"elements={self.get_unique_elements()}, "
+            f"dtype={self.dtype})"
         )
 
     def select(self, element: Element) -> Array:
         """
-        Return all atom indices of the element.
+        Retrieve the indices of all atoms that correspond to the given element.
 
         :param element: element name (e.g. `H` for hydrogen)
         :return: atom indices
         """
-        return jnp.nonzero(self.atom_type == self.element_map[element])[0]
+        return jnp.nonzero(
+            self.atom_types == self.element_map.element_to_atom_type[element]
+        )[0]
 
-    # @jax.jit
-    def calculate_distance(
+    @jax.jit
+    def calculate_distances(
         self,
-        atom_index: Array,
-        neighbor_index: Optional[Array] = None,
+        atom_indices: Optional[Array] = None,
+        neighbor_indices: Optional[Array] = None,
     ) -> Tuple[Array, Array]:
         """
         Calculate distances between specific atoms (given by atom indices)
         and the neighboring atoms in the structure.
-        This method also returns the corresponding position difference.
+        This method optionally also returns the corresponding position differences.
 
-        If no neighbor index is given, all atoms in the structure
-        will be considered as neighbor atoms.
+        If atom indices are not specified, all atoms in the structure will be taken into account.
+        Similarly, if neighbor indices are not provided, all neighboring atoms will be considered.
 
-        :param atom_index: array of atom indices
-        :type atom_index: Array
-        :param neighbor_index: indices of neighbor atoms, defaults to None
-        :type neighbor_index: Optional[Array], optional
-        :return:  distances, position differences
-        :rtype: Tuple[Array, Array]
-        """
-        atom_position = self.position[jnp.asarray([atom_index])].reshape(-1, 3)
-        if neighbor_index is not None:
-            neighbor_position = self.position[jnp.atleast_1d(neighbor_index)]
+        :param atom_indices: array of atom indices (zero-based index)
+        :type atom_indices: Optional[Array], optional
+        :param neighbor_indices: indices of neighbor atoms, defaults to None
+        :type neighbor_indices: Optional[Array], optional
+        :type neighbor_indices: bool, optional
+        :param return_position_differences: whether returning position differences, defaults to False
+        :type return_position_differences: bool, optional
+        :return:  distances between atoms
+        :rtype: Tuple[Array, ...]
+        """
+        if atom_indices is not None:
+            atom_positions = self.positions[
+                jnp.asarray([atom_indices])
+            ].reshape(-1, 3)
         else:
-            neighbor_position = self.position
+            atom_positions = self.positions
 
-        dis, dx = _calculate_distance(
-            atom_position, neighbor_position, self.box.lattice
-        )
-        return jnp.squeeze(dis), jnp.squeeze(dx)
+        if neighbor_indices is not None:
+            neighbor_positions = self.positions[
+                jnp.atleast_1d(neighbor_indices)
+            ]
+        else:
+            neighbor_positions = self.positions
 
-    # --------------------------------------------------------------------------------------
+        distances, position_differences = _calculate_distances(
+            atom_positions,
+            neighbor_positions,
+            self.lattice,
+        )
+        return jnp.squeeze(distances), jnp.squeeze(position_differences)
 
     def to_dict(self) -> Dict[str, np.ndarray]:
         """
-        Return arrays of atomic attributes in form of dictionary of numpy arrays.
-        To be used, for example, for dumping structure data into a file.
+        The atomic attributes are represented as a dictionary of NumPy arrays.
+        This format can be employed, for instance, when saving the structure data into a file.
 
         :return: dictionary of atom attributes.
         :rtype: Dict[str, np.ndarray]
         """
         data = dict()
         for atom_attr in self._get_atom_attributes():
             array: Array = getattr(self, atom_attr)
             data[atom_attr] = np.asarray(array)
         return data
 
-    def to_ase_atoms(self) -> AseAtoms:
+    def to_ase(self) -> AseAtoms:
         """
-        An ASE representation of the structure.
-        The returned atoms object can be used to visualize or modify the structure using the ASE package.
+        Represent the structure as ASE atoms.
 
-        .. warning::
-            This works only for orthogonal cells.
+        The returned object can be utilized with the `ASE`_ package
+        for visualization or modification of the structure.
 
-        :return: ASE representation of the structure
-        :rtype: AseAtoms
+        :return: `ASE`_ representation of the structure
+
+        .. _ASE: https://wiki.fysik.dtu.dk/ase/index.html
         """
-        logger.info("Creating a representation of the structure in form of ASE atoms")
+        logger.info("Creating an ASE representation of the structure")
+        to_element = self.element_map.atom_type_to_element
         return AseAtoms(
-            symbols=[self.element_map(int(at)) for at in self.atom_type],
-            positions=[units.TO_ANGSTROM * np.asarray(pos) for pos in self.position],
-            cell=units.TO_ANGSTROM * np.asarray(self.box.lattice) if self.box else None,
+            symbols=[to_element[int(at)] for at in self.atom_types],
+            positions=[
+                units.TO_ANGSTROM * np.asarray(pos) for pos in self.positions
+            ],
+            cell=units.TO_ANGSTROM * np.asarray(self.box.lattice)
+            if self.box is not None
+            else None,
             pbc=True if self.box else False,
-            charges=[np.asarray(ch) for ch in self.charge],
+            charges=[np.asarray(ch) for ch in self.charges],
         )
 
-    # --------------------------------------------------------------------------------------
-
     def _get_energy_offset(self, atom_energy: Dict[Element, float]) -> Array:
-        """Return a array of energy offset."""
-
-        energy_offset: Array = jnp.empty_like(self.energy)
-        for element in self.elements:
+        energy_offset: Array = jnp.empty_like(self.energies)
+        for element in self.get_unique_elements():
             energy_offset = energy_offset.at[self.select(element)].set(
                 atom_energy[element]
             )
         return energy_offset
 
     def remove_energy_offset(self, atom_energy: Dict[Element, float]) -> None:
         """
-        Remove the input atom reference energies from the per-atom and total energy.
+        Remove the input reference energies to individual atoms and the total energy.
 
         :param atom_energy: atom reference energy
+        :type atom_energy: Dict[Element, float]]
         """
         energy_offset: Array = self._get_energy_offset(atom_energy)
-        self.energy -= energy_offset
+        self.energies -= energy_offset
         self.total_energy -= energy_offset.sum()
 
     def add_energy_offset(self, atom_energy: Dict[Element, float]) -> None:
         """
-        Add the input atom reference energies from the per-atom and total energy.
+        Add the input reference energies to individual atoms and the total energy.
 
         :param atom_energy: atom reference energy
+        :type atom_energy: Dict[Element, float]]
         """
         energy_offset = self._get_energy_offset(atom_energy)
-        self.energy += energy_offset
+        self.energies += energy_offset
         self.total_energy += energy_offset.sum()
 
-    def get_com_position(self) -> Array:
-        """Return center of mass position."""
-        return _get_center_of_mass(self.position, self.mass)
-
-    # --------------------------------------------------------------------------------------
-
-    def get_inputs(self) -> Dict[Element, Inputs]:
-        """A tuple of required info which are used for training and evaluating the potential."""
-
-        def extract_input() -> Generator[Tuple[Element, Inputs], None, None]:
-            for element in self.elements:
-                atom_index: Array = self.select(element)
+    def get_center_of_mass_position(self) -> Array:
+        """Get center of mass position."""
+        return _calculate_center_of_mass(self.positions, self.get_masses())
+
+    def get_per_element_inputs(self) -> Dict[Element, Inputs]:
+        """Get required info per element for training and evaluating a potential."""
+
+        def extract_inputs() -> Iterator[Tuple[Element, Inputs]]:
+            for element in self.get_unique_elements():
+                atom_indices: Array = self.select(element)
                 yield element, Inputs(
-                    self.position[atom_index],
-                    self.position,
-                    self.atom_type,
-                    self.box.lattice,  # type:ignore
+                    self.positions[atom_indices],
+                    self.positions,
+                    self.atom_types,
+                    self.lattice,
                     tree_util.tree_map(
-                        lambda x: jnp.asarray(x), self.element_map.element_to_atype
+                        lambda x: jnp.asarray(x),
+                        self.element_map.element_to_atom_type,
                     ),
                 )
 
-        return {element: input for element, input in extract_input()}
+        return {element: input for element, input in extract_inputs()}
 
-    def get_positions(self) -> Dict[Element, Array]:
+    def get_per_element_positions(self) -> Dict[Element, Array]:
         """Get position of atoms per element."""
 
-        def extract_position() -> Generator[Tuple[Element, Array], None, None]:
-            for element in self.elements:
-                atom_index: Array = self.select(element)
-                yield element, self.position[atom_index]
+        def extract_positions() -> Iterator[Tuple[Element, Array]]:
+            for element in self.get_unique_elements():
+                atom_indices = self.select(element)
+                yield element, self.positions[atom_indices]
 
-        return {element: position for element, position in extract_position()}
+        return {element: position for element, position in extract_positions()}
 
-    def get_forces(self) -> Dict[Element, Array]:
+    def get_per_element_forces(self) -> Dict[Element, Array]:
         """Get force components per element."""
 
-        def extract_force() -> Generator[Tuple[Element, Array], None, None]:
-            for element in self.elements:
-                atom_index: Array = self.select(element)
-                yield element, self.force[atom_index]
+        def extract_forces() -> Iterator[Tuple[Element, Array]]:
+            for element in self.get_unique_elements():
+                atom_indices = self.select(element)
+                yield element, self.forces[atom_indices]
+
+        return {element: force for element, force in extract_forces()}
 
-        return {element: force for element, force in extract_force()}
+
+class Inputs(NamedTuple):
+    """Represent array data of Structure for computing energy and forces."""
+
+    atom_positions: Array
+    positions: Array
+    atom_types: Array
+    lattice: Array
+    emap: Dict[Element, Array]
 
 
 register_jax_pytree_node(Structure)
```

### Comparing `jaxip-0.6.1/jaxip/config.py` & `jaxip-0.7.0/jaxip/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 
     def to_json(self, file: Path) -> None:
         """Dump configuration into a json file."""
         with open(str(Path(file)), "w") as fp:
             json.dump(self.dict(), fp, indent=4)
 
     @classmethod
-    def create_from_json(cls, file: Path) -> _CFG:
+    def from_json(cls, file: Path) -> _CFG:
         """Create a configuration instance from the input json file."""
         with open(str(Path(file)), "r") as fp:
             kwargs = json.load(fp)
         return cls(**kwargs)
```

### Comparing `jaxip-0.6.1/jaxip/datasets/runner.py` & `jaxip-0.7.0/jaxip/datasets/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,19 +86,19 @@
         data: DefaultDict = defaultdict(list)
         while True:
             line: str = file.readline()
             if not line:
                 break
             keyword, tokens = tokenize(line)
             if keyword == "atom":
-                data["position"].append([float(t) for t in tokens[:3]])
-                data["element"].append(tokens[3])
-                data["charge"].append(float(tokens[4]))
-                data["energy"].append(float(tokens[5]))
-                data["force"].append([float(t) for t in tokens[6:9]])
+                data["positions"].append([float(t) for t in tokens[:3]])
+                data["elements"].append(tokens[3])
+                data["charges"].append(float(tokens[4]))
+                data["energies"].append(float(tokens[5]))
+                data["forces"].append([float(t) for t in tokens[6:9]])
             elif keyword == "lattice":
                 data["lattice"].append([float(t) for t in tokens[:3]])
             elif keyword == "energy":
                 data["total_energy"].append(float(tokens[0]))
             elif keyword == "charge":
                 data["total_charge"].append(float(tokens[0]))
             elif keyword == "comment":
```

### Comparing `jaxip-0.6.1/jaxip/datasets/transformer.py` & `jaxip-0.7.0/jaxip/datasets/transformer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Any, Dict, Optional, Protocol
 
 from jaxip.atoms.structure import Structure
-from jaxip.types import Dtype
-from jaxip.types import dtype as _dtype
+from jaxip.types import Dtype, _dtype
 
 
 class TransformerInterface(Protocol):
     """
     A base transformer class which applies on the structure dataset.
     """
 
@@ -25,15 +24,11 @@
         r_cutoff: Optional[float] = None,
         dtype: Optional[Dtype] = None,
     ) -> None:
         self.r_cutoff: Optional[float] = r_cutoff
         self.dtype: Dtype = _dtype.FLOATX if dtype is None else dtype
 
     def __call__(self, data: Dict[str, Any]) -> Structure:
-        return Structure.create_from_dict(
-            data,
-            r_cutoff=self.r_cutoff,
-            dtype=self.dtype,
-        )
+        return Structure.from_dict(data, dtype=self.dtype)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}()"
```

### Comparing `jaxip-0.6.1/jaxip/descriptors/acsf/_acsf.py` & `jaxip-0.7.0/jaxip/descriptors/acsf/_acsf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from functools import partial
 from typing import Callable, Dict, Protocol, Tuple
 
 import jax
 import jax.numpy as jnp
 from jax import jit, lax, vmap
 
-from jaxip.atoms._neighbor import _calculate_cutoff_mask_per_atom
-from jaxip.atoms._structure import _calculate_distance_per_atom
+from jaxip.atoms._structure import _calculate_distances_per_atom
+from jaxip.atoms.neighbor import _calculate_masks_per_atom
 from jaxip.descriptors.acsf.angular import AngularSymmetryFunction
 from jaxip.descriptors.acsf.radial import RadialSymmetryFunction
 from jaxip.descriptors.acsf.symmetry import EnvironmentElements
 from jaxip.types import Array, Element
 
 
 @jit
@@ -18,18 +18,20 @@
     radial: Dict[EnvironmentElements, RadialSymmetryFunction],
     atype: Array,
     dist_i: Array,
     emap: Dict[Element, Array],
 ) -> Array:
     elements: EnvironmentElements = [k for k in radial.keys()][0]
 
-    mask_cutoff_i = _calculate_cutoff_mask_per_atom(
+    mask_cutoff_i = _calculate_masks_per_atom(
         dist_i, jnp.asarray(radial[elements].r_cutoff)
     )
-    mask_cutoff_and_atype_ij = mask_cutoff_i & (atype == emap[elements.neighbor_j])
+    mask_cutoff_and_atype_ij = mask_cutoff_i & (
+        atype == emap[elements.neighbor_j]
+    )
 
     return jnp.sum(
         radial[elements](dist_i),
         where=mask_cutoff_and_atype_ij,
         axis=0,
     )
 
@@ -42,15 +44,15 @@
     dist_i: Array,
     lattice: Array,
     emap: Dict[Element, Array],
 ) -> Array:
     elements: EnvironmentElements = [k for k in angular.keys()][0]
 
     # cutoff-radius mask
-    mask_cutoff_i = _calculate_cutoff_mask_per_atom(
+    mask_cutoff_i = _calculate_masks_per_atom(
         dist_i, jnp.asarray(angular[elements].r_cutoff)
     )
     # mask for neighboring element j
     at_j = emap[elements.neighbor_j]
     mask_cutoff_and_atype_ij = mask_cutoff_i & (atype == at_j)
     # mask for neighboring element k
     at_k = emap[elements.neighbor_k]  # type: ignore
@@ -108,15 +110,15 @@
         jnp.inner(Rij, diff_i) / true_op,
         1.0,
     )
     cost = jnp.where(is_zero, 0.0, cost)  # type: ignore
 
     rjk = jnp.where(  # diff_jk = diff_ji - diff_ik
         mask_ik,
-        _calculate_distance_per_atom(Rij, diff_i, lattice)[0],
+        _calculate_distances_per_atom(Rij, diff_i, lattice)[0],
         0.0,
     )  # second tuple output for Rjk
 
     value = jnp.where(
         mask_ij,
         jnp.sum(
             kernel(rij, dist_i, rjk, cost),
@@ -148,27 +150,30 @@
 ) -> Array:
     """
     Compute descriptor values per atom in the structure (via atom id).
     """
     dtype = single_atom_position.dtype
     result: Array = jnp.empty(acsf.num_symmetry_functions, dtype=dtype)
 
-    dist_i, diff_i = _calculate_distance_per_atom(
+    dist_i, diff_i = _calculate_distances_per_atom(
         single_atom_position, neighbor_positions, lattice
     )
 
     # Loop over the radial terms
     for index, (elements, radial) in enumerate(acsf.radial_symmetry_functions):
         result = result.at[index].set(
-            _calculate_radial_acsf_per_atom({elements: radial}, atype, dist_i, emap)
+            _calculate_radial_acsf_per_atom(
+                {elements: radial}, atype, dist_i, emap
+            )
         )
 
     # Loop over the angular terms
     for index, (elements, angular) in enumerate(
-        acsf.angular_symmetry_functions, start=acsf.num_radial_symmetry_functions
+        acsf.angular_symmetry_functions,
+        start=acsf.num_radial_symmetry_functions,
     ):
         result = result.at[index].set(
             _calculate_angular_acsf_per_atom(
                 {elements: angular}, atype, diff_i, dist_i, lattice, emap
             )
         )
```

### Comparing `jaxip-0.6.1/jaxip/descriptors/acsf/acsf.py` & `jaxip-0.7.0/jaxip/descriptors/acsf/acsf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import itertools
 from dataclasses import dataclass
 from typing import Optional, Tuple
 
 import jax.numpy as jnp
 
 from jaxip.atoms.structure import Structure
-from jaxip.descriptors.acsf._acsf import (_calculate_descriptor,
-                                          _calculate_grad_descriptor_per_atom)
+from jaxip.descriptors.acsf._acsf import (
+    _calculate_descriptor,
+    _calculate_grad_descriptor_per_atom,
+)
 from jaxip.descriptors.acsf.angular import AngularSymmetryFunction
 from jaxip.descriptors.acsf.radial import RadialSymmetryFunction
-from jaxip.descriptors.acsf.symmetry import (BaseSymmetryFunction,
-                                             EnvironmentElements)
+from jaxip.descriptors.acsf.symmetry import BaseSymmetryFunction, EnvironmentElements
 from jaxip.descriptors.descriptor import DescriptorInterface
 from jaxip.logger import logger
 from jaxip.pytree import BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.types import Array, Element
 
 
 @dataclass
@@ -100,57 +101,58 @@
                 f"Unknown input symmetry function type {symmetry_function}",
                 exception=TypeError,
             )
 
     def __call__(
         self,
         structure: Structure,
-        atom_index: Optional[Array] = None,
+        atom_indices: Optional[Array] = None,
     ) -> Array:
         """
         Calculate descriptor values for the input given structure and atom index.
 
         :param structure: input structure instance
         :type structure: Structure
-        :param atom_index: index for atom(s), defaults select all atom indices
+        :param atom_indices: atom indices, defaults select all atom indices
         of type the central element of the descriptor.
-        :type atom_index: Optional[Array], optional
+        :type atom_indices: Optional[Array], optional
         :return: descriptor values
         :rtype: Array
         """
 
         if self.num_symmetry_functions == 0:
             logger.warning(
                 f"No symmetry function defined yet:"
                 f" radial={self.num_radial_symmetry_functions}"
                 f", angular={self.num_angular_symmetry_functions}"
             )
 
-        if atom_index is None:
-            atom_index = structure.select(self.element)
+        if atom_indices is None:
+            atom_indices = structure.select(self.element)
         else:
-            atom_index = jnp.atleast_1d(atom_index)  # type: ignore
+            atom_indices = jnp.atleast_1d(atom_indices)  # type: ignore
             # Check aid atom type match the central element
             if not jnp.all(
-                structure.element_map.element_to_atype[self.element]
-                == structure.atom_type[atom_index]
+                structure.element_map.element_to_atom_type[self.element]
+                == structure.atom_types[atom_indices]
             ):
                 logger.error(
-                    f"Inconsistent central element '{self.element}': input aid={atom_index}"
-                    f" (atype='{int(structure.atom_type[atom_index])}')",
+                    f"Inconsistent central element '{self.element}': "
+                    f" input atom indices={atom_indices}"
+                    f" (atom_types='{int(structure.atom_types[atom_indices])}')",
                     exception=ValueError,
                 )
 
         return _calculate_descriptor(
             self,
-            structure.position[atom_index],
-            structure.position,
-            structure.atom_type,
-            structure.box.lattice,
-            structure.element_map.element_to_atype,
+            structure.positions[atom_indices],
+            structure.positions,
+            structure.atom_types,
+            structure.lattice,
+            structure.element_map.element_to_atom_type,
         )
 
     def grad(
         self,
         structure: Structure,
         atom_index: int,
     ) -> Array:
@@ -166,21 +168,21 @@
                 f"Unexpected {atom_index=}."
                 f" The index must be between [0, {structure.natoms})",
                 ValueError,
             )
 
         return _calculate_grad_descriptor_per_atom(
             self,
-            structure.position[
+            structure.positions[
                 atom_index
             ],  # must be a single atom position shape=(1, 3)
-            structure.position,
-            structure.atom_type,
-            structure.box.lattice,
-            structure.element_map.element_to_atype,
+            structure.positions,
+            structure.atom_types,
+            structure.lattice,
+            structure.element_map.element_to_atom_type,
         )
 
     @property
     def num_radial_symmetry_functions(self) -> int:
         """Return number of `two-body` (radial) symmetry functions."""
         return len(self.radial_symmetry_functions)
 
@@ -201,15 +203,18 @@
     @property
     def r_cutoff(self) -> float:  # type: ignore
         """Return the maximum cutoff radius for list of the symmetry functions."""
         return max(
             [
                 cfn.r_cutoff
                 for (_, cfn) in itertools.chain(
-                    *[self.radial_symmetry_functions, self.angular_symmetry_functions]
+                    *[
+                        self.radial_symmetry_functions,
+                        self.angular_symmetry_functions,
+                    ]
                 )
             ]
         )
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(element='{self.element}'"
```

### Comparing `jaxip-0.6.1/jaxip/descriptors/acsf/angular.py` & `jaxip-0.7.0/jaxip/descriptors/acsf/angular.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/descriptors/acsf/cutoff.py` & `jaxip-0.7.0/jaxip/descriptors/acsf/cutoff.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/descriptors/acsf/radial.py` & `jaxip-0.7.0/jaxip/descriptors/acsf/radial.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/descriptors/acsf/symmetry.py` & `jaxip-0.7.0/jaxip/descriptors/acsf/symmetry.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/descriptors/descriptor.py` & `jaxip-0.7.0/jaxip/descriptors/descriptor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/descriptors/scaler.py` & `jaxip-0.7.0/jaxip/descriptors/scaler.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 from jaxip.logger import logger
 from jaxip.types import Array, Dtype
-from jaxip.types import dtype as _dtype
+from jaxip.types import _dtype
 
 
 class Scaler:
     """
     Scale descriptor values.
 
     Scaling parameters are calculated by fitting over the samples in the dataset.
```

### Comparing `jaxip-0.6.1/jaxip/logger.py` & `jaxip-0.7.0/jaxip/logger.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/models/nn/activation.py` & `jaxip-0.7.0/jaxip/models/nn/activation.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/models/nn/initializer.py` & `jaxip-0.7.0/jaxip/models/nn/initializer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/models/nn/network.py` & `jaxip-0.7.0/jaxip/models/nn/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from flax import linen as nn
 from frozendict import frozendict
 
 from jaxip.logger import logger
 from jaxip.models.model import ModelInterface
 from jaxip.models.nn.activation import _activation_function_map
 from jaxip.types import Array, Dtype
-from jaxip.types import dtype as _dtype
+from jaxip.types import _dtype
 
 
 class NeuralNetworkModel(nn.Module, ModelInterface):
     """Neural network model that outputs energy."""
 
     hidden_layers: Tuple[Tuple[int, str], ...]
     output_layer: Tuple[int, str] = (1, "identity")
```

### Comparing `jaxip-0.6.1/jaxip/potentials/_energy.py` & `jaxip-0.7.0/jaxip/potentials/_energy.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     params: frozendict,
     inputs: Inputs,
 ) -> Array:
     """Compute model output per-atom energy."""
     x = _calculate_descriptor(
         atomic_potential.descriptor,
         positions,
-        inputs.position,
-        inputs.atype,
+        inputs.positions,
+        inputs.atom_types,
         inputs.lattice,
         inputs.emap,
     )
     x = atomic_potential.scaler(x)
     atomic_energy = atomic_potential.model.apply({"params": params}, x)
     return atomic_energy  # type: ignore
```

### Comparing `jaxip-0.6.1/jaxip/potentials/_force.py` & `jaxip-0.7.0/jaxip/potentials/_force.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/potentials/atomic_potential.py` & `jaxip-0.7.0/jaxip/potentials/atomic_potential.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,17 @@
         :return: model energy output
         """
         element: Element = self.descriptor.element  # type: ignore
         aid: Array = structure.select(element)
 
         return _compute_atomic_energy(
             self,
-            structure.position[aid],
+            structure.positions[aid],
             params,
-            structure.get_inputs()[element],
+            structure.get_per_element_inputs()[element],
         )
 
     @property
     def model_input_size(self) -> int:
         """Return size of the model input."""
         return self.descriptor.num_descriptors
```

### Comparing `jaxip-0.6.1/jaxip/potentials/nnp/gradient_descent.py` & `jaxip-0.7.0/jaxip/potentials/nnp/gradient_descent.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 
 from jaxip.atoms.structure import Structure
 from jaxip.datasets.dataset import DatasetInterface
 from jaxip.logger import logger
 from jaxip.potentials._energy import _energy_fn
 from jaxip.potentials._force import _compute_force
 from jaxip.potentials.nnp.metrics import ErrorMetric
-from jaxip.potentials.nnp.nnp import \
-    NeuralNetworkPotentialInterface as PotentialInterface
-from jaxip.potentials.nnp.settings import \
-    NeuralNetworkPotentialSettings as PotentialSettings
+from jaxip.potentials.nnp.nnp import (
+    NeuralNetworkPotentialInterface as PotentialInterface,
+)
+from jaxip.potentials.nnp.settings import (
+    NeuralNetworkPotentialSettings as PotentialSettings,
+)
 from jaxip.types import Array, Element
 
 
 def _mse_loss(*, logits: Array, targets: Array) -> Array:
     return ((targets - logits) ** 2).mean()
 
 
@@ -114,17 +116,19 @@
             loss_energy_per_epoch: Array = jnp.array(0.0)
             loss_force_per_epoch: Array = jnp.array(0.0)
             num_updates_per_epoch: int = 0
 
             # Loop over batches
             for _ in tqdm(range(steps)):
                 structures: List[Structure] = random.choices(dataset, k=batch_size)
-                xbatch = tuple(structure.get_inputs() for structure in structures)
+                xbatch = tuple(
+                    structure.get_per_element_inputs() for structure in structures
+                )
                 ybatch = tuple(
-                    (structure.total_energy, structure.get_forces())
+                    (structure.total_energy, structure.get_per_element_forces())
                     for structure in structures
                 )
 
                 batch = xbatch, ybatch
                 states, metrics = self.train_step(states, batch)
 
                 loss_per_epoch += metrics["loss"]
```

### Comparing `jaxip-0.6.1/jaxip/potentials/nnp/kalman_filter.py` & `jaxip-0.7.0/jaxip/potentials/nnp/kalman_filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from jaxip.potentials._force import _compute_force
 from jaxip.potentials.atomic_potential import AtomicPotential
 from jaxip.potentials.nnp.nnp import \
     NeuralNetworkPotentialInterface as PotentialInterface
 from jaxip.potentials.nnp.settings import \
     NeuralNetworkPotentialSettings as PotentialSettings
 from jaxip.types import Array, Element
-from jaxip.types import dtype as default_dtype
+from jaxip.types import _dtype
 
 
 def _tree_flatten(pytree: Dict) -> Array:
     return flatten_util.ravel_pytree(pytree)[0].reshape(-1, 1)  # type: ignore
 
 
 class KalmanFilterUpdater:
@@ -68,15 +68,15 @@
         # Initialize state vector
         W, tree_unflatten = flatten_util.ravel_pytree(model_params)  # type: ignore
         self.W: Array = W.reshape(-1, 1)
         self._unflatten_state_vector: Callable = tree_unflatten
         self.num_states: int = self.W.shape[0]
         # Error covariance matrix
         self.P: Array = (1.0 / self.epsilon) * jnp.identity(
-            self.num_states, dtype=default_dtype.FLOATX
+            self.num_states, dtype=_dtype.FLOATX
         )
 
     def fit(
         self,
         dataset: DatasetInterface,
     ) -> defaultdict:
         """
@@ -97,29 +97,29 @@
 
         def compute_energy_error(
             model_params: Dict[Element, frozendict], structure: Structure
         ) -> Array:
             E_ref: Array = structure.total_energy
             E_pot: Array = _compute_energy(
                 frozendict(atomic_potential),
-                structure.get_positions(),
+                structure.get_per_element_positions(),
                 model_params,
-                structure.get_inputs(),
+                structure.get_per_element_inputs(),
             )
             return (E_ref - E_pot)[0] / structure.natoms
 
         def compute_force_error(state_vector: Array, structure: Structure) -> Array:
             model_params: Dict = self._unflatten_state_vector(state_vector)
-            F_ref: Array = _tree_flatten(structure.get_forces())
+            F_ref: Array = _tree_flatten(structure.get_per_element_forces())
             F_pot: Array = _tree_flatten(
                 _compute_force(
                     frozendict(atomic_potential),
-                    structure.get_positions(),
+                    structure.get_per_element_positions(),
                     model_params,
-                    structure.get_inputs(),
+                    structure.get_per_element_inputs(),
                 )
             )
             return (F_ref - F_pot)[..., 0]
 
         grad_energy_error: Callable = jax.grad(compute_energy_error)
         jacob_force_error: Callable = jax.jacrev(compute_force_error)
 
@@ -181,34 +181,34 @@
                 # Update learning rate
                 if (self.kalman_type == 0) and (self.eta < self.eta_max):
                     self.eta *= np.exp(self.eta_tau)
 
                 # Measurement noise
                 if self.kalman_type == 0:
                     A += (1.0 / self.eta) * jnp.identity(
-                        num_observations, dtype=default_dtype.FLOATX
+                        num_observations, dtype=_dtype.FLOATX
                     )
                 elif self.kalman_type == 1:
                     A += self.lambda0 * jnp.identity(
-                        num_observations, dtype=default_dtype.FLOATX
+                        num_observations, dtype=_dtype.FLOATX
                     )
 
                 # Kalman gain matrix
                 K = X @ jnp.linalg.inv(A)
 
                 # Update error covariance matrix
                 self.P -= K @ X.transpose()
 
                 # Forgetting factor
                 if self.kalman_type == 1:
                     self.P *= 1.0 / self.lambda0
 
                 # Process noise.
                 self.P += self.q * jnp.identity(
-                    self.num_states, dtype=default_dtype.FLOATX
+                    self.num_states, dtype=_dtype.FLOATX
                 )
 
                 # Update state vector
                 self.W += K @ Xi
 
                 # Anneal process noise
                 if self.q > self.q_min:
```

### Comparing `jaxip-0.6.1/jaxip/potentials/nnp/metrics.py` & `jaxip-0.7.0/jaxip/potentials/nnp/metrics.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/potentials/nnp/nnp.py` & `jaxip-0.7.0/jaxip/potentials/nnp/nnp.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/potentials/nnp/potential.py` & `jaxip-0.7.0/jaxip/potentials/nnp/potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 from jaxip.models.nn.initializer import UniformInitializer
 from jaxip.models.nn.network import NeuralNetworkModel
 from jaxip.potentials._energy import _compute_energy
 from jaxip.potentials._force import _compute_force
 from jaxip.potentials.atomic_potential import AtomicPotential
 from jaxip.potentials.nnp.gradient_descent import GradientDescentUpdater
 from jaxip.potentials.nnp.kalman_filter import KalmanFilterUpdater
-from jaxip.potentials.nnp.settings import \
-    NeuralNetworkPotentialSettings as PotentialSettings
+from jaxip.potentials.nnp.settings import (
+    NeuralNetworkPotentialSettings as PotentialSettings,
+)
 from jaxip.types import Array, Element
 
 
 class UpdaterInterface(Protocol):
     """Interface for potential weight updaters."""
 
     def fit(self, dataset: DatasetInterface) -> Dict:
@@ -54,18 +55,18 @@
     .. code-block:: python
         :linenos:
 
         from jaxip.potentials import NeuralNetworkPotential
         from jaxip.potentials.nnp import NeuralNetworkPotentialSettings as Settings
 
         # Method #1 (potential file)
-        nnp1 = NeuralNetworkPotential.create_from_file("input.nn")
+        nnp1 = NeuralNetworkPotential.from_file("input.nn")
 
         # Method #2 (json file)
-        nnp3 = NeuralNetworkPotential.create_from_file('h2o.json')
+        nnp3 = NeuralNetworkPotential.from_file('h2o.json')
 
         # Method #3 (dictionary of parameters)
         settings = Settings(**params_dict)
         nnp3 = NeuralNetworkPotential(settings)
     """
 
     settings: PotentialSettings = field(repr=False)
@@ -75,27 +76,27 @@
     )
     model_params: Dict[Element, frozendict] = field(
         default_factory=dict, repr=False, init=False
     )
     updater: Optional[UpdaterInterface] = field(default=None, repr=False, init=False)
 
     @classmethod
-    def create_from_file(cls, filename: Path) -> NeuralNetworkPotential:
+    def from_file(cls, filename: Path) -> NeuralNetworkPotential:
         """Create an instance of the potential from input file (RuNNer format)."""
         logger.info("Creating potential from input file (RuNNer format)")
         potfile = Path(filename)
         suffix: str = potfile.suffix.lower()
         if ".json" == suffix:
             logger.info(f"Initializing from json file: {potfile.name}")
-            settings = PotentialSettings.create_from_json(potfile)
+            settings = PotentialSettings.from_json(potfile)
         else:
             logger.info(
                 f"Initializing from original RuNNer file format: {potfile.name}"
             )
-            settings = PotentialSettings.create_from_file(potfile)
+            settings = PotentialSettings.from_file(potfile)
 
         return NeuralNetworkPotential(
             settings=settings,  # type: ignore
             output_dir=potfile.parent,
         )
 
     def __post_init__(self) -> None:
@@ -295,34 +296,34 @@
 
         :param structure: Structure
         :return: total energy
         """
 
         return _compute_energy(
             frozendict(self.atomic_potential),  # must be hashable
-            structure.get_positions(),
+            structure.get_per_element_positions(),
             self.model_params,
-            structure.get_inputs(),
+            structure.get_per_element_inputs(),
         )
 
-    def compute_force(self, structure: Structure) -> Array:
+    def compute_forces(self, structure: Structure) -> Array:
         """
         Compute force components.
 
         :param structure: input structure
         :return: predicted force components for all atoms
         """
         force_dict: Dict[Element, Array] = _compute_force(
             frozendict(self.atomic_potential),  # must be hashable
-            structure.get_positions(),
+            structure.get_per_element_positions(),
             self.model_params,
-            structure.get_inputs(),
+            structure.get_per_element_inputs(),
         )
-        force: Array = jnp.empty_like(structure.force)
-        for element in structure.elements:
+        force: Array = jnp.empty_like(structure.forces)
+        for element in structure.get_unique_elements():
             atom_index: Array = structure.select(element)
             force = force.at[atom_index].set(force_dict[element])
 
         return force
 
     # ------------------------------------------------------------------------
 
@@ -332,15 +333,15 @@
         No gradient history is required here.
         """
         print("Fitting descriptor scaler...")
         try:
             dataset_size: int = len(dataset)
             for index in tqdm(range(dataset_size)):
                 structure: Structure = dataset[index]
-                elements: Tuple[Element, ...] = structure.elements
+                elements: Tuple[Element, ...] = structure.get_unique_elements()
                 for element in elements:
                     x: Array = self.atomic_potential[element].descriptor(structure)
                     self.atomic_potential[element].scaler.fit(x)
         except KeyboardInterrupt:
             print("Keyboard Interrupt")
         else:
             print("Done.")
```

### Comparing `jaxip-0.6.1/jaxip/potentials/nnp/settings.py` & `jaxip-0.7.0/jaxip/potentials/nnp/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     cutoff_type: str = "tanh"
     scale_type: str = "center"
     scale_min_short: float = 0.0
     scale_max_short: float = 1.0
     symfunction_short: List[SymFuncArgs] = Field(default_factory=list)
 
     @classmethod
-    def create_from_file(cls, filename: Path) -> NeuralNetworkPotentialSettings:
+    def from_file(cls, filename: Path) -> NeuralNetworkPotentialSettings:
         """
         Read all potential settings from the input file.
 
         Parameters such as `elements`, `cutoff type`, `symmetry functions`, `neural network`, `training parameters`, etc
         (see `here <https://compphysvienna.github.io/n2p2/topics/keywords.html>`_).
         """
```

### Comparing `jaxip-0.6.1/jaxip/pytree.py` & `jaxip-0.7.0/jaxip/pytree.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,37 +28,41 @@
     """
 
     def _tree_flatten(self) -> Tuple[Tuple[Any, ...], Dict[str, Any]]:
         children: Tuple[Any, ...] = tuple(
             getattr(self, attr) for attr in self._get_jit_dynamic_attributes()
         )
         aux_data: Dict[str, Any] = {
-            attr: getattr(self, attr) for attr in self._get_jit_static_attributes()
+            attr: getattr(self, attr)
+            for attr in self._get_jit_static_attributes()
         }
         return (children, aux_data)
 
     @classmethod
     def _tree_unflatten(
         cls, aux_data: Dict[str, Any], children: Tuple[Any, ...]
     ) -> BaseJaxPytreeDataClass:
         return cls(*children, **aux_data)  # type: ignore
 
     def __hash__(self) -> int:
         """
-        Define hash method based on the `JAX JIT compilation` static attributes.
-        This is useful when wants to identify changes on the static arguments of a jit-compiled method.
+        Define hash based on the `JAX JIT compilation` static attributes.
+        This is used for detecting changes on the static arguments
+        of the jit-compiled method.
         """
         aux_data: Dict[str, Any] = self._tree_flatten()[1]
         return hash(tuple(frozenset(sorted(aux_data.items()))))
 
     @classmethod
     def _get_jit_dynamic_attributes(cls) -> Tuple[str, ...]:
         """Get JAX JIT compilation dynamic attribute names (i.e. jax.ndarray)."""
         return tuple(
-            attr for attr, dtype in cls.__annotations__.items() if "Array" in str(dtype)
+            attr
+            for attr, dtype in cls.__annotations__.items()
+            if "Array" in str(dtype)
         )
 
     @classmethod
     def _get_jit_static_attributes(cls) -> Tuple[str, ...]:
         """Get JAX JIT compilation static attribute names."""
         dynamic_attributes = cls._get_jit_dynamic_attributes()
         return tuple(
@@ -78,15 +82,17 @@
         if sorted(available) != sorted(expected):  # type: ignore
             logger.error(
                 f"Expecting JIT {tag} attributes: {expected} but got {available}",
                 exception=AssertionError,
             )
 
     @classmethod
-    def _assert_jit_static_attributes(cls, expected: Tuple[str, ...] = tuple()) -> None:
+    def _assert_jit_static_attributes(
+        cls, expected: Tuple[str, ...] = tuple()
+    ) -> None:
         cls._assert_jit_attributes(
             cls._get_jit_static_attributes(), expected, tag="static"
         )
 
     @classmethod
     def _assert_jit_dynamic_attributes(
         cls, expected: Tuple[str, ...] = tuple()
```

### Comparing `jaxip-0.6.1/jaxip/simulation/mc.py` & `jaxip-0.7.0/jaxip/simulation/mc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 from dataclasses import replace
 from typing import Optional, Protocol, Tuple
 
 import jax.numpy as jnp
 import numpy as np
 
-from jaxip.atoms import Structure
+from jaxip.atoms.structure import Structure
 from jaxip.logger import logger
 from jaxip.types import Array, Element
 from jaxip.units import units
 
-KB = units.BOLTZMANN_CONSTANT
+KB: float = units.BOLTZMANN_CONSTANT
 
 
 class PotentialInterface(Protocol):
     def __call__(self, structure: Structure) -> Array:
         ...
 
-    def compute_force(self, structure: Structure) -> Array:
+    def compute_forces(self, structure: Structure) -> Array:
         ...
 
 
 class MCSimulator:
     def __init__(
         self,
         potential: PotentialInterface,
         initial_structure: Structure,
         temperature: float,
         translate_step: float,
         movements_per_step: int = 1,
-        atomic_mass: Optional[Array] = None,
+        atomic_masses: Optional[Array] = None,
         random_seed: int = 12345,
     ) -> None:
         """
         A Monte Carlo simulator to predict configuration space of particles.
 
         :param potential: input potential function
         :type potential: PotentialInterface
         :param initial_structure: initial structure of atoms
         :type initial_structure: Structure
         :param translate_step: maximum translate step in Bohr unit
         :type time_step: float
         :param temperature: desired temperature of the system
         :type temperature: float
-        :param atomic_mass: atomic mass of atoms in the input structure, defaults to None
-        :type atomic_mass: Optional[Array], optional
+        :param atomic_masses: atomic mass of atoms in the input structure, defaults to None
+        :type atomic_masses: Optional[Array], optional
         :param random_seed: seed for generating random atom movements, defaults to 12345
         :type random_seed: int, optional
 
         This simulator is intended to be used for small systems of atoms during
         the potential training in order to generate new dataset.
         """
 
         logger.debug(f"Initializing {self.__class__.__name__}")
         self.potential = potential
         self.temperature = temperature
         self.translate_step = translate_step
         self.movements_per_step = movements_per_step
 
-        self.mass: Array
-        if atomic_mass is not None:
-            self.mass = atomic_mass.reshape(-1, 1)
+        self.masses: Array
+        if atomic_masses is not None:
+            self.masses = atomic_masses.reshape(-1, 1)
         else:
             logger.info("Extracting atomc masses from input structure")
-            self.mass = initial_structure.mass.reshape(-1, 1)
+            self.masses = initial_structure.get_masses().reshape(-1, 1)
 
         self.step: int = 0
         self.energy = self.potential(initial_structure)
         self._structure = replace(initial_structure)
         np.random.seed(random_seed)
 
     def update(self) -> None:
@@ -80,16 +80,16 @@
             low=-self.translate_step,
             high=self.translate_step,
             size=(self.movements_per_step, 3),
         )
         atom_indices = np.random.randint(
             low=0, high=self.natoms, size=(self.movements_per_step,)
         )
-        new_position = self._structure.position.at[atom_indices].add(displacements)
-        new_structure = replace(self._structure, position=new_position)
+        new_position = self._structure.positions.at[atom_indices].add(displacements)
+        new_structure = replace(self._structure, positions=new_position)
         new_energy = self.potential(new_structure)
 
         accept: bool = False
         if new_energy <= self.energy:
             accept = True
         else:
             prob = jnp.exp(-(new_energy - self.energy) / (KB * self.temperature))
@@ -104,24 +104,23 @@
         return (
             f"{self.step:<10} "
             f"Temp[K]:{self.temperature:<15.10f} "
             f"Epot[Ha]:{self.get_potential_energy():<15.10f} "
         )
 
     @property
-    def position(self) -> Array:
-        return self._structure.position
+    def positions(self) -> Array:
+        return self._structure.positions
 
     @property
     def natoms(self) -> int:
         return self._structure.natoms
 
-    @property
-    def elements(self) -> Tuple[Element]:
-        return self._structure.elements
+    def get_elements(self) -> Tuple[Element]:
+        return self._structure.get_elements()
 
     def get_structure(self) -> Structure:
         return replace(
             self._structure,
             total_energy=self.potential(self._structure),
         )
```

### Comparing `jaxip-0.6.1/jaxip/simulation/md.py` & `jaxip-0.7.0/jaxip/simulation/md.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,181 +1,181 @@
 from dataclasses import replace
 from typing import Optional, Protocol, Tuple
 
 import jax
 import jax.numpy as jnp
 
 from jaxip.atoms import Structure
-from jaxip.atoms._structure import _get_center_of_mass
+from jaxip.atoms._structure import _calculate_center_of_mass
 from jaxip.logger import logger
 from jaxip.simulation.thermostat import BrendsenThermostat
 from jaxip.types import Array, Element
 from jaxip.units import units
 
-KB = units.BOLTZMANN_CONSTANT
+KB: float = units.BOLTZMANN_CONSTANT
 
 
 class PotentialInterface(Protocol):
     def __call__(self, structure: Structure) -> Array:
         ...
 
-    def compute_force(self, structure: Structure) -> Array:
+    def compute_forces(self, structure: Structure) -> Array:
         ...
 
 
 @jax.jit
-def _get_kinetic_energy(velocity: Array, mass: Array) -> Array:
-    return 0.5 * jnp.sum(mass * velocity * velocity)
+def _get_kinetic_energy(velocities: Array, masses: Array) -> Array:
+    return 0.5 * jnp.sum(masses * velocities * velocities)
 
 
 @jax.jit
-def _get_temperature(velocity: Array, mass: Array) -> Array:
-    kinetic_energy = _get_kinetic_energy(velocity, mass)
-    natoms = velocity.shape[0]
+def _get_temperature(velocities: Array, masses: Array) -> Array:
+    kinetic_energy = _get_kinetic_energy(velocities, masses)
+    natoms = velocities.shape[0]
     return 2 * kinetic_energy / (3 * natoms * KB)
 
 
 @jax.jit
 def _get_virial_term(
-    velocity: Array,
-    mass: Array,
-    position: Array,
-    force: Array,
+    velocities: Array,
+    masses: Array,
+    positions: Array,
+    forces: Array,
 ) -> Array:
-    return 2 * _get_kinetic_energy(velocity, mass) + (position * force).sum()
+    return 2 * _get_kinetic_energy(velocities, masses) + (positions * forces).sum()
 
 
 def _get_potential_energy(
     potential: PotentialInterface,
     structure: Structure,
 ) -> Array:
     return potential(structure)
 
 
-def _compute_force(
+def _compute_forces(
     potential: PotentialInterface,
     structure: Structure,
 ) -> Array:
-    return potential.compute_force(structure)
+    return potential.compute_forces(structure)
 
 
 class MDSimulator:
     def __init__(
         self,
         potential: PotentialInterface,
         initial_structure: Structure,
         time_step: float,
-        initial_velocity: Optional[Array] = None,
+        initial_velocities: Optional[Array] = None,
         temperature: Optional[float] = None,
         thermostat: Optional[BrendsenThermostat] = None,
-        atomic_mass: Optional[Array] = None,
+        atomic_masses: Optional[Array] = None,
         random_seed: int = 12345,
     ) -> None:
         """
         A molecular dynamics simulator to predict trajectory of particles over time.
 
         :param potential: input potential function
         :type potential: PotentialInterface
         :param initial_structure: initial structure of atoms
         :type initial_structure: Structure
         :param time_step: time step in Hartree time unit
         :type time_step: float
-        :param initial_velocity: Initial velocity of atom,
+        :param initial_velocities: Initial atom velocities,
             otherwise it can be randomly generated from the input temperature, defaults to None
-        :type initial_velocity: Optional[Array], optional
-        :param temperature: input temperature which can be used for generating random velocity
+        :type initial_velocities: Optional[Array], optional
+        :param temperature: input temperature which can be used for generating random velocities
             or setting target temperature for internally initialized thermostat if needed, defaults to None
         :type temperature: Optional[float], optional
         :param thermostat: input thermostat that controls the temperature of the system
             to the desired value, defaults to None
         :type thermostat: Optional[BrendsenThermostat], optional
-        :param atomic_mass: atomic mass of atoms in the input structure, defaults to None
-        :type atomic_mass: Optional[Array], optional
+        :param atomic_masses: atomic mass of atoms in the input structure, defaults to None
+        :type atomic_masses: Optional[Array], optional
         :param random_seed: seed for generating random velocities, defaults to 12345
         :type random_seed: int, optional
 
         This simulator is intended to be used for small systems of atoms during
         the potential training in order to generate new dataset.
         """
 
         logger.debug(f"Initializing {self.__class__.__name__}")
         self.potential = potential
         self.time_step = time_step
         self.thermostat = thermostat
 
-        self.mass: Array
-        if atomic_mass is not None:
-            self.mass = atomic_mass.reshape(-1, 1)
+        self.masses: Array
+        if atomic_masses is not None:
+            self.masses = atomic_masses.reshape(-1, 1)
         else:
             logger.info("Extracting atomc masses from input structure")
-            self.mass = initial_structure.mass.reshape(-1, 1)
+            self.masses = initial_structure.get_masses().reshape(-1, 1)
 
-        self.velocity: Array
-        if initial_velocity is not None:
-            self.velocity = initial_velocity
+        self.velocities: Array
+        if initial_velocities is not None:
+            self.velocities = initial_velocities
         else:
             assert (
                 temperature is not None
-            ), "At least one of initial temperature or initial velocity must be given"
+            ), "At least one of input initial temperature or initial velocities must be given"
             logger.info(f"Generating random velocities ({temperature:0.2f} K)")
-            self.velocity = self.generate_random_velocity(
-                temperature, mass=self.mass, seed=random_seed
+            self.velocities = self.generate_random_velocities(
+                temperature, masses=self.masses, seed=random_seed
             )
 
         if (self.thermostat is None) and (temperature is not None):
             logger.info(f"Initializing thermostat ({temperature:0.2f} K)")
-            logger.info("Setting default thermostat constant to 100x timestep")
+            logger.info("Setting default thermostat constant to 100x time step")
             self.thermostat = BrendsenThermostat(
                 target_temperature=temperature,
                 time_constant=100 * self.time_step,
             )
 
         self.step: int = 0
         self.elapsed_time: float = 0.0
-        self.force = _compute_force(self.potential, initial_structure)
-        self.temperature = _get_temperature(self.velocity, self.mass)
+        self.forces = _compute_forces(self.potential, initial_structure)
+        self.temperature = _get_temperature(self.velocities, self.masses)
         self._structure = replace(initial_structure)
 
     def update(self) -> None:
         """Update parameters for next time step."""
         self.verlet_integration()
         self.step += 1
         self.elapsed_time += self.time_step
-        self.temperature = _get_temperature(self.velocity, self.mass)
+        self.temperature = _get_temperature(self.velocities, self.masses)
         if self.thermostat is not None:
-            self.velocity = self.thermostat.get_rescaled_velocity(self)
-            self.temperature = _get_temperature(self.velocity, self.mass)
+            self.velocities = self.thermostat.get_rescaled_velocities(self)
+            self.temperature = _get_temperature(self.velocities, self.masses)
 
     def verlet_integration(self) -> None:
         """Update atom positions and velocities based on Verlet algorithm."""
-        new_position = (
-            self.position
-            + self.velocity * self.time_step
-            + 0.5 * self.force * self.time_step * self.time_step
+        new_positions = (
+            self.positions
+            + self.velocities * self.time_step
+            + 0.5 * self.forces * self.time_step * self.time_step
         )
-        new_force = _compute_force(self.potential, self._structure)
-        self.velocity += 0.5 * (self.force + new_force) * self.time_step
-        self.force = new_force
-        self._structure = replace(self._structure, position=new_position)
+        new_forces = _compute_forces(self.potential, self._structure)
+        self.velocities += 0.5 * (self.forces + new_forces) * self.time_step
+        self.forces = new_forces
+        self._structure = replace(self._structure, positions=new_positions)
 
     @classmethod
-    def generate_random_velocity(
+    def generate_random_velocities(
         cls,
         temperature: float,
-        mass: Array,
+        masses: Array,
         seed: int,
     ) -> Array:
         """Generate Maxwell-Boltzmann distributed random velocities."""
         key = jax.random.PRNGKey(seed)
-        mass = mass.reshape(-1, 1)
-        natoms = mass.shape[0]
-        velocity = jax.random.normal(key, shape=(natoms, 3))
-        velocity *= jnp.sqrt(temperature / _get_temperature(velocity, mass))
-        velocity -= _get_center_of_mass(velocity, mass)
-        return velocity
+        masses = masses.reshape(-1, 1)
+        natoms = masses.shape[0]
+        velocities = jax.random.normal(key, shape=(natoms, 3))
+        velocities *= jnp.sqrt(temperature / _get_temperature(velocities, masses))
+        velocities -= _calculate_center_of_mass(velocities, masses)
+        return velocities
 
     def repr_physical_params(self) -> str:
         """Represent current physical parameters."""
         return (
             f"{self.step:<10} "
             f"time[ps]:{units.TO_PICO_SECOND * self.elapsed_time:<10.5f} "
             f"Temp[K]:{self.temperature:<10.5f} "
@@ -183,54 +183,51 @@
             f"Epot[Ha]:{self.get_potential_energy():<15.10f} "
             f"Pres[kb]:{self.get_pressure() * units.TO_KILO_BAR:<10.5f}"
             if self._structure.box
             else ""
         )
 
     @property
-    def position(self) -> Array:
-        return self._structure.position
+    def positions(self) -> Array:
+        return self._structure.positions
 
     @property
     def natoms(self) -> int:
         return self._structure.natoms
 
-    @property
-    def elements(self) -> Tuple[Element]:
-        return self._structure.elements
+    def get_elements(self) -> Tuple[Element]:
+        return self._structure.get_elements()
 
     def get_structure(self) -> Structure:
         return replace(
             self._structure,
-            force=self.force,
+            forces=self.forces,
             total_energy=self.potential(self._structure),
         )
 
     def get_pressure(self) -> Array:
         assert (
             self._structure.box
         ), "Calulating pressure... input structure must have PBC box"
         volume = self._structure.box.volume
         virial = _get_virial_term(
-            self.velocity,
-            self.mass,
-            self.position,
-            self.force,
+            self.velocities,
+            self.masses,
+            self.positions,
+            self.forces,
         )
         return virial / (3.0 * volume)  # type: ignore
 
-    def get_com_velocity(self) -> Array:
-        """Return center of mass velocity."""
-        return _get_center_of_mass(self.velocity, self.mass)
-
-    def get_com_position(self) -> Array:
-        """Return center of mass position."""
-        return _get_center_of_mass(self.position, self.mass)
+    def get_center_of_mass_velocity(self) -> Array:
+        return _calculate_center_of_mass(self.velocities, self.masses)
+
+    def get_center_of_mass_position(self) -> Array:
+        return _calculate_center_of_mass(self.positions, self.masses)
 
     def get_potential_energy(self) -> Array:
         return _get_potential_energy(self.potential, self._structure)
 
     def get_kinetic_energy(self) -> Array:
-        return _get_kinetic_energy(self.velocity, self.mass)
+        return _get_kinetic_energy(self.velocities, self.masses)
 
     def get_total_energy(self) -> Array:
         return self.get_potential_energy() + self.get_kinetic_energy()
```

### Comparing `jaxip-0.6.1/jaxip/simulation/thermostat.py` & `jaxip-0.7.0/jaxip/simulation/thermostat.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 
 from jaxip.types import Array
 
 
 class MDSimulatorInterface(Protocol):
     temperature: float
     time_step: float
-    velocity: Array
+    velocities: Array
 
 
 class BrendsenThermostat:
     """Control simulation temperature using Brendsen algorithm."""
 
     def __init__(
         self,
         target_temperature: float,
         time_constant: float,
     ) -> None:
         self.target_temperature = target_temperature
         self.time_constant = time_constant
 
-    def get_rescaled_velocity(
+    def get_rescaled_velocities(
         self,
         simulator: MDSimulatorInterface,
     ) -> Array:
         scaling_factor = jnp.sqrt(
             1.0
             + (simulator.time_step / self.time_constant)
             * (simulator.temperature / self.target_temperature - 1.0)
         )
-        return simulator.velocity / scaling_factor
+        return simulator.velocities / scaling_factor
```

### Comparing `jaxip-0.6.1/jaxip/types.py` & `jaxip-0.7.0/jaxip/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 from dataclasses import dataclass
 
 import jax.numpy as jnp
+from jax._src.numpy.lax_numpy import _ScalarMeta
+from jaxlib.xla_extension import ArrayImpl
 
-Array = jnp.ndarray
-Dtype = jnp.dtype
+Array = ArrayImpl
+Dtype = _ScalarMeta
 Element = str
+Scalar = ArrayImpl
 
 
 @dataclass
 class DataType:
     """
-    A configuration class for arrays data type.
-    It is globally used as default dtype for arrays, indices, etc.
+    A configuration for array data type.
 
+    It is globally used as default dtype for arrays, indices, etc.
     User can modify any default dtype, for example, via setting the global
-    floating point precision of `FLOATX` to single (float32) or double (float64).
+    floating point precision (`FLOATX`) to a single (float32)
+    or double (float64).
     """
 
-    FLOATX: Dtype = jnp.float32  # type: ignore
-    INT: Dtype = jnp.int32  # type: ignore
-    UINT: Dtype = jnp.uint32  # type: ignore
-    INDEX: Dtype = jnp.int32  # type: ignore
+    FLOATX: Dtype = jnp.float32
+    INT: Dtype = jnp.int32
+    UINT: Dtype = jnp.uint32
+    INDEX: Dtype = jnp.int32
+
+
+_dtype = DataType()
 
 
-dtype: DataType = DataType()
+# def set_as_default(dtype: Dtype) -> None:
+#     global _dtype
+#     _dtype = dtype
```

### Comparing `jaxip-0.6.1/jaxip/units.py` & `jaxip-0.7.0/jaxip/units.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/utils/attribute.py` & `jaxip-0.7.0/jaxip/utils/attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, Optional
 
 import jax.numpy as jnp
 
 from jaxip.logger import logger
 from jaxip.types import Array, Dtype
-from jaxip.types import dtype as _dtype
+from jaxip.types import _dtype
 
 
 def set_as_attribute(
     obj: Any,
     items: Dict[str, Any],
     prefix: str = "",
     postfix: str = "",
```

### Comparing `jaxip-0.6.1/jaxip/utils/batch.py` & `jaxip-0.7.0/jaxip/utils/batch.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/utils/compare.py` & `jaxip-0.7.0/jaxip/utils/compare.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     :param structure1: first structure
     :param structure2: second structure
     :param error: a list of error metrics including `RMSE`, `RMSEpa`, `MSE`, and `MSEpa`. Defaults to [`RMSEpa`]
     :param return_difference: whether return energy and force array differences or not, defaults to False
     :return: a dictionary of error metrics.
     """
     assert all(
-        structure1.atom_type == structure2.atom_type
+        structure1.atom_types == structure2.atom_types
     ), "Expected similar structures with the same atom types."
 
     result: Dict[str, Any] = dict()
-    frc_diff: Array = structure1.force - structure2.force
+    frc_diff: Array = structure1.forces - structure2.forces
     eng_diff: Array = structure1.total_energy - structure2.total_energy
     errors = [errors] if isinstance(errors, str) else errors
     print(f"Comparing two structures, error metrics: {', '.join(errors)}")
     errors = [x.lower() for x in errors]
 
     if "rmse" in errors:
         result["force_RMSE"] = jnp.sqrt(jnp.mean(frc_diff**2))
```

### Comparing `jaxip-0.6.1/jaxip/utils/profiler.py` & `jaxip-0.7.0/jaxip/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip/utils/tokenize.py` & `jaxip-0.7.0/jaxip/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/jaxip.egg-info/PKG-INFO` & `jaxip-0.7.0/jaxip.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.6.1
+Version: 0.7.0
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -88,14 +88,15 @@
 This script demonstrates the process of evaluating an array of atomic-centered symmetry functions (`ACSF`_) 
 for a specific element, which can be utilized to evaluate the descriptor values for any structure. 
 The resulting values can then be used to construct a machine learning potential.
 
 .. _ACSF: https://aip.scitation.org/doi/10.1063/1.3553717
 
 
+
 .. code-block:: python
 
         from jaxip.datasets import RunnerDataset
         from jaxip.descriptors import ACSF
         from jaxip.descriptors.acsf import CutoffFunction, G2, G3
 
         # Read atomic structure dataset (e.g. water molecules)
@@ -103,22 +104,23 @@
         structure = structures[0]
 
         # Define ACSF descriptor for hydrogen element
         descriptor = ACSF(element='H')
 
         # Add radial and angular symmetry functions
         cfn = CutoffFunction(r_cutoff=12.0, cutoff_type='tanh')
-        descriptor.add( G2(cfn, eta=0.5, r_shift=0.0), 'H')
-        descriptor.add( G3(cfn, eta=0.001, zeta=2.0, lambda0=1.0, r_shift=12.0), 'H', 'O')
+        descriptor.add(G2(cfn, eta=0.5, r_shift=0.0), 'H')
+        descriptor.add(G3(cfn, eta=0.001, zeta=2.0, lambda0=1.0, r_shift=12.0), 'H', 'O')
+        print(descriptor)
 
-        # Compute descriptor values
-        descriptor(structure)
+        values = descriptor(structure)
+        print("Descriptor values:\n", values)
 
-        # Compute gradient
-        descriptor.grad(structure, atom_index=0)
+        gradient = descriptor.grad(structure, atom_index=0)
+        print("Descriptor gradient:\n", gradient)
 
 
 -------------------------------------
 Training a machine learning potential
 -------------------------------------
 This example illustrates how to quickly create a `high-dimensional neural network 
 potential` (`HDNNP`_) instance from an in input setting files and train it on input structures. 
@@ -133,15 +135,15 @@
         from jaxip.potentials import NeuralNetworkPotential
 
         # Read atomic data
         structures = RunnerDataset("input.data")
         structure = structures[0]
 
         # Instantiate potential from input settings file
-        nnp = NeuralNetworkPotential.create_from_file("input.nn")
+        nnp = NeuralNetworkPotential.from_file("input.nn")
 
         # Fit descriptor scaler and model weights
         nnp.fit_scaler(structures)
         nnp.fit_model(structures)
         nnp.save()
 
         # Or loading from files
@@ -150,12 +152,20 @@
         # Total energy
         nnp(structure)
 
         # Force components
         nnp.compute_force(structure)
 
 
+
+Example files: `input.data`_ and `input.nn`_
+
+.. _input.data: https://drive.google.com/file/d/1VMckgIv_OUvCOXQ0pYzaF5yl9AwR0rBy/view?usp=sharing
+.. _input.nn: https://drive.google.com/file/d/15Oq9gAJ2xXVMcHyWXlRukfJFevyVO7lI/view?usp=sharing
+
+
+
 License
 -------
 
 This project is licensed under the GNU General Public License (GPL) version 3 - 
 see the `LICENSE <https://github.com/hghcomphys/jaxip/blob/main/LICENSE>`_ file for details.
```

### Comparing `jaxip-0.6.1/jaxip.egg-info/SOURCES.txt` & `jaxip-0.7.0/jaxip.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 docs/jaxip.simulation.rst
 docs/jaxip.utils.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/theory.rst
 docs/usage.rst
-docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
-docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
-docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
-docs/_build/html/_images/notebooks_tutorials_38_0.png
-docs/_build/html/_images/notebooks_tutorials_45_0.png
-docs/_build/html/_images/notebooks_tutorials_51_0.png
+docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png
+docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png
+docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png
+docs/_build/html/_images/notebooks_getting_started_38_0.png
+docs/_build/html/_images/notebooks_getting_started_45_0.png
+docs/_build/html/_images/notebooks_getting_started_51_0.png
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 docs/images/flowchart.drawio.png
 docs/images/water.png
 jaxip/__init__.py
 jaxip/_version.py
@@ -52,16 +52,14 @@
 jaxip.egg-info/SOURCES.txt
 jaxip.egg-info/dependency_links.txt
 jaxip.egg-info/entry_points.txt
 jaxip.egg-info/not-zip-safe
 jaxip.egg-info/requires.txt
 jaxip.egg-info/top_level.txt
 jaxip/atoms/__init__.py
-jaxip/atoms/_box.py
-jaxip/atoms/_neighbor.py
 jaxip/atoms/_structure.py
 jaxip/atoms/box.py
 jaxip/atoms/element.py
 jaxip/atoms/neighbor.py
 jaxip/atoms/structure.py
 jaxip/datasets/__init__.py
 jaxip/datasets/dataset.py
@@ -91,28 +89,28 @@
 jaxip/potentials/nnp/gradient_descent.py
 jaxip/potentials/nnp/kalman_filter.py
 jaxip/potentials/nnp/metrics.py
 jaxip/potentials/nnp/nnp.py
 jaxip/potentials/nnp/potential.py
 jaxip/potentials/nnp/settings.py
 jaxip/simulation/__init__.py
+jaxip/simulation/lj.py
 jaxip/simulation/mc.py
 jaxip/simulation/md.py
 jaxip/simulation/run.py
 jaxip/simulation/thermostat.py
 jaxip/utils/__init__.py
 jaxip/utils/attribute.py
 jaxip/utils/batch.py
 jaxip/utils/compare.py
 jaxip/utils/profiler.py
 jaxip/utils/tokenize.py
 tests/__init__.py
 tests/h2o.data
 tests/h2o.json
-tests/ljpot.py
 tests/scaling.001.data
 tests/scaling.008.data
 tests/test_acsf.py
 tests/test_mc.py
 tests/test_md.py
 tests/test_nn.py
 tests/test_nnp.py
```

### Comparing `jaxip-0.6.1/setup.py` & `jaxip-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/tests/.ipynb_checkpoints/h2o-checkpoint.data` & `jaxip-0.7.0/tests/.ipynb_checkpoints/h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/tests/.ipynb_checkpoints/h2o-checkpoint.json` & `jaxip-0.7.0/tests/.ipynb_checkpoints/h2o-checkpoint.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/tests/.ipynb_checkpoints/input.h2o-checkpoint.data` & `jaxip-0.7.0/tests/.ipynb_checkpoints/input.h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/tests/.ipynb_checkpoints/test-checkpoint.ipynb` & `jaxip-0.7.0/tests/.ipynb_checkpoints/test-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/tests/h2o.data` & `jaxip-0.7.0/tests/h2o.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/tests/h2o.json` & `jaxip-0.7.0/tests/h2o.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/tests/ljpot.py` & `jaxip-0.7.0/jaxip/simulation/lj.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,70 @@
 import os
 from functools import partial
+from typing import Tuple, cast
 
 import jax
 import jax.numpy as jnp
 
+from jaxip.atoms.neighbor import Neighbor
 from jaxip.atoms.structure import Structure
 from jaxip.types import Array
-from jaxip.units import units
 
 os.environ["JAX_ENABLE_X64"] = "1"
 os.environ["JAX_PLATFORM_NAME"] = "cpu"
 
 
-@partial(jax.jit, static_argnums=0)
-def _compute_pair_energy(obj, r: Array) -> Array:
+# @partial(jax.jit, static_argnums=0)
+def _compute_pair_energies(obj, r: Array) -> Array:
     term = obj.sigma / r
     term6 = term**6
     return 4.0 * obj.epsilon * term6 * (term6 - 1.0)
 
 
-@partial(jax.jit, static_argnums=0)
-def _compute_pair_force(obj, r: Array, R: Array) -> Array:
+# @partial(jax.jit, static_argnums=0)
+def _compute_pair_forces(obj, r: Array, R: Array) -> Array:
     term = obj.sigma / r
     term6 = term**6
     force_factor = -24.0 * obj.epsilon / (r * r) * term6 * (2.0 * term6 - 1.0)
     return jnp.expand_dims(force_factor, axis=-1) * R
 
 
+def _get_neighbor_data(
+    structure: Structure,
+    r_cutoff: float,
+) -> Tuple[Array, Array, Array]:
+    if structure.neighbor is None:
+        structure.update_neighbor(r_cutoff)
+    neighbor = cast(Neighbor, structure.neighbor)
+    return (neighbor.masks, neighbor.rij, neighbor.Rij)
+
+
 class LJPotential:
+    """An implementation of Lennard-Jones potential."""
+
     def __init__(
         self,
         sigma: float,
         epsilon: float,
         r_cutoff: float,
     ) -> None:
         self.sigma = sigma
         self.epsilon = epsilon
         self.r_cutoff = r_cutoff
 
+    @partial(jax.jit, static_argnums=0)
     def __call__(self, structure: Structure) -> Array:
-        r, _ = structure.calculate_distance(atom_index=jnp.arange(structure.natoms))
-        mask = (0 < r) & (r < self.r_cutoff)
-        pair_energies = _compute_pair_energy(self, r)
-        return 0.5 * jnp.where(mask, pair_energies, 0.0).sum()  # type: ignore
-
-    def compute_force(self, structure: Structure) -> Array:
-        r, R = structure.calculate_distance(atom_index=jnp.arange(structure.natoms))
-        mask = (0 < r) & (r < self.r_cutoff)
+        """Compute total energy."""
+        masks, rij, _ = _get_neighbor_data(structure, self.r_cutoff)
+        pair_energies = _compute_pair_energies(self, rij)
+        return 0.5 * jnp.where(masks, pair_energies, 0.0).sum()  # type: ignore
+
+    @partial(jax.jit, static_argnums=0)
+    def compute_forces(self, structure: Structure) -> Array:
+        """Compute force component for each atoms."""
+        masks, rij, Rij = _get_neighbor_data(structure, self.r_cutoff)
         pair_forces = jnp.where(
-            jnp.expand_dims(mask, axis=-1),
-            _compute_pair_force(self, r, R),
-            jnp.zeros_like(R),
+            jnp.expand_dims(masks, axis=-1),
+            _compute_pair_forces(self, rij, Rij),
+            jnp.zeros_like(Rij),
         )
         return jnp.sum(pair_forces, axis=1)  # type: ignore
```

### Comparing `jaxip-0.6.1/tests/test_acsf.py` & `jaxip-0.7.0/tests/test_acsf.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,42 +56,42 @@
                 ),
             ),
         ),
     )
 
 
 class TestACSF:
-    lj_structure: Structure = Structure.create_from_dict(
+    lj_structure: Structure = Structure.from_dict(
         {
-            "position": [[0.0, 0.0, 0.0], [0.588897275, 0.588897275, 0.588897275]],
-            "element": ["Ne", "Ne"],
+            "positions": [[0.0, 0.0, 0.0], [0.588897275, 0.588897275, 0.588897275]],
+            "elements": ["Ne", "Ne"],
         }
     )
-    h2o_structure: Structure = Structure.create_from_dict(
+    h2o_structure: Structure = Structure.from_dict(
         {
             "lattice": [
                 [11.8086403654, 0.0, 0.0],
                 [0.0, 11.8086403654, 0.0],
                 [0.0, 0.0, 11.8086403654],
             ],
-            "position": [
+            "positions": [
                 [0.2958498542, -0.8444146738, 1.9618569793],
                 [1.7226932399, -1.8170359274, 0.5237867306],
                 [1.2660050151, -4.3958431356, 0.822408813],
                 [2.5830855482, 6.6971705174, 2.042321518],
                 [6.3733092527, 4.0651032678, 1.6571254123],
                 [4.5893132971, 4.2984466507, 3.33215409],
                 [-2.2136818837, 1.3673642557, 2.7768013741],
                 [-1.9466635812, -0.3397746484, 3.3828743394],
                 [-0.4559776878, 0.1681476423, -5.430449296],
                 [-1.2831542798, 4.5473991714, -2.294184217],
                 [-2.3516507887, 0.9376745482, -4.0756290424],
                 [-1.7819663898, 4.1957022409, -4.0621741923],
             ],
-            "element": ["O", "H", "H", "O", "H", "H", "O", "H", "H", "O", "H", "H"],
+            "elements": ["O", "H", "H", "O", "H", "H", "O", "H", "H", "O", "H", "H"],
         }
     )
 
     @pytest.mark.parametrize(
         "acsf, expected",
         [
             (
@@ -157,8 +157,8 @@
     def test_acsf_with_pbc(
         self,
         acsf: ACSF,
         structure: Structure,
         expected: Array,
     ) -> None:
         assert acsf(structure).shape == expected[0]
-        assert jnp.allclose(acsf(structure, atom_index=jnp.asarray(0)), expected[1])
+        assert jnp.allclose(acsf(structure, atom_indices=jnp.asarray(0)), expected[1])
```

### Comparing `jaxip-0.6.1/tests/test_mc.py` & `jaxip-0.7.0/tests/test_mc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import os
 from typing import Tuple
 
 import jax.numpy as jnp
 import pytest
 from ase import Atoms
 
-from .ljpot import LJPotential
 from jaxip.atoms.structure import Structure
+from jaxip.simulation.lj import LJPotential
 from jaxip.simulation.mc import MCSimulator
 from jaxip.units import units
 
 os.environ["JAX_ENABLE_X64"] = "1"
 os.environ["JAX_PLATFORM_NAME"] = "cpu"
 
 
 def get_structure() -> Structure:
     d = 6  # Angstrom
     uc = Atoms("He", positions=[(d / 2, d / 2, d / 2)], cell=(d, d, d))
-    s = Structure.create_from_ase(uc.repeat((2, 2, 2)))
+    s = Structure.from_ase(uc.repeat((2, 2, 2)))
     return s
 
 
-def get_potential():
+def get_potential() -> LJPotential:
     return LJPotential(
         sigma=2.5238 * units.FROM_ANGSTROM,
         epsilon=4.7093e-04 * units.FROM_ELECTRON_VOLT,
         r_cutoff=6.3095 * units.FROM_ANGSTROM,
     )
 
 
@@ -71,16 +71,16 @@
         ],
     )
     def test_structure_attributes(
         self,
         mc: MCSimulator,
         structure: Structure,
     ) -> None:
-        assert jnp.allclose(mc.position, structure.position)
-        assert jnp.allclose(mc.mass, structure.mass)
+        assert jnp.allclose(mc.positions, structure.positions)
+        assert jnp.allclose(mc.masses, structure.get_masses())
 
     @pytest.mark.parametrize(
         "mc, expected",
         [
             (
                 mc,
                 (
```

### Comparing `jaxip-0.6.1/tests/test_md.py` & `jaxip-0.7.0/tests/test_md.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import os
 from typing import Tuple
 
 import jax.numpy as jnp
 import pytest
 from ase import Atoms
 
-
-from .ljpot import LJPotential
 from jaxip.atoms.structure import Structure
+from jaxip.simulation.lj import LJPotential
 from jaxip.simulation.md import MDSimulator
 from jaxip.units import units
 
 os.environ["JAX_ENABLE_X64"] = "1"
 os.environ["JAX_PLATFORM_NAME"] = "cpu"
 
 
 def get_structure() -> Structure:
     d = 6  # Angstrom
     uc = Atoms("He", positions=[(d / 2, d / 2, d / 2)], cell=(d, d, d))
-    s = Structure.create_from_ase(uc.repeat((2, 2, 2)))
+    s = Structure.from_ase(uc.repeat((2, 2, 2)))
     return s
 
 
-def get_potential():
+def get_potential() -> LJPotential:
     return LJPotential(
         sigma=2.5238 * units.FROM_ANGSTROM,
         epsilon=4.7093e-04 * units.FROM_ELECTRON_VOLT,
         r_cutoff=6.3095 * units.FROM_ANGSTROM,
     )
 
 
@@ -57,19 +56,19 @@
         self,
         md: MDSimulator,
         expected: Tuple,
     ) -> None:
         assert md.step == 0
         assert jnp.allclose(md.elapsed_time, 0.0)
         assert jnp.allclose(md.time_step, expected[0])
-        assert jnp.allclose(md.get_com_velocity(), jnp.zeros(3))
+        assert jnp.allclose(md.get_center_of_mass_velocity(), jnp.zeros(3))
         assert jnp.allclose(md.temperature, expected[1])
         assert jnp.allclose(md.get_pressure(), expected[2])
         assert jnp.allclose(md.get_total_energy(), expected[3])
-        assert jnp.allclose(md.get_com_position(), expected[4])
+        assert jnp.allclose(md.get_center_of_mass_position(), expected[4])
 
     @pytest.mark.parametrize(
         "md, structure",
         [
             (
                 md,
                 get_structure(),
@@ -77,16 +76,16 @@
         ],
     )
     def test_structure_attributes(
         self,
         md: MDSimulator,
         structure: Structure,
     ) -> None:
-        assert jnp.allclose(md.position, structure.position)
-        assert jnp.allclose(md.mass, structure.mass)
+        assert jnp.allclose(md.positions, structure.positions)
+        assert jnp.allclose(md.masses, structure.get_masses())
 
     @pytest.mark.parametrize(
         "md, expected",
         [
             (
                 md,
                 (
@@ -104,12 +103,9 @@
         md: MDSimulator,
         expected: Tuple,
     ) -> None:
         md.update()
         assert md.step == 1
         assert jnp.allclose(md.elapsed_time, expected[0])
         assert jnp.allclose(md.time_step, expected[0])
-        assert jnp.allclose(md.get_com_velocity(), jnp.zeros(3))
-        assert jnp.allclose(md.temperature, expected[1])
-        assert jnp.allclose(md.get_pressure(), expected[2])
-        assert jnp.allclose(md.get_total_energy(), expected[3])
-        assert jnp.allclose(md.get_com_position(), expected[4])
+        assert jnp.allclose(md.get_center_of_mass_velocity(), jnp.zeros(3))
+        assert jnp.allclose(md.get_center_of_mass_position(), expected[4])
```

### Comparing `jaxip-0.6.1/tests/test_nn.py` & `jaxip-0.7.0/tests/test_nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import jax
 import jax.numpy as jnp
 import pytest
 from frozendict import frozendict
 
 from jaxip.models.nn.initializer import UniformInitializer
 from jaxip.models.nn.network import NeuralNetworkModel
-from jaxip.types import dtype as _dtype
+from jaxip.types import _dtype
 
 
 class TestNeuralNetworkModel:
     nn_1: NeuralNetworkModel = NeuralNetworkModel(hidden_layers=((2, "tanh"),))
     nn_2: NeuralNetworkModel = NeuralNetworkModel(
         hidden_layers=((4, "tanh"), (8, "identity")),
         param_dtype=jnp.float64,  # type: ignore
```

### Comparing `jaxip-0.6.1/tests/test_nnp.py` & `jaxip-0.7.0/tests/test_nnp.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 os.environ["JAX_PLATFORM_NAME"] = "cpu"
 
 import jax.numpy as jnp
 import pytest
 
 from jaxip.datasets import RunnerDataset
 from jaxip.potentials import NeuralNetworkPotential
-from jaxip.potentials.nnp.settings import \
-    NeuralNetworkPotentialSettings as PotentialSettings
+from jaxip.potentials.nnp.settings import (
+    NeuralNetworkPotentialSettings as PotentialSettings,
+)
 
 dataset_file = Path("tests", "h2o.data")
 potential_file = Path("tests", "h2o.json")
 
 
 class TestNeuralNetworkPotential:
     dataset = RunnerDataset(dataset_file)
-    nnp: NeuralNetworkPotential = NeuralNetworkPotential.create_from_file(
-        potential_file
-    )
+    nnp: NeuralNetworkPotential = NeuralNetworkPotential.from_file(potential_file)
 
     @pytest.mark.parametrize(
         "nnp, expected",
         [
             (
                 nnp,
                 (
@@ -38,15 +37,15 @@
     def test_settings(
         self,
         nnp: NeuralNetworkPotential,
         expected: Tuple,
     ) -> None:
         assert nnp.num_elements == expected[0]
         assert nnp.elements == expected[1]
-        assert nnp.settings == PotentialSettings.create_from_json(potential_file)
+        assert nnp.settings == PotentialSettings.from_json(potential_file)
 
     @pytest.mark.parametrize(
         "nnp, dataset, expected",
         [
             (
                 nnp,
                 dataset,
@@ -78,15 +77,15 @@
         dataset: RunnerDataset,
         expected: Tuple,
     ) -> None:
         nnp.fit_scaler(dataset)
 
         # total energy
         assert jnp.allclose(nnp(dataset[0]), expected[0])
-        assert jnp.allclose(nnp.compute_force(dataset[0]), expected[1])
+        assert jnp.allclose(nnp.compute_forces(dataset[0]), expected[1])
 
     @pytest.mark.parametrize(
         "nnp, dataset",
         [
             (
                 nnp,
                 dataset,
```

### Comparing `jaxip-0.6.1/tests/test_runner.py` & `jaxip-0.7.0/tests/test_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,45 +14,45 @@
 h2o_filename = Path("tests", "h2o.data")
 H2O_DATA = {
     "lattice": [
         [11.8086403654, 0.0, 0.0],
         [0.0, 11.8086403654, 0.0],
         [0.0, 0.0, 11.8086403654],
     ],
-    "position": [
+    "positions": [
         [-0.0075149684, -0.99679652, 2.0432096893],
         [1.6785530169, -1.7652744389, 0.6272511261],
         [1.3209809278, -4.4733785988, 0.478346376],
         [2.5377510183, 6.6473573365, 1.7994898202],
         [6.4670963607, 4.0467540271, 1.709941368],
         [4.5666176862, 4.2124641117, 3.1394587162],
         [-2.7259110493, 1.4093199553, 3.2330757488],
         [-1.9756708773, -0.2319865595, 3.5377751905],
         [-0.4456843495, 0.2034309079, -5.3880816361],
         [-0.5311245372, 4.5221524303, -3.0878691928],
         [-2.2546133518, 0.9970025001, -3.8398101183],
         [-1.9353630189, 4.1351176211, -4.0833580223],
     ],
-    "element": ["O", "H", "H", "O", "H", "H", "O", "H", "H", "O", "H", "H"],
-    "charge": [
+    "elements": ["O", "H", "H", "O", "H", "H", "O", "H", "H", "O", "H", "H"],
+    "charges": [
         0.442739,
         -0.244991,
         -0.31647,
         0.437298,
         -0.132604,
         -0.161461,
         0.452464,
         -0.432144,
         -0.0865354,
         0.430147,
         -0.0713622,
         -0.317081,
     ],
-    "energy": [-0.0, -0.0, -0.0, -0.0, -0.0, -0.0, 0.0, -0.0, -0.0, -0.0, -0.0, -0.0],
-    "force": [
+    "energies": [-0.0, -0.0, -0.0, -0.0, -0.0, -0.0, 0.0, -0.0, -0.0, -0.0, -0.0, -0.0],
+    "forces": [
         [0.0576867169, -0.2578270722, -0.2339365489],
         [-0.5157027617, -1.4143481512, -0.1199800167],
         [0.261360575, 2.1511972322, 0.444809068],
         [0.1560563599, -0.4345566594, -0.2367582949],
         [0.3723498983, 0.1835258917, -0.51876176],
         [-0.4569867202, -0.1613043018, 0.6545692241],
         [0.0005268906, -0.0777825655, -0.2173794536],
@@ -60,15 +60,15 @@
         [-0.3358675037, -0.0775036969, 0.0481281739],
         [0.239214439, 0.0010185589, 0.3207105856],
         [0.3703935397, -0.16099179, -0.1473258662],
         [-0.3212920481, 0.2033815711, -0.343463465],
     ],
     "total_energy": [-32.2949885081],
     "total_charge": [-6e-07],
-    "atom_type": [2, 1, 1, 2, 1, 1, 2, 1, 1, 2, 1, 1],
+    "atom_types": [2, 1, 1, 2, 1, 1, 2, 1, 1, 2, 1, 1],
 }
 
 
 class TestRunnerDataset:
     h2o: RunnerDataset = RunnerDataset(filename=h2o_filename)
     h2o_raw: RunnerDataset = RunnerDataset(
         filename=h2o_filename, transform=lambda x: x  # type: ignore
@@ -151,13 +151,13 @@
     def test_loading_structure(
         self,
         dataset: RunnerDataset,
         expected: Tuple,
     ) -> None:
         structure: Structure = dataset[1]
         for i, attr in enumerate(Structure._get_atom_attributes()):
-            if attr == "position":
+            if attr == "positions":
                 assert jnp.allclose(
-                    structure.position, structure.box.shift_inside_box(expected[i])
+                    structure.positions, structure.box.shift_inside_box(expected[i])
                 )
             else:
                 assert jnp.allclose(getattr(structure, attr), expected[i])
```

### Comparing `jaxip-0.6.1/tests/test_scaler.py` & `jaxip-0.7.0/tests/test_scaler.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import jax.numpy as jnp
 import pytest
 from jax import random
 
 from jaxip.descriptors.scaler import Scaler
 from jaxip.types import Array
-from jaxip.types import dtype as _dtype
+from jaxip.types import _dtype
 from jaxip.utils.batch import create_batch
 
 key = random.PRNGKey(2023)
 key, subkey = random.split(key, 2)
 
 
 class TestStructure:
```

### Comparing `jaxip-0.6.1/tests/test_structure.py` & `jaxip-0.7.0/tests/test_structure.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,87 +1,89 @@
 import os
 from typing import Any, Dict, Tuple
 
 import jax.numpy as jnp
 import pytest
 
 from jaxip.atoms.structure import Structure
-from jaxip.types import dtype as _dtype
+from jaxip.types import _dtype
 
 os.environ["JAX_ENABLE_X64"] = "1"
 os.environ["JAX_PLATFORM_NAME"] = "cpu"
 
 
 LJ_DATA: Dict[str, Any] = {
-    "position": [[0.0, 0.0, 0.0], [0.583123772, 0.583123772, 0.583123772]],
-    "element": ["Ne", "Ne"],
-    "charge": [0.0, 0.0],
-    "energy": [0.0, 0.0],
-    "force": [
+    "positions": [[0.0, 0.0, 0.0], [0.583123772, 0.583123772, 0.583123772]],
+    "elements": ["Ne", "Ne"],
+    "charges": [0.0, 0.0],
+    "energies": [0.0, 0.0],
+    "forces": [
         [-11.4260918, -11.4260918, -11.4260918],
         [11.4260918, 11.4260918, 11.4260918],
     ],
     "total_energy": [-0.21838404],
-    "comment": ["r = 1.01000000E+00, E = -2.18384040E-01, dEdr = -1.97905715E+01"],
+    "comment": [
+        "r = 1.01000000E+00, E = -2.18384040E-01, dEdr = -1.97905715E+01"
+    ],
     "total_charge": [],
     "lattice": [],
-    "atom_type": [1, 1],
-    "mass": [36785.88642640456] * 2,
+    "atom_types": [1, 1],
+    "masses": [36785.88642640456] * 2,
 }
 
 H2O_DATA: Dict[str, Any] = {
     "lattice": [
         [11.8086403654, 0.0, 0.0],
         [0.0, 11.8086403654, 0.0],
         [0.0, 0.0, 11.8086403654],
     ],
-    "position": [
+    "positions": [
         [0.2958498542, -0.8444146738, 1.9618569793],
         [1.7226932399, -1.8170359274, 0.5237867306],
         [1.2660050151, -4.3958431356, 0.822408813],
         [2.5830855482, 6.6971705174, 2.042321518],
         [6.3733092527, 4.0651032678, 1.6571254123],
         [4.5893132971, 4.2984466507, 3.33215409],
         [-2.2136818837, 1.3673642557, 2.7768013741],
         [-1.9466635812, -0.3397746484, 3.3828743394],
         [-0.4559776878, 0.1681476423, -5.430449296],
         [-1.2831542798, 4.5473991714, -2.294184217],
         [-2.3516507887, 0.9376745482, -4.0756290424],
         [-1.7819663898, 4.1957022409, -4.0621741923],
     ],
-    "element": ["O", "H", "H", "O", "H", "H", "O", "H", "H", "O", "H", "H"],
-    "charge": [
+    "elements": ["O", "H", "H", "O", "H", "H", "O", "H", "H", "O", "H", "H"],
+    "charges": [
         0.423192,
         -0.243872,
         -0.313417,
         0.439248,
         -0.136408,
         -0.154832,
         0.418857,
         -0.401243,
         -0.0766178,
         0.411994,
         -0.0691934,
         -0.297707,
     ],
-    "energy": [
+    "energies": [
         0.0,
         0.0,
         0.0,
         0.0,
         0.0,
         0.0,
         0.0,
         0.0,
         0.0,
         0.0,
         0.0,
         0.0,
     ],
-    "force": [
+    "forces": [
         [-0.4727795521, -0.0084561951, 0.0460983059],
         [0.1920381912, 0.0587784661, 0.6142110612],
         [-0.8869675228, -0.7832124482, -0.7448845423],
         [0.7405673293, 0.4095246028, 0.1627052569],
         [-0.7272286968, 0.2123232582, 0.5568660265],
         [0.6038769757, -0.0797700393, -0.5249089268],
         [-0.2617806281, -0.2369410958, 0.1869405738],
@@ -89,94 +91,107 @@
         [-0.1108903386, -0.3317914324, -0.6560763592],
         [-0.1172658121, -0.1885000212, -0.5958629059],
         [-0.1934543148, 0.5415107499, 0.4505828542],
         [0.0216973013, -0.0334599566, 0.508882732],
     ],
     "total_energy": [-32.1390027258],
     "total_charge": [8.0e-07],
-    "atom_type": [2, 1, 1, 2, 1, 1, 2, 1, 1, 2, 1, 1],
-    "mass": [29164.39033379815, 1837.4714329938454, 1837.4714329938454] * 4,
+    "atom_types": [2, 1, 1, 2, 1, 1, 2, 1, 1, 2, 1, 1],
+    "masses": [29164.39033379815, 1837.4714329938454, 1837.4714329938454] * 4,
 }
 
 
 class TestStructure:
-    lj: Structure = Structure.create_from_dict(
-        LJ_DATA, dtype=jnp.float32  # type: ignore
-    )  # type: ignore
-    h2o: Structure = Structure.create_from_dict(H2O_DATA, r_cutoff=11.0)
+    lj: Structure = Structure.from_dict(LJ_DATA, dtype=jnp.float32)
+    h2o: Structure = Structure.from_dict(H2O_DATA)
     atom_attributes: Tuple[str, ...] = tuple(
-        ["position", "force", "energy", "total_energy", "charge", "total_charge"]
+        [
+            "positions",
+            "forces",
+            "energies",
+            "total_energy",
+            "charges",
+            "total_charge",
+        ]
     )
 
     @pytest.mark.parametrize(
         "structure, expected",
         [
             (
                 lj,
                 tuple(
-                    jnp.asarray(LJ_DATA[attr])
+                    jnp.array(LJ_DATA[attr])
                     for attr in Structure._get_atom_attributes()
                 ),
             ),
             (
                 h2o,
                 tuple(
-                    jnp.asarray(H2O_DATA[attr])
+                    jnp.array(H2O_DATA[attr])
                     for attr in Structure._get_atom_attributes()
                 ),
             ),
         ],
     )
     def test_atom_attributes(
         self,
         structure: Structure,
         expected: Tuple,
     ) -> None:
         for i, attr in enumerate(Structure._get_atom_attributes()):
-            if attr == "position":
-                assert jnp.allclose(
-                    structure.position, structure.box.shift_inside_box(expected[i])
+            if attr == "positions":
+                expected_positions = (
+                    expected[i]
+                    if structure.box is None
+                    else structure.box.shift_inside_box(expected[i])
                 )
+                assert jnp.allclose(structure.positions, expected_positions)
             else:
                 assert jnp.allclose(getattr(structure, attr), expected[i])
 
     @pytest.mark.parametrize(
         "structure, expected",
         [
             (
                 lj,
                 (
                     2,
                     ("Ne",),
                     None,
                     jnp.float32,
                     None,
-                    jnp.asarray(LJ_DATA["mass"]),
+                    jnp.array(LJ_DATA["masses"]),
+                    tuple(LJ_DATA["elements"]),
                 ),
             ),
             (
                 h2o,
                 (
                     12,
                     ("H", "O"),
                     11.0,
                     _dtype.FLOATX,
-                    jnp.asarray(H2O_DATA["lattice"]),
-                    jnp.asarray(H2O_DATA["mass"]),
+                    jnp.array(H2O_DATA["lattice"]),
+                    jnp.array(H2O_DATA["masses"]),
+                    tuple(H2O_DATA["elements"]),
                 ),
             ),
         ],
     )
     def test_general_attributes(
         self,
         structure: Structure,
         expected: Tuple,
     ) -> None:
+        if expected[2] is not None:
+            structure.update_neighbor(expected[2])
         assert structure.natoms == expected[0]
-        assert structure.elements == expected[1]
+        assert structure.get_unique_elements() == expected[1]
         assert structure.r_cutoff == expected[2]
         assert structure.dtype == expected[3]
         if structure.lattice is None:
             assert structure.lattice is expected[4]
         else:
             assert jnp.allclose(structure.lattice, expected[4])
-        assert jnp.allclose(structure.mass, expected[5])
+        assert jnp.allclose(structure.get_masses(), expected[5])
+        assert structure.get_elements() == expected[6]
```

### Comparing `jaxip-0.6.1/tests/weights.001.pkl` & `jaxip-0.7.0/tests/weights.001.pkl`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.1/tests/weights.008.pkl` & `jaxip-0.7.0/tests/weights.008.pkl`

 * *Files identical despite different names*

