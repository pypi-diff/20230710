# Comparing `tmp/openvino_model_api-0.1.2.tar.gz` & `tmp/openvino_model_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvino_model_api-0.1.2.tar", last modified: Wed Jun  7 12:34:17 2023, max compression
+gzip compressed data, was "openvino_model_api-0.1.3.tar", last modified: Mon Jul 10 12:17:39 2023, max compression
```

## Comparing `openvino_model_api-0.1.2.tar` & `openvino_model_api-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 wov       (1000) wov       (1000)        0 2023-06-07 12:34:17.423834 openvino_model_api-0.1.2/
--rw-rw-r--   0 wov       (1000) wov       (1000)     6935 2023-06-07 12:34:17.423834 openvino_model_api-0.1.2/PKG-INFO
-drwxrwxr-x   0 wov       (1000) wov       (1000)        0 2023-06-07 12:34:17.423834 openvino_model_api-0.1.2/openvino_model_api.egg-info/
--rw-rw-r--   0 wov       (1000) wov       (1000)     6935 2023-06-07 12:34:17.000000 openvino_model_api-0.1.2/openvino_model_api.egg-info/PKG-INFO
--rw-rw-r--   0 wov       (1000) wov       (1000)     2996 2023-06-07 12:34:17.000000 openvino_model_api-0.1.2/openvino_model_api.egg-info/SOURCES.txt
--rw-rw-r--   0 wov       (1000) wov       (1000)        1 2023-06-07 12:34:17.000000 openvino_model_api-0.1.2/openvino_model_api.egg-info/dependency_links.txt
--rw-rw-r--   0 wov       (1000) wov       (1000)      157 2023-06-07 12:34:17.000000 openvino_model_api-0.1.2/openvino_model_api.egg-info/requires.txt
--rw-rw-r--   0 wov       (1000) wov       (1000)        9 2023-06-07 12:34:17.000000 openvino_model_api-0.1.2/openvino_model_api.egg-info/top_level.txt
--rw-rw-r--   0 wov       (1000) wov       (1000)       38 2023-06-07 12:34:17.423834 openvino_model_api-0.1.2/setup.cfg
--rwxrwxr-x   0 wov       (1000) wov       (1000)     1636 2023-06-07 09:20:54.000000 openvino_model_api-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:17:39.342082 openvino_model_api-0.1.3/
+-rw-rw-rw-   0        0        0     7087 2023-07-10 12:17:39.342082 openvino_model_api-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-10 12:17:39.342082 openvino_model_api-0.1.3/openvino_model_api.egg-info/
+-rw-rw-rw-   0        0        0     7087 2023-07-10 12:17:39.000000 openvino_model_api-0.1.3/openvino_model_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3588 2023-07-10 12:17:39.000000 openvino_model_api-0.1.3/openvino_model_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 12:17:39.000000 openvino_model_api-0.1.3/openvino_model_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-07-10 12:17:39.000000 openvino_model_api-0.1.3/openvino_model_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 12:17:39.000000 openvino_model_api-0.1.3/openvino_model_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 12:17:39.342082 openvino_model_api-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1681 2023-06-10 06:44:08.000000 openvino_model_api-0.1.3/setup.py
```

### Comparing `openvino_model_api-0.1.2/PKG-INFO` & `openvino_model_api-0.1.3/openvino_model_api.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-Metadata-Version: 2.1
-Name: openvino_model_api
-Version: 0.1.2
-Summary: Model API: model wrappers and pipelines for inference with OpenVINO
-Home-page: https://github.com/openvinotoolkit/model_api
-Author: Intel(R) Corporation
-License: OSI Approved :: Apache Software License
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: ovms
-Provides-Extra: tests
-
-# OpenVINO Model API
-Model API is a set of wrapper classes for particular tasks and model architectures, simplifying data preprocess and postprocess as well as routine procedures (model loading, asynchronous execution, etc.). It is aimed at simplifying end-to-end model inference for different deployment scenarious, including local execution and serving. The Model API is based on the OpenVINO inference API.
-
-## How it works
-Model API searches for additional information required for model inference, data, pre/postprocessing, label names, etc. directly in OpenVINO Intermediate Representation. This information is used to prepare the inference data, process and ouput the inference results in a human-readable format.
-
-## Features
-- Python and C++ API
-- Automatic prefetch of public models from [OpenVINO Model Zoo](https://github.com/openvinotoolkit/open_model_zoo) (Python only)
-- Syncronous and asynchronous inference
-- Local inference and servring through the rest API (Python only)
-- Model preprocessing embedding for faster inference
-
-## Installation
-### Python
-- Clone this repository
-- Navigate to `model_api/python` folder
-- Run `pip install .`
-### C++
-- Install dependencies. For installation on Ubuntu, you can use the following script:
-  ```bash
-  chmod +x model_api/cpp/install_dependencies.sh
-  sudo model_api/cpp/install_dependencies.sh
-  ```
-
-- Build library:
-   - Create `build` folder and navigate into it:
-   ```
-   mkdir build && cd build
-   ```
-   - Run cmake:
-   ```
-   cmake ../model_api/cpp -DOpenCV_DIR=<OpenCV cmake dir> -DOpenVINO_DIR=<OpenVINO cmake dir>
-   ```
-   - Build:
-   ```
-   cmake --build . -j
-   ```
-   - To build a `.tar.gz` package with the library, run:
-   ```
-    make package
-    ```
-
-## Usage
-### Python
-```python
-from openvino.model_api.models import DetectionModel
-
-# Create a model (downloaded and cached automatically for OpenVINO Model Zoo models)
-# Use URL to work with served model, e.g. "localhost:9000/models/ssd300"
-ssd = DetectionModel.create_model("ssd300")
-
-# Run synchronous inference locally
-detections = ssd(image)  # image is numpy.ndarray
-
-# Print the list of Detection objects with box coordinates, confidence and label string
-print(f"Detection results: {detections}")
-```
-
-### C++
-```cpp
-#include <models/detection_model.h>
-#include <models/results.h>
-
-// Load the model fetched using Python API
-auto model = DetectionModel::create_model("~/.cache/omz/public/ssd300/FP16/ssd300.xml");
-
-// Run synchronous inference locally
-auto result = model->infer(image); // image is cv::Mat
-
-// Iterate over the vector of DetectedObject with box coordinates, confidence and label string
-for (auto& obj : result->objects) {
-    std::cout << obj.label << " | " << obj.confidence << " | " << int(obj.x) << " | " << int(obj.y) << " | "
-        << int(obj.x + obj.width) << " | " << int(obj.y + obj.height) << std::endl;
-}
-```
-
-Model's static method `create_model()` has two overloads. One constructs the model from a string (a path or a model name) (shown above) and the other takes an already constructed `InferenceAdapter`.
-
-# Prepare a model for `InferenceAdapter`
-There are usecases when it is not possible to modify an internal `ov::Model` and it is hidden behind `InferenceAdapter`. For example the model can be served using [OVMS](https://github.com/openvinotoolkit/model_server). `create_model()` can construct a model from a given `InferenceAdapter`. That approach assumes that the model in `InferenceAdapter` was already configured by `create_model()` called with a string (a path or a model name). It is possible to prepare such model using C++ or Python:
-C++
-```Cpp
-auto model = DetectionModel::create_model("~/.cache/omz/public/ssd300/FP16/ssd300.xml");
-const std::shared_ptr<ov::Model>& ov_model = model->getModel();
-ov::serialize(ov_model, "serialized.xml");
-```
-Python
-```python
-model = DetectionModel.create_model("~/.cache/omz/public/ssd300/FP16/ssd300.xml")
-model.save("serialized.xml")
-```
-After that the model can be constructed from `InferenceAdapter`:
-```cpp
-ov::Core core;
-std::shared_ptr<ov::Model> ov_model = core.read_model("serialized.xml");
-std::shared_ptr<InferenceAdapter> adapter = std::make_shared<OpenVINOInferenceAdapter>();
-adapter->loadModel(ov_model, core);
-auto model = DetectionModel::create_model(adapter);
-```
-
-For more details please refer to the [examples](https://github.com/openvinotoolkit/model_api/tree/master/examples) of this project.
-
-## Supported models
-### Python:
-- Image Classification:
-  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#classification-models)
-- Object Detection:
-  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#object-detection-models):
-    - SSD-based models (e.g. "ssd300", "ssdlite_mobilenet_v2", etc.)
-    - YOLO-based models (e.g. "yolov3", "yolov4", etc.)
-    - CTPN: "ctpn"
-    - DETR: "detr-resnet50"
-    - CenterNet: "ctdet_coco_dlav0_512"
-    - FaceBoxes: "faceboxes-pytorch"
-    - RetinaFace: "retinaface-resnet50-pytorch"
-    - Ultra Lightweight Face Detection: "ultra-lightweight-face-detection-rfb-320" and "ultra-lightweight-face-detection-slim-320"
-    - NanoDet with ShuffleNetV2: "nanodet-m-1.5x-416"
-    - NanoDet Plus with ShuffleNetV2: "nanodet-plus-m-1.5x-416"
-- Semantic Segmentation:
-  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#semantic-segmentation-models)
-- Instance Segmentation:
-  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#instance-segmentation-models)
-
-
-### C++:
-- Image Classification:
-  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#classification-models)
-- Object Detection:
-  - SSD-based models (e.g. "ssd300", "ssdlite_mobilenet_v2", etc.)
-    - YOLO-based models (e.g. "yolov3", "yolov4", etc.)
-    - CenterNet: "ctdet_coco_dlav0_512"
-    - FaceBoxes: "faceboxes-pytorch"
-    - RetinaFace: "retinaface-resnet50-pytorch"
-- Semantic Segmentation:
-  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#semantic-segmentation-models)
-
-[Model configuration](https://github.com/openvinotoolkit/model_api/blob/master/docs/model-configuration.md) discusses possible configurations.
+Metadata-Version: 2.1
+Name: openvino-model-api
+Version: 0.1.3
+Summary: Model API: model wrappers and pipelines for inference with OpenVINO
+Home-page: https://github.com/openvinotoolkit/model_api
+Author: Intel(R) Corporation
+License: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: ovms
+Provides-Extra: tests
+
+# OpenVINO Model API
+Model API is a set of wrapper classes for particular tasks and model architectures, simplifying data preprocess and postprocess as well as routine procedures (model loading, asynchronous execution, etc.). It is aimed at simplifying end-to-end model inference for different deployment scenarious, including local execution and serving. The Model API is based on the OpenVINO inference API.
+
+## How it works
+Model API searches for additional information required for model inference, data, pre/postprocessing, label names, etc. directly in OpenVINO Intermediate Representation. This information is used to prepare the inference data, process and ouput the inference results in a human-readable format.
+
+## Features
+- Python and C++ API
+- Automatic prefetch of public models from [OpenVINO Model Zoo](https://github.com/openvinotoolkit/open_model_zoo) (Python only)
+- Syncronous and asynchronous inference
+- Local inference and servring through the rest API (Python only)
+- Model preprocessing embedding for faster inference
+
+## Installation
+### Python
+- Clone this repository
+- Navigate to `model_api/python` folder
+- Run `pip install .`
+### C++
+- Install dependencies. For installation on Ubuntu, you can use the following script:
+  ```bash
+  chmod +x model_api/cpp/install_dependencies.sh
+  sudo model_api/cpp/install_dependencies.sh
+  ```
+
+- Build library:
+   - Create `build` folder and navigate into it:
+   ```
+   mkdir build && cd build
+   ```
+   - Run cmake:
+   ```
+   cmake ../model_api/cpp -DOpenCV_DIR=<OpenCV cmake dir> -DOpenVINO_DIR=<OpenVINO cmake dir>
+   ```
+   - Build:
+   ```
+   cmake --build . -j
+   ```
+   - To build a `.tar.gz` package with the library, run:
+   ```
+    make package
+    ```
+
+## Usage
+### Python
+```python
+from openvino.model_api.models import DetectionModel
+
+# Create a model (downloaded and cached automatically for OpenVINO Model Zoo models)
+# Use URL to work with served model, e.g. "localhost:9000/models/ssd300"
+ssd = DetectionModel.create_model("ssd300")
+
+# Run synchronous inference locally
+detections = ssd(image)  # image is numpy.ndarray
+
+# Print the list of Detection objects with box coordinates, confidence and label string
+print(f"Detection results: {detections}")
+```
+
+### C++
+```cpp
+#include <models/detection_model.h>
+#include <models/results.h>
+
+// Load the model fetched using Python API
+auto model = DetectionModel::create_model("~/.cache/omz/public/ssd300/FP16/ssd300.xml");
+
+// Run synchronous inference locally
+auto result = model->infer(image); // image is cv::Mat
+
+// Iterate over the vector of DetectedObject with box coordinates, confidence and label string
+for (auto& obj : result->objects) {
+    std::cout << obj.label << " | " << obj.confidence << " | " << int(obj.x) << " | " << int(obj.y) << " | "
+        << int(obj.x + obj.width) << " | " << int(obj.y + obj.height) << std::endl;
+}
+```
+
+Model's static method `create_model()` has two overloads. One constructs the model from a string (a path or a model name) (shown above) and the other takes an already constructed `InferenceAdapter`.
+
+# Prepare a model for `InferenceAdapter`
+There are usecases when it is not possible to modify an internal `ov::Model` and it is hidden behind `InferenceAdapter`. For example the model can be served using [OVMS](https://github.com/openvinotoolkit/model_server). `create_model()` can construct a model from a given `InferenceAdapter`. That approach assumes that the model in `InferenceAdapter` was already configured by `create_model()` called with a string (a path or a model name). It is possible to prepare such model using C++ or Python:
+C++
+```Cpp
+auto model = DetectionModel::create_model("~/.cache/omz/public/ssd300/FP16/ssd300.xml");
+const std::shared_ptr<ov::Model>& ov_model = model->getModel();
+ov::serialize(ov_model, "serialized.xml");
+```
+Python
+```python
+model = DetectionModel.create_model("~/.cache/omz/public/ssd300/FP16/ssd300.xml")
+model.save("serialized.xml")
+```
+After that the model can be constructed from `InferenceAdapter`:
+```cpp
+ov::Core core;
+std::shared_ptr<ov::Model> ov_model = core.read_model("serialized.xml");
+std::shared_ptr<InferenceAdapter> adapter = std::make_shared<OpenVINOInferenceAdapter>();
+adapter->loadModel(ov_model, core);
+auto model = DetectionModel::create_model(adapter);
+```
+
+For more details please refer to the [examples](https://github.com/openvinotoolkit/model_api/tree/master/examples) of this project.
+
+## Supported models
+### Python:
+- Image Classification:
+  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#classification-models)
+- Object Detection:
+  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#object-detection-models):
+    - SSD-based models (e.g. "ssd300", "ssdlite_mobilenet_v2", etc.)
+    - YOLO-based models (e.g. "yolov3", "yolov4", etc.)
+    - CTPN: "ctpn"
+    - DETR: "detr-resnet50"
+    - CenterNet: "ctdet_coco_dlav0_512"
+    - FaceBoxes: "faceboxes-pytorch"
+    - RetinaFace: "retinaface-resnet50-pytorch"
+    - Ultra Lightweight Face Detection: "ultra-lightweight-face-detection-rfb-320" and "ultra-lightweight-face-detection-slim-320"
+    - NanoDet with ShuffleNetV2: "nanodet-m-1.5x-416"
+    - NanoDet Plus with ShuffleNetV2: "nanodet-plus-m-1.5x-416"
+- Semantic Segmentation:
+  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#semantic-segmentation-models)
+- Instance Segmentation:
+  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#instance-segmentation-models)
+
+
+### C++:
+- Image Classification:
+  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#classification-models)
+- Object Detection:
+  - SSD-based models (e.g. "ssd300", "ssdlite_mobilenet_v2", etc.)
+    - YOLO-based models (e.g. "yolov3", "yolov4", etc.)
+    - CenterNet: "ctdet_coco_dlav0_512"
+    - FaceBoxes: "faceboxes-pytorch"
+    - RetinaFace: "retinaface-resnet50-pytorch"
+- Semantic Segmentation:
+  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#semantic-segmentation-models)
+
+[Model configuration](https://github.com/openvinotoolkit/model_api/blob/master/docs/model-configuration.md) discusses possible configurations.
```

### Comparing `openvino_model_api-0.1.2/openvino_model_api.egg-info/PKG-INFO` & `openvino_model_api-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-Metadata-Version: 2.1
-Name: openvino-model-api
-Version: 0.1.2
-Summary: Model API: model wrappers and pipelines for inference with OpenVINO
-Home-page: https://github.com/openvinotoolkit/model_api
-Author: Intel(R) Corporation
-License: OSI Approved :: Apache Software License
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: ovms
-Provides-Extra: tests
-
-# OpenVINO Model API
-Model API is a set of wrapper classes for particular tasks and model architectures, simplifying data preprocess and postprocess as well as routine procedures (model loading, asynchronous execution, etc.). It is aimed at simplifying end-to-end model inference for different deployment scenarious, including local execution and serving. The Model API is based on the OpenVINO inference API.
-
-## How it works
-Model API searches for additional information required for model inference, data, pre/postprocessing, label names, etc. directly in OpenVINO Intermediate Representation. This information is used to prepare the inference data, process and ouput the inference results in a human-readable format.
-
-## Features
-- Python and C++ API
-- Automatic prefetch of public models from [OpenVINO Model Zoo](https://github.com/openvinotoolkit/open_model_zoo) (Python only)
-- Syncronous and asynchronous inference
-- Local inference and servring through the rest API (Python only)
-- Model preprocessing embedding for faster inference
-
-## Installation
-### Python
-- Clone this repository
-- Navigate to `model_api/python` folder
-- Run `pip install .`
-### C++
-- Install dependencies. For installation on Ubuntu, you can use the following script:
-  ```bash
-  chmod +x model_api/cpp/install_dependencies.sh
-  sudo model_api/cpp/install_dependencies.sh
-  ```
-
-- Build library:
-   - Create `build` folder and navigate into it:
-   ```
-   mkdir build && cd build
-   ```
-   - Run cmake:
-   ```
-   cmake ../model_api/cpp -DOpenCV_DIR=<OpenCV cmake dir> -DOpenVINO_DIR=<OpenVINO cmake dir>
-   ```
-   - Build:
-   ```
-   cmake --build . -j
-   ```
-   - To build a `.tar.gz` package with the library, run:
-   ```
-    make package
-    ```
-
-## Usage
-### Python
-```python
-from openvino.model_api.models import DetectionModel
-
-# Create a model (downloaded and cached automatically for OpenVINO Model Zoo models)
-# Use URL to work with served model, e.g. "localhost:9000/models/ssd300"
-ssd = DetectionModel.create_model("ssd300")
-
-# Run synchronous inference locally
-detections = ssd(image)  # image is numpy.ndarray
-
-# Print the list of Detection objects with box coordinates, confidence and label string
-print(f"Detection results: {detections}")
-```
-
-### C++
-```cpp
-#include <models/detection_model.h>
-#include <models/results.h>
-
-// Load the model fetched using Python API
-auto model = DetectionModel::create_model("~/.cache/omz/public/ssd300/FP16/ssd300.xml");
-
-// Run synchronous inference locally
-auto result = model->infer(image); // image is cv::Mat
-
-// Iterate over the vector of DetectedObject with box coordinates, confidence and label string
-for (auto& obj : result->objects) {
-    std::cout << obj.label << " | " << obj.confidence << " | " << int(obj.x) << " | " << int(obj.y) << " | "
-        << int(obj.x + obj.width) << " | " << int(obj.y + obj.height) << std::endl;
-}
-```
-
-Model's static method `create_model()` has two overloads. One constructs the model from a string (a path or a model name) (shown above) and the other takes an already constructed `InferenceAdapter`.
-
-# Prepare a model for `InferenceAdapter`
-There are usecases when it is not possible to modify an internal `ov::Model` and it is hidden behind `InferenceAdapter`. For example the model can be served using [OVMS](https://github.com/openvinotoolkit/model_server). `create_model()` can construct a model from a given `InferenceAdapter`. That approach assumes that the model in `InferenceAdapter` was already configured by `create_model()` called with a string (a path or a model name). It is possible to prepare such model using C++ or Python:
-C++
-```Cpp
-auto model = DetectionModel::create_model("~/.cache/omz/public/ssd300/FP16/ssd300.xml");
-const std::shared_ptr<ov::Model>& ov_model = model->getModel();
-ov::serialize(ov_model, "serialized.xml");
-```
-Python
-```python
-model = DetectionModel.create_model("~/.cache/omz/public/ssd300/FP16/ssd300.xml")
-model.save("serialized.xml")
-```
-After that the model can be constructed from `InferenceAdapter`:
-```cpp
-ov::Core core;
-std::shared_ptr<ov::Model> ov_model = core.read_model("serialized.xml");
-std::shared_ptr<InferenceAdapter> adapter = std::make_shared<OpenVINOInferenceAdapter>();
-adapter->loadModel(ov_model, core);
-auto model = DetectionModel::create_model(adapter);
-```
-
-For more details please refer to the [examples](https://github.com/openvinotoolkit/model_api/tree/master/examples) of this project.
-
-## Supported models
-### Python:
-- Image Classification:
-  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#classification-models)
-- Object Detection:
-  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#object-detection-models):
-    - SSD-based models (e.g. "ssd300", "ssdlite_mobilenet_v2", etc.)
-    - YOLO-based models (e.g. "yolov3", "yolov4", etc.)
-    - CTPN: "ctpn"
-    - DETR: "detr-resnet50"
-    - CenterNet: "ctdet_coco_dlav0_512"
-    - FaceBoxes: "faceboxes-pytorch"
-    - RetinaFace: "retinaface-resnet50-pytorch"
-    - Ultra Lightweight Face Detection: "ultra-lightweight-face-detection-rfb-320" and "ultra-lightweight-face-detection-slim-320"
-    - NanoDet with ShuffleNetV2: "nanodet-m-1.5x-416"
-    - NanoDet Plus with ShuffleNetV2: "nanodet-plus-m-1.5x-416"
-- Semantic Segmentation:
-  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#semantic-segmentation-models)
-- Instance Segmentation:
-  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#instance-segmentation-models)
-
-
-### C++:
-- Image Classification:
-  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#classification-models)
-- Object Detection:
-  - SSD-based models (e.g. "ssd300", "ssdlite_mobilenet_v2", etc.)
-    - YOLO-based models (e.g. "yolov3", "yolov4", etc.)
-    - CenterNet: "ctdet_coco_dlav0_512"
-    - FaceBoxes: "faceboxes-pytorch"
-    - RetinaFace: "retinaface-resnet50-pytorch"
-- Semantic Segmentation:
-  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#semantic-segmentation-models)
-
-[Model configuration](https://github.com/openvinotoolkit/model_api/blob/master/docs/model-configuration.md) discusses possible configurations.
+Metadata-Version: 2.1
+Name: openvino_model_api
+Version: 0.1.3
+Summary: Model API: model wrappers and pipelines for inference with OpenVINO
+Home-page: https://github.com/openvinotoolkit/model_api
+Author: Intel(R) Corporation
+License: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: ovms
+Provides-Extra: tests
+
+# OpenVINO Model API
+Model API is a set of wrapper classes for particular tasks and model architectures, simplifying data preprocess and postprocess as well as routine procedures (model loading, asynchronous execution, etc.). It is aimed at simplifying end-to-end model inference for different deployment scenarious, including local execution and serving. The Model API is based on the OpenVINO inference API.
+
+## How it works
+Model API searches for additional information required for model inference, data, pre/postprocessing, label names, etc. directly in OpenVINO Intermediate Representation. This information is used to prepare the inference data, process and ouput the inference results in a human-readable format.
+
+## Features
+- Python and C++ API
+- Automatic prefetch of public models from [OpenVINO Model Zoo](https://github.com/openvinotoolkit/open_model_zoo) (Python only)
+- Syncronous and asynchronous inference
+- Local inference and servring through the rest API (Python only)
+- Model preprocessing embedding for faster inference
+
+## Installation
+### Python
+- Clone this repository
+- Navigate to `model_api/python` folder
+- Run `pip install .`
+### C++
+- Install dependencies. For installation on Ubuntu, you can use the following script:
+  ```bash
+  chmod +x model_api/cpp/install_dependencies.sh
+  sudo model_api/cpp/install_dependencies.sh
+  ```
+
+- Build library:
+   - Create `build` folder and navigate into it:
+   ```
+   mkdir build && cd build
+   ```
+   - Run cmake:
+   ```
+   cmake ../model_api/cpp -DOpenCV_DIR=<OpenCV cmake dir> -DOpenVINO_DIR=<OpenVINO cmake dir>
+   ```
+   - Build:
+   ```
+   cmake --build . -j
+   ```
+   - To build a `.tar.gz` package with the library, run:
+   ```
+    make package
+    ```
+
+## Usage
+### Python
+```python
+from openvino.model_api.models import DetectionModel
+
+# Create a model (downloaded and cached automatically for OpenVINO Model Zoo models)
+# Use URL to work with served model, e.g. "localhost:9000/models/ssd300"
+ssd = DetectionModel.create_model("ssd300")
+
+# Run synchronous inference locally
+detections = ssd(image)  # image is numpy.ndarray
+
+# Print the list of Detection objects with box coordinates, confidence and label string
+print(f"Detection results: {detections}")
+```
+
+### C++
+```cpp
+#include <models/detection_model.h>
+#include <models/results.h>
+
+// Load the model fetched using Python API
+auto model = DetectionModel::create_model("~/.cache/omz/public/ssd300/FP16/ssd300.xml");
+
+// Run synchronous inference locally
+auto result = model->infer(image); // image is cv::Mat
+
+// Iterate over the vector of DetectedObject with box coordinates, confidence and label string
+for (auto& obj : result->objects) {
+    std::cout << obj.label << " | " << obj.confidence << " | " << int(obj.x) << " | " << int(obj.y) << " | "
+        << int(obj.x + obj.width) << " | " << int(obj.y + obj.height) << std::endl;
+}
+```
+
+Model's static method `create_model()` has two overloads. One constructs the model from a string (a path or a model name) (shown above) and the other takes an already constructed `InferenceAdapter`.
+
+# Prepare a model for `InferenceAdapter`
+There are usecases when it is not possible to modify an internal `ov::Model` and it is hidden behind `InferenceAdapter`. For example the model can be served using [OVMS](https://github.com/openvinotoolkit/model_server). `create_model()` can construct a model from a given `InferenceAdapter`. That approach assumes that the model in `InferenceAdapter` was already configured by `create_model()` called with a string (a path or a model name). It is possible to prepare such model using C++ or Python:
+C++
+```Cpp
+auto model = DetectionModel::create_model("~/.cache/omz/public/ssd300/FP16/ssd300.xml");
+const std::shared_ptr<ov::Model>& ov_model = model->getModel();
+ov::serialize(ov_model, "serialized.xml");
+```
+Python
+```python
+model = DetectionModel.create_model("~/.cache/omz/public/ssd300/FP16/ssd300.xml")
+model.save("serialized.xml")
+```
+After that the model can be constructed from `InferenceAdapter`:
+```cpp
+ov::Core core;
+std::shared_ptr<ov::Model> ov_model = core.read_model("serialized.xml");
+std::shared_ptr<InferenceAdapter> adapter = std::make_shared<OpenVINOInferenceAdapter>();
+adapter->loadModel(ov_model, core);
+auto model = DetectionModel::create_model(adapter);
+```
+
+For more details please refer to the [examples](https://github.com/openvinotoolkit/model_api/tree/master/examples) of this project.
+
+## Supported models
+### Python:
+- Image Classification:
+  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#classification-models)
+- Object Detection:
+  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#object-detection-models):
+    - SSD-based models (e.g. "ssd300", "ssdlite_mobilenet_v2", etc.)
+    - YOLO-based models (e.g. "yolov3", "yolov4", etc.)
+    - CTPN: "ctpn"
+    - DETR: "detr-resnet50"
+    - CenterNet: "ctdet_coco_dlav0_512"
+    - FaceBoxes: "faceboxes-pytorch"
+    - RetinaFace: "retinaface-resnet50-pytorch"
+    - Ultra Lightweight Face Detection: "ultra-lightweight-face-detection-rfb-320" and "ultra-lightweight-face-detection-slim-320"
+    - NanoDet with ShuffleNetV2: "nanodet-m-1.5x-416"
+    - NanoDet Plus with ShuffleNetV2: "nanodet-plus-m-1.5x-416"
+- Semantic Segmentation:
+  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#semantic-segmentation-models)
+- Instance Segmentation:
+  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#instance-segmentation-models)
+
+
+### C++:
+- Image Classification:
+  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#classification-models)
+- Object Detection:
+  - SSD-based models (e.g. "ssd300", "ssdlite_mobilenet_v2", etc.)
+    - YOLO-based models (e.g. "yolov3", "yolov4", etc.)
+    - CenterNet: "ctdet_coco_dlav0_512"
+    - FaceBoxes: "faceboxes-pytorch"
+    - RetinaFace: "retinaface-resnet50-pytorch"
+- Semantic Segmentation:
+  - [OpenVINO Model Zoo models](https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md#semantic-segmentation-models)
+
+[Model configuration](https://github.com/openvinotoolkit/model_api/blob/master/docs/model-configuration.md) discusses possible configurations.
```

### Comparing `openvino_model_api-0.1.2/setup.py` & `openvino_model_api-0.1.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-#!/usr/bin/env python3
-"""
- Copyright (c) 2021-2023 Intel Corporation
-
- Licensed under the Apache License, Version 2.0 (the "License");
- you may not use this file except in compliance with the License.
- You may obtain a copy of the License at
-
-      http://www.apache.org/licenses/LICENSE-2.0
-
- Unless required by applicable law or agreed to in writing, software
- distributed under the License is distributed on an "AS IS" BASIS,
- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
- See the License for the specific language governing permissions and
- limitations under the License.
-"""
-
-from pathlib import Path
-
-from setuptools import find_packages, setup
-
-SETUP_DIR = Path(__file__).resolve().parent
-
-setup(
-    name="openvino_model_api",
-    version="0.1.2",
-    description="Model API: model wrappers and pipelines for inference with OpenVINO",
-    author="Intel(R) Corporation",
-    url="https://github.com/openvinotoolkit/model_api",
-    packages=find_packages(SETUP_DIR),
-    package_dir={"openvino": str(SETUP_DIR / "openvino")},
-    classifiers=[
-        "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3",
-    ],
-    license="OSI Approved :: Apache Software License",
-    python_requires=">=3.7",
-    install_requires=(SETUP_DIR / "requirements.txt").read_text(),
-    extras_require={
-        "ovms": (SETUP_DIR / "requirements_ovms.txt").read_text(),
-        "tests": ["pytest", "openvino-dev[onnx,pytorch,tensorflow2]"],
-    },
-    long_description=(SETUP_DIR.parents[1] / "README.md").read_text(),
-    long_description_content_type="text/markdown",
-)
+#!/usr/bin/env python3
+"""
+ Copyright (c) 2021-2023 Intel Corporation
+
+ Licensed under the Apache License, Version 2.0 (the "License");
+ you may not use this file except in compliance with the License.
+ You may obtain a copy of the License at
+
+      http://www.apache.org/licenses/LICENSE-2.0
+
+ Unless required by applicable law or agreed to in writing, software
+ distributed under the License is distributed on an "AS IS" BASIS,
+ WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+ See the License for the specific language governing permissions and
+ limitations under the License.
+"""
+
+from pathlib import Path
+
+from setuptools import find_packages, setup
+
+SETUP_DIR = Path(__file__).resolve().parent
+
+setup(
+    name="openvino_model_api",
+    version="0.1.3",
+    description="Model API: model wrappers and pipelines for inference with OpenVINO",
+    author="Intel(R) Corporation",
+    url="https://github.com/openvinotoolkit/model_api",
+    packages=find_packages(SETUP_DIR),
+    package_dir={"openvino": str(SETUP_DIR / "openvino")},
+    classifiers=[
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python :: 3",
+    ],
+    license="OSI Approved :: Apache Software License",
+    python_requires=">=3.7",
+    install_requires=(SETUP_DIR / "requirements.txt").read_text(),
+    extras_require={
+        "ovms": (SETUP_DIR / "requirements_ovms.txt").read_text(),
+        "tests": ["pytest", "openvino-dev[onnx,pytorch,tensorflow2]"],
+    },
+    long_description=(SETUP_DIR.parents[1] / "README.md").read_text(),
+    long_description_content_type="text/markdown",
+)
```

