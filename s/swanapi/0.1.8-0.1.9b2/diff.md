# Comparing `tmp/swanapi-0.1.8-py3-none-any.whl.zip` & `tmp/swanapi-0.1.9b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 9341 bytes, number of entries: 14
--rw-r--r--  2.0 unx       62 b- defN 23-Jul-08 12:12 swanapi/__init__.py
--rw-r--r--  2.0 unx     7611 b- defN 23-Jul-09 11:38 swanapi/base_inference.py
+Zip file size: 11147 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      158 b- defN 23-Jul-10 19:07 swanapi/__init__.py
+-rw-r--r--  2.0 unx    10349 b- defN 23-Jul-10 20:37 swanapi/base_inference.py
 -rw-r--r--  2.0 unx      863 b- defN 23-Jul-09 17:55 swanapi/make_build.py
--rw-r--r--  2.0 unx     1850 b- defN 23-Jul-09 16:44 swanapi/server.py
+-rw-r--r--  2.0 unx     2759 b- defN 23-Jul-10 19:56 swanapi/server.py
+-rw-r--r--  2.0 unx      562 b- defN 23-Jul-10 19:06 swanapi/swan_types.py
 -rw-r--r--  2.0 unx     1065 b- defN 23-Jul-09 07:52 swanapi/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 09:38 swanapi/docker_builder/__init__.py
 -rw-r--r--  2.0 unx     3889 b- defN 23-Jul-09 18:35 swanapi/docker_builder/config.py
--rw-r--r--  2.0 unx     3338 b- defN 23-Jul-09 18:35 swanapi/docker_builder/generate_dockerfile.py
+-rw-r--r--  2.0 unx     3348 b- defN 23-Jul-09 18:53 swanapi/docker_builder/generate_dockerfile.py
 -rw-r--r--  2.0 unx     1419 b- defN 23-Jul-09 18:39 swanapi/docker_builder/runner.py
--rw-r--r--  2.0 unx      347 b- defN 23-Jul-09 18:39 swanapi-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 18:39 swanapi-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Jul-09 18:39 swanapi-0.1.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-09 18:39 swanapi-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1139 b- defN 23-Jul-09 18:39 swanapi-0.1.8.dist-info/RECORD
-14 files, 21733 bytes uncompressed, 7437 bytes compressed:  65.8%
+-rw-r--r--  2.0 unx      349 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1228 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/RECORD
+15 files, 26139 bytes uncompressed, 9105 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: swanapi/make_build.py
 Comment: 
 
 Filename: swanapi/server.py
 Comment: 
 
+Filename: swanapi/swan_types.py
+Comment: 
+
 Filename: swanapi/utils.py
 Comment: 
 
 Filename: swanapi/docker_builder/__init__.py
 Comment: 
 
 Filename: swanapi/docker_builder/config.py
@@ -21,23 +24,23 @@
 
 Filename: swanapi/docker_builder/generate_dockerfile.py
 Comment: 
 
 Filename: swanapi/docker_builder/runner.py
 Comment: 
 
-Filename: swanapi-0.1.8.dist-info/METADATA
+Filename: swanapi-0.1.9b2.dist-info/METADATA
 Comment: 
 
-Filename: swanapi-0.1.8.dist-info/WHEEL
+Filename: swanapi-0.1.9b2.dist-info/WHEEL
 Comment: 
 
-Filename: swanapi-0.1.8.dist-info/entry_points.txt
+Filename: swanapi-0.1.9b2.dist-info/entry_points.txt
 Comment: 
 
-Filename: swanapi-0.1.8.dist-info/top_level.txt
+Filename: swanapi-0.1.9b2.dist-info/top_level.txt
 Comment: 
 
-Filename: swanapi-0.1.8.dist-info/RECORD
+Filename: swanapi-0.1.9b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swanapi/__init__.py

```diff
@@ -1,3 +1,5 @@
 from .server import SwanInference
+from .base_inference import SwanRequests
+from .swan_types import Files
 
-__all__ = ["SwanInference"]
+__all__ = ["SwanInference", "SwanRequests", "Files"]
```

## swanapi/base_inference.py

```diff
@@ -1,165 +1,237 @@
 from .utils import check_elements_in_list, is_float, is_list, is_dict
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 import inspect
 import numpy as np
 import cv2
 import base64
+import requests
+from .swan_types import Files
 
 
 class BaseInference:
     def __init__(self):
         # self.mode's options - ["both", "input_only", "output_only"]
         self.mode = "both"
         self.fn = None
-        self.inputs = None
-        self.outputs = None
+        self.backbone_inputs = None
+        self.backbone_outputs = None
         self.signature = None
         self.fn_param_names = None
         self.TYPES = {
             "text": str,
             "image": Union[bytes, str],
             "number": Union[int, float],
             "list": list,
             "dict": dict,
         }
         self.types_list = list(self.TYPES.keys())
         self.outputs_typing = None
-        self.prediction_inputs = None
-        self.prediction_inputs_keys = None
-        self.prediction_output_num_variables = None
+        self.requests_inputs = None
+        self.requests_inputs_param_names = None
+        self.requests_outputs_variables_num = None
 
-    def inference_type_checker(self) -> None:
+    def backbone_type_checker(self) -> None:
         # 如果fn是列表，报错
         if isinstance(self.fn, list):
             raise DeprecationWarning(
                 "The `fn` parameter only accepts a single function, support for a list "
                 "of functions has been deprecated."
             )
 
         # 如果输入、输出定义为None或空列表，报错
-        if (self.inputs is None or self.inputs == []) and (self.outputs is None or self.outputs == []):
+        if (self.backbone_inputs is None or self.backbone_inputs == []) and \
+                (self.backbone_outputs is None or self.backbone_outputs == []):
             raise ValueError("Must provide at least one of `inputs` or `outputs`")
         # 如果输出为空，但是输入不为空
-        elif self.outputs is None or self.outputs == []:
-            self.outputs = []
+        elif self.backbone_outputs is None or self.backbone_outputs == []:
+            self.backbone_outputs = []
             self.mode = "input_only"
         # 如果输入为空，但是输出不为空
-        elif self.inputs is None or self.inputs == []:
-            self.inputs = []
+        elif self.backbone_inputs is None or self.backbone_inputs == []:
+            self.backbone_inputs = []
             self.mode = "output_only"
 
         # 类型检查: 输入、输出的类型是否为str或list, 如果类型是str，转换为list
-        assert isinstance(self.inputs, (str, list))
-        assert isinstance(self.outputs, (str, list))
-        if not isinstance(self.inputs, list):
-            self.inputs = [self.inputs]
-        if not isinstance(self.outputs, list):
-            self.outputs = [self.outputs]
+        assert isinstance(self.backbone_inputs, (str, list))
+        assert isinstance(self.backbone_outputs, (str, list))
+        if not isinstance(self.backbone_inputs, list):
+            self.backbone_inputs = [self.backbone_inputs]
+        if not isinstance(self.backbone_outputs, list):
+            self.backbone_outputs = [self.backbone_outputs]
 
-        # 类型检查: 输入的类型是否在io_types中
+        # 类型检查: 输入的类型是否在self.types_list中
         if self.mode == "both":
-            assert check_elements_in_list(self.inputs, self.types_list)
-            assert check_elements_in_list(self.outputs, self.types_list)
+            assert check_elements_in_list(self.backbone_inputs, self.types_list)
+            assert check_elements_in_list(self.backbone_outputs, self.types_list)
         elif self.mode == "input_only":
-            assert check_elements_in_list(self.inputs, self.types_list)
+            assert check_elements_in_list(self.backbone_inputs, self.types_list)
         else:
-            assert check_elements_in_list(self.outputs, self.types_list)
+            assert check_elements_in_list(self.backbone_outputs, self.types_list)
 
-    def get_fn_information(self) -> None:
-        # 得到fn函数的签名信息
-        self.signature = inspect.signature(self.fn)
-
-        # 得到fn函数的参数名
-        self.fn_param_names = [param for param in self.signature.parameters]
-
-        # 判断输入的数量是否与定义的一致
-        assert len(self.fn_param_names) == len(self.inputs), ValueError("输入的数量与定义的不一致")
-
-    def prediction_input_type_checker(self, inputs: Dict[str, Any]) -> None:
-        self.prediction_inputs = inputs
-
-        self.prediction_inputs_keys = list(self.prediction_inputs.keys())
-        assert check_elements_in_list(self.prediction_inputs_keys, self.fn_param_names)  # 判断请求输入的参数名是否与定义的一致
+    def backbone_get_fn_parameters(self) -> None:
+        # 使用inspect库，得到fn函数的签名变量
+        signature = inspect.signature(self.fn)
+
+        # 得到fn函数的参数名列表，形如["input_image", "input_text"]
+        self.fn_param_names = [param for param in signature.parameters]
+
+        # 判断inputs的数量是否大于fn定义的数量
+        # 如果大于，则报错
+        # 如果小于，则截取fn定义的前len(inputs)个参数
+        if len(self.fn_param_names) < len(self.backbone_inputs):
+            raise ValueError("SwanInference中inputs的长度不应该大于fn的参数个数")
+        else:
+            self.fn_param_names = self.fn_param_names[: len(self.backbone_inputs)]
 
-    def prediction_input_converter(self) -> None:
-        # 根据post输入类型，做相应的转换
-        for iter, (keys, values) in enumerate(self.prediction_inputs.items()):
+    def requests_input_type_checker(self, requests_inputs: Dict[str, Any]) -> None:
+        """
+        检查网络请求的输入参数：
+        1. 长度是否合格-与len(self.backbones)相等
+        2. 参数名是否与self.fn_param_names匹配
+        """
+        # self.requests_inputs - 用户输入的完整json字典
+        self.requests_inputs = requests_inputs
+        # 获取网络请求的参数个数
+        self.requests_inputs_param_names = list(self.requests_inputs.keys())
+        # 判断网络请求输入的参数的个数是否与inputs定义的个数一致
+        assert len(self.requests_inputs_param_names) == len(self.backbone_inputs), "请求传入的参数数量与inputs定义的不一致"
+        # 判断网络请求输入的参数名是否与fn定义的一致
+        assert check_elements_in_list(self.requests_inputs_param_names, self.fn_param_names), "请求传入的参数key与fn定义的不一致"
+
+    def requests_input_converter(self) -> None:
+        # 对于每一个requests内容的输入类型，做相应的转换
+        for iter, param_name in enumerate(self.fn_param_names):
+            # param_name : 'input_image', 'custom_size_height', 'custom_size_width'
+            # 获取内容values
+            values = self.requests_inputs[param_name]
             # 对于输入的类型为image的情况
-            if self.inputs[iter] == "image":
+            if self.backbone_inputs[iter] == "image":
                 if isinstance(values, bytes):
-                    self.prediction_inputs[keys] = cv2.imdecode(np.frombuffer(values, np.uint8), cv2.IMREAD_UNCHANGED)
+
+                    self.requests_inputs[param_name] = \
+                        cv2.cvtColor(cv2.imdecode(np.frombuffer(values, np.uint8), cv2.IMREAD_COLOR),
+                                     cv2.COLOR_RGB2BGR)
                 # 如果输入的是字符串，则作为图像路径处理
                 elif isinstance(values, str):
-                    self.prediction_inputs[keys] = cv2.imread(values, cv2.IMREAD_UNCHANGED)
+                    self.requests_inputs[param_name] = cv2.imread(values, cv2.IMREAD_UNCHANGED)
                 else:
-                    raise TypeError("输入的类型与定义的image类型不一致")
+                    raise TypeError("网络请求中{}的类型与定义的image类型不一致".format(param_name))
 
             # 对于输入的类型为number的情况
-            elif self.inputs[iter] == "number":
-                assert is_float(values), "输入的类型与定义的number类型不一致"
-                self.prediction_inputs[keys] = float(values)
+            elif self.backbone_inputs[iter] == "number":
+                assert is_float(values), "网络请求中{}的类型与定义的number类型不一致".format(param_name)
+                self.requests_inputs[param_name] = float(values)
+
             # 对于输入的类型为text的情况
-            elif self.inputs[iter] == "text":
-                assert isinstance(values, str), "输入的类型与定义的text类型不一致"
-                self.prediction_inputs[keys] = values
+            elif self.backbone_inputs[iter] == "text":
+                assert isinstance(values, str), "网络请求中{}的类型与定义的text类型不一致".format(param_name)
+                self.requests_inputs[param_name] = values
+
             # 对于输入的类型为list的情况
-            elif self.inputs[iter] == "list":
-                self.prediction_inputs[keys] = is_list(values)
+            elif self.backbone_inputs[iter] == "list":
+                self.requests_inputs[param_name] = is_list(values)
+
             # 对于输入的类型为dict的情况
-            elif self.inputs[iter] == self.TYPES["dict"]:
-                self.prediction_inputs[keys] = is_dict(values)
+            elif self.backbone_inputs[iter] == "dict":
+                self.requests_inputs[param_name] = is_dict(values)
+
             else:
-                raise TypeError("输入的类型与定义的不一致")
+                raise TypeError("backbone_type_checker have BUGs")
 
-    def prediction_output_type_checker(self, result: Any) -> None:
-        # 判断返回值类型是否为元组
+    def requests_output_type_checker(self, result: Any) -> None:
+        # 根据result得到返回变量数量
         if isinstance(result, tuple):
-            self.prediction_output_num_variables = len(result)
+            self.requests_outputs_variables_num = len(result)
+        # Todo:对于输出为0/None的兼容性开发
         elif result is None:
-            self.prediction_output_num_variables = 0
+            self.requests_outputs_variables_num = 0
         else:
-            self.prediction_output_num_variables = 1
+            self.requests_outputs_variables_num = 1
 
-        assert self.prediction_output_num_variables == len(self.outputs), "输出的数量与定义的不一致"
+        assert self.requests_outputs_variables_num == len(self.backbone_outputs), "fn输出的数量与outputs定义的不一致"
 
-    def prediction_output_converter(self, result: Any) -> Dict[str, Any]:
-        # 如果输出的变量数量1
-        if self.prediction_output_num_variables == 1:
-            if self.outputs == ["image"]:
-                assert isinstance(result, np.ndarray)
-                result = cv2.imencode(".jpg", result)[1].tostring()
-                result = base64.b64encode(result)
-            elif self.outputs == ["text"]:
-                assert isinstance(result, str)
-            elif self.outputs == ["number"]:
-                assert isinstance(result, (int, float))
-            elif self.outputs == ["dict"]:
-                assert isinstance(result, dict)
-            elif self.outputs == ["list"]:
-                assert isinstance(result, list)
-            result_json = {"content": result}
-        # 如果输出的变量数量>=2
-        elif self.prediction_output_num_variables >= 2:
+    def requests_output_converter(self, result: Any) -> Union[Dict[str, Any], None]:
+        if self.requests_outputs_variables_num == 1:
+            result = [result]
+        elif self.requests_outputs_variables_num > 1:
             result = list(result)
-            result_json = {}
-            for iter, output in enumerate(self.outputs):
-                if output == "image":
-                    assert isinstance(result[iter], np.ndarray)
-                    result[iter] = cv2.imencode(".jpg", result[iter])[1].tostring()
-                    result_json[iter] = {"content": base64.b64encode(result[iter])}
-                elif output == "text":
-                    assert isinstance(result[iter], str)
-                    result_json[iter] = {"content": result[iter]}
-                elif output == "number":
-                    assert isinstance(result[iter], (int, float))
-                    result_json[iter] = {"content": result[iter]}
-                elif self.outputs == ["dict"]:
-                    assert isinstance(result, dict)
-                    result_json[iter] = {"content": result[iter]}
-                elif self.outputs == ["list"]:
-                    assert isinstance(result, list)
-                    result_json[iter] = {"content": result[iter]}
         else:
-            result_json = {"content": None}
+            return None
+        result_json = {}
+        for iter, backbone_output in enumerate(self.backbone_outputs):
+            if result[iter] is None:
+                result_json[iter] = {"content": None}
+            elif backbone_output == "image":
+                assert isinstance(result[iter], np.ndarray)
+                result[iter] = cv2.cvtColor(result[iter], cv2.COLOR_RGB2BGR)
+                result[iter] = cv2.imencode(".jpg", result[iter])[1].tostring()
+                result_json[iter] = {"content": base64.b64encode(result[iter])}
+            elif backbone_output == "text":
+                assert isinstance(result[iter], str)
+                result_json[iter] = {"content": result[iter]}
+            elif backbone_output == "number":
+                assert isinstance(result[iter], (int, float))
+                result_json[iter] = {"content": result[iter]}
+            elif backbone_output == ["dict"]:
+                assert isinstance(result, dict)
+                result_json[iter] = {"content": result[iter]}
+            elif backbone_output == ["list"]:
+                assert isinstance(result, list)
+                result_json[iter] = {"content": result[iter]}
+            else:
+                raise TypeError("类型检查模块存在Bug")
 
         return result_json
+
+
+class BaseRequests:
+    """
+    增加在Python端快速调用SwanAPI服务的类。
+    主要降低API调用的门槛，尤其是对图像等数据类型。
+    必要输入：
+    - url: str, API的url地址
+    - inputs: Json
+    - methods: 请求的类型，可选值为["GET", "POST", "PUT", "DELETE"]
+    """
+
+    def base_request(self,
+                     url: str,
+                     inputs: Dict[str, Any],
+                     methods: str):
+        payload = {}
+        files = []
+        headers = {}
+
+        for key, value in inputs.items():
+            # 如果value的类型是文件类型
+            if isinstance(value, Files):
+                files.append((key, value.content()))
+            else:
+                payload[key] = value
+
+        inputs_dict = {}
+        if len(files) != 0:
+            inputs_dict['files'] = files
+        if len(payload) != 0:
+            inputs_dict['data'] = payload
+
+        response = requests.request(methods, url, headers=headers, **inputs_dict)
+        return response.json()
+
+    def post(self,
+             url: str,
+             inputs: Dict[str, Any],
+             ):
+        return self.base_request(url, inputs, "POST")
+
+    def get(self,
+            url: str,
+            inputs: Dict[str, Any],
+            ):
+        return self.base_request(url, inputs, "get")
+
+
+def SwanRequests(url: str,
+                 inputs: Dict[str, Any],
+                 methods: str = "POST"):
+    return BaseRequests().base_request(url, inputs, methods)
```

## swanapi/server.py

```diff
@@ -4,54 +4,78 @@
 from .base_inference import BaseInference
 import json
 
 app = Flask("SwanAPI Server")
 
 
 class SwanInference(BaseInference):
+    """
+    我们将分为两个生命周期：
+    1. Backbone: 以fn, inputs和outputs为基础，构建一个推理骨架
+    2. Requests: 接受Web请求，将Web请求转换为推理函数的输入，将推理函数的输出转换为Web请求的输出
+    """
+
     def __init__(self):
         super().__init__()
 
     def inference(self,
                   fn: Callable,
                   inputs: Union[list[str], str, None] = None,
                   outputs: Union[list[str], str, None] = None,
                   description: str = None
                   ) -> None:
+        """
+        用户构建backbone的入口函数
+        """
         self.fn = fn
-        self.inputs = inputs
-        self.outputs = outputs
+        self.backbone_inputs = inputs
+        self.backbone_outputs = outputs
         self.description = description
+        self.backbone()
 
+    def backbone(self) -> None:
+        """
+        以fn, inputs和outputs为基础，构建一个推理骨架Backbone
+        """
         # 检查fn、inputs和outputs的类型是否符合规范
-        self.inference_type_checker()
+        self.backbone_type_checker()
         # 得到fn的形参名称
-        self.get_fn_information()
-
-    def prediction(self, **inputs):
-        # 检查Web输入的类型是否符合规范
-        self.prediction_input_type_checker(inputs)
-        # 根据类型转换为推理函数的输入
-        self.prediction_input_converter()
+        self.backbone_get_fn_parameters()
 
-        result = self.fn(**self.prediction_inputs)
-
-        self.prediction_output_type_checker(result)
-        result_json = self.prediction_output_converter(result)
+    def requests(self, **inputs):
+        # 检查Web输入的类型是否符合Backbone定义的输入类型
+        self.requests_input_type_checker(inputs)
+        # 根据类型转换为符合Backbone定义的输入类型
+        self.requests_input_converter()
+
+        # 调用fn, 得到结果
+        result = self.fn(**self.requests_inputs)
+
+        # 检查结果是否符合Backbone定义的输出类型
+        self.requests_output_type_checker(result)
+        # 根据Backbone定义的输出类型进行转换
+        result_json = self.requests_output_converter(result)
 
+        # 将结果转换为json格式
         return json.dumps(result_json, default=bytes_encoder)
 
     def launch(self,
-               server_name="0.0.0.0",
-               port=8000
-               ):
+               server_name: str = "0.0.0.0",
+               port: int = 8000
+               ) -> None:
+        """
+        启动Web服务, 基于Flask
+        :param server_name: 又被称为Host, 表示IP地址
+        :param port: 端口号
+        """
+
         @app.route("/predictions/", methods=["POST", "GET"])
         def get_prediction():
             inputs = request.form.to_dict()
             files = request.files
             file_data = {}
             for field_name, file in files.items():
                 file_data[field_name] = file.read()
             inputs.update(file_data)
-            return self.prediction(**inputs)
+            return self.requests(**inputs)
 
         app.run(host=server_name, port=port)
```

## swanapi/docker_builder/generate_dockerfile.py

```diff
@@ -52,15 +52,15 @@
 
     def get_apt_packages(self):
         if self.config.system_packages is not None:
             apt_packages = ""
             for package in self.config.system_packages:
                 apt_packages += package + " "
             return """
-RUN apt-get install -y --no-install-recommends {}
+RUN apt-get install -y --no-install-recommends {} \n
 """.format(apt_packages)
         else:
             return ""
 
     def get_python_packages(self, prepackages):
         prepackages_text = ""
         package_text = ""
@@ -68,24 +68,24 @@
         if len(prepackages) == 0 and len(self.config.python_packages) == 0:
             return ""
         if len(prepackages) != 0:
             for prepackage in prepackages:
                 prepackages_text += " pip3 install --no-cache-dir {} ".format(prepackage)
                 if prepackage != prepackages[-1]:
                     prepackages_text += "&& \ \n   "
-            prepackages_text = "RUN" + prepackages_text
+            prepackages_text = "RUN" + prepackages_text + "\n"
 
         if len(self.config.python_packages) != 0:
             for package in self.config.python_packages:
                 package_text += " pip3 install --no-cache-dir {} ".format(package)
                 if package != self.config.python_packages[-1]:
                     package_text += "&& \ \n   "
-            package_text = "RUN" + package_text
+            package_text = "RUN" + package_text + '\n'
 
-        return prepackages_text + "\n" + package_text + "\n"
+        return prepackages_text + '\n' + package_text
 
     def get_clean(self):
         return """
 RUN echo "==> Clean up..."  && \ 
     rm -rf ~/.cache/pip
     """
```

## Comparing `swanapi-0.1.8.dist-info/RECORD` & `swanapi-0.1.9b2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-swanapi/__init__.py,sha256=T69A5YM84uwabbMeLbIZuDpk6R7ZcA51IrNFJOfRyq8,62
-swanapi/base_inference.py,sha256=rx-hZRfL4fK91zkqt2O134gZS7_hmG893gWUWXGatkE,7611
+swanapi/__init__.py,sha256=h4WVKn4K78msugS-evjCc2iydSU5K8lyGYHeJm3vcQM,158
+swanapi/base_inference.py,sha256=udI0rNdobPZLRS_-qUXnbQ4cbJsoBeew2Q0UzwfUklk,10349
 swanapi/make_build.py,sha256=P4WsA52pftJyNLrU986UKkYPY88VLzRMgQJ6s_UUTY0,863
-swanapi/server.py,sha256=VYblGUvpBEYKb4NN5cXWFvybXqU5o9qsMNpdf01bp2o,1850
+swanapi/server.py,sha256=_8CvGMp69-WSvNr6zfZlAb6-Mnxi1b-H9daH2vkXEpE,2759
+swanapi/swan_types.py,sha256=6rjoLVOqyahSQXilAVtMVS4e50MNeCMEBinPu3jR_JE,562
 swanapi/utils.py,sha256=VE09kmCHcSnPzCgCRdumEu5vnKjMwFAzWl29FoU6vs0,1065
 swanapi/docker_builder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swanapi/docker_builder/config.py,sha256=CspWGMAyxZz_rd2JecCrsC4nL75Zh3o7XGAXMVHa32o,3889
-swanapi/docker_builder/generate_dockerfile.py,sha256=o9WDfAlemjxP17gy0inWU1mF3HJG05PQtsyOeEzk51c,3338
+swanapi/docker_builder/generate_dockerfile.py,sha256=bbd2u94MgyZq883WrTtk936TM-6eUYTuc1ZqgVdgM90,3348
 swanapi/docker_builder/runner.py,sha256=uDToZ5UfgshahcnKbu8Eb7enLLry2pVHn7e2bJB56vk,1419
-swanapi-0.1.8.dist-info/METADATA,sha256=xATSodZjDMUR8t23ytcvzDbrLbOD5l_lRYyZr9VapRA,347
-swanapi-0.1.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swanapi-0.1.8.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
-swanapi-0.1.8.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
-swanapi-0.1.8.dist-info/RECORD,,
+swanapi-0.1.9b2.dist-info/METADATA,sha256=xQB2b5pTSJxvPa-OBXu8KJ51kMLan0jMKDwmWcjv3tw,349
+swanapi-0.1.9b2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swanapi-0.1.9b2.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
+swanapi-0.1.9b2.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
+swanapi-0.1.9b2.dist-info/RECORD,,
```

