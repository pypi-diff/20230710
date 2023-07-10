# Comparing `tmp/perceval-quandela-0.8.1.tar.gz` & `tmp/perceval-quandela-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval-quandela-0.8.1.tar", last modified: Tue Mar 21 10:40:03 2023, max compression
+gzip compressed data, was "perceval-quandela-0.9.0.tar", last modified: Mon Jul 10 10:16:34 2023, max compression
```

## Comparing `perceval-quandela-0.8.1.tar` & `perceval-quandela-0.9.0.tar`

### file list

```diff
@@ -1,113 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.738670 perceval-quandela-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-03-21 10:40:03.738670 perceval-quandela-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.726670 perceval-quandela-0.8.1/perceval/
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.726670 perceval-quandela-0.8.1/perceval/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/algorithm/abstract_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/algorithm/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/algorithm/qrng.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/algorithm/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.726670 perceval-quandela-0.8.1/perceval/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/backends/cliffords2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/backends/mps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/backends/naive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.726670 perceval-quandela-0.8.1/perceval/backends/processor/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/backends/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/backends/processor/stepper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/backends/slos.py
--rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/backends/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.730670 perceval-quandela-0.8.1/perceval/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/_mode_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/abstract_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/component_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.730670 perceval-quandela-0.8.1/perceval/components/computation/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/computation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/computation/time_delays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.730670 perceval-quandela-0.8.1/perceval/components/core_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/core_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/core_catalog/generic_2mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/core_catalog/heralded_cnot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/core_catalog/postprocessed_cnot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    36272 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/linear_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/non_unitary_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/predefined_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/source.py
--rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/components/unitary_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.730670 perceval-quandela-0.8.1/perceval/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/converters/qiskit_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.730670 perceval-quandela-0.8.1/perceval/rendering/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/_mplot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/_processor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.730670 perceval-quandela-0.8.1/perceval/rendering/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/canvas/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/canvas/mplot_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/canvas/svg_canvas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.730670 perceval-quandela-0.8.1/perceval/rendering/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/circuit/abstract_skin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/circuit/phys_skin.py
--rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/circuit/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/circuit/skin_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/circuit/symb_skin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/rendering/pdisplay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.734670 perceval-quandela-0.8.1/perceval/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/runtime/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/runtime/job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/runtime/local_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/runtime/remote_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/runtime/remote_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/runtime/rpc_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.734670 perceval-quandela-0.8.1/perceval/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/serialization/_circuit_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/serialization/_component_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/serialization/_matrix_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/serialization/_parameter_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/serialization/_schema_circuit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/serialization/_state_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/serialization/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/serialization/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/serialization/serialize_binary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.734670 perceval-quandela-0.8.1/perceval/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.734670 perceval-quandela-0.8.1/perceval/utils/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/algorithms/circuit_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/algorithms/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/algorithms/match.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/algorithms/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/algorithms/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/algorithms/simplification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/algorithms/solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/mlstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/polarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    24055 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/perceval/utils/statevector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:40:03.738670 perceval-quandela-0.8.1/perceval_quandela.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-03-21 10:40:03.000000 perceval-quandela-0.8.1/perceval_quandela.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-03-21 10:40:03.000000 perceval-quandela-0.8.1/perceval_quandela.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 10:40:03.000000 perceval-quandela-0.8.1/perceval_quandela.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-21 10:40:03.000000 perceval-quandela-0.8.1/perceval_quandela.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-21 10:40:03.000000 perceval-quandela-0.8.1/perceval_quandela.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-21 10:40:03.738670 perceval-quandela-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-03-21 10:39:58.000000 perceval-quandela-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.668261 perceval-quandela-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-10 10:16:34.668261 perceval-quandela-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.660261 perceval-quandela-0.9.0/perceval/
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.660261 perceval-quandela-0.9.0/perceval/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/algorithm/abstract_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/algorithm/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/algorithm/qrng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/algorithm/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.660261 perceval-quandela-0.9.0/perceval/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/backends/_abstract_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/backends/_clifford2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/backends/_mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/backends/_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/backends/_slos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.660261 perceval-quandela-0.9.0/perceval/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/_mode_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/abstract_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21723 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/component_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.660261 perceval-quandela-0.9.0/perceval/components/core_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/core_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/core_catalog/generic_2mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/core_catalog/heralded_cnot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/core_catalog/heralded_cz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/core_catalog/postprocessed_cnot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35994 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/linear_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/non_unitary_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/predefined_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/unitary_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.660261 perceval-quandela-0.9.0/perceval/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/converters/converter_statevector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/converters/qiskit_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.664261 perceval-quandela-0.9.0/perceval/rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/_mplot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/_processor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.664261 perceval-quandela-0.9.0/perceval/rendering/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/canvas/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/canvas/latex_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/canvas/mplot_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/canvas/svg_canvas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.664261 perceval-quandela-0.9.0/perceval/rendering/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/circuit/abstract_skin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/circuit/phys_skin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22799 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/circuit/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/circuit/skin_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/circuit/symb_skin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/pdisplay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.664261 perceval-quandela-0.9.0/perceval/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/local_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/remote_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/remote_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/rpc_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.664261 perceval-quandela-0.9.0/perceval/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/_circuit_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/_component_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/_matrix_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/_parameter_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/_schema_circuit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/_state_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/serialize_binary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.664261 perceval-quandela-0.9.0/perceval/simulators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/_simulator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/delay_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/loss_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/polarization_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/simulator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/simulator_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.668261 perceval-quandela-0.9.0/perceval/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.668261 perceval-quandela-0.9.0/perceval/utils/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/circuit_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/simplification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/mlstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/polarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/postselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/stategenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/statevector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.668261 perceval-quandela-0.9.0/perceval_quandela.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-10 10:16:34.000000 perceval-quandela-0.9.0/perceval_quandela.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-10 10:16:34.000000 perceval-quandela-0.9.0/perceval_quandela.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:16:34.000000 perceval-quandela-0.9.0/perceval_quandela.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 10:16:34.000000 perceval-quandela-0.9.0/perceval_quandela.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-10 10:16:34.000000 perceval-quandela-0.9.0/perceval_quandela.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 10:16:34.668261 perceval-quandela-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/setup.py
```

### Comparing `perceval-quandela-0.8.1/LICENSE` & `perceval-quandela-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/PKG-INFO` & `perceval-quandela-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: perceval-quandela
-Version: 0.8.1
+Version: 0.9.0
 Summary: A powerful Quantum Photonic Framework
 Home-page: https://github.com/Quandela/Perceval
 Author: Perceval@Quandela.com
 Author-email: Perceval@Quandela.com
 Project-URL: Documentation, https://perceval.quandela.net/docs/
 Project-URL: Source, https://github.com/Quandela/Perceval
 Project-URL: Tracker, https://github.com/Quandela/Perceval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
 
 [![GitHub release](https://img.shields.io/github/v/release/Quandela/Perceval.svg?style=plastic)](https://github.com/Quandela/Perceval/releases/latest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Perceval?style=plastic)
 [![CI](https://github.com/Quandela/Perceval/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Quandela/Perceval/actions/workflows/python-publish.yml)
 
 [![CI](https://github.com/Quandela/Perceval/actions/workflows/autotests.yml/badge.svg)](https://github.com/Quandela/Perceval/actions/workflows/autotests.yml)
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: perceval-quandela Version: 0.8.1 Summary: A
+Metadata-Version: 2.1 Name: perceval-quandela Version: 0.9.0 Summary: A
 powerful Quantum Photonic Framework Home-page: https://github.com/Quandela/
 Perceval Author: Perceval@Quandela.com Author-email: Perceval@Quandela.com
 Project-URL: Documentation, https://perceval.quandela.net/docs/ Project-URL:
 Source, https://github.com/Quandela/Perceval Project-URL: Tracker, https://
 github.com/Quandela/Perceval/issues Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: test License-File: LICENSE [![GitHub release](https://
-img.shields.io/github/v/release/Quandela/Perceval.svg?style=plastic)](https://
-github.com/Quandela/Perceval/releases/latest) ![PyPI - Python Version](https://
+markdown License-File: LICENSE [![GitHub release](https://img.shields.io/
+github/v/release/Quandela/Perceval.svg?style=plastic)](https://github.com/
+Quandela/Perceval/releases/latest) ![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/Perceval?style=plastic) [![CI](https://
 github.com/Quandela/Perceval/actions/workflows/python-publish.yml/badge.svg)]
 (https://github.com/Quandela/Perceval/actions/workflows/python-publish.yml) [!
 [CI](https://github.com/Quandela/Perceval/actions/workflows/autotests.yml/
 badge.svg)](https://github.com/Quandela/Perceval/actions/workflows/
 autotests.yml) [![CI](https://github.com/Quandela/Perceval/actions/workflows/
 build-and-deploy-docs.yml/badge.svg)](https://github.com/Quandela/Perceval/
```

### Comparing `perceval-quandela-0.8.1/README.md` & `perceval-quandela-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/__init__.py` & `perceval-quandela-0.9.0/perceval/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 __version__ = get_distribution("perceval-quandela").version
 
 from .components import *
 from .backends import *
 from .utils import *
 from .rendering import *
 from .runtime import *
+from .simulators import Simulator, SimulatorFactory, DelaySimulator, LossSimulator, PolarizationSimulator
 
 
 def register_plugin(name, silent=False):
     try:
         plugin = importlib.import_module(name)
         assert plugin.register(silent) is True
     except Exception as e:
```

### Comparing `perceval-quandela-0.8.1/perceval/algorithm/__init__.py` & `perceval-quandela-0.9.0/perceval/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/algorithm/abstract_algorithm.py` & `perceval-quandela-0.9.0/perceval/algorithm/abstract_algorithm.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/algorithm/analyzer.py` & `perceval-quandela-0.9.0/perceval/algorithm/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,18 @@
         logical_perf = []
         if expected is not None:
             normalize = True
             self.error_rate = 0
 
         # Compute probabilities for all input states
         for idx, i_state in enumerate(self.input_states_list):
-            self._processor.with_input(i_state)
+            if i_state.has_polarization:
+                self._processor.with_polarized_input(i_state)
+            else:
+                self._processor.with_input(i_state)
             job = self._sampler.probs
             job.name = f'{self.default_job_name} {idx+1}/{len(self.input_states_list)}'
             probs_output = job.execute_sync()
             probs = probs_output['results']
             probs_res[i_state] = probs
             if 'logical_perf' in probs_output:
                 logical_perf.append(probs_output['logical_perf'])
```

### Comparing `perceval-quandela-0.8.1/perceval/algorithm/qrng.py` & `perceval-quandela-0.9.0/perceval/algorithm/qrng.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/backends/__init__.py` & `perceval-quandela-0.9.0/perceval/backends/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,34 +24,34 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import warnings
 
-from .template import Backend
-from .cliffords2017 import CliffordClifford2017Backend
-from .naive import NaiveBackend
-from .slos import SLOSBackend
-from .mps import MPSBackend
+from ._abstract_backends import ABackend, ASamplingBackend, AProbAmpliBackend
+from ._clifford2017 import Clifford2017Backend
+from ._naive import NaiveBackend
+from ._slos import SLOSBackend
+from ._mps import MPSBackend
 
 
 BACKEND_LIST = {
-    CliffordClifford2017Backend.name: CliffordClifford2017Backend,
-    MPSBackend.name: MPSBackend,
-    NaiveBackend.name: NaiveBackend,
-    SLOSBackend.name: SLOSBackend,
+    "CliffordClifford2017": Clifford2017Backend,
+    "MPS": MPSBackend,
+    "Naive": NaiveBackend,
+    "SLOS": SLOSBackend
 }
 
 
 class BackendFactory:
     @staticmethod
-    def get_backend(backend_name="SLOS"):
+    def get_backend(backend_name: str = "SLOS") -> ABackend:
         name = backend_name
         if name in BACKEND_LIST:
-            return BACKEND_LIST[name]
+            return BACKEND_LIST[name]()
         warnings.warn(f'Backend "{name}" not found. Falling back on SLOS')
-        return BACKEND_LIST['SLOS']
+        return BACKEND_LIST['SLOS']()
 
     @staticmethod
     def list():
         return list(BACKEND_LIST.keys())
```

### Comparing `perceval-quandela-0.8.1/perceval/backends/mps.py` & `perceval-quandela-0.9.0/perceval/backends/_mps.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,91 +31,99 @@
 import copy
 
 import numpy as np
 from math import factorial
 from scipy.special import comb
 from collections import defaultdict
 
-from .template import Backend
-from perceval.utils import BasicState, Matrix
+from ._abstract_backends import AProbAmpliBackend
+from perceval.utils import BasicState
 from perceval.components import ACircuit
 
 
-class MPSBackend(Backend):
-    """Step-by-step circuit propagation algorithm, works on a circuit. Approximate the probability amplitudes with a cutoff.
+class MPSBackend(AProbAmpliBackend):
+    """Step-by-step circuit propagation algorithm, works on a circuit.
+    Approximate the probability amplitudes with a cutoff.
     - For now only supports Phase shifters and Beam Splitters
     - TODO: link to the quandelibc computation
     """
 
-    def __init__(self,
-                 cu: Union[ACircuit, Matrix],
-                 use_symbolic: bool = None,
-                 n: int = None,
-                 mask: list = None):
-        super().__init__(cu, use_symbolic, n, mask)
-        for r, c in self._C:
-            assert c.compute_unitary(use_symbolic=False).shape[0] <= 2,\
-                "MPS backend can not be used with components of using more than 2 modes"
+    def __init__(self):
+        super().__init__()
         self._s_min = 1e-8
-        self.cutoff = self.m
-        self.res = defaultdict(lambda: defaultdict(lambda: np.array([0])))
-        self.current_input = None
-
-    name = "MPS"
-    supports_symbolic = False
-    supports_circuit_computing = True
-
-    def set_cutoff(self, cutoff: int):
-        assert isinstance(cutoff, int), "cutoff must be an integer"
-        self.cutoff = cutoff
+        self._cutoff = None
+        self._compiled_input = None
+        self._res = defaultdict(lambda: defaultdict(lambda: np.array([0])))
+        # Doubts : Nested dictionary why?
+        self._current_input = None
+
+    @property
+    def name(self) -> str:
+        return "MPS"
+
+    def set_cutoff(self, cutoff_val: int):
+        assert isinstance(cutoff_val, int), "cutoff must be an integer"
+        self._cutoff = cutoff_val
+
+    def set_circuit(self, circuit: ACircuit):
+        super().set_circuit(circuit)
+        C = self._circuit
+        for r, c in C:
+            assert c.compute_unitary(use_symbolic=False).shape[0] <= 2, \
+                "MPS backend can not be used with components of using more than 2 modes"
+        if self._cutoff is None:
+            self._cutoff = C.m
+
+    def set_input_state(self, input_state: BasicState):
+        super().set_input_state(input_state)
+        self.compile()
 
     def apply(self, r, c):
         u = c.compute_unitary(False)
         k_mode = r[0]
         if len(u) == 2:
             self.update_state(k_mode, u)  # --> quandelibc
         elif len(u) == 1:
             self.update_state_1_mode(k_mode, u)  # --> quandelibc
 
-    def compile(self, input_state: BasicState) -> bool:
-        var = [float(p) for p in self._C.get_parameters()]
-        if self._compiled_input and self._compiled_input[0] == var and input_state in self.res:
+    def compile(self) -> bool:
+        C = self._circuit
+        var = [float(p) for p in C.get_parameters()]
+        if self._compiled_input and self._compiled_input[0] == var and self._input_state in self._res:
             return False
-        self._compiled_input = copy.copy((var, input_state))
-        self.current_input = None
+        self._compiled_input = copy.copy((var, self._input_state))
+        self._current_input = None
 
         # TODO : allow any StateVector as in stepper, or a list as in SLOS
-        input_state *= BasicState([0] * (self.m - input_state.m))
-        self.n = input_state.n
+        # self._input_state *= BasicState([0] * (self._input_state.m - self._input_state.m))
+        self.n = self._input_state.n
         self.d = self.n + 1
-        self.cutoff = min(self.cutoff, self.d ** (self.m//2))
-        self.gamma = np.zeros((self.m, self.cutoff, self.cutoff, self.d), dtype='complex_')
-        for i in range(self.m):
-            self.gamma[i, 0, 0, input_state[i]] = 1
-        self.sv = np.zeros((self.m, self.cutoff))
+        self._cutoff = min(self._cutoff, self.d ** (self._input_state.m//2))
+        self._gamma = np.zeros((self._input_state.m, self._cutoff, self._cutoff, self.d), dtype='complex_')
+        for i in range(self._input_state.m):
+            self._gamma[i, 0, 0, self._input_state[i]] = 1
+        self.sv = np.zeros((self._input_state.m, self._cutoff))
         self.sv[:, 0] = 1
 
-        for r, c in self._C:
+        for r, c in C:
             self.apply(r, c)
 
-        self.res[tuple(input_state)]["gamma"] = self.gamma.copy()
-        self.res[tuple(input_state)]["sv"] = self.sv.copy()
+        self._res[tuple(self._input_state)]["gamma"] = self._gamma.copy()
+        self._res[tuple(self._input_state)]["sv"] = self.sv.copy()
         return True
 
-    def prob_be(self, input_state, output_state):
-        return abs(self.probampli_be(input_state, output_state))**2
-
-    def probampli_be(self, input_state, output_state):
+    def prob_amplitude(self, output_state: BasicState) -> complex:
         # TODO: put in quandelibc
+        m = self._input_state.m
         mps_in_list = []
-        self.current_input = tuple(input_state)
-        for k in range(self.m - 1):
-            mps_in_list.append(self.res[tuple(input_state)]["gamma"][k, :, :, output_state[k]])
+        self._current_input = tuple(self._input_state)
+        for k in range(m - 1):
+            mps_in_list.append(self._res[tuple(self._input_state)]["gamma"][k, :, :, output_state[k]])
             mps_in_list.append(self._sv_diag(k))
-        mps_in_list.append(self.res[tuple(input_state)]["gamma"][self.m-1, :, :, output_state[self.m-1]])
+        mps_in_list.append(self._res[tuple(self._input_state)]["gamma"][self._input_state.m-1, :, :, output_state[self._input_state.m-1]])
         return np.linalg.multi_dot(mps_in_list)[0, 0]
 
     @staticmethod
     def preferred_command() -> str:
         return 'probampli'
 
 # ################ From here, everything must be in quandelibc ##############################
@@ -126,64 +134,64 @@
         big_u = np.zeros((d, d), dtype='complex_')
         for i in range(d):
             big_u[i, i] = u[0, 0] ** i
 
         return big_u
 
     def update_state_1_mode(self, k, u):
-        self.gamma[k] = np.tensordot(self.gamma[k], self._transition_matrix_1_mode(u), axes=(2,0))
+        self._gamma[k] = np.tensordot(self._gamma[k], self._transition_matrix_1_mode(u), axes=(2, 0))
 
     def update_state(self, k, u):
 
-        if 0 < k < self.m - 2:
-            theta = np.tensordot(self._sv_diag(k - 1), self.gamma[k, :], axes=(1, 0))
+        if 0 < k < self._input_state.m - 2:
+            theta = np.tensordot(self._sv_diag(k - 1), self._gamma[k, :], axes=(1, 0))
             theta = np.tensordot(theta, self._sv_diag(k), axes=(1, 0))
-            theta = np.tensordot(theta, self.gamma[k + 1, :], axes=(2, 0))
+            theta = np.tensordot(theta, self._gamma[k + 1, :], axes=(2, 0))
             theta = np.tensordot(theta, self._sv_diag(k + 1), axes=(2, 0))
             theta = np.tensordot(theta, self._transition_matrix(u), axes=([1, 2], [0, 1]))
             theta = theta.swapaxes(1, 2).swapaxes(0, 1).swapaxes(2, 3)
-            theta = theta.reshape(self.d * self.cutoff, self.d * self.cutoff)
+            theta = theta.reshape(self.d * self._cutoff, self.d * self._cutoff)
 
         elif k == 0:
-            theta = np.tensordot(self.gamma[k, :], self._sv_diag(k), axes=(1, 0))
-            theta = np.tensordot(theta, self.gamma[k + 1, :], axes=(2, 0))
+            theta = np.tensordot(self._gamma[k, :], self._sv_diag(k), axes=(1, 0))
+            theta = np.tensordot(theta, self._gamma[k + 1, :], axes=(2, 0))
             theta = np.tensordot(theta, self._sv_diag(k + 1), axes=(2, 0))
             theta = np.tensordot(theta, self._transition_matrix(u),
                                  axes=([1, 2], [0, 1]))  # Pretty weird thing... To check
             theta = theta.swapaxes(1, 2).swapaxes(0, 1).swapaxes(2, 3)
-            theta = theta.reshape(self.d * self.cutoff, self.d * self.cutoff)
+            theta = theta.reshape(self.d * self._cutoff, self.d * self._cutoff)
 
-        elif k == self.m - 2:
-            theta = np.tensordot(self._sv_diag(k - 1), self.gamma[k, :], axes=(1, 0))
+        elif k == self._input_state.m - 2:
+            theta = np.tensordot(self._sv_diag(k - 1), self._gamma[k, :], axes=(1, 0))
             theta = np.tensordot(theta, self._sv_diag(k), axes=(1, 0))
-            theta = np.tensordot(theta, self.gamma[k + 1, :], axes=(2, 0))
+            theta = np.tensordot(theta, self._gamma[k + 1, :], axes=(2, 0))
             theta = np.tensordot(theta, self._transition_matrix(u), axes=([1, 3], [0, 1]))
             theta = theta.swapaxes(1, 2).swapaxes(0, 1).swapaxes(2, 3)
-            theta = theta.reshape(self.d * self.cutoff, self.d * self.cutoff)
+            theta = theta.reshape(self.d * self._cutoff, self.d * self._cutoff)
 
         v, s, w = np.linalg.svd(theta)
 
-        v = v.reshape(self.d, self.cutoff, self.d * self.cutoff).swapaxes(0, 1).swapaxes(1, 2)[:, :self.cutoff]
-        w = w.reshape(self.d * self.cutoff, self.d, self.cutoff).swapaxes(1, 2)[:self.cutoff]
-        s = s[:self.cutoff]
+        v = v.reshape(self.d, self._cutoff, self.d * self._cutoff).swapaxes(0, 1).swapaxes(1, 2)[:, :self._cutoff]
+        w = w.reshape(self.d * self._cutoff, self.d, self._cutoff).swapaxes(1, 2)[:self._cutoff]
+        s = s[:self._cutoff]
 
         self.sv[k] = np.where(s > self._s_min, s, 0)
 
         if k > 0:
             rank = np.nonzero(self.sv[k - 1])[0][-1] + 1
-            self.gamma[k, :rank] = v[:rank] / self.sv[k - 1, :rank][:, np.newaxis, np.newaxis]
-            self.gamma[k, rank:] = 0
+            self._gamma[k, :rank] = v[:rank] / self.sv[k - 1, :rank][:, np.newaxis, np.newaxis]
+            self._gamma[k, rank:] = 0
         else:
-            self.gamma[k] = v
-        if k < self.m - 2:
+            self._gamma[k] = v
+        if k < self._input_state.m - 2:
             rank = np.nonzero(self.sv[k + 1])[0][-1] + 1
-            self.gamma[k + 1, :, :rank] = (w[:, :rank] / self.sv[k + 1, :rank][:, np.newaxis])
-            self.gamma[k + 1, :, rank:] = 0
+            self._gamma[k + 1, :, :rank] = (w[:, :rank] / self.sv[k + 1, :rank][:, np.newaxis])
+            self._gamma[k + 1, :, rank:] = 0
         else:
-            self.gamma[k + 1] = w
+            self._gamma[k + 1] = w
 
     def _transition_matrix(self, u):
         "This function computes the elements (I,J) = (i_k, i_k+1, j_k, j_k+1) of the matrix U_k,k+1."
         d = self.d
         big_u = np.zeros((d,d,d,d), dtype = 'complex_')
         for i1 in range(d):
             for i2 in range(d):
@@ -197,14 +205,14 @@
                             *(u1**k1*u2**k2*u3**(i1-k1)*u4**(i2-k2))\
                             *(np.sqrt(factorial(k1+k2)*factorial(itot-k1-k2)))
 
                 big_u[i1,i2,:] = outputs/(np.sqrt(factorial(i1)*factorial(i2)))
         return big_u
 
     def _sv_diag(self, k):
-        if self.res[self.current_input]["sv"].any():
-            sv = self.res[self.current_input]["sv"]
+        if self._res[self._current_input]["sv"].any():
+            sv = self._res[self._current_input]["sv"]
         else:
             sv = self.sv
-        sv_diag = np.zeros((self.cutoff, self.cutoff))
+        sv_diag = np.zeros((self._cutoff, self._cutoff))
         np.fill_diagonal(sv_diag, sv[k, :])
         return sv_diag
```

### Comparing `perceval-quandela-0.8.1/perceval/backends/naive.py` & `perceval-quandela-0.9.0/perceval/backends/_abstract_backends.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,46 +23,78 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import math
-import numpy as np
+from abc import ABC, abstractmethod
 
-from .template import Backend
-import exqalibur as xq
+from perceval.components import ACircuit
+from perceval.utils import BasicState, BSDistribution, allstate_iterator, StateVector
 
 
-class NaiveBackend(Backend):
-    """Naive algorithm, no clever calculation path, does not cache anything,
-       recompute all states on the fly"""
-    name = "Naive"
-    supports_symbolic = False
-    supports_circuit_computing = False
-
-    def probampli_be(self, input_state, output_state):
-        if input_state.n != output_state.n:
-            return 0
-        Ust = np.empty((input_state.n, input_state.n), dtype=complex)
-        colidx = 0
-        p = 1
-        for ok in range(self._realm):
-            p *= math.factorial(output_state[ok])
-        for ik in range(self._realm):
-            p *= math.factorial(input_state[ik])
-            for i in range(input_state[ik]):
-                rowidx = 0
-                for ok in range(self._realm):
-                    for j in range(output_state[ok]):
-                        Ust[rowidx, colidx] = self._U[ok, ik]
-                        rowidx += 1
-                colidx += 1
-        return xq.permanent_cx(Ust, n_threads=1)/math.sqrt(p)
+class ABackend(ABC):
+    def __init__(self):
+        self._circuit = None
+        self._umat = None
+        self._input_state = None
+
+    def set_circuit(self, circuit: ACircuit):
+        assert not circuit.requires_polarization, "Circuit must not contain polarized components"
+        self._input_state = None
+        self._circuit = circuit
+        self._umat = circuit.compute_unitary()
+
+    def set_input_state(self, input_state: BasicState):
+        self._check_state(input_state)
+        self._input_state = input_state
+
+    def _check_state(self, state: BasicState):
+        assert self._circuit.m == state.m, f'Circuit({self._circuit.m}) and state({state.m}) size mismatch'
+        assert not state.has_annotations, 'State should be composed of indistinguishable photons only'
+
+    @property
+    @abstractmethod
+    def name(self) -> str:
+        """Each backend has to expose its name as a string"""
 
-    def prob_be(self, input_state, output_state):
-        return abs(self.probampli_be(input_state, output_state))**2
+    @staticmethod
+    @abstractmethod
+    def preferred_command() -> str:
+        pass
+
+
+class ASamplingBackend(ABackend):
+    @abstractmethod
+    def sample(self):
+        """Request samples from the circuit given an input state"""
+
+    @staticmethod
+    def preferred_command() -> str:
+        return "sample"
+
+
+class AProbAmpliBackend(ABackend):
+    @abstractmethod
+    def prob_amplitude(self, output_state: BasicState) -> complex:
+        pass
+
+    def probability(self, output_state: BasicState) -> float:
+        return abs(self.prob_amplitude(output_state)) ** 2
+
+    def prob_distribution(self) -> BSDistribution:
+        bsd = BSDistribution()
+        for output_state in allstate_iterator(self._input_state):
+            bsd.add(output_state, self.probability(output_state))
+        return bsd
+
+    def evolve(self) -> StateVector:
+        res = StateVector()
+        for output_state in allstate_iterator(self._input_state):
+            res[output_state] = self.prob_amplitude(output_state)
+        res.normalize()
+        return res
 
     @staticmethod
     def preferred_command() -> str:
-        return 'probampli'
+        return "prob_amplitude"
```

### Comparing `perceval-quandela-0.8.1/perceval/backends/processor/__init__.py` & `perceval-quandela-0.9.0/perceval/utils/algorithms/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from .stepper import StepperBackend
+from .match import Match
+import perceval.utils.algorithms.norm as norm
```

### Comparing `perceval-quandela-0.8.1/perceval/backends/slos.py` & `perceval-quandela-0.9.0/perceval/backends/_slos.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,42 +23,41 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import numpy as np
-import sympy as sp
+from ._abstract_backends import AProbAmpliBackend
+from perceval.utils import allstate_iterator, Matrix, BasicState, BSDistribution, StateVector
 
-from .template import Backend
-from perceval.utils import Matrix, BasicState
 import exqalibur as xq
+import numpy as np
+from typing import Dict, List
 
 
-class ComputePath:
-    """A `ComputePath` is the minimal computing graph for covering a set of input states
-    """
+class _Path:
+    """A `Path` is the minimal computing graph for covering a set of input states"""
 
-    def __init__(self, n, states, targets, backend):
+    def __init__(self, n, m, states, targets, backend):
         self._n = n
+        self._m = m
         self._backend = backend
-        self.coefs = Matrix.zeros((backend.mk_l[n], 1),
-                                  use_symbolic=self._backend.is_symbolic())
+        self.coefs = Matrix.zeros((backend._mk_l[n], 1), use_symbolic=self._backend._symb)
         if n == 0:
             self.coefs.fill(1)
 
         if targets is None:
             targets = [list(state) for state in states]
         self._targets = []
         self._states = []
         self._children = {}
         for t, s in zip(targets, states):
             if sum(t) == 0:
-                backend.state_mapping[s] = self
+                backend._state_mapping[s] = self
             else:
                 self._targets.append(t)
                 self._states.append(s)
         self._decompose()
 
     def _decompose(self):
         targets = self._targets
@@ -77,129 +76,144 @@
                 if one_target[max_index]:
                     one_target[max_index] -= 1
                     current_targets.append(one_target)
                     current_states.append(one_state)
                 else:
                     new_targets.append(one_target)
                     new_states.append(one_state)
-            self._children[max_index] = ComputePath(self._n+1,
-                                                    current_states, current_targets,
-                                                    self._backend)
+            self._children[max_index] = _Path(self._n + 1, self._m,
+                                              current_states, current_targets,
+                                              self._backend)
             targets = new_targets
             states = new_states
 
     def compute(self, u, parent_coefs: Matrix = None, mk: int = None):
         r"""Given the precompiled compute path, update all the coefficients"""
         if parent_coefs is not None:
-            if self._backend._use_symbolic:
+            if self._backend._symb:
                 self.coefs.fill(0)
                 for parent_idx, coef_parent in enumerate(parent_coefs):
-                    for j in range(self._backend._realm):
-                        idx = self._backend.fsms[self._n].get(parent_idx, j)
+                    for j in range(self._m):
+                        idx = self._backend._fsms[self._n].get(parent_idx, j)
                         if idx != xq.npos:
                             self.coefs[idx] += coef_parent * u[j, mk]
             else:
-                self._backend.fsms[self._n].compute_slos_layer(u, self._backend._realm, mk, self.coefs, parent_coefs)
+                self._backend._fsms[self._n].compute_slos_layer(u, self._m, mk, self.coefs, parent_coefs)
 
         for mk, child in self._children.items():
             child.compute(u, self.coefs, mk)
 
 
-class SLOSBackend(Backend):
-    """Strong Linear Optic Simulator"""
-    name = "SLOS"
-    supports_symbolic = True
-    supports_circuit_computing = False
-
-    def __init__(self, u, use_symbolic=None, n=None, mask=None):
-        super().__init__(u, use_symbolic=use_symbolic, n=n, mask=mask)
-        self._compute_path = None
-        self._changed_unitary(None)
-
-    def _changed_unitary(self, prev_u):
-        if self._compute_path is not None and prev_u is not None and prev_u.shape == self._U.shape:
-            self._calculation()
+class SLOSBackend(AProbAmpliBackend):
+    def __init__(self, mask=None, n=None, use_symbolic=False):
+        super().__init__()
+        self._reset()
+        self._symb = use_symbolic
+        self._mask_str = mask
+        self._n = n
+        self._mask = None
+
+    @property
+    def name(self) -> str:
+        return "SLOS"
+
+    def _reset(self):
+        self._fsms = [[]]
+        self._fsas = {}
+        self._mk_l: List[int] = [1]
+        self._path_roots: List[_Path] = []
+        self._state_mapping: Dict[BasicState, _Path] = {}
+        self._mask = None
+
+    def _compute_path(self, umat):
+        for path in self._path_roots:
+            path.compute(umat)
+
+    def set_circuit(self, circuit):
+        previous_circuit = self._circuit
+        assert not circuit.requires_polarization, "Circuit must not contain polarized components"
+        self._input_state = None
+        self._circuit = circuit
+        self._umat = circuit.compute_unitary(use_symbolic=self._symb)
+        if self._path_roots and previous_circuit.m == circuit.m:
+            # Use the previously deployed paths to store the new circuit's coefs
+            self._compute_path(self._umat)
         else:
-            self.mk_l = [1]
-            self.fsms = [[]]
-            self.fsas = {}
-            self._compute_path = None
-            self.state_mapping = {}
+            self._reset()
+            if self._mask_str is not None:
+                assert self._n is not None, "Photon count (n) is required when using a mask"
+                self._mask = xq.FSMask(circuit.m, self._n, self._mask_str)
+
+    def set_input_state(self, input_state: BasicState):
+        self.preprocess([input_state])
+        super().set_input_state(input_state)
 
-    def _compilation(self, input_states):
+    def _deploy(self, input_list: List[BasicState]):
         # allocate the fsas and fsms for covering all the input_states respecting possible mask
         # after calculation, we only need to keep fsa for input_state n
         # during calculation we need to keep current fsa and previous fsa
-        if not self.fsas:
-            current_fsa = xq.FSArray(self._realm, 0)
-        else:
-            current_fsa = self.fsas[max(self.fsas.keys())]
-        for input_state in input_states:
-            if input_state.n < len(self.fsms) and input_state.n not in self.fsas:
+        m = self._circuit.m
+        current_fsa = xq.FSArray(m, 0) if len(self._fsas) == 0 else self._fsas[max(self._fsas.keys())]
+        for input_state in input_list:
+            n = input_state.n
+            if n < len(self._fsms) and n not in self._fsas:
                 # we are missing the intermediate states - let us retrieve/load it back
-                current_fsa = (self._mask and xq.FSArray(self._realm, input_state.n, self._mask)
-                               or xq.FSArray(self._realm, input_state.n))
-            for k in range(len(self.fsms), input_state.n+1):
+                current_fsa = xq.FSArray(m, n, self._mask) if self._mask else xq.FSArray(m, n)
+            for k in range(len(self._fsms), n + 1):
                 fsa_n_m1 = current_fsa
-                if self._mask:
-                    current_fsa = xq.FSArray(self._realm, k, self._mask)
-                else:
-                    current_fsa = xq.FSArray(self._realm, k)
-                self.mk_l.append(current_fsa.count())
-                self.fsms.append(xq.FSMap(current_fsa, fsa_n_m1, True))
-            if input_state.n not in self.fsas:
-                self.fsas[input_state.n] = current_fsa
-
-    def get_mask(self):
-        return self._mask
-
-    def _calculation(self):
-        """
-        Simulation step: update computation path coef with unitary U
-        :return:
-        """
-        self._compute_path.compute(self._U)
-
-    def compile(self, input_states):
-        if isinstance(input_states, BasicState):
-            input_states = [input_states]
-        # build the necessary fsa/fsms
-        self._compilation(input_states)
+                current_fsa = xq.FSArray(m, k, self._mask) if self._mask else xq.FSArray(m, k)
+                self._mk_l.append(current_fsa.count())
+                self._fsms.append(xq.FSMap(current_fsa, fsa_n_m1, True))
+            if n not in self._fsas:
+                self._fsas[n] = current_fsa
+
+    def preprocess(self, input_list: List[BasicState]) -> bool:
         # now check if we have a path for the input states
         found_new = False
-        for input_state in input_states:
+        for input_state in input_list:
+            found_new = (input_state not in self._state_mapping)
             if found_new:
                 break
-            found_new = input_state not in self.state_mapping
         if not found_new:
             return False
-        self._compute_path = ComputePath(0, input_states, None, self)
-        self._calculation()
+
+        self._deploy(input_list)  # build the necessary fsa/fsms
+        new_path = _Path(0, self._circuit.m, input_list, None, self)
+        new_path.compute(self._umat)
+        self._path_roots.append(new_path)
         return True
 
-    def probampli_be(self, input_state, output_state, norm=True):
-        if input_state.n != output_state.n:
-            return 0
-        output_idx = self.fsas[output_state.n].find(output_state)
+    def prob_amplitude(self, output_state: BasicState) -> complex:
+        if self._input_state.n != output_state.n:
+            return complex(0)
+        output_idx = self._fsas[output_state.n].find(output_state)
         assert output_idx != xq.npos
-        non_normalized_result = self.state_mapping[input_state].coefs[output_idx, 0]
-        if not norm:
-            return non_normalized_result
-        if self._use_symbolic:
-            return non_normalized_result * sp.sqrt(output_state.prodnfact()/input_state.prodnfact())
-        else:
-            return non_normalized_result * np.sqrt(output_state.prodnfact()/input_state.prodnfact())
+        non_normalized_result = self._state_mapping[self._input_state].coefs[output_idx, 0]
+        return non_normalized_result * np.sqrt(output_state.prodnfact() / self._input_state.prodnfact())
 
-    def prob_be(self, input_state, output_state):
-        return abs(self.probampli_be(input_state, output_state, False))**2\
-               * output_state.prodnfact()/input_state.prodnfact()
-
-    # The following SLOS-specific optimization is broken for polarized states/circuits
-    # def all_prob(self, input_state):
-    #     self.compile(input_state)
-    #     c = np.copy(self.state_mapping[input_state].coefs).reshape(self.fsas[input_state.n].count())
-    #     self.fsas[input_state.n].norm_coefs(c)
-    #     return abs(c)**2 / input_state.prodnfact()
-
-    @staticmethod
-    def preferred_command() -> str:
-        return 'probampli'
+    def prob_distribution(self) -> BSDistribution:
+        istate = self._input_state
+        c = np.copy(self._state_mapping[istate].coefs).reshape(self._fsas[istate.n].count())
+        bsd = BSDistribution()
+        iprodnfact = istate.prodnfact()
+        for output_state, unnormed_pa in zip(allstate_iterator(self._input_state, self._mask), c):
+            bsd.add(output_state, (abs(unnormed_pa) ** 2) * output_state.prodnfact() / iprodnfact)
+        return bsd
+
+    def all_prob(self, input_state: BasicState):
+        """SLOS specific signature, to enhance optimization in some computations"""
+        self.set_input_state(input_state)
+        c = np.copy(self._state_mapping[self._input_state].coefs).reshape(self._fsas[self._input_state.n].count())
+        c = abs(c)**2 / self._input_state.prodnfact()
+        for idx, (output_state, _) in enumerate(zip(allstate_iterator(self._input_state, self._mask), c)):
+            c[idx] = c[idx] * output_state.prodnfact()
+        return c
+
+    def evolve(self) -> StateVector:
+        istate = self._input_state
+        c = np.copy(self._state_mapping[istate].coefs).reshape(self._fsas[istate.n].count())
+        res = StateVector()
+        iprodnfact = istate.prodnfact()
+        for output_state, pa in zip(allstate_iterator(self._input_state, self._mask), c):
+            res[output_state] = pa * np.sqrt(output_state.prodnfact() / iprodnfact)
+        res.normalize()
+        return res
```

### Comparing `perceval-quandela-0.8.1/perceval/backends/template.py` & `perceval-quandela-0.9.0/perceval/simulators/simulator.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,340 +22,322 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+from ._simulator_utils import _to_bsd, _inject_annotation, _merge_sv, _annot_state_mapping
+from .simulator_interface import ISimulator
+from perceval.components import ACircuit
+from perceval.utils import BasicState, BSDistribution, StateVector, SVDistribution, PostSelect, global_params
+from perceval.backends import AProbAmpliBackend
+
+from copy import copy
+from multipledispatch import dispatch
+from numbers import Number
+from typing import Callable, Set, Union, Optional
+
+
+class Simulator(ISimulator):
+    """
+    A simulator class relying on a probability amplitude capable backend to simulate the output of a unitary
+    non-polarized circuit given an BasicState, StateVector or SVDistribution input. The simulator is able to evolve
+    or simulate the sampling a states with annotated photons.
+
+    :param backend: A probability amplitude capable backend object
+    """
+
+    def __init__(self, backend: AProbAmpliBackend):
+        self._backend = backend
+        self._invalidate_cache()
+        self._postselect: PostSelect = PostSelect()
+        self._logical_perf: float = 1
+        self._physical_perf: float = 1
+        self._rel_precision: float = 1e-6  # Precision relative to the highest probability of interest in probs_svd
+        self._min_detected_photons: int = 0
 
-from abc import ABC, abstractmethod
-import logging
-import random
-from typing import List, Tuple, Union, Iterator, Optional
-
-from perceval.utils import Matrix, StateVector, BasicState
-from perceval.utils.statevector import convert_polarized_state, build_spatial_output_states
-from ..components.linear_circuit import ACircuit, _matrix_double_for_polarization
-
-import exqalibur as xq
-import numpy as np
-
-
-class Backend(ABC):
-    name = None
-    supports_symbolic = None
-    supports_circuit_computing = None
-
-    def __init__(self,
-                 cu: Union[ACircuit, Matrix],
-                 use_symbolic: bool = None,
-                 use_polarization: Optional[bool] = None,
-                 n: int = None,
-                 mask: list = None):
-        r"""
-        :param cu: a circuit to simulate or a unitary Matrix symbolic or numeric
-        :param use_symbolic: define if calculation should be symbolic or numeric:
-            - None: decides based on U nature and backend capacity
-            - True: calculation will be symbolic
-            - False: calculation will be numeric
-        :param n: expected number of input photons, necessary for applying masks
-        :param mask: a mask for output states that we are interested in
-        """
-        self._logger = logging.getLogger(self.name)
-        if not self.supports_circuit_computing:
-            if isinstance(cu, ACircuit):
-                if cu.requires_polarization:
-                    if use_polarization is None:
-                        use_polarization = True
-                    else:
-                        assert use_polarization, "use polarization can not be False for circuit with polarization"
-                elif use_polarization is None:
-                    use_polarization = False
-                u = cu.compute_unitary(use_symbolic, use_polarization=use_polarization)
-            else:
-                if use_polarization is None:
-                    use_polarization = False
-                u = cu
-                assert u.ndim == 2 and u.shape[0] == u.shape[1], "simulator works on square matrix"
-            self._requires_polarization = use_polarization
-            self._C = None
-            if not self.supports_symbolic:
-                if not u.defined or use_symbolic:
-                    assert not u.is_symbolic, "%s backend does not support symbolic calculation" % self.name
-                if not use_symbolic:
-                    self._U = u.tonp()
-            else:
-                if use_symbolic and not u.is_symbolic:
-                    self._U = Matrix(u, use_symbolic=True)
-                elif use_symbolic is False and u.is_symbolic:
-                    self._U = u.tonp()
-                else:
-                    use_symbolic = u.is_symbolic()
-                    self._U = u
-            self._realm: int = u.shape[0]
-            self._m: int = self._requires_polarization and u.shape[0] >> 1 or u.shape[0]
-            "number of modes"
-        else:
-            assert isinstance(cu, ACircuit), \
-                "Component Based simulation works on circuit"
-            assert not use_symbolic or self.supports_symbolic, \
-                "%s backend does not support symbolic calculation" % self.name
-            # component based simulation - we keep the circuit
-            self._U = None
-            self._C = cu
-            self._m = self._realm = cu.m
-
-        self._use_symbolic = use_symbolic
-        self._n: int = n  # number of photons - is required when using a mask
-
-        self._mask = None
-        if mask is not None:
-            assert n is not None, "number of photons required when using a mask"
-            self._mask = xq.FSMask(self._m, n, mask)
+    @property
+    def precision(self):
+        return self._rel_precision
 
-        self._compiled_input = None
+    @precision.setter
+    def precision(self, value: float):
+        assert isinstance(value, Number) and value >= 0., "Precision must be a positive number"
+        self._rel_precision = value
 
-    def _changed_unitary(self, prev_u) -> None:
-        """Notify change of unitary - might be used for backend with compiled states
+    def set_min_detected_photon_filter(self, value: int):
         """
-        return
+        Set a minimum number of detected photons in the output distributions
 
-    @property
-    def is_symbolic(self):
-        return self._U.is_symbolic
+        :param value: The minimum photon count
+        """
+        self._min_detected_photons = value
 
     @property
-    def m(self):
-        return self._m
+    def logical_perf(self):
+        return self._logical_perf
 
-    @property
-    def U(self):
-        return self._U
+    def set_postselection(self, postselect: PostSelect):
+        """Set a post-selection function
 
-    @U.setter
-    def U(self, u):
-        prev_u = self._U
-        self._U = u
-        self._changed_unitary(prev_u)
-
-    def _check_state_size(self, state: BasicState):
-        if self.m != state.m:
-            raise ValueError(
-                f'State/circuit size mismatch: circuit({self._m}) and state({state.m}) should be the same size')
-
-    @abstractmethod
-    def prob_be(self, input_state, output_state):
-        pass
-
-    @abstractmethod
-    def probampli_be(self, input_state, output_state):
-        pass
-
-    def prob(self,
-             input_state: BasicState,
-             output_state: BasicState,
-             skip_compile: bool = False
-             ) -> float:
-        r"""
-        gives the probability of an output state given an input state
-        :param input_state: the input state
-        :param output_state: the output state
-        :return: float probability
+        :param postselect: a PostSelect object
         """
-        self._check_state_size(input_state)
-        self._check_state_size(output_state)
-        if input_state.n == 0:
-            return 1 if output_state.n == 0 else 0
-        if self._U is None or (not self._requires_polarization and not input_state.has_polarization):
-            if input_state.has_annotations:
-                input_states = input_state.separate_state()
-                all_prob = 0
-                for p_output_state in BasicState(output_state).partition(
-                        [input_state.n for input_state in input_states]):
-                    prob = 1
-                    for i_state, o_state in zip(input_states, p_output_state):
-                        if not skip_compile:
-                            self.compile(i_state)
-                        prob *= self.prob_be(i_state, o_state)
-                    all_prob += prob
-                return all_prob
-            if not skip_compile:
-                self.compile(input_state)
-            return self.prob_be(input_state, output_state)
-        spatial_mode_input_state, prep_matrix_input = convert_polarized_state(input_state)
-        _U_ref = self._U
-        _realm_ref = self._realm
-        if not self._requires_polarization:
-            _U_new = _matrix_double_for_polarization(self._m, self._U)
-            self._realm = 2 * self._realm
-        else:
-            _U_new = self._U
-        _U_new = _U_new @ prep_matrix_input
-        if isinstance(output_state, BasicState) and output_state.has_polarization:
-            # if output state is polarized, we will directly compute probabilities for it
-            spatial_mode_output_state, un_prep_matrix_output = convert_polarized_state(output_state, inverse=True)
-            self.U = un_prep_matrix_output @ _U_new
-            self.compile(spatial_mode_input_state)
-            prob = self.prob_be(spatial_mode_input_state, spatial_mode_output_state)
-        else:
-            # for each polarized mode with k photons, we have to calculate probabilities on the spatial mode, ies all
-            # |m,l> for m+l = k
-            self.U = _U_new
-            self.compile(spatial_mode_input_state)
-            prob = 0
-            for spatial_output in build_spatial_output_states(output_state):
-                prob += self.prob_be(spatial_mode_input_state, spatial_output)
-        self._U = _U_ref
-        self._realm = _realm_ref
-        return prob
-
-    def all_prob(self, input_state: BasicState) -> np.ndarray:
-        allprobs = []
-        for (output, prob_output) in self.allstateprob_iterator(input_state):
-            allprobs.append(prob_output)
-        return np.asarray(allprobs)
-
-    def probampli(self,
-                  input_state: BasicState,
-                  output_state: BasicState,
-                  ) -> complex:
-        """Gives the probability amplitude of an output state given an input state
-
-        :param input_state: the input state
-        :param output_state: the output state
-        :return: complex probability amplitude
+        self._postselect = postselect
+
+    def clear_postselection(self):
+        """Clear the post-selection function"""
+        self._postselect = PostSelect()
+
+    def set_circuit(self, circuit: ACircuit):
+        """Set a circuit for simulation.
+
+        :param circuit: a unitary circuit without polarized components
+        """
+        self._invalidate_cache()
+        self._backend.set_circuit(circuit)
+
+    @dispatch(BasicState, BasicState)
+    def prob_amplitude(self, input_state: BasicState, output_state: BasicState) -> complex:
+        """Compute the probability amplitude of an output fock state versus an input fock state.
+
+        :param input_state: A fock state with or without photon annotations
+        :param output_state: A fock state with or without photon annotations. If the input state holds annotations,
+            the output state must hold the same ones, otherwise the computed probability amplitude is 0.
+
+            >>> simulator.set_circuit(Circuit(1))  # One mode identity
+            >>> simulator.prob_amplitude(BasicState('|{_:0}>'), BasicState('|{_:1}>'))
+            0
+            >>> simulator.prob_amplitude(BasicState('|{_:0}>'), BasicState('|{_:0}>'))
+            1
+
+        :return: The complex probability amplitude
         """
-        self._check_state_size(input_state)
-        self._check_state_size(output_state)
         if input_state.n == 0:
             return complex(1) if output_state.n == 0 else complex(0)
-        if self._U is None or (not self._requires_polarization and not input_state.has_polarization):
-            self.compile(input_state)
-            return self.probampli_be(input_state, output_state)
-        spatial_mode_input_state, prep_matrix_input = convert_polarized_state(input_state)
-        _U_ref = self._U
-        _realm_ref = self._realm
-        if not self._requires_polarization:
-            self._U = _matrix_double_for_polarization(self._m, self._U)
-            self._realm = 2 * self._realm
-        self.compile(spatial_mode_input_state)
-        self._U = self._U @ prep_matrix_input
-        if output_state.has_polarization:
-            # if output state is polarized, we will directly calculate probabilities for it
-            spatial_mode_output_state, un_prep_matrix_output = convert_polarized_state(output_state, inverse=True)
-            self._U = un_prep_matrix_output @ self._U
-            prob_ampli = self.probampli_be(spatial_mode_input_state, spatial_mode_output_state)
-        else:
-            # for each polarized mode with k photons, we have to calculate probabilities on the spatial mode, ies all
-            # |m,l> for m+l = k
-            prob_ampli = 0
-            for spatial_output in build_spatial_output_states(output_state):
-                prob_ampli += self.probampli_be(spatial_mode_input_state, spatial_output)
-        self._U = _U_ref
-        self._realm = _realm_ref
-        return prob_ampli
-
-    def allstateprob_iterator(self,
-                              input_state: Union[BasicState, StateVector]) \
-            -> Iterator[Tuple[BasicState, float]]:
-        """Iterator on all possible output states compatibles with mask generating (`StateVector`, probability)
-
-        :param input_state: a given input state
-        :return: list of (output_state, probability)
-        """
-        skip_compile = False
-        for output_state in self.allstate_iterator(input_state):
-            if isinstance(input_state, StateVector) and len(input_state) > 1:
-                # a superposed state cannot have distinguishable particles
-                probampli = 0
-                sv = input_state
-                for inp_state in sv:
-                    probampli += self.probampli(inp_state, output_state) * sv[inp_state]
-                yield output_state, abs(probampli) ** 2
-            else:
-                # TODO: should not have a special case here
-                if isinstance(input_state, StateVector):
-                    input_state = input_state[0]
-                yield output_state, self.prob(input_state, output_state, skip_compile=skip_compile)
-                skip_compile = True
-
-    def allstate_iterator(self, input_state: Union[BasicState, StateVector]) -> BasicState:
-        """Iterator on all possible output states compatible with mask generating StateVector
-
-        :param input_state: a given input state (basic or superposed)
-        :return: the next output state
-        """
-        m = self.m
-        ns = input_state.n
-        if not isinstance(ns, list):
-            ns = [ns]
-        for n in ns:
-            if self._mask:
-                output_array = xq.FSArray(m, n, self._mask)
+        input_map = _annot_state_mapping(input_state)
+        output_map = _annot_state_mapping(output_state)
+        if len(input_map) != len(output_map):
+            return complex(0)
+        probampli = 1
+        for annot, in_s in input_map.items():
+            if annot not in output_map:
+                return complex(0)
+            self._backend.set_input_state(in_s)
+            probampli *= self._backend.prob_amplitude(output_map[annot])
+        return probampli
+
+    @dispatch(StateVector, BasicState)
+    def prob_amplitude(self, input_state: StateVector, output_state: BasicState) -> complex:
+        result = complex(0)
+        for state, pa in input_state.items():
+            result += self.prob_amplitude(state, output_state) * pa
+        return result
+
+    @dispatch(BasicState, BasicState)
+    def probability(self, input_state: BasicState, output_state: BasicState) -> float:
+        """Compute the probability of an output fock state versus an input fock state, simulating a measure.
+
+        :param input_state: A fock state with or without photon annotations
+        :param output_state: A fock state, annotations are ignored
+        :return: The probability (float between 0 and 1)
+        """
+        if input_state.n == 0:
+            return 1 if output_state.n == 0 else 0
+        input_list = input_state.separate_state(keep_annotations=False)
+        result = 0
+        for p_output_state in output_state.partition(
+                [input_state.n for input_state in input_list]):
+            prob = 1
+            for i_state, o_state in zip(input_list, p_output_state):
+                self._backend.set_input_state(i_state)
+                prob *= self._backend.probability(o_state)
+            result += prob
+        return result
+
+    @dispatch(StateVector, BasicState)
+    def probability(self, input_state: StateVector, output_state: BasicState) -> float:
+        output_state.clear_annotations()
+        sv_out = self.evolve(input_state)  # This is not as optimized as it could be
+        result = 0
+        for state, pa in sv_out.items():
+            state.clear_annotations()
+            if state == output_state:
+                result += abs(pa) ** 2
+        return result
+
+    def _invalidate_cache(self):
+        self._evolve = {}
+        self._probd = {}
+        self.DEBUG_evolve_count = 0
+        self.DEBUG_merge_count = 0
+
+    def _evolve_cache(self, input_list: Set[BasicState]):
+        for state in input_list:
+            if state not in self._evolve:
+                self._backend.set_input_state(state)
+                self._evolve[state] = self._backend.evolve()
+                self.DEBUG_evolve_count += 1
+
+    def _probs_cache(self, input_list: Set[BasicState]):
+        for state in input_list:
+            if state not in self._probd:
+                self._backend.set_input_state(state)
+                self._probd[state] = self._backend.prob_distribution()
+                self.DEBUG_evolve_count += 1
+
+    def _merge_probability_dist(self, input_list) -> BSDistribution:
+        results = BSDistribution()
+        for input_state in input_list:
+            results = BSDistribution.tensor_product(results, _to_bsd(self._evolve[input_state]), merge_modes=True)
+            self.DEBUG_merge_count += 1
+        return results
+
+    def _post_select_on_distribution(self, bsd: BSDistribution) -> BSDistribution:
+        self._logical_perf = 1
+        if not self._postselect.has_condition:
+            bsd.normalize()
+            return bsd
+        result = BSDistribution()
+        for state, prob in bsd.items():
+            if self._postselect(state):
+                result[state] = prob
             else:
-                output_array = xq.FSArray(m, n)
-            for output_state in output_array:
-                yield BasicState(output_state)
-
-    def evolve(self, input_state: [BasicState, StateVector]) -> StateVector:
-        r"""StateVector evolution through a circuit
-
-        :param input_state: the input_state
-        :return: the output_state
-        """
-        output_state = StateVector(None)
-        for basic_output_state in self.allstate_iterator(input_state):
-            if isinstance(input_state, StateVector):
-                sv = input_state
-                for inp_state in sv:
-                    output_state[basic_output_state] += self.probampli(inp_state, basic_output_state) * sv[inp_state]
+                self._logical_perf -= prob
+        result.normalize()
+        return result
+
+    @dispatch(BasicState)
+    def probs(self, input_state: BasicState) -> BSDistribution:
+        """
+        Compute the probability distribution from a state input
+        :param input_state: The input fock state or state vector
+        :return: The post-selected output state distribution (BSDistribution)
+        """
+        input_list = input_state.separate_state(keep_annotations=False)
+        self._evolve_cache(set(input_list))
+        result = self._merge_probability_dist(input_list)
+        return self._post_select_on_distribution(result)
+
+    @dispatch(StateVector)
+    def probs(self, input_state: StateVector) -> BSDistribution:
+        if len(input_state) == 1:
+            return self.probs(input_state[0])
+        return self._post_select_on_distribution(_to_bsd(self.evolve(input_state)))
+
+    def probs_svd(self, input_dist: SVDistribution, progress_callback: Optional[Callable] = None):
+        """
+        Compute the probability distribution from a SVDistribution input and as well as performance scores
+
+        :param input_dist: A state vector distribution describing the input to simulate
+        :param progress_callback: A function with the signature `func(progress: float, message: str)`
+
+        :return: A dictionary of the form { "results": BSDistribution, "physical_perf": float, "logical_perf": float }
+        * results is the post-selected output state distribution
+        * physical_perf is the performance computed from the detected photon filter
+        * logical_perf is the performance computed from the post-selection
+        """
+
+        """Trim input SVD given _rel_precision threshold"""
+        max_p = 0
+        for sv, p in input_dist.items():
+            if max(sv.n) >= self._min_detected_photons:
+                max_p = p
+                break
+        p_threshold = max(global_params['min_p'], max_p * self._rel_precision)
+        svd = SVDistribution({state: pr for state, pr in input_dist.items() if pr > p_threshold})
+
+        """decomposed input:
+        From a SVD = {
+            pa_11*bs_11 + ... + pa_n1*bs_n1: p1,
+            pa_12*bs_12 + ... + pa_n2*bs_n2: p2,
+            ...
+            pa_1k*bs_1k + ... + pa_nk*bs_nk: pk
+        }
+        the following data structure is built:
+        [
+            (p1, [
+                    (pa_11, [bs_11,]),
+                    ...
+                    (pa_n1, [bs_n1,])
+                 ]
+            ),
+            (pk, [
+                    (pa_1k, [bs_1k,]),
+                    ...
+                    (pa_nk, [bs_nk,])
+                 ]
+            )
+        ]
+        where [bs_xy,] is the list of the un-annotated separated basic state (bs_xy.separate_state())
+        """
+        decomposed_input = []
+        for sv, prob in svd.items():
+            if min(sv.n) >= self._min_detected_photons:
+                decomposed_input.append((prob, [(abs(pa)**2, st.separate_state(keep_annotations=False)) for st, pa in sv.items()]))
             else:
-                output_state[basic_output_state] += self.probampli(input_state, basic_output_state)
-        output_state.normalize()
-        return output_state
-
-    def compile(self, input_states: Union[StateVector, List[StateVector]]) -> bool:
-        """
-        Compile a simulator to work with one or specific input_states - might do nothing for some backends
-        :param input_states: list of input states
-        :return: True if any compilation happened, False otherwise
-        """
-        return False
-
-    def sample(self, input_state: Union[BasicState, StateVector]) -> BasicState:
-        r"""Return one sample for the circuit according to the output probability distribution given an input state
-        """
-        prob = random.random()
-        output_state = None
-        for (output_state, state_prob) in self.allstateprob_iterator(input_state):
-            if state_prob >= prob:
-                return output_state
-            prob -= state_prob
-        return output_state
-
-    def samples(self, input_state: Union[BasicState, StateVector], count: int) -> List[BasicState]:
-        r"""Return samples for the circuit according to the output probability distribution given an input state
-
-        :param input_state: a given input state
-        :param count: the number of returned samples
-        """
-        if count == 1:  # Faster in this case
-            return [self.sample(input_state)]
-        states, p = zip(*self.allstateprob_iterator(input_state))
-        rng = np.random.default_rng()
-        results = rng.choice(states, count, p=np.array(p) / sum(p))
-        return list(results)
-
-    def set_cutoff(self, cutoff: int):
-        r"""
-        Set the cutoff dimension for the MPS simulator.
-        """
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def preferred_command() -> str:
-        pass
-
-    @staticmethod
-    def available_commands() -> List[str]:
-        return ['prob', 'prob_be', 'probampli', 'probampli_be', 'sample', 'samples', 'evolve']
+                self._physical_perf -= prob
+        input_set = set([state for s in decomposed_input for t in s[1] for state in t[1]])
+        self._probs_cache(input_set)
+
+        """Reconstruct output probability distribution"""
+        res = BSDistribution()
+        for idx, (prob0, sv_data) in enumerate(decomposed_input):
+            """First, recombine evolved state vectors given a single input"""
+            result_bsd = BSDistribution()
+            for probampli, instate_list in sv_data:
+                prob_sv = abs(probampli)**2
+                evolved_in_s = BSDistribution()
+                for in_s in instate_list:
+                    evolved_in_s = BSDistribution.tensor_product(evolved_in_s, self._probd[in_s],
+                                                                 merge_modes=True,
+                                                                 prob_threshold=p_threshold/(prob_sv*prob0))
+                    self.DEBUG_merge_count += 1
+                for bs, p in evolved_in_s.items():
+                    result_bsd[bs] += prob_sv*p
+
+            """Then, add the resulting distribution the """
+            for bs, p in result_bsd.items():
+                res[bs] += p*prob0
+
+            if progress_callback:
+                exec_request = progress_callback((idx + 1) / len(decomposed_input), 'probs')
+                if exec_request is not None and 'cancel_requested' in exec_request and exec_request['cancel_requested']:
+                    raise RuntimeError("Cancel requested")
+        return {'results': self._post_select_on_distribution(res),
+                'physical_perf': self._physical_perf,
+                'logical_perf': self._logical_perf}
+
+    def evolve(self, input_state: Union[BasicState, StateVector]) -> StateVector:
+        """
+        Evolve a state through the circuit
+
+        :param input_state: The input fock state or state vector
+        :return: The output state vector
+        """
+        if not isinstance(input_state, StateVector):
+            input_state = StateVector(input_state)
+
+        # Decay input to a list of basic states without annotations and evolve each of them
+        decomposed_input = [(pa, st.separate_state(keep_annotations=True)) for st, pa in input_state.items()]
+        input_list = [copy(state) for t in decomposed_input for state in t[1]]
+        for state in input_list:
+            state.clear_annotations()
+        self._evolve_cache(set(input_list))
+
+        result_sv = StateVector()
+        for probampli, instate_list in decomposed_input:
+            reslist = []
+            for in_s in instate_list:
+                annotation = in_s.get_photon_annotation(0)
+                in_s.clear_annotations()
+                reslist.append(_inject_annotation(self._evolve[in_s], annotation))
+
+            # Recombine results for one basic state input
+            evolved_in_s = reslist.pop(0)
+            for sv in reslist:
+                evolved_in_s = _merge_sv(evolved_in_s, sv)
+                self.DEBUG_merge_count += 1
+            result_sv += evolved_in_s * probampli
+
+        result_sv.normalize()
+        return result_sv
```

### Comparing `perceval-quandela-0.8.1/perceval/components/__init__.py` & `perceval-quandela-0.9.0/perceval/components/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,14 @@
 from .abstract_component import AComponent
 from .abstract_processor import AProcessor
 from .linear_circuit import Circuit, ACircuit
 from .predefined_circuit import PredefinedCircuit
 from .processor import Processor
 from .source import Source
 
-from .port import Port, Herald, Encoding, PortLocation, LogicalState
-from .unitary_components import *
+from .port import Port, Herald, PortLocation, LogicalState
+from .unitary_components import BSConvention, BS, PS, WP, HWP, QWP, PR, Unitary, PERM, PBS
 from .non_unitary_components import TD, LC
 from .component_catalog import Catalog
 from ._mode_connector import ModeConnector, UnavailableModeException
 
 catalog = Catalog('perceval.components.core_catalog')
```

### Comparing `perceval-quandela-0.8.1/perceval/components/_mode_connector.py` & `perceval-quandela-0.9.0/perceval/components/_mode_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         super().__init__(f"Invalid mapping ({mapping}){because}")
 
 
 class ModeConnector:
     """
     Resolves a mapping supporting multiple syntaxes in order to connect two objects.
     The left object must be a Processor
-    The right object can be a Processor, a (linear or non-linear) component
+    The right object can be a Processor, a (unitary or non-unitary) component
     """
 
     def __init__(self, left_processor, right_obj, mapping):
         self._lp = left_processor
         self._ro = right_obj  # Can either be a component or a processor
         self._r_is_component = isinstance(right_obj, AComponent)  # False means it is a Processor
         self._map = mapping
```

### Comparing `perceval-quandela-0.8.1/perceval/components/abstract_component.py` & `perceval-quandela-0.9.0/perceval/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/components/abstract_processor.py` & `perceval-quandela-0.9.0/perceval/components/abstract_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,20 +25,21 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from abc import ABC, abstractmethod
 import copy
+from deprecated import deprecated
 from enum import Enum
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Union, Callable
 
 from perceval.components.linear_circuit import Circuit, ACircuit
 from ._mode_connector import ModeConnector, UnavailableModeException
-from perceval.utils import BasicState, StateVector, SVDistribution, Parameter
+from perceval.utils import BasicState, SVDistribution, Parameter, PostSelect
 from .port import LogicalState, Herald, PortLocation, APort
 from .abstract_component import AComponent
 from .unitary_components import PERM, Unitary
 from .non_unitary_components import TD
 from .source import Source
 from perceval.utils.algorithms.simplification import perm_compose, simplify
 
@@ -58,15 +59,15 @@
         self._min_detected_photons = None
 
         self._reset_circuit()
 
     def _reset_circuit(self):
         self._in_ports: Dict = {}
         self._out_ports: Dict = {}
-        self._postprocess = None
+        self._postselect: PostSelect = None
 
         self._is_unitary: bool = True
         self._has_td: bool = False
 
         self._n_heralds: int = 0
         self._anon_herald_num: int = 0  # This is not a herald count!
         self._components: List[AComponent] = []  # Any type of components, not only unitary ones
@@ -99,14 +100,19 @@
 
     def clear_parameters(self):
         self._parameters = {}
 
     def clear_input_and_circuit(self):
         self._reset_circuit()
         self._input_state = None
+        self._circuit_changed()
+
+    def _circuit_changed(self):
+        # Can be used by child class
+        pass
 
     def min_detected_photons_filter(self, n: int):
         r"""
         Sets-up a state post-selection on the number of detected photons. With thresholded detectors, this will
         actually filter on "click" count.
 
         :param n: Minimum expected photons
@@ -135,38 +141,47 @@
             if k > 0 and self.is_threshold:
                 k = 1
             new_state.append(k)
         return BasicState(new_state)
 
     @property
     def post_select_fn(self):
-        return self._postprocess
+        return self._postselect
+
+    @deprecated(version="0.9", reason="use set_postselection(PostSelect) instead")
+    def set_postprocess(self, postprocess_func: Callable):  # Deprecated in order to avoid free Python function
+        self._postselect = postprocess_func
 
-    def set_postprocess(self, postprocess_func):
+    def set_postselection(self, postselect: PostSelect):
         r"""
         Set a logical post-selection function. Along with the heralded modes, this function has an impact
         on the logical performance of the processor
 
-        :param postprocess_func: Sets a post-selection function. Its signature must be `func(s: BasicState) -> bool`.
+        :param postselect: Sets a post-selection function. Its signature must be `func(s: BasicState) -> bool`.
             If None is passed as parameter, removes the previously defined post-selection function.
         """
-        self._postprocess = postprocess_func
+        assert isinstance(postselect, PostSelect), "Parameter must be a PostSelect object"
+        self._postselect = postselect
 
+    @deprecated(version="0.9", reason="use clear_postselection() instead")
     def clear_postprocess(self):
-        self._postprocess = None
+        self.clear_postselection()
+
+    def clear_postselection(self):
+        self._postselect = None
 
     def _state_selected(self, state: BasicState) -> bool:
         """
         Computes if the state is selected given heralds and post selection function
         """
         for m, v in self.heralds.items():
             if state[m] != v:
                 return False
-        if self._postprocess is not None:
-            return self._postprocess(state)
+        if self._postselect is not None:
+            return self._postselect(state)
         return True
 
     def copy(self, subs: Union[dict, list] = None):
         new_proc = copy.deepcopy(self)
         new_proc._components = []
         for r, c in self._components:
             new_proc._components.append((r, c.copy(subs=subs)))
@@ -208,15 +223,15 @@
         Example:
 
         >>> p = Processor("SLOS", 6)
         >>> p.add(0, BS())  # Modes (0, 1) connected to (0, 1) of the added beam splitter
         >>> p.add([2,5], BS())  # Modes (2, 5) of the processor's output connected to (0, 1) of the added beam splitter
         >>> p.add({2:0, 5:1}, BS())  # Same as above
         """
-        if self._postprocess is not None:
+        if self._postselect is not None:
             raise RuntimeError("Cannot add any component to a processor with a post-process function. You may remove the post-process function by calling clear_postprocess()")
 
         self._simulator = None  # Invalidate simulator which will have to be recreated later on
         if self._n_moi is None:
             if isinstance(mode_mapping, int):
                 self._n_moi = (component.m if isinstance(component, ACircuit) else component.circuit_size) + mode_mapping
             else:
@@ -224,14 +239,15 @@
         connector = ModeConnector(self, component, mode_mapping)
         if isinstance(component, AProcessor):
             self._compose_processor(connector, component, keep_port)
         elif isinstance(component, AComponent):
             self._add_component(connector.resolve(), component)
         else:
             raise RuntimeError(f"Cannot add {type(component)} object to a Processor")
+        self._circuit_changed()
         return self
 
     def _compose_processor(self, connector, processor, keep_port: bool):
         self._is_unitary = self._is_unitary and processor._is_unitary
         self._has_td = self._has_td or processor._has_td
         mode_mapping = connector.resolve()
         if not keep_port:
@@ -274,22 +290,20 @@
             if isinstance(port, Herald):
                 self._add_herald(port_mode, port.expected, port.user_given_name)
             else:
                 if self.are_modes_free(range(port_mode, port_mode + port.m)):
                     self.add_port(port_mode, port, PortLocation.OUTPUT)
 
         # Retrieve post process function from the other processor
-        if processor._postprocess is not None:
+        if processor._postselect is not None:
             if perm_component is None:
-                self._postprocess = processor._postprocess
+                self._postselect = processor._postselect
             else:
-                perm = perm_component.perm_vector
                 c_first = perm_modes[0]
-                self._postprocess = lambda s: processor._postprocess([s[perm.index(ii) + c_first]
-                                                                      for ii in range(processor.circuit_size)])
+                self._postselect = processor._postselect.apply_permutation(perm_inv.perm_vector, c_first)
 
     def _add_component(self, mode_mapping, component):
         perm_modes, perm_component = ModeConnector.generate_permutation(mode_mapping)
         if perm_component is not None:
             self._components.append((perm_modes, perm_component))
 
         sorted_modes = list(range(min(mode_mapping), min(mode_mapping)+component.m))
@@ -489,14 +503,18 @@
                 pos[port_range[0]] = port.expected
         return pos
 
     def _with_logical_input(self, input_state: LogicalState):
         input_state = input_state.to_basic_state(list(self._in_ports.keys()))
         self.with_input(input_state)
 
+    @abstractmethod
+    def check_input(self, input_state: BasicState):
+        r"""Check if a basic state input matches with the current processor configuration"""
+
     @property
     def source_distribution(self) -> Union[SVDistribution, None]:
         r"""
         Retrieve the computed input distribution.
         :return: the input SVDistribution if `with_input` was called previously, otherwise None.
         """
         return self._inputs_map
```

### Comparing `perceval-quandela-0.8.1/perceval/components/component_catalog.py` & `perceval-quandela-0.9.0/perceval/components/component_catalog.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/components/computation/__init__.py` & `perceval-quandela-0.9.0/perceval/utils/globals.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,8 +23,11 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from .time_delays import count_TD, count_independant_TD, expand_TD
+global_params = {
+    "min_p": 1e-16,
+    "min_complex_component": 1e-6
+}
```

### Comparing `perceval-quandela-0.8.1/perceval/components/core_catalog/__init__.py` & `perceval-quandela-0.9.0/perceval/components/core_catalog/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,10 +25,11 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .heralded_cnot import HeraldedCnotItem
 from .postprocessed_cnot import PostProcessedCnotItem
+from .heralded_cz import HeraldedCzItem
 from .generic_2mode import Generic2ModeItem
 
-catalog = [HeraldedCnotItem, PostProcessedCnotItem, Generic2ModeItem]
+catalog = [HeraldedCnotItem, PostProcessedCnotItem, HeraldedCzItem, Generic2ModeItem]
```

### Comparing `perceval-quandela-0.8.1/perceval/components/core_catalog/generic_2mode.py` & `perceval-quandela-0.9.0/perceval/components/core_catalog/generic_2mode.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/components/core_catalog/heralded_cnot.py` & `perceval-quandela-0.9.0/perceval/components/core_catalog/postprocessed_cnot.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,58 +26,50 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from perceval.components import Circuit, Processor
 from perceval.components.unitary_components import *
 from perceval.components.component_catalog import CatalogItem, AsType
-from perceval.components.port import Herald, Port, Encoding
+from perceval.components.port import Port
+from perceval.utils import Encoding, PostSelect
 
 
-class HeraldedCnotItem(CatalogItem):
-    article_ref = "https://doi.org/10.1073/pnas.1018839108"
-    description = r"""CNOT gate with 4 heralded modes"""
+class PostProcessedCnotItem(CatalogItem):
+    article_ref = "https://journals.aps.org/pra/abstract/10.1103/PhysRevA.65.062324"
+    description = r"""CNOT gate with 2 heralded modes and a post-selection function"""
     str_repr = r"""                      ╭─────╮
 ctrl (dual rail) ─────┤     ├───── ctrl (dual rail)
                  ─────┤     ├─────
                       │     │
 data (dual rail) ─────┤     ├───── data (dual rail)
                  ─────┤     ├─────
                       ╰─────╯"""
 
-    R1 = 0.228
-    R2 = 0.758
-    theta1 = BS.r_to_theta(R1)
-    theta2 = BS.r_to_theta(R2)
-
     def __init__(self):
-        super().__init__("heralded cnot")
+        super().__init__("postprocessed cnot")
         self._default_opts['type'] = AsType.PROCESSOR
 
     def build(self):
-        c_hcnot = (Circuit(8, name="Heralded CNOT")
-                   .add((0, 1, 2), PERM([1, 2, 0]))
-                   .add((4, 5), BS.H())
-                   .add((5, 6, 7), PERM([1, 2, 0]))
-                   .add((3, 4), BS.H())
-                   .add((2, 3), BS.H(theta=self.theta1, phi_bl=np.pi, phi_tr=np.pi/2, phi_tl=-np.pi/2))
-                   .add((4, 5), BS.H(theta=self.theta1))
-                   .add((3, 4), BS.H())
-                   .add((5, 6, 7), PERM([2, 1, 0]))
-                   .add((1, 2), PERM([1, 0]))
-                   .add((2, 3), BS.H(theta=self.theta2))
-                   .add((4, 5), BS.H(theta=self.theta2, phi_bl=np.pi, phi_tr=np.pi/2, phi_tl=-np.pi/2))
-                   .add((5, 6), PERM([1, 0]))
-                   .add((4, 5), BS.H())
-                   .add((4, 5), PERM([1, 0]))
-                   .add((0, 1, 2), PERM([2, 1, 0])))
+        theta_13 = BS.r_to_theta(1/3)
+        c_cnot = (Circuit(6, name="PostProcessed CNOT")
+                  .add(0, PERM([0, 2, 3, 4, 1]))  # So that both heralded modes are on the bottom of the gate
+                  .add((0, 1), BS.H(theta_13))
+                  .add((0, 1), PERM([1, 0]))
+                  .add((3, 4), BS.H())
+                  .add((2, 3), PERM([1, 0]))
+                  .add((2, 3), BS.H(theta_13))
+                  .add((2, 3), PERM([1, 0]))
+                  .add((4, 5), BS.H(theta_13))
+                  .add((3, 4), BS.H())
+                  .add(0, PERM([4, 0, 1, 2, 3])))  # So that both heralded modes are on the bottom of the gate
 
         if self._opt('type') == AsType.CIRCUIT:
-            return c_hcnot
+            return c_cnot
         elif self._opt('type') == AsType.PROCESSOR:
-            p = Processor(self._opt('backend'), c_hcnot)
-            return p.add_herald(0, 0) \
-                    .add_herald(1, 1) \
-                    .add_port(2, Port(Encoding.DUAL_RAIL, 'ctrl')) \
-                    .add_port(4, Port(Encoding.DUAL_RAIL, 'data')) \
-                    .add_herald(6, 0) \
-                    .add_herald(7, 1)
+            p = Processor(self._opt('backend'), c_cnot)
+            p.add_port(0, Port(Encoding.DUAL_RAIL, 'ctrl')) \
+             .add_port(2, Port(Encoding.DUAL_RAIL, 'data')) \
+             .add_herald(4, 0) \
+             .add_herald(5, 0)
+            p.set_postselection(PostSelect("[0,1]==1 & [2,3]==1"))
+            return p
```

### Comparing `perceval-quandela-0.8.1/perceval/components/core_catalog/postprocessed_cnot.py` & `perceval-quandela-0.9.0/perceval/components/core_catalog/heralded_cnot.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,51 +23,61 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from perceval.components import Circuit, Processor
-from perceval.components.unitary_components import *
+from perceval.components import Circuit, Processor, BS, PERM, Port
 from perceval.components.component_catalog import CatalogItem, AsType
-from perceval.components.port import Herald, Port, Encoding
+from perceval.utils import Encoding
 
 
-def _post_process(s):
-    return (s[1] or s[2]) and (s[3] or s[4])
-
-
-class PostProcessedCnotItem(CatalogItem):
-    article_ref = "https://journals.aps.org/pra/abstract/10.1103/PhysRevA.65.062324"
-    description = r"""CNOT gate with 2 heralded modes and a post-processing function"""
+class HeraldedCnotItem(CatalogItem):
+    article_ref = "https://doi.org/10.1073/pnas.1018839108"
+    description = r"""CNOT gate with 4 heralded modes"""
     str_repr = r"""                      ╭─────╮
 ctrl (dual rail) ─────┤     ├───── ctrl (dual rail)
                  ─────┤     ├─────
                       │     │
 data (dual rail) ─────┤     ├───── data (dual rail)
                  ─────┤     ├─────
                       ╰─────╯"""
 
+    R1 = 0.228
+    R2 = 0.758
+    theta1 = BS.r_to_theta(R1)
+    theta2 = BS.r_to_theta(R2)
+
     def __init__(self):
-        super().__init__("postprocessed cnot")
+        super().__init__("heralded cnot")
         self._default_opts['type'] = AsType.PROCESSOR
 
     def build(self):
-        theta_13 = BS.r_to_theta(1/3)
-        c_cnot = (Circuit(6, name="PostProcessed CNOT")
-                  .add((0, 1), BS.H(theta_13, phi_bl=np.pi, phi_tr=np.pi/2, phi_tl=-np.pi/2))
-                  .add((3, 4), BS.H())
-                  .add((2, 3), BS.H(theta_13, phi_bl=np.pi, phi_tr=np.pi/2, phi_tl=-np.pi/2))
-                  .add((4, 5), BS.H(theta_13))
-                  .add((3, 4), BS.H()))
+        c_hcnot = (Circuit(8, name="Heralded CNOT")
+                   .add(1, PERM([2, 4, 3, 0, 1]))
+                   .add(4, BS.H())
+                   .add(3, PERM([1, 3, 0, 4, 2]))
+                   .add(3, BS.H())
+                   .add(3, PERM([2, 0, 1]))
+                   .add(2, BS.H(theta=self.theta1))
+                   .add(4, BS.H(theta=self.theta1))
+                   .add(3, PERM([1, 2, 0]))
+                   .add(3, BS.H())
+                   .add(1, PERM([2, 0, 3, 1, 6, 5, 4]))
+                   .add(2, BS.H(theta=self.theta2))
+                   .add(2, PERM([1, 0]))
+                   .add(4, BS.H(theta=self.theta2))
+                   .add(4, PERM([1, 2, 0]))
+                   .add(4, BS.H())
+                   .add(1, PERM([4, 3, 0, 2, 1])))
 
         if self._opt('type') == AsType.CIRCUIT:
-            return c_cnot
+            return c_hcnot
         elif self._opt('type') == AsType.PROCESSOR:
-            p = Processor(self._opt('backend'), c_cnot)
-            p.add_herald(0, 0) \
-             .add_port(1, Port(Encoding.DUAL_RAIL, 'ctrl')) \
-             .add_port(3, Port(Encoding.DUAL_RAIL, 'data')) \
-             .add_herald(5, 0)
-            p.set_postprocess(_post_process)
-            return p
+            p = Processor(self._opt('backend'), c_hcnot)
+            return p.add_port(0, Port(Encoding.DUAL_RAIL, 'ctrl')) \
+                    .add_port(2, Port(Encoding.DUAL_RAIL, 'data')) \
+                    .add_herald(4, 0) \
+                    .add_herald(5, 1) \
+                    .add_herald(6, 0) \
+                    .add_herald(7, 1)
```

### Comparing `perceval-quandela-0.8.1/perceval/components/detector.py` & `perceval-quandela-0.9.0/perceval/components/detector.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/components/linear_circuit.py` & `perceval-quandela-0.9.0/perceval/components/linear_circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,30 +34,20 @@
 from typing import Callable, Optional, Union, Tuple, Type, List
 
 import numpy as np
 import sympy as sp
 import scipy.optimize as so
 
 from perceval.components.abstract_component import AParametrizedComponent
-from perceval.utils import Parameter, Matrix, MatrixN, global_params
+from perceval.utils import Parameter, Matrix, MatrixN, matrix_double, global_params
 import perceval.utils.algorithms.decomposition as decomposition
 from perceval.utils.algorithms.match import Match
 from perceval.utils.algorithms.solve import solve
 
 
-def _matrix_double_for_polarization(m, u):
-    pu = Matrix(m * 2, u.is_symbolic())
-    pu.fill(0)
-    for k1 in range(0, m):
-        for k2 in range(0, m):
-            pu[2 * k1, 2 * k2] = u[k1, k2]
-            pu[2 * k1 + 1, 2 * k2 + 1] = u[k1, k2]
-    return pu
-
-
 class ACircuit(AParametrizedComponent, ABC):
     """
     Abstract linear optics circuit class. A circuit is defined by a dimension `m`, and by parameters.
     Parameters can be fixed (value) or variables.
     """
     _supports_polarization = False
 
@@ -93,15 +83,15 @@
         if self._supports_polarization:
             assert use_polarization is not False, "polarized circuit cannot generates non-polarized unitary"
             use_polarization = True
         elif use_polarization is None:
             use_polarization = False
         u = self._compute_unitary(assign, use_symbolic)
         if use_polarization and not self._supports_polarization:
-            return _matrix_double_for_polarization(self._m, u)
+            return matrix_double(u)
         return u
 
     @property
     def requires_polarization(self):
         return self._supports_polarization
 
     @property
```

### Comparing `perceval-quandela-0.8.1/perceval/components/non_unitary_components.py` & `perceval-quandela-0.9.0/perceval/components/non_unitary_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,16 @@
         """
         Applies a channel loss to r-th mode on an input StateVector sv
         Channel loss is treated as a beam splitter with a reflectivity equal to the loss. This beam splitter
         being connected to a "virtual" mode containing lost photons
 
         The output state vector contains BasicStates which are 1 mode bigger than the ones in input:
         (input modes count + the virtual mode)
+
+        Warning: this method loses annotations! However, it is not currently used in LC simulation (see: LossSimulator)
         """
         # Assumes r of size 1
         # Returns a stateVector of size m + 1. Stepper backend should support this
         if isinstance(sv, BasicState):
             sv = StateVector(sv)
 
         r = r[0]
```

### Comparing `perceval-quandela-0.8.1/perceval/components/port.py` & `perceval-quandela-0.9.0/perceval/components/port.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,25 +28,17 @@
 # SOFTWARE.
 
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import List
 
 from perceval.utils import BasicState
+from perceval.utils import Encoding
 from .abstract_component import AComponent
 
-
-class Encoding(Enum):
-    DUAL_RAIL = 0
-    POLARIZATION = 1
-    QUDIT = 2
-    TIME = 3
-    RAW = 4
-
-
 def _port_size(encoding: Encoding):
     if encoding == Encoding.DUAL_RAIL:
         return 2
     elif encoding == Encoding.POLARIZATION:
         return 1
     elif encoding == Encoding.TIME:
         return 1
```

### Comparing `perceval-quandela-0.8.1/perceval/components/predefined_circuit.py` & `perceval-quandela-0.9.0/perceval/components/predefined_circuit.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/components/processor.py` & `perceval-quandela-0.9.0/perceval/components/processor.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,74 +28,70 @@
 # SOFTWARE.
 from numpy import Inf
 
 from .abstract_processor import AProcessor, ProcessorType
 from .port import LogicalState
 from .source import Source
 from .linear_circuit import ACircuit
-from .computation import count_TD, count_independant_TD, expand_TD
-from perceval.utils import SVDistribution, BSDistribution, BSSamples, BasicState, StateVector, global_params
-from perceval.backends import BACKEND_LIST
-from perceval.backends.processor import StepperBackend
+from perceval.utils import SVDistribution, BSDistribution, BSSamples, BasicState, StateVector
+from perceval.backends import ABackend, ASamplingBackend, BACKEND_LIST
 
 from multipledispatch import dispatch
 from typing import Dict, Callable, Union, List
 
 
 class Processor(AProcessor):
     """
     Generic definition of processor as a source + components (both unitary and non-unitary) + ports
     + optional post-processing logic
 
-    :param backend_name: Name of the simulator backend to run
+    :param backend: Name or instance of a simulation backend
     :param m_circuit: can either be:
 
         - an int: number of modes of interest (MOI). A mode of interest is any non-heralded mode.
         >>> p = Processor("SLOS", 5)
 
         - a circuit: the input circuit to start with. Other components can still be added afterwards with `add()`
         >>> p = Processor("SLOS", BS() // PS() // BS())
 
     :param source: the Source used by the processor (defaults to perfect source)
     """
-    def __init__(self, backend_name: str, m_circuit: Union[int, ACircuit] = None, source: Source = Source(),
+    def __init__(self, backend: Union[ABackend, str], m_circuit: Union[int, ACircuit] = None, source: Source = Source(),
                  name: str = None):
         super().__init__()
         self._source = source
         self.name = "Local processor" if name is None else name
 
         if isinstance(m_circuit, ACircuit):
             self._n_moi = m_circuit.m
             self.add(0, m_circuit)
         else:
             self._n_moi = m_circuit  # number of modes of interest (MOI)
 
         self._inputs_map: Union[SVDistribution, None] = None
-        self._simulator = None
-        assert backend_name in BACKEND_LIST, f"Simulation backend '{backend_name}' does not exist"
-        self._backend_name = backend_name
-
-    def _setup_simulator(self, **kwargs):
-        if self._is_unitary:
-            self._simulator = BACKEND_LIST[self._backend_name](self.linear_circuit(), **kwargs)
+        if isinstance(backend, str):
+            assert backend in BACKEND_LIST, f"Simulation backend '{backend}' does not exist"
+            self.backend = BACKEND_LIST[backend]()
         else:
-            if "probampli" not in BACKEND_LIST[self._backend_name].available_commands():
-                raise RuntimeError(f"{self._backend_name} backend cannot be used on a non-unitary processor")
-            self._simulator = StepperBackend(self.non_unitary_circuit(),
-                                             m=self.circuit_size,
-                                             backend_name=self._backend_name,
-                                             min_detected_photons_filter=self._min_detected_photons)
+            self.backend = backend
+        self._simulator = None
 
     def type(self) -> ProcessorType:
         return ProcessorType.SIMULATOR
 
     @property
     def is_remote(self) -> bool:
         return False
 
+    def check_input(self, input_state: BasicState):
+        assert self.m is not None, "A circuit has to be set before the input state"
+        expected_input_length = self.m
+        assert len(input_state) == expected_input_length, \
+            f"Input length not compatible with circuit (expects {expected_input_length}, got {len(input_state)})"
+
     @dispatch(LogicalState)
     def with_input(self, input_state: LogicalState) -> None:
         r"""
         Set up the processor input with a LogicalState. Computes the input probability distribution.
 
         :param input_state: A LogicalState of length the input port count. Enclosed values have to match with ports
         encoding.
@@ -104,51 +100,34 @@
 
     @dispatch(BasicState)
     def with_input(self, input_state: BasicState) -> None:
         """
         Simulates plugging the photonic source on certain modes and turning it on.
         Computes the input probability distribution
 
-        :param input_state: Expected input BasicState of length `self.m` (heralded modes are managed
-        automatically)
+        :param input_state: Expected input BasicState of length `self.m` (heralded modes are managed automatically)
         The properties of the source will alter the input state. A perfect source always delivers the expected state as
         an input. Imperfect ones won't.
         """
+        self.check_input(input_state)
         input_list = [0] * self.circuit_size
-        self._inputs_map = SVDistribution()
-        assert self.m is not None, "A circuit has to be set before the input state"
-        expected_input_length = self.m
-        assert len(input_state) == expected_input_length, \
-            f"Input length not compatible with circuit (expects {expected_input_length}, got {len(input_state)})"
         input_idx = 0
         expected_photons = 0
+        # Build real input state (merging ancillas + expected input) and compute expected photon count
         for k in range(self.circuit_size):
-            distribution = SVDistribution(StateVector("|0>"))
             if k in self.heralds:
-                if self.heralds[k] == 1:
-                    distribution = self._source.probability_distribution()
-                    input_list[k] = 1
-                    expected_photons += 1
+                input_list[k] = self.heralds[k]
+                expected_photons += self.heralds[k]
             else:
-                if input_state[input_idx] > 0:
-                    distribution = self._source.probability_distribution(input_state[input_idx])
-                    input_list[k] = input_state[input_idx]
-                    expected_photons += 1
+                input_list[k] = input_state[input_idx]
+                expected_photons += input_state[input_idx]
                 input_idx += 1
-            self._inputs_map *= distribution  # combine distributions
-
-        # Needed to do this at the end
-        used_input_map = SVDistribution()
-        for state, prob in self._inputs_map.items():
-            if prob:
-                used_input_map[_find_equivalent(state[0])] += prob
-
-        self._inputs_map = used_input_map
 
         self._input_state = BasicState(input_list)
+        self._inputs_map = self._source.generate_distribution(self._input_state)
         self._min_detected_photons = expected_photons
         if 'min_detected_photons' in self._parameters:
             self._min_detected_photons = self._parameters['min_detected_photons']
 
     @dispatch(StateVector)
     def with_input(self, sv: StateVector):
         r"""
@@ -176,180 +155,121 @@
                     raise ValueError(
                         f'Input distribution contains states with a bad size ({state.m}), expected {self.circuit_size}')
         self._inputs_map = svd
         self._min_detected_photons = expected_photons
         if 'min_detected_photons' in self._parameters:
             self._min_detected_photons = self._parameters['min_detected_photons']
 
+    def _circuit_changed(self):
+        # Override parent's method to reset the internal simulator as soon as the component list changes
+        self._simulator = None
+
+    def with_polarized_input(self, bs: BasicState):
+        assert bs.has_polarization, "BasicState is not polarized, please use with_input instead"
+        self._input_state = bs
+        self._inputs_map = SVDistribution(bs)
+        self._min_detected_photons = bs.n
+        if 'min_detected_photons' in self._parameters:
+            self._min_detected_photons = self._parameters['min_detected_photons']
+
     def clear_input_and_circuit(self):
         super().clear_input_and_circuit()
         self._inputs_map = None
-        self._simulator = None
 
     def _compose_processor(self, connector, processor, keep_port: bool):
         assert isinstance(processor, Processor), "can not mix types of processors"
         super(Processor, self)._compose_processor(connector, processor, keep_port)
 
-    def _init_command(self, command_name: str):
-        assert self._inputs_map is not None, "Input is missing, please call with_inputs()"
-        if self._backend_name == "CliffordClifford2017" and self._has_td:
-            raise NotImplementedError(
-                "Time delays are not implemented within CliffordClifford2017 backend. Please use another one.")
-        if not self._has_td:  # TODO: remove quickfix by something clever :  self._simulator is None and
-            self._setup_simulator()
-
     def _state_preselected_physical(self, input_state: StateVector) -> bool:
         return max(input_state.n) >= self._min_detected_photons
 
     def _state_selected_physical(self, output_state: BasicState) -> bool:
         if self.is_threshold:
             modes_with_photons = len([n for n in output_state if n > 0])
             return modes_with_photons >= self._min_detected_photons
         return output_state.n >= self._min_detected_photons
 
     def samples(self, count: int, progress_callback=None) -> Dict:
-        self._init_command("samples")
+        assert isinstance(self.backend, ASamplingBackend), "A sampling backend is required to call samples method"
+        pre_physical_perf = 1
+        # Rework input map so that it contains only states with enough photons
+        input_svd = SVDistribution()
+        for sv, p in self._inputs_map.items():
+            if self._state_preselected_physical(sv):
+                if len(sv) > 1:
+                    raise RuntimeError("Cannot sample on a superposed state")
+                input_svd[sv] = p
+            else:
+                pre_physical_perf -= p
+
+        self.backend.set_circuit(self.linear_circuit())
         output = BSSamples()
+        selected_inputs = []
+        idx = 0
         not_selected_physical = 0
         not_selected = 0
-        selected_inputs = self._inputs_map.sample(count)
-        idx = 0
         while len(output) < count:
-            selected_input = selected_inputs[idx]
-            idx += 1
             if idx == len(selected_inputs):
                 idx = 0
-                selected_inputs = self._inputs_map.sample(count)
-            if not self._state_preselected_physical(selected_input):
-                not_selected_physical += 1
-                continue
-            sampled_state = self._simulator.sample(selected_input)
+                selected_inputs = input_svd.sample(count)
+            selected_bs = selected_inputs[idx][0]
+            idx += 1
+
+            # Sampling
+            if selected_bs.has_annotations:  # In case of annotations, input must be separately sampled, then recombined
+                bs_list = selected_bs.separate_state()
+                sampled_components = []
+                for bs in bs_list:
+                    self.backend.set_input_state(bs)
+                    sampled_components.append(self.backend.sample())
+                sampled_state = sampled_components.pop()
+                for component in sampled_components:
+                    sampled_state = sampled_state.merge(component)
+            else:
+                self.backend.set_input_state(selected_bs)
+                sampled_state = self.backend.sample()
+
+            # Post-processing
             if not self._state_selected_physical(sampled_state):
                 not_selected_physical += 1
                 continue
             if self._state_selected(sampled_state):
                 output.append(self.postprocess_output(sampled_state))
             else:
                 not_selected += 1
+
+            # Progress handling
             if progress_callback:
                 exec_request = progress_callback(len(output)/count, "sampling")
                 if exec_request is not None and 'cancel_requested' in exec_request and exec_request['cancel_requested']:
                     break
 
-        physical_perf = (count + not_selected) / (count + not_selected + not_selected_physical)
+        physical_perf = pre_physical_perf * (count + not_selected) / (count + not_selected + not_selected_physical)
         logical_perf = count / (count + not_selected)
         return {'results': output, 'physical_perf': physical_perf, 'logical_perf': logical_perf}
 
     def probs(self, progress_callback: Callable = None) -> Dict:
-        self._init_command("probs")
-        output = BSDistribution()
-        p_logic_discard = 0
-        if not self._has_td:
-            input_length = len(self._inputs_map)
-            physical_perf = 1
-
-            for idx, (input_state, input_prob) in enumerate(self._inputs_map.items()):
-                if not self._state_preselected_physical(input_state):
-                    physical_perf -= input_prob
-                else:
-                    for (output_state, p) in self._simulator.allstateprob_iterator(input_state):
-                        if p < global_params['min_p']:
-                            continue
-                        output_prob = p * input_prob
-                        if not self._state_selected_physical(output_state):
-                            physical_perf -= output_prob
-                            continue
-                        if self._state_selected(output_state):
-                            output[self.postprocess_output(output_state)] += output_prob
-                        else:
-                            p_logic_discard += output_prob
-                if progress_callback:
-                    exec_request = progress_callback(idx/input_length, 'probs')
-                    if exec_request is not None and 'cancel_requested' in exec_request and exec_request['cancel_requested']:
-                        raise RuntimeError("Cancel requested")
-
-        else:
-            # Create a bigger processor with no heralds to represent the time delays
-            p_comp = self.flatten()
-            TD_number = count_TD(p_comp)
-            depth = count_independant_TD(p_comp, self.circuit_size) + 1
-            p_comp, extend_m = expand_TD(p_comp, depth, self.circuit_size, TD_number, True)
-            # p_comp = simplify(p_comp, extend_m)
-            extended_p = _expand_TD_processor(p_comp,
-                                              self._backend_name,
-                                              depth,
-                                              extend_m,
-                                              self._input_state,
-                                              self._min_detected_photons,
-                                              self.source)
-
-            res = extended_p.probs(progress_callback=progress_callback)
-
-            # Now reduce the states.
-            interest_m = [(depth - 1) * self.circuit_size, depth * self.circuit_size]
-            extended_out = res["results"]
-
-            second_perf = 1
-            for out_state, output_prob in extended_out.items():
-                reduced_out_state = out_state[interest_m[0]: interest_m[1]]
-                if not self._state_selected_physical(reduced_out_state):
-                    second_perf -= output_prob
-                    continue
-                if self._state_selected(reduced_out_state):
-                    output[self.postprocess_output(reduced_out_state)] += output_prob
-                else:
-                    p_logic_discard += output_prob
-            physical_perf = second_perf * res["physical_perf"]
-
-        if physical_perf < global_params['min_p']:
-            physical_perf = 0
-        all_p = sum(v for v in output.values())
-        if all_p == 0:
-            return {'results': output, 'physical_perf': physical_perf}
-        logical_perf = 1 - p_logic_discard / (p_logic_discard + all_p)
-        output.normalize()
-        return {'results': output, 'physical_perf': physical_perf, 'logical_perf': logical_perf}
+        # assert self._inputs_map is not None, "Input is missing, please call with_inputs()"
+        if self._simulator is None:
+            from perceval.simulators import SimulatorFactory  # Avoids a circular import
+            self._simulator = SimulatorFactory.build(self)
+        res = self._simulator.probs_svd(self._inputs_map, progress_callback=progress_callback)
+        lperf = 1
+        pperf = 1
+        postprocessed_res = BSDistribution()
+        for state, prob in res['results'].items():
+            if not self._state_selected_physical(state):
+                pperf -= prob
+                continue
+            if self._state_selected(state):
+                postprocessed_res[self.postprocess_output(state)] += prob
+            else:
+                lperf -= prob
+        postprocessed_res.normalize()
+        res['logical_perf'] = res['logical_perf']*lperf if 'logical_perf' in res else lperf
+        res['physical_perf'] = res['physical_perf']*pperf if 'physical_perf' in res else pperf
+        res['results'] = postprocessed_res
+        return res
 
     @property
     def available_commands(self) -> List[str]:
-        return [BACKEND_LIST[self._backend_name].preferred_command()=="samples" and "samples" or "probs"]
-
-
-def _expand_TD_processor(components: list, backend_name: str, depth: int, m: int,
-                         input_states: Union[SVDistribution, BasicState], min_detected_photons: int,
-                         source: Source):
-    p = Processor(backend_name, m, source)
-    if isinstance(input_states, SVDistribution):
-        input_states = input_states ** depth * SVDistribution(BasicState([0] * (m - depth * next(iter(input_states)).m)))
-    else:  # BasicState
-        input_states = input_states ** depth * BasicState([0] * (m - depth * input_states.m))
-
-    p.with_input(input_states)
-    for r, c in components:
-        p.add(r, c)
-    p.min_detected_photons_filter(min_detected_photons)
-    return p
-
-
-def _find_equivalent(state):
-    if not state.has_annotations:
-        return state
-    annot_numbers = dict()
-    i = 0
-    new_state = "|"
-
-    for mode in range(state.m):
-        if not state[mode]:
-            new_state += "0,"
-            continue
-        annotations = state.get_mode_annotations(mode)
-        for n in range(state[mode]):
-            annot = annotations[n]["_"]
-            if annot is not None:
-                nb = int(annot.real)
-                if nb not in annot_numbers:
-                    annot_numbers[nb] = i
-                    i += 1
-                new_state += "{_:" + f"{annot_numbers[nb]}" + "}"
-        new_state += ","
-    new_state = new_state[:-1] + ">"
-    return StateVector(new_state)
+        return ["samples" if self.backend.preferred_command() == "sample" else "probs"]
```

### Comparing `perceval-quandela-0.8.1/perceval/components/source.py` & `perceval-quandela-0.9.0/perceval/components/source.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import math
 
-from perceval.utils import SVDistribution, StateVector
+from perceval.utils import SVDistribution, StateVector, BasicState, anonymize_annotations
 from typing import Dict, List, Union
 
 
 class Source:
     r"""Definition of a source
     We build on a phenomenological model first introduced in ref. [1] where an imperfect quantum-dot based single-photon
     source is modeled by a statistical mixture of Fock states. The model developed here, first introduced in ref. [2],
@@ -130,36 +130,59 @@
             if self._multiphoton_model == "distinguishable" else 0  # Noise photon or signal
 
         (p1to1, p2to1, p2to2) = self._get_probs()
         p0 = 1 - (p1to1 + 2 * p2to1 + p2to2)  # 2 * p2to1 because of symmetry
 
         dist = []  # Distribution represented as a list of annotations on 1 mode + probability
         self._add(dist, 0, p0)
-        if distinguishability or (self._multiphoton_model == "distinguishable" and p2to2):
+        if self.partially_distinguishible:
             self._add(dist, ["_:0", "_:%s" % second_photon],  (1 - distinguishability) * p2to2)
             self._add(dist, ["_:%s" % distinguishable_photon, "_:%s" % second_photon], distinguishability * p2to2)
             self._add(dist, ["_:%s" % distinguishable_photon], distinguishability * (p1to1 + p2to1))
             self._add(dist, ["_:0"], (1 - distinguishability) * (p1to1 + p2to1))
             self._add(dist, ["_:%s" % second_photon], p2to1)
         else:
             # Just avoids annotations
             self._add(dist, 2, p2to2)
             self._add(dist, 1, p1to1 + 2 * p2to1)
         return dist
 
+    @property
+    def partially_distinguishible(self):
+        return self._indistinguishability != 1 \
+            or (self._multiphoton_model == "distinguishable" and self._multiphoton_component)
+
     def probability_distribution(self, nphotons: int = 1) -> SVDistribution:
         r"""returns SVDistribution on 1 mode associated to the source
 
         :param nphotons: Require `nphotons` in the mode (default 1).
         """
+        if nphotons == 0:
+            return SVDistribution(StateVector("|0>"))
         dist_all = []
         for p in range(nphotons):
             d1 = self._generate_one_photon_distribution()
             dist_all = self._merge_photon_distributions(dist_all, d1)
 
         svd = SVDistribution()
         for photons, prob in dist_all:
             if isinstance(photons, int):
                 svd.add(StateVector([photons]), prob)
             else:
                 svd.add(StateVector([len(photons)], {0: photons}), prob)
         return svd
+
+    def generate_distribution(self, expected_input: BasicState):
+        """
+        Simulates plugging the photonic source on certain modes and turning it on.
+        Computes the input probability distribution
+
+        :param expected_input: Expected input BasicState
+        The properties of the source will alter the input state. A perfect source always delivers the expected state as
+        an input. Imperfect ones won't.
+        """
+        dist = SVDistribution()
+        for photon_count in expected_input:
+            dist *= self.probability_distribution(photon_count)
+        if self.partially_distinguishible:
+            dist = anonymize_annotations(dist, annot_tag='_')
+        return dist
```

### Comparing `perceval-quandela-0.8.1/perceval/components/unitary_components.py` & `perceval-quandela-0.9.0/perceval/components/unitary_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,18 +403,18 @@
         permutation = self.perm_vector
         inv = np.empty_like(permutation)
         inv[permutation] = np.arange(len(inv), dtype=inv.dtype)
         inv = [inv[i].item() for i in range(len(inv))]
 
         nsv = copy(sv)
         nsv.clear()
-        nsv.update({BasicState(state.set_slice(slice(min_r, max_r), BasicState([state[i + min_r]
-                                                                                for i in inv]))):
-                        prob_ampli for state, prob_ampli in sv.items()})
-
+        nsv.update({
+            BasicState(state.set_slice(slice(min_r, max_r), BasicState([state[i + min_r] for i in inv]))): prob_ampli
+            for state, prob_ampli in sv.items()
+        })
         return nsv
 
 
 class PBS(Unitary):
     """Polarized beam spliter"""
     _supports_polarization = True
     DEFAULT_NAME = "PBS"
```

### Comparing `perceval-quandela-0.8.1/perceval/converters/__init__.py` & `perceval-quandela-0.9.0/perceval/rendering/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from .qiskit_converter import QiskitConverter
+from .pdisplay import pdisplay, pdisplay_to_file
+from .format import Format
```

### Comparing `perceval-quandela-0.8.1/perceval/converters/qiskit_converter.py` & `perceval-quandela-0.9.0/perceval/converters/qiskit_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from perceval.components import Port, Encoding, Circuit, Processor, Source
-from perceval.utils import P, BasicState
+from perceval.components import Port, Circuit, Processor, Source
+from perceval.utils import P, BasicState, Encoding
 from perceval.utils.algorithms.optimize import optimize
 from perceval.utils.algorithms.norm import frobenius
 import perceval.components.unitary_components as comp
 
 
 min_precision_gate = 1e-4
 
@@ -43,14 +43,15 @@
     :param catalog: a component library to use for the conversion. It must contain CNOT gates.
     :param backend_name: backend name used in the converted processor
     :param source: the source used as input for the converted processor (default perfect source).
     """
     def __init__(self, catalog, backend_name: str = "SLOS", source: Source = Source()):
         self._source = source
         self._heralded_cnot_builder = catalog["heralded cnot"]
+        self._heralded_cz_builder = catalog["heralded cz"]
         self._postprocessed_cnot_builder = catalog["postprocessed cnot"]
         self._generic_2mode_builder = catalog["generic 2 mode circuit"]
         self._lower_phase_component = Circuit(2) // (0, comp.PS(P("phi2")))
         self._upper_phase_component = Circuit(2) // (1, comp.PS(P("phi1")))
         self._two_phase_component = Circuit(2) // (0, comp.PS(P("phi1"))) // (1, comp.PS(P("phi2")))
         self._backend_name = backend_name
 
@@ -86,41 +87,45 @@
             if isinstance(instruction[0], qiskit.circuit.barrier.Barrier):
                 continue
             # some limitation in the conversion, in particular measure
             assert isinstance(instruction[0], qiskit.circuit.gate.Gate), "cannot convert (%s)" % instruction[0]
 
             if instruction[0].num_qubits == 1:
                 # one mode gate
-                ins = self._create_one_mode_gate(instruction[0].to_matrix())
+                ins = self._create_one_qubit_gate(instruction[0].to_matrix())
                 ins._name = instruction[0].name
                 p.add(instruction[1][0].index * 2, ins.copy())
             else:
                 c_idx = instruction[1][0].index * 2
                 c_data = instruction[1][1].index * 2
                 c_first = min(c_idx, c_data)
 
                 if instruction[0].name == "swap":
                     # c_idx and c_data are consecutive - not necessarily ordered
                     p.add(c_first, comp.PERM([2, 3, 0, 1]))
+                elif instruction[0].name == "cz":
+                    cz_processor = self._heralded_cz_builder.build()
+                    mode_map = {c_idx: 0, c_idx + 1: 1, c_data: 2, c_data + 1: 3}
+                    p.add(mode_map, cz_processor)
                 elif instruction[0].name == "cx":
                     cnot_idx += 1
                     if use_postselection and cnot_idx == n_cnot:
                         cnot_processor = self._postprocessed_cnot_builder.build()
-                        mode_map = {c_idx: 1, c_idx + 1: 2, c_data: 3, c_data + 1: 4}
+                        mode_map = {c_idx: 0, c_idx + 1: 1, c_data: 2, c_data + 1: 3}
                     else:
                         cnot_processor = self._heralded_cnot_builder.build()
-                        mode_map = {c_idx: 2, c_idx + 1: 3, c_data: 4, c_data + 1: 5}
+                        mode_map = {c_idx: 0, c_idx + 1: 1, c_data: 2, c_data + 1: 3}
                     p.add(mode_map, cnot_processor)
 
                 else:
                     raise RuntimeError("Gate not yet supported: %s" % instruction[0].name)
         p.with_input(default_input_state)
         return p
 
-    def _create_one_mode_gate(self, u):
+    def _create_one_qubit_gate(self, u):
         if abs(u[1, 0]) + abs(u[0, 1]) < 2 * min_precision_gate:
             # diagonal matrix - we can handle with phases, we consider that gate unitary parameters has
             # limited numeric precision
             if abs(u[0, 0] - 1) < min_precision_gate:
                 if abs(u[1, 1] - 1) < min_precision_gate:
                     return None
                 ins = self._upper_phase_component.copy()
```

### Comparing `perceval-quandela-0.8.1/perceval/rendering/__init__.py` & `perceval-quandela-0.9.0/perceval/rendering/format.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,9 +23,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from .pdisplay import pdisplay, pdisplay_to_file
-from .format import Format
+from enum import Enum
+
+
+class Format(Enum):
+    TEXT = 1
+    MPLOT = 2
+    HTML = 3
+    LATEX = 4
```

### Comparing `perceval-quandela-0.8.1/perceval/rendering/_mplot_utils.py` & `perceval-quandela-0.9.0/perceval/rendering/_mplot_utils.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/rendering/_processor_utils.py` & `perceval-quandela-0.9.0/perceval/rendering/_processor_utils.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/rendering/canvas/__init__.py` & `perceval-quandela-0.9.0/perceval/rendering/canvas/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,7 +26,8 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .canvas import Canvas
 from .mplot_canvas import MplotCanvas
 from .svg_canvas import SvgCanvas
+from .latex_canvas import LatexCanvas
```

### Comparing `perceval-quandela-0.8.1/perceval/rendering/canvas/canvas.py` & `perceval-quandela-0.9.0/perceval/rendering/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/rendering/canvas/mplot_canvas.py` & `perceval-quandela-0.9.0/perceval/rendering/canvas/mplot_canvas.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/rendering/canvas/svg_canvas.py` & `perceval-quandela-0.9.0/perceval/rendering/canvas/svg_canvas.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/rendering/circuit/__init__.py` & `perceval-quandela-0.9.0/perceval/rendering/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/rendering/circuit/abstract_skin.py` & `perceval-quandela-0.9.0/perceval/rendering/circuit/abstract_skin.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/rendering/circuit/phys_skin.py` & `perceval-quandela-0.9.0/perceval/rendering/circuit/phys_skin.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/rendering/circuit/renderer.py` & `perceval-quandela-0.9.0/perceval/rendering/circuit/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from abc import ABC, abstractmethod
 import copy
 import math
 from typing import Any, Tuple
 
 from perceval.rendering.circuit import ASkin, ModeStyle
 from perceval.rendering.format import Format
-from perceval.rendering.canvas import Canvas, MplotCanvas, SvgCanvas
+from perceval.rendering.canvas import Canvas, MplotCanvas, SvgCanvas, LatexCanvas
 from perceval.components import ACircuit, Circuit, PortLocation, PERM, Herald
 from perceval.utils.format import format_parameters
 
 
 class PortPos:
     def __init__(self, x, y, fixed=True):
         self.x = x
@@ -557,16 +557,16 @@
 ) -> ICircuitRenderer:
     """
     Creates a renderer given the selected format. Dispatches parameters to generated canvas objects
     A skin object is needed for circuit graphic rendering.
     """
     if output_format == Format.TEXT:
         return TextRenderer(n)
-    if output_format == Format.LATEX:
-        raise NotImplementedError("Latex format is not supported for circuit rendering")
-
+    
     assert skin is not None, "A skin must be selected for circuit graphical rendering"
     if output_format == Format.HTML:
         canvas = SvgCanvas(**opts)
+    elif output_format == Format.LATEX:
+        canvas = LatexCanvas(**opts)
     else:
         canvas = MplotCanvas(**opts)
     return CanvasRenderer(n, canvas, skin)
```

### Comparing `perceval-quandela-0.8.1/perceval/rendering/circuit/skin_common.py` & `perceval-quandela-0.9.0/perceval/rendering/circuit/skin_common.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/rendering/circuit/symb_skin.py` & `perceval-quandela-0.9.0/perceval/rendering/circuit/symb_skin.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/rendering/format.py` & `perceval-quandela-0.9.0/perceval/converters/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from enum import Enum
-
-
-class Format(Enum):
-    TEXT = 1
-    MPLOT = 2
-    HTML = 3
-    LATEX = 4
+from .qiskit_converter import QiskitConverter
+from .converter_statevector import StatevectorConverter
```

### Comparing `perceval-quandela-0.8.1/perceval/rendering/pdisplay.py` & `perceval-quandela-0.9.0/perceval/rendering/pdisplay.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,15 @@
             if value.real != 0:
                 real_part = simple_float(value.real, nsimplify=nsimplify, precision=precision)[1]
             if value.imag != 0:
                 imag_part = "I*" + simple_float(value.imag, nsimplify=nsimplify, precision=precision)[1]
             value = real_part + imag_part
         else:
             value = str(value)
-        d.append([k, value])
+        d.append([str(k), value])
 
     headers = ["state", "probability"]
     if isinstance(sv, StateVector):
         headers[1] = "prob. ampl."
     elif isinstance(sv, BSCount):
         headers[1] = "count"
     s_states = tabulate(d, headers=headers, tablefmt=_TABULATE_FMT_MAPPING[output_format])
@@ -285,15 +285,15 @@
         elif isinstance(o, complex):
             res = simple_complex(o, **opts_simple)[1]
         else:
             raise RuntimeError("pdisplay not defined for type %s" % type(o))
 
     if isinstance(res, drawsvg.Drawing):
         return res
-    elif in_notebook and output_format != Format.TEXT:
+    elif in_notebook and output_format != Format.TEXT and output_format != Format.LATEX:
         display(HTML(res))
     else:
         print(res)
 
 
 def pdisplay_to_file(o, path: str, output_format: Format = None, **opts):
     if output_format is None:
@@ -320,9 +320,14 @@
                 res.save_png(path)  # May fail when rasterization is not available (i.e. on Windows)
             else:
                 res.save_svg(path)
             return
         except:
             pass
 
+    if output_format == Format.LATEX:
+        with open(path, 'w', encoding='utf-8') as f_out:
+            f_out.write(res)
+        return
+
     warnings.warn(
         f"No output file could be created for {type(o)} object (format = {output_format.name}) at path {path}")
```

### Comparing `perceval-quandela-0.8.1/perceval/runtime/__init__.py` & `perceval-quandela-0.9.0/perceval/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/runtime/job.py` & `perceval-quandela-0.9.0/perceval/runtime/job.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/runtime/job_status.py` & `perceval-quandela-0.9.0/perceval/runtime/job_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 
 class JobStatus:
     def __init__(self):
         self._status: RunningStatus = RunningStatus.WAITING
         self._init_time_start = time()
         self._running_time_start = None
+        self._duration = None
         self._completed_time = None
         self._running_progress: float = 0
         self._running_phase: Optional[str] = None
         self._stop_message = None
         self._waiting_progress: Optional[int] = None
         self._last_progress_time: float = 0
 
@@ -81,35 +82,50 @@
     def start_run(self):
         self._running_time_start = time()
         self._status = RunningStatus.RUNNING
 
     def stop_run(self, cause: RunningStatus = RunningStatus.SUCCESS, mesg: Optional[str] = None):
         self._status = cause
         self._completed_time = time()
+        self._duration = self._completed_time - self._init_time_start
         if cause == RunningStatus.SUCCESS:
             self._running_progress = 1
         self._stop_message = mesg
 
     def update_progress(self, progress: float, phase: Optional[str] = None):
         if self._status == RunningStatus.WAITING:
             self.start_run()
         self._running_progress = progress
         self._running_phase = phase
         now = time()
-        if self._last_progress_time is not None and self._last_progress_time - now > 5:
+        if self._last_progress_time and self._last_progress_time - now > 5:
             sleep(0.001)
         self._last_progress_time = now
 
-    def update_times(self, start_time: float, duration: int):
-        if start_time is None:
-            return
-
-        self._init_time_start = start_time
-        if duration is not None:
-            self._completed_time = start_time + duration
+    def update_times(self, creation_datetime: float, start_time: float, duration: int):
+        if creation_datetime:
+            self._init_time_start = creation_datetime
+        if start_time:
+            self._running_time_start = start_time
+        if duration:
+            self._duration = duration
+            if self.completed:
+                self._completed_time = self._running_time_start + self._duration
+
+    @property
+    def creation_timestamp(self):
+        return self._init_time_start
+
+    @property
+    def start_timestamp(self):
+        return self._running_time_start
+
+    @property
+    def duration(self):
+        return self._duration
 
     @property
     def waiting(self):
         return self._status == RunningStatus.WAITING
 
     @property
     def running(self):
@@ -133,9 +149,12 @@
 
     @property
     def progress(self):
         return self._running_progress
 
     @property
     def running_time(self):
+        if self._duration:
+            return self._duration
+
         assert self.completed
         return self._completed_time - self._running_time_start
```

### Comparing `perceval-quandela-0.8.1/perceval/runtime/local_job.py` & `perceval-quandela-0.9.0/perceval/runtime/local_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,10 +104,15 @@
     def get_results(self) -> Any:
         if not self.is_complete:
             raise RuntimeError('The job is still running, results are not available yet.')
         job_status = self.status
         if job_status.status != RunningStatus.SUCCESS:
             raise RuntimeError('The job failed with exception: ' + job_status.stop_message)
         if self._result_mapping_function:
-            self._results['results'] = self._result_mapping_function(self._results['results'],
-                                                                     **self._delta_parameters)
+            if 'results' in self._results:
+                self._results['results'] = self._result_mapping_function(self._results['results'],
+                                                                         **self._delta_parameters)
+            elif 'results_list' in self._results:
+                for res in self._results["results_list"]:
+                    res["results"] = self._result_mapping_function(res['results'],
+                                                                   **self._delta_parameters)
         return self._results
```

### Comparing `perceval-quandela-0.8.1/perceval/runtime/remote_job.py` & `perceval-quandela-0.9.0/perceval/runtime/remote_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,27 @@
 from requests.exceptions import HTTPError, ConnectionError
 
 from .job import Job
 from .job_status import JobStatus, RunningStatus
 from perceval.serialization import deserialize, serialize
 
 
+def _extract_job_times(response):
+    creation_datetime = None
+    start_time = None
+    duration = None
+    try:
+        creation_datetime = float(response['creation_datetime'])
+        start_time = float(response['start_time'])
+        duration = int(response['duration'])
+    except:
+        pass
+    return creation_datetime, duration, start_time
+
+
 class RemoteJob(Job):
     STATUS_REFRESH_DELAY = 1  # minimum job status refresh period (in s)
     _MAX_ERROR = 5
 
     def __init__(self, request_data, rpc_handler, job_name, delta_parameters=None, job_context=None,
                  command_param_names=None, refresh_progress_delay: int = 3):
         r"""
@@ -121,23 +134,20 @@
 
             self._job_status.status = RunningStatus.from_server_response(response['status'])
             if self._job_status.running:
                 self._job_status.update_progress(float(response['progress']), response['progress_message'])
             elif self._job_status.failed:
                 self._job_status._stop_message = response['failure_code']
 
-            start_time = None
-            duration = None
-            try:
-                start_time = float(response['start_time'])
-                duration = int(response['duration'])
-            except:
-                pass
+            creation_datetime, duration, start_time = _extract_job_times(response)
+            self._job_status.update_times(creation_datetime, start_time, duration)
 
-            self._job_status.update_times(start_time, duration)
+            name = response.get("name")
+            if name and name != self.name:
+                self.name = name
 
         return self._job_status
 
     def _handle_unnamed_params(self, args, kwargs):
         if len(args) > len(self._param_names):
             raise RuntimeError(f'Too many unnamed parameter: {len(args)}, expected {len(self._param_names)}')
         for idx, unnamed_arg in enumerate(args):
@@ -190,9 +200,13 @@
         results = deserialize(json.loads(response['results']))
         if "job_context" in results and 'result_mapping' in results["job_context"]:
             path_parts = results["job_context"]["result_mapping"]
             module = __import__(path_parts[0], fromlist=path_parts[1])
             result_mapping_function = getattr(module, path_parts[1])
             # retrieve delta parameters from the response
             self._delta_parameters = results["job_context"].get("mapping_delta_parameters", {})
-            results["results"] = result_mapping_function(results["results"], **self._delta_parameters)
+            if "results_list" in results:
+                for res in results["results_list"]:
+                    res["results"] = result_mapping_function(res["results"], **self._delta_parameters)
+            else:
+                results["results"] = result_mapping_function(results["results"], **self._delta_parameters)
         return results
```

### Comparing `perceval-quandela-0.8.1/perceval/runtime/remote_processor.py` & `perceval-quandela-0.9.0/perceval/runtime/remote_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,28 +22,30 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
+import uuid
 from typing import Dict, List
 from multipledispatch import dispatch
 from pkg_resources import get_distribution
 
 from perceval.components.abstract_processor import AProcessor, ProcessorType
 from perceval.components.linear_circuit import Circuit, ACircuit
 from perceval.components.source import Source
 from perceval.components.port import PortLocation, APort, LogicalState
 from perceval.utils import BasicState
 from perceval.serialization import deserialize, serialize
 from .remote_job import RemoteJob
 from .rpc_handler import RPCHandler
 
+__process_id__ = uuid.uuid4()
+
 QUANDELA_CLOUD_URL = 'https://api.cloud.quandela.com'
 
 
 class RemoteProcessor(AProcessor):
     def __init__(self, name: str, token: str, url: str = QUANDELA_CLOUD_URL, m: int = None):
         super().__init__()
         self.name = name
@@ -125,32 +127,36 @@
         :param input_state: A LogicalState of length the input port count. Enclosed values have to match with ports
         encoding.
         """
         self._with_logical_input(input_state)
 
     @dispatch(BasicState)
     def with_input(self, input_state: BasicState) -> None:
+        self.check_input(input_state)
+        self._input_state = input_state
+
+    def check_input(self, input_state: BasicState) -> None:
         if 'max_photon_count' in self.constraints and input_state.n > self.constraints['max_photon_count']:
             raise RuntimeError(
                 f"Too many photons in input state ({input_state.n} > {self.constraints['max_photon_count']})")
         if 'min_photon_count' in self.constraints and input_state.n < self.constraints['min_photon_count']:
             raise RuntimeError(
                 f"Not enough photons in input state ({input_state.n} < {self.constraints['min_photon_count']})")
         if self._n_moi is not None and input_state.m != self._n_moi:
             raise RuntimeError(f"Input state and circuit size do not match ({input_state.m} != {self._n_moi})")
-        self._input_state = input_state
 
     @property
     def available_commands(self) -> List[str]:
         return self._specs.get("available_commands", [])
 
     def prepare_job_payload(self, command: str, circuitless: bool = False, inputless: bool = False, **kwargs):
         j = {
             'platform_name': self.name,
-            'pcvl_version': get_distribution("perceval-quandela").version
+            'pcvl_version': get_distribution("perceval-quandela").version,
+            'process_id': str(__process_id__)
         }
         payload = {
             'command': command,
             **kwargs
         }
         if self._components and not circuitless:
             payload['circuit'] = serialize(self.linear_circuit())
```

### Comparing `perceval-quandela-0.8.1/perceval/runtime/rpc_handler.py` & `perceval-quandela-0.9.0/perceval/runtime/rpc_handler.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/serialization/__init__.py` & `perceval-quandela-0.9.0/perceval/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/serialization/_circuit_serialization.py` & `perceval-quandela-0.9.0/perceval/serialization/_circuit_serialization.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/serialization/_component_deserialization.py` & `perceval-quandela-0.9.0/perceval/serialization/_component_deserialization.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/serialization/_matrix_serialization.py` & `perceval-quandela-0.9.0/perceval/serialization/_matrix_serialization.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/serialization/_parameter_serialization.py` & `perceval-quandela-0.9.0/perceval/serialization/_parameter_serialization.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/serialization/_schema_circuit_pb2.py` & `perceval-quandela-0.9.0/perceval/serialization/_schema_circuit_pb2.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/serialization/_state_serialization.py` & `perceval-quandela-0.9.0/perceval/serialization/_state_serialization.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/serialization/deserialize.py` & `perceval-quandela-0.9.0/perceval/serialization/deserialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from perceval.components import Circuit
 from perceval.utils import Matrix, BSDistribution, SVDistribution, BasicState, BSCount
 from perceval.serialization import _matrix_serialization, deserialize_state
 from ._state_serialization import deserialize_statevector, deserialize_bssamples
 import perceval.serialization._component_deserialization as _cd
 from perceval.serialization import _schema_circuit_pb2 as pb
 from base64 import b64decode
+from zlib import decompress
 
 
 _MATRIX_PREFIX = ":PCVL:Matrix:"
 _CIRCUIT_PREFIX = ":PCVL:ACircuit:"
 
 
 def deserialize_float(floatstring):
@@ -131,14 +132,22 @@
         for k, v in obj.items():
             r[deserialize(k)] = deserialize(v)
     elif isinstance(obj, list):
         r = []
         for k in obj:
             r.append(deserialize(k))
     elif isinstance(obj, str) and obj.startswith(":PCVL:"):
+        if obj.startswith(":PCVL:zip:"):
+            # if zip found -> update obj
+            # STEPS: remove prefix -> decode b64 encoding -> decompress -> decode utf-8 (byte-> str)
+            zip_prefix = ":PCVL:zip:"
+            obj = obj[len(zip_prefix):]
+            obj = b64decode(obj)
+            obj = (decompress(obj)).decode('utf-8')
+
         p = obj[6:].find(":")
         cl = obj[6:p+6]
         sobj = obj[p+7:]
         if cl == "BasicState":
             r = BasicState(sobj)
         elif cl == "StateVector":
             r = deserialize_statevector(sobj)
```

### Comparing `perceval-quandela-0.8.1/perceval/serialization/serialize_binary.py` & `perceval-quandela-0.9.0/perceval/serialization/serialize_binary.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/utils/__init__.py` & `perceval-quandela-0.9.0/perceval/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,19 +23,21 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from .matrix import Matrix, MatrixN, MatrixS
+from .matrix import Matrix, MatrixN, MatrixS, matrix_double
 from .format import simple_float, simple_complex, format_parameters
 from .parameter import Parameter, P, Expression, E
 from .mlstr import mlstr
 from .statevector import BasicState, StateVector, SVDistribution, BSDistribution, BSCount, BSSamples, \
-    tensorproduct, AnnotatedBasicState, allstate_iterator
-from .polarization import Polarization
-from .random import random_seed
+    tensorproduct, AnnotatedBasicState, allstate_iterator, anonymize_annotations
+from .polarization import Polarization, convert_polarized_state, build_spatial_output_states
+from .postselect import PostSelect
+from ._random import random_seed
 from .globals import global_params
 from .conversion import samples_to_sample_count, samples_to_probs, sample_count_to_samples, sample_count_to_probs,\
     probs_to_samples, probs_to_sample_count
+from .stategenerator import StateGenerator, Encoding
 from exqalibur import Annotation  # Used to provide the Annotation class to the perceval root namespace
```

### Comparing `perceval-quandela-0.8.1/perceval/utils/algorithms/__init__.py` & `perceval-quandela-0.9.0/perceval/simulators/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,9 +23,13 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from .match import Match
-import perceval.utils.algorithms.norm as norm
+from .delay_simulator import DelaySimulator
+from .loss_simulator import LossSimulator
+from .polarization_simulator import PolarizationSimulator
+from .simulator import Simulator
+from .simulator_factory import SimulatorFactory
+from .stepper import Stepper
```

### Comparing `perceval-quandela-0.8.1/perceval/utils/algorithms/circuit_optimizer.py` & `perceval-quandela-0.9.0/perceval/utils/algorithms/circuit_optimizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,19 +37,22 @@
     matrix. However, the optimizer will get as close as possible. The metric to measure the distance between the target
     unitary and the optimized interferometer is the matrix fidelity available in `perceval.utils.algorithms.norm`.
 
     CircuitOptimizer can be configured with the following parameters:
     :param threshold: Error threshold = 1-fidelity - i.e. the lower the threshold, the better the output fidelity
                       (default 1e-6)
     :param ntrials: Number of optimization trials (default 4)
+    :param max_eval_per_trial: maximum number of evaluations per optimization trial (default 200000)
     """
 
-    def __init__(self, threshold: float = 1e-6, ntrials: int = 4):
+    def __init__(self, threshold: float = 1e-6, ntrials: int = 4, max_eval_per_trial: int = 200000):
+
         self.threshold = threshold
         self.trials = ntrials
+        self.max_eval_per_trial = max_eval_per_trial
 
     @property
     def threshold(self):
         return self._threshold
 
     @threshold.setter
     def threshold(self, value):
@@ -61,14 +64,22 @@
     def trials(self):
         return self._trials
 
     @trials.setter
     def trials(self, value):
         self._trials = value
 
+    @property
+    def max_eval_per_trial(self):
+        return self._max_eval_per_trial
+
+    @max_eval_per_trial.setter
+    def max_eval_per_trial(self, value):
+        self._max_eval_per_trial = value
+
     def optimize(self,
                  target: Union[ACircuit, Matrix],
                  template: ACircuit
                  ) -> Tuple[ACircuit, float]:
         """
         Optimize a template circuit unitary's fidelity with a target matrix or circuit.
 
@@ -78,31 +89,31 @@
 
         >>> def mzi(i):
         >>>    return Circuit(2) // PS(P(f"phi_1_{i}")) // BS() // PS(P(f"phi_2_{i}")) // BS()
         >>> def ps(i):
         >>>    return PS(P(f"phi_3_{i}"))
         >>> template = Circuit.generic_interferometer(12, mzi, phase_shifter_fun_gen=ps, phase_at_output=True)
         >>> random_unitary = Matrix.random_unitary(12)
-        >>> fidelity, result_circuit = CircuitOptimizer().optimize(random_unitary, template)
+        >>> result_circuit, fidelity = CircuitOptimizer().optimize(random_unitary, template)
         """
         if isinstance(target, ACircuit):
             target = target.compute_unitary()
         assert template.m == target.shape[0], \
             f"Template circuit and target size should be the same ({template.m} != {target.m})"
         assert not target.is_symbolic(), "Target must not contain variables"
 
         optimizer = xq.CircuitOptimizer(serialize_binary(target), serialize_binary(template))
-        optimizer.set_max_eval_per_trial(50000)
+        optimizer.set_max_eval_per_trial(self._max_eval_per_trial)
         optimizer.set_threshold(self._threshold)
         optimized_circuit = deserialize_circuit(optimizer.optimize(self._trials))
         return optimized_circuit, optimizer.fidelity
 
     def optimize_rectangle(self,
                            target: Matrix,
-                           template_component_generator_func: Callable[[int],ACircuit] = None,
+                           template_component_generator_func: Callable[[int], ACircuit] = None,
                            phase_at_output: bool = True,
                            allow_error: bool = False,
                            ) -> ACircuit:
         """
         Optimize a rectangular circuit to reach a target unitary matrix fidelity.
 
         :param target: Target unitary matrix
```

### Comparing `perceval-quandela-0.8.1/perceval/utils/algorithms/decomposition.py` & `perceval-quandela-0.9.0/perceval/utils/algorithms/decomposition.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/utils/algorithms/match.py` & `perceval-quandela-0.9.0/perceval/utils/algorithms/match.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/utils/algorithms/norm.py` & `perceval-quandela-0.9.0/perceval/utils/algorithms/norm.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/utils/algorithms/optimize.py` & `perceval-quandela-0.9.0/perceval/utils/algorithms/optimize.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/utils/algorithms/simplification.py` & `perceval-quandela-0.9.0/perceval/utils/algorithms/simplification.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/utils/algorithms/solve.py` & `perceval-quandela-0.9.0/perceval/utils/algorithms/solve.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/utils/conversion.py` & `perceval-quandela-0.9.0/perceval/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/utils/format.py` & `perceval-quandela-0.9.0/perceval/utils/format.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/utils/globals.py` & `perceval-quandela-0.9.0/perceval/utils/_random.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,11 +23,21 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-global_params = {
-    "min_p": 1e-16,
-    "min_complex_component": 1e-6
-}
+import random
+import numpy as np
+
+
+def random_seed(seed=None):
+    """
+    seed: int = None
+    Initialize the seed used for random number generation
+
+    :param seed: if None, use a time-based seed
+    :return: the actual seed used
+    """
+    random.seed(seed)
+    np.random.seed(seed)
```

### Comparing `perceval-quandela-0.8.1/perceval/utils/matrix.py` & `perceval-quandela-0.9.0/perceval/utils/matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -286,7 +286,18 @@
 
     def inv(self) -> MatrixN:
         """returns inverse of the Matrix
 
         :return:
         """
         return np.linalg.inv(self)
+
+
+def matrix_double(u: Matrix):
+    m = u.shape[0]
+    pu = Matrix(m * 2, u.is_symbolic())
+    pu.fill(0)
+    for k1 in range(0, m):
+        for k2 in range(0, m):
+            pu[2 * k1, 2 * k2] = u[k1, k2]
+            pu[2 * k1 + 1, 2 * k2 + 1] = u[k1, k2]
+    return pu
```

### Comparing `perceval-quandela-0.8.1/perceval/utils/mlstr.py` & `perceval-quandela-0.9.0/perceval/utils/mlstr.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.8.1/perceval/utils/parameter.py` & `perceval-quandela-0.9.0/perceval/utils/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             if v > max_v:
                 p = int((v-max_v)/(max_v-min_v))
                 v = v - (p+1) * (max_v-min_v)
             elif v < min_v:
                 p = int((min_v-v)/(max_v-min_v))
                 v = v + (p+1) * (max_v-min_v)
         if (min_v is not None and v < min_v) or (max_v is not None and v > max_v):
-            raise ValueError("value %f out of bound [%f,%f]", v, min_v, max_v)
+            raise ValueError("value %f out of bound [%f,%f]" %(v, min_v, max_v))
         return v
 
     def check_value(self, v):
         return self._check_value(v, self._min, self._max, self._periodic)
 
     def set_value(self, v: float, force: bool = False):
         r"""Define the value of a non-fixed parameter
```

### Comparing `perceval-quandela-0.8.1/perceval/utils/polarization.py` & `perceval-quandela-0.9.0/perceval/utils/polarization.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,19 +24,23 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
-from typing import Union, Tuple, Any
 
+import numpy as np
 import re
 import sympy as sp
-import numpy as np
+from typing import Union, Tuple, Any
+
+from .statevector import BasicState
+from .matrix import Matrix
+
 
 class Polarization:
     r"""Polarization class
 
     This class is defined values used by polarization annotations `P`
 
     :param v: a string (``[HVADLR]``), a single angle or a pair of angle definition either symbolic or numeric.
@@ -55,15 +59,15 @@
             elif v == "A":
                 self.theta_phi = (sp.pi/2, sp.pi)
             elif v == "R":
                 self.theta_phi = (sp.pi/2, 3*sp.pi/2)
             elif v == "L":
                 self.theta_phi = (sp.pi/2, sp.pi/2)
             else:
-                raise ValueError("undefined value '%s' for polarization")
+                raise ValueError("undefined value '%s' for polarization" %v)
         elif isinstance(v, tuple):
             if len(v) != 2:
                 raise ValueError("Polarization is defined by 2 angles")
             for vs in v:
                 if isinstance(vs, sp.Expr):
                     if len(vs.free_symbols):
                         raise ValueError("Polarization cannot have variables")
@@ -153,7 +157,87 @@
             if self.theta_phi[1] == 3*sp.pi/2:
                 return "R"
             if self.theta_phi[1] == sp.pi/2:
                 return "L"
         if self.theta_phi[1] == 0:
             return str(self.theta_phi[0])
         return "(%s,%s)" % (str(self.theta_phi[0]), str(self.theta_phi[1]))
+
+
+def _rec_build_spatial_output_states(lfs: list, output: list):
+    if len(lfs) == 0:
+        yield BasicState(output)
+    else:
+        if lfs[0] == 0:
+            yield from _rec_build_spatial_output_states(lfs[1:], output+[0, 0])
+        else:
+            for k in range(lfs[0]+1):
+                yield from _rec_build_spatial_output_states(lfs[1:], output+[k, lfs[0]-k])
+
+
+def build_spatial_output_states(state: BasicState):
+    yield from _rec_build_spatial_output_states(list(state), [])
+
+
+def _is_orthogonal(v1, v2, use_symbolic):
+    if use_symbolic:
+        orth = sp.conjugate(v1[0]) * v2[0] + sp.conjugate(v1[1]) * v2[1]
+        return orth == 0
+    orth = np.conjugate(v1[0]) * v2[0] + np.conjugate(v1[1]) * v2[1]
+    return abs(orth) < 1e-6
+
+
+def convert_polarized_state(state: BasicState,
+                            use_symbolic: bool = False,
+                            inverse: bool = False) -> Tuple[BasicState, Matrix]:
+    r"""Convert a polarized BasicState into an expanded BasicState vector
+
+    :param inverse:
+    :param use_symbolic:
+    :param state:
+    :return:
+    """
+    idx = 0
+    input_state = []
+    prep_matrix = None
+    for k_m in range(state.m):
+        input_state += [0, 0]
+        if state[k_m]:
+            vectors = []
+            for k_n in range(state[k_m]):
+                # for each state we can handle up to two orthogonal vectors
+                annot = state.get_photon_annotation(idx)
+                idx += 1
+                v_hv = Polarization(annot.get("P", complex(Polarization(0)))).project_eh_ev(use_symbolic)
+                v_idx = None
+                for i, v in enumerate(vectors):
+                    if v == v_hv:
+                        v_idx = i
+                        break
+                if v_idx is None:
+                    if len(vectors) == 2:
+                        raise ValueError("use statevectors to handle more than 2 orthogonal vectors")
+                    if len(vectors) == 0 or _is_orthogonal(vectors[0], v_hv, use_symbolic):
+                        v_idx = len(vectors)
+                        vectors.append(v_hv)
+                    else:
+                        raise ValueError("use statevectors to handle non orthogonal vectors")
+                input_state[-2+v_idx] += 1
+            if vectors:
+                eh1, ev1 = vectors[0]
+                if len(vectors) == 1:
+                    if use_symbolic:
+                        eh2 = -sp.conjugate(ev1)
+                        ev2 = sp.conjugate(eh1)
+                    else:
+                        eh2 = -np.conjugate(ev1)
+                        ev2 = np.conjugate(eh1)
+                else:
+                    eh2, ev2 = vectors[1]
+                if prep_matrix is None:
+                    prep_matrix = Matrix.eye(2*state.m, use_symbolic)
+                prep_state_matrix = Matrix([[eh1, eh2],
+                                            [ev1, ev2]], use_symbolic)
+                if inverse:
+                    prep_state_matrix = prep_state_matrix.inv()
+                prep_matrix[2*k_m:2*k_m+2, 2*k_m:2*k_m+2] = prep_state_matrix
+    return BasicState(input_state), prep_matrix
```

### Comparing `perceval-quandela-0.8.1/perceval/utils/statevector.py` & `perceval-quandela-0.9.0/perceval/utils/statevector.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,96 +31,74 @@
 
 import random
 import warnings
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from copy import copy
 import itertools
+from multipledispatch import dispatch
 from typing import Dict, List, Union, Tuple, Optional
 from deprecated import deprecated
 
-from .matrix import Matrix
-from .format import simple_complex, simple_float
+from .format import simple_complex
 from .globals import global_params
-from .polarization import Polarization
 import numpy as np
 import sympy as sp
 
 from exqalibur import FockState, FSArray
 
 
-class BasicState(FockState):
-    r"""Basic states
-    """
-
-    def __init__(self, *args, **kwargs):
-        super(BasicState, self).__init__(*args, **kwargs)
-
-    def __len__(self):
-        return self.m
-
-    def __copy__(self):
-        return BasicState(self)
+def _fockstate_add(self, other):
+    return StateVector(self) + other
 
-    def __add__(self, o):
-        return StateVector(self) + o
+def _fockstate_sub(self, other):
+    return StateVector(self) - other
 
-    def __sub__(self, o):
-        if not isinstance(o, StateVector):
-            o = StateVector(o)
-        return StateVector(self) - o
-
-    def separate_state(self):
-        return [BasicState(s) for s in super(BasicState, self).separate_state()]
-
-    def __mul__(self, s):
-        if isinstance(s, StateVector):
-            return StateVector(self) * s
-        return BasicState(super(BasicState, self).__mul__(s))
+def _fockstate_pow(self, power: int):
+    bs = self.__copy__()
+    for i in range(power - 1):
+        bs = bs * self
+    return bs
 
-    def __pow__(self, power):
-        return BasicState(power * list(self))
+def _fockstate_partition(self, distribution_photons: List[int]):
+    r"""Given a distribution of photon, find all possible partition of the BasicState - disregard possible annotation
 
-    def __getitem__(self, item):
-        it = super().__getitem__(item)
-        if isinstance(it, FockState):
-            it = BasicState(it)
-        return it
-
-    def set_slice(self, slice, state):
-        return BasicState(super().set_slice(slice, state))
-
-    def partition(self, distribution_photons: List[int]):
-        r"""Given a distribution of photon, find all possible partition of the BasicState - disregard possible annotation
-
-        :param distribution_photons:
-        :return:
-        """
-        def _partition(one_list: list, distribution: list, current: list, all_res: list):
-            if len(distribution) == 0:
-                all_res.append(copy(current))
-                return
-            for one_subset in itertools.combinations(one_list, distribution[0]):
-                current.append(one_subset)
-                _partition(list(set(one_list)-set(one_subset)), distribution[1:], current, all_res)
-                current.pop()
-
-        all_photons = list(range(self.n))
-        partitions_idx = []
-        _partition(all_photons, distribution_photons, [], partitions_idx)
-        partitions_states = set()
-        for partition in partitions_idx:
-            o_state = []
-            for a_subset in partition:
-                state = [0] * self.m
-                for photon_id in a_subset:
-                    state[self.photon2mode(photon_id)] += 1
-                o_state.append(BasicState(state))
-            partitions_states.add(tuple(o_state))
-        return list(partitions_states)
+    :param distribution_photons:
+    :return:
+    """
+    def _partition(one_list: list, distribution: list, current: list, all_res: list):
+        if len(distribution) == 0:
+            all_res.append(copy(current))
+            return
+        for one_subset in itertools.combinations(one_list, distribution[0]):
+            current.append(one_subset)
+            _partition(list(set(one_list)-set(one_subset)), distribution[1:], current, all_res)
+            current.pop()
+
+    all_photons = list(range(self.n))
+    partitions_idx = []
+    _partition(all_photons, distribution_photons, [], partitions_idx)
+    partitions_states = set()
+    for partition in partitions_idx:
+        o_state = []
+        for a_subset in partition:
+            state = [0] * self.m
+            for photon_id in a_subset:
+                state[self.photon2mode(photon_id)] += 1
+            o_state.append(BasicState(state))
+        partitions_states.add(tuple(o_state))
+    return list(partitions_states)
+
+
+# Define BasicState as exqalibur FockState + redefine some methods
+BasicState = FockState
+BasicState.__add__ = _fockstate_add
+BasicState.__sub__ = _fockstate_sub
+BasicState.__pow__ = _fockstate_pow  # Using issue #210 fix before moving the fix to exqalibur
+BasicState.partition = _fockstate_partition  # TODO use the cpp version of this call
 
 
 def allstate_iterator(input_state: Union[BasicState, StateVector], mask=None) -> BasicState:
     """Iterator on all possible output states compatible with mask generating StateVector
 
     :param input_state: a given input state vector
     :param mask: an optional mask
@@ -250,15 +228,15 @@
             if i != len(binary) - 1:
                 power_state *= power_state
         return out
 
     def __copy__(self):
         sv_copy = StateVector(None)
         for k, v in self.items():
-            sv_copy[k] = v
+            sv_copy[copy(k)] = v
         sv_copy._has_symbolic = self._has_symbolic
         sv_copy._normalized = self._normalized
         sv_copy.m = self.m
         return sv_copy
 
     def __add__(self, other):
         r"""Add two StateVectors"""
@@ -279,14 +257,16 @@
         copy_state.m = self.m
         if other._has_symbolic:
             copy_state._has_symbolic = True
         return copy_state
 
     def __sub__(self, other):
         r"""Sub two StateVectors"""
+        if isinstance(other, BasicState):
+            other = StateVector(other)
         return self + -1 * other
 
     def sample(self) -> BasicState:
         r"""Sample a single BasicState from the statevector.
         It does not perform a measure - so do not change the value of the statevector
 
         :return: a BasicState
@@ -312,15 +292,16 @@
         """
         self.normalize()
         weight = [abs(self[key])**2 for key in self.keys()]
         rng = np.random.default_rng()
         return [BasicState(x) for x in rng.choice(list(self.keys()), shots, p=weight)]
 
     def measure(self, modes: Union[int, List[int]]) -> Dict[BasicState, Tuple[float, StateVector]]:
-        r"""perform a measure on one or multiple modes and collapse the remaining statevector
+        r"""perform a measure on one or multiple modes and collapse the remaining statevector. The resulting
+        statevector are not normalised by default.
 
         :param modes: the mode to measure
         :return: a dictionary - key is the possible measures, values are pairs (probability, BasicState vector)
         """
         self.normalize()
         if isinstance(modes, int):
             modes = [modes]
@@ -361,35 +342,38 @@
             for key in self.keys():
                 if nkey == 1:
                     self[key] = 1
                 else:
                     self[key] /= norm
             self._normalized = True
 
-    def __str__(self):
-        if not self:
+    def __str__(self, nsimplify=True):
+        if not self.keys():
             return "|>"
         self_copy = copy(self)
         self_copy.normalize()
         ls = []
         for key, value in self_copy.items():
             if value == 1:
                 ls.append(str(key))
             else:
                 if isinstance(value, sp.Expr):
                     ls.append(str(value) + "*" + str(key))
                 else:
-                    value = simple_complex(value)[1]
-                    if value[1:].find("-") != -1 or value.find("+") != -1:
-                        value = "("+value+")"
+                    if nsimplify:
+                        value = simple_complex(value)[1]
+                        if value[1:].find("-") != -1 or value.find("+") != -1:
+                            value = f"({value})"
+                    else:
+                        value = str(value)
                     ls.append( value + "*" + str(key))
         return "+".join(ls).replace("+-", "-")
 
     def __hash__(self):
-        return self.__str__().__hash__()
+        return self.__str__(nsimplify=False).__hash__()
 
 
 def tensorproduct(states: List[Union[StateVector, BasicState]]):
     r""" Computes states[0] * states[1] * ...
     """
     if len(states) == 1:
         return states[0]
@@ -407,28 +391,41 @@
         if sum_probs == 0:
             warnings.warn("Unable to normalize a distribution with only null probabilities")
             return
         for sv in self.keys():
             self[sv] /= sum_probs
 
     def add(self, obj, proba: float):
-        if proba != 0:
+        if proba > global_params['min_p']:
             self[obj] += proba
 
     def __str__(self):
         return "{\n  "\
-               + "\n  ".join(["%s: %s" % (str(k), simple_float(v, nsimplify=True)[1]) for k, v in self.items()])\
+               + "\n  ".join(["%s: %s" % (str(k), v) for k, v in self.items()])\
                + "\n}"
 
     def __copy__(self):
         distribution_copy = type(self)()
         for k, prob in self.items():
             distribution_copy[copy(k)] = prob
         return distribution_copy
 
+    def __pow__(self, power):
+        # Fast exponentiation
+        binary = [int(i) for i in bin(power)[2:]]
+        binary.reverse()
+        power_distrib = self
+        out = type(self)()
+        for i in range(len(binary)):
+            if binary[i] == 1:
+                out *= power_distrib
+            if i != len(binary) - 1:
+                power_distrib *= power_distrib
+        return out
+
     @abstractmethod
     def sample(self, count: int, non_null: bool = True):
         pass
 
 
 class SVDistribution(ProbabilityDistribution):
     r"""Time-Independent Probabilistic distribution of StateVectors
@@ -453,43 +450,30 @@
 
     def __getitem__(self, key):
         if isinstance(key, BasicState):
             key = StateVector(key)
         assert isinstance(key, StateVector), "SVDistribution key must be a BasicState or a StateVector"
         return super().__getitem__(key)
 
-    def __mul__(self, svd):
+    def __mul__(self, other):
         r"""Combines two `SVDistribution`
 
-        :param svd:
-        :return:
+        :param other: State / distribution to multiply with
+        :return: The result of the tensor product
         """
+        if isinstance(other, (BasicState, StateVector)):
+            other = SVDistribution(other)
         if len(self) == 0:
-            return svd
+            return other
         new_svd = SVDistribution()
         for sv1, proba1 in self.items():
-            for sv2, proba2 in svd.items():
-                # assert len(sv1) == 1 and len(sv2) == 1, "can only combine basic states"
+            for sv2, proba2 in other.items():
                 new_svd[sv1*sv2] = proba1 * proba2
-
         return new_svd
 
-    def __pow__(self, power):
-        # Fast exponentiation
-        binary = [int(i) for i in bin(power)[2:]]
-        binary.reverse()
-        power_svd = self
-        out = SVDistribution()
-        for i in range(len(binary)):
-            if binary[i] == 1:
-                out *= power_svd
-            if i != len(binary) - 1:
-                power_svd *= power_svd
-        return out
-
     def normalize(self):
         sum_probs = sum(list(self.values()))
         for sv in self.keys():
             self[sv] /= sum_probs
 
     def sample(self, count: int, non_null: bool = True) -> List[StateVector]:
         r""" Generate a sample StateVector from the `SVDistribution`
@@ -505,14 +489,40 @@
         states = list(d.keys())
         probs = list(d.values())
         rng = np.random.default_rng()
         results = rng.choice(states, count, p=np.array(probs) / sum(probs))
         return list(results)
 
 
+@dispatch(StateVector, annot_tag=str)
+def anonymize_annotations(sv: StateVector, annot_tag: str = "a"):
+    m = sv.m
+    annot_map = {}
+    result = StateVector()
+    for bs, pa in sv.items():
+        s = [""] * m
+        for i in range(bs.n):
+            mode = bs.photon2mode(i)
+            annot = bs.get_photon_annotation(i)
+            if annot_map.get(str(annot)) is None:
+                annot_map[str(annot)] = f"{{{annot_tag}:{len(annot_map)}}}"
+            s[mode] += annot_map[str(annot)]
+        result += StateVector("|" + ",".join([v and v or "0" for v in s]) + ">") * pa
+    result.normalize()
+    return result
+
+@dispatch(SVDistribution, annot_tag=str)
+def anonymize_annotations(svd: SVDistribution, annot_tag: str = "a"):
+    sv_dist = defaultdict(lambda: 0)
+    for k, p in svd.items():
+        state = anonymize_annotations(k, annot_tag=annot_tag)
+        sv_dist[state] += p
+    return SVDistribution({k: v for k, v in sorted(sv_dist.items(), key=lambda x: -x[1])})
+
+
 class BSDistribution(ProbabilityDistribution):
 
     def __init__(self, d: Optional[BasicState, Dict] = None):
         super().__init__()
         if d is not None:
             if isinstance(d, BasicState):
                 self[d] = 1
@@ -547,14 +557,33 @@
         # numpy transforms iterables of ints to a nparray in rng.choice call
         # Thus, we need to convert back the results to BasicStates
         output = BSSamples()
         for s in results:
             output.append(BasicState(s))
         return output
 
+    def __mul__(self, other):
+        return BSDistribution.tensor_product(self, other)
+
+    @staticmethod
+    def tensor_product(bsd1, bsd2, merge_modes: bool = False, prob_threshold: float = 0):
+        if len(bsd1) == 0:
+            return bsd2
+        new_dist = BSDistribution()
+        for bs1, proba1 in bsd1.items():
+            for bs2, proba2 in bsd2.items():
+                if proba1 * proba2 < prob_threshold:
+                    continue
+                if merge_modes:
+                    bs = bs1.merge(bs2)
+                else:
+                    bs = bs1 * bs2
+                new_dist[bs] += proba1 * proba2
+        return new_dist
+
 
 class BSCount(defaultdict):
     def __init__(self, d: Optional[Dict] = None):
         super().__init__(int)
         if d is not None:
             for k, v in d.items():
                 self[BasicState(k)] = v
@@ -588,87 +617,7 @@
         sz = len(self)
         n_to_display = min(sz, 10)
         s = '[' + ', '.join([str(bs) for bs in self[:n_to_display]])
         if sz > n_to_display:
             s += f', ... (size={sz})'
         s += ']'
         return s
-
-
-def _rec_build_spatial_output_states(lfs: list, output: list):
-    if len(lfs) == 0:
-        yield BasicState(output)
-    else:
-        if lfs[0] == 0:
-            yield from _rec_build_spatial_output_states(lfs[1:], output+[0, 0])
-        else:
-            for k in range(lfs[0]+1):
-                yield from _rec_build_spatial_output_states(lfs[1:], output+[k, lfs[0]-k])
-
-
-def build_spatial_output_states(state: BasicState):
-    yield from _rec_build_spatial_output_states(list(state), [])
-
-
-def _is_orthogonal(v1, v2, use_symbolic):
-    if use_symbolic:
-        orth = sp.conjugate(v1[0]) * v2[0] + sp.conjugate(v1[1]) * v2[1]
-        return orth == 0
-    orth = np.conjugate(v1[0]) * v2[0] + np.conjugate(v1[1]) * v2[1]
-    return abs(orth) < 1e-6
-
-
-def convert_polarized_state(state: BasicState,
-                            use_symbolic: bool = False,
-                            inverse: bool = False) -> Tuple[BasicState, Matrix]:
-    r"""Convert a polarized BasicState into an expanded BasicState vector
-
-    :param inverse:
-    :param use_symbolic:
-    :param state:
-    :return:
-    """
-    idx = 0
-    input_state = []
-    prep_matrix = None
-    for k_m in range(state.m):
-        input_state += [0, 0]
-        if state[k_m]:
-            vectors = []
-            for k_n in range(state[k_m]):
-                # for each state we can handle up to two orthogonal vectors
-                annot = state.get_photon_annotation(idx)
-                idx += 1
-                v_hv = Polarization(annot.get("P", complex(Polarization(0)))).project_eh_ev(use_symbolic)
-                v_idx = None
-                for i, v in enumerate(vectors):
-                    if v == v_hv:
-                        v_idx = i
-                        break
-                if v_idx is None:
-                    if len(vectors) == 2:
-                        raise ValueError("use statevectors to handle more than 2 orthogonal vectors")
-                    if len(vectors) == 0 or _is_orthogonal(vectors[0], v_hv, use_symbolic):
-                        v_idx = len(vectors)
-                        vectors.append(v_hv)
-                    else:
-                        raise ValueError("use statevectors to handle non orthogonal vectors")
-                input_state[-2+v_idx] += 1
-            if vectors:
-                eh1, ev1 = vectors[0]
-                if len(vectors) == 1:
-                    if use_symbolic:
-                        eh2 = -sp.conjugate(ev1)
-                        ev2 = sp.conjugate(eh1)
-                    else:
-                        eh2 = -np.conjugate(ev1)
-                        ev2 = np.conjugate(eh1)
-                else:
-                    eh2, ev2 = vectors[1]
-                if prep_matrix is None:
-                    prep_matrix = Matrix.eye(2*state.m, use_symbolic)
-                prep_state_matrix = Matrix([[eh1, eh2],
-                                            [ev1, ev2]], use_symbolic)
-                if inverse:
-                    prep_state_matrix = prep_state_matrix.inv()
-                prep_matrix[2*k_m:2*k_m+2, 2*k_m:2*k_m+2] = prep_state_matrix
-    return BasicState(input_state), prep_matrix
```

### Comparing `perceval-quandela-0.8.1/perceval_quandela.egg-info/PKG-INFO` & `perceval-quandela-0.9.0/perceval_quandela.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: perceval-quandela
-Version: 0.8.1
+Version: 0.9.0
 Summary: A powerful Quantum Photonic Framework
 Home-page: https://github.com/Quandela/Perceval
 Author: Perceval@Quandela.com
 Author-email: Perceval@Quandela.com
 Project-URL: Documentation, https://perceval.quandela.net/docs/
 Project-URL: Source, https://github.com/Quandela/Perceval
 Project-URL: Tracker, https://github.com/Quandela/Perceval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
 
 [![GitHub release](https://img.shields.io/github/v/release/Quandela/Perceval.svg?style=plastic)](https://github.com/Quandela/Perceval/releases/latest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Perceval?style=plastic)
 [![CI](https://github.com/Quandela/Perceval/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Quandela/Perceval/actions/workflows/python-publish.yml)
 
 [![CI](https://github.com/Quandela/Perceval/actions/workflows/autotests.yml/badge.svg)](https://github.com/Quandela/Perceval/actions/workflows/autotests.yml)
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: perceval-quandela Version: 0.8.1 Summary: A
+Metadata-Version: 2.1 Name: perceval-quandela Version: 0.9.0 Summary: A
 powerful Quantum Photonic Framework Home-page: https://github.com/Quandela/
 Perceval Author: Perceval@Quandela.com Author-email: Perceval@Quandela.com
 Project-URL: Documentation, https://perceval.quandela.net/docs/ Project-URL:
 Source, https://github.com/Quandela/Perceval Project-URL: Tracker, https://
 github.com/Quandela/Perceval/issues Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: test License-File: LICENSE [![GitHub release](https://
-img.shields.io/github/v/release/Quandela/Perceval.svg?style=plastic)](https://
-github.com/Quandela/Perceval/releases/latest) ![PyPI - Python Version](https://
+markdown License-File: LICENSE [![GitHub release](https://img.shields.io/
+github/v/release/Quandela/Perceval.svg?style=plastic)](https://github.com/
+Quandela/Perceval/releases/latest) ![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/Perceval?style=plastic) [![CI](https://
 github.com/Quandela/Perceval/actions/workflows/python-publish.yml/badge.svg)]
 (https://github.com/Quandela/Perceval/actions/workflows/python-publish.yml) [!
 [CI](https://github.com/Quandela/Perceval/actions/workflows/autotests.yml/
 badge.svg)](https://github.com/Quandela/Perceval/actions/workflows/
 autotests.yml) [![CI](https://github.com/Quandela/Perceval/actions/workflows/
 build-and-deploy-docs.yml/badge.svg)](https://github.com/Quandela/Perceval/
```

### Comparing `perceval-quandela-0.8.1/perceval_quandela.egg-info/SOURCES.txt` & `perceval-quandela-0.9.0/perceval_quandela.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -6,49 +6,48 @@
 perceval/__init__.py
 perceval/algorithm/__init__.py
 perceval/algorithm/abstract_algorithm.py
 perceval/algorithm/analyzer.py
 perceval/algorithm/qrng.py
 perceval/algorithm/sampler.py
 perceval/backends/__init__.py
-perceval/backends/cliffords2017.py
-perceval/backends/mps.py
-perceval/backends/naive.py
-perceval/backends/slos.py
-perceval/backends/template.py
-perceval/backends/processor/__init__.py
-perceval/backends/processor/stepper.py
+perceval/backends/_abstract_backends.py
+perceval/backends/_clifford2017.py
+perceval/backends/_mps.py
+perceval/backends/_naive.py
+perceval/backends/_slos.py
 perceval/components/__init__.py
 perceval/components/_mode_connector.py
 perceval/components/abstract_component.py
 perceval/components/abstract_processor.py
 perceval/components/component_catalog.py
 perceval/components/detector.py
 perceval/components/linear_circuit.py
 perceval/components/non_unitary_components.py
 perceval/components/port.py
 perceval/components/predefined_circuit.py
 perceval/components/processor.py
 perceval/components/source.py
 perceval/components/unitary_components.py
-perceval/components/computation/__init__.py
-perceval/components/computation/time_delays.py
 perceval/components/core_catalog/__init__.py
 perceval/components/core_catalog/generic_2mode.py
 perceval/components/core_catalog/heralded_cnot.py
+perceval/components/core_catalog/heralded_cz.py
 perceval/components/core_catalog/postprocessed_cnot.py
 perceval/converters/__init__.py
+perceval/converters/converter_statevector.py
 perceval/converters/qiskit_converter.py
 perceval/rendering/__init__.py
 perceval/rendering/_mplot_utils.py
 perceval/rendering/_processor_utils.py
 perceval/rendering/format.py
 perceval/rendering/pdisplay.py
 perceval/rendering/canvas/__init__.py
 perceval/rendering/canvas/canvas.py
+perceval/rendering/canvas/latex_canvas.py
 perceval/rendering/canvas/mplot_canvas.py
 perceval/rendering/canvas/svg_canvas.py
 perceval/rendering/circuit/__init__.py
 perceval/rendering/circuit/abstract_skin.py
 perceval/rendering/circuit/phys_skin.py
 perceval/rendering/circuit/renderer.py
 perceval/rendering/circuit/skin_common.py
@@ -66,23 +65,34 @@
 perceval/serialization/_matrix_serialization.py
 perceval/serialization/_parameter_serialization.py
 perceval/serialization/_schema_circuit_pb2.py
 perceval/serialization/_state_serialization.py
 perceval/serialization/deserialize.py
 perceval/serialization/serialize.py
 perceval/serialization/serialize_binary.py
+perceval/simulators/__init__.py
+perceval/simulators/_simulator_utils.py
+perceval/simulators/delay_simulator.py
+perceval/simulators/loss_simulator.py
+perceval/simulators/polarization_simulator.py
+perceval/simulators/simulator.py
+perceval/simulators/simulator_factory.py
+perceval/simulators/simulator_interface.py
+perceval/simulators/stepper.py
 perceval/utils/__init__.py
+perceval/utils/_random.py
 perceval/utils/conversion.py
 perceval/utils/format.py
 perceval/utils/globals.py
 perceval/utils/matrix.py
 perceval/utils/mlstr.py
 perceval/utils/parameter.py
 perceval/utils/polarization.py
-perceval/utils/random.py
+perceval/utils/postselect.py
+perceval/utils/stategenerator.py
 perceval/utils/statevector.py
 perceval/utils/algorithms/__init__.py
 perceval/utils/algorithms/circuit_optimizer.py
 perceval/utils/algorithms/decomposition.py
 perceval/utils/algorithms/match.py
 perceval/utils/algorithms/norm.py
 perceval/utils/algorithms/optimize.py
```

### Comparing `perceval-quandela-0.8.1/setup.py` & `perceval-quandela-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,13 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=package_list,
-    install_requires=['sympy', 'numpy', 'scipy', 'tabulate', 'matplotlib', 'exqalibur~=0.1.0', 'multipledispatch',
-                      'protobuf>=4.21.2', 'drawsvg>=2.0', 'Deprecated', 'requests'],
+    install_requires=['sympy', 'numpy', 'scipy', 'tabulate', 'matplotlib', 'exqalibur~=0.2.0', 'multipledispatch',
+                      'protobuf>=3.20.3', 'drawsvg>=2.0', 'Deprecated', 'requests', 'networkx~=3.1', 'latexcodec'],
     setup_requires=["scmver"],
-    extras_require={"test": ["pytest", "pytest-cov", "pytest-benchmark"]},
     python_requires=">=3.7",
     scmver=True
 )
```

