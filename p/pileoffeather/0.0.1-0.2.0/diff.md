# Comparing `tmp/pileoffeather-0.0.1.tar.gz` & `tmp/pileoffeather-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pileoffeather-0.0.1.tar", last modified: Sun Jul  9 14:45:11 2023, max compression
+gzip compressed data, was "pileoffeather-0.2.0.tar", last modified: Mon Jul 10 13:41:10 2023, max compression
```

## Comparing `pileoffeather-0.0.1.tar` & `pileoffeather-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 14:45:11.734517 pileoffeather-0.0.1/
--rw-rw-rw-   0        0        0     1070 2023-07-09 14:44:27.000000 pileoffeather-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      363 2023-07-09 14:45:11.734517 pileoffeather-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1661 2023-07-09 14:44:27.000000 pileoffeather-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 14:45:11.718896 pileoffeather-0.0.1/pileoffeather/
--rw-rw-rw-   0        0        0       68 2023-07-09 14:43:17.000000 pileoffeather-0.0.1/pileoffeather/__init__.py
--rw-rw-rw-   0        0        0      839 2023-07-09 14:43:19.000000 pileoffeather-0.0.1/pileoffeather/pod.py
--rw-rw-rw-   0        0        0     6522 2023-07-09 14:43:23.000000 pileoffeather-0.0.1/pileoffeather/pof.py
-drwxrwxrwx   0        0        0        0 2023-07-09 14:45:11.734517 pileoffeather-0.0.1/pileoffeather.egg-info/
--rw-rw-rw-   0        0        0      363 2023-07-09 14:45:11.000000 pileoffeather-0.0.1/pileoffeather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-07-09 14:45:11.000000 pileoffeather-0.0.1/pileoffeather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 14:45:11.000000 pileoffeather-0.0.1/pileoffeather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-09 14:45:11.000000 pileoffeather-0.0.1/pileoffeather.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-09 14:45:11.000000 pileoffeather-0.0.1/pileoffeather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 14:45:11.734517 pileoffeather-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      526 2023-07-09 14:43:14.000000 pileoffeather-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:41:10.298520 pileoffeather-0.2.0/
+-rw-rw-rw-   0        0        0     1070 2023-07-09 14:44:27.000000 pileoffeather-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      349 2023-07-10 13:41:10.298520 pileoffeather-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3752 2023-07-10 13:10:38.000000 pileoffeather-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 13:41:10.282897 pileoffeather-0.2.0/pileoffeather/
+-rw-rw-rw-   0        0        0       68 2023-07-09 14:43:17.000000 pileoffeather-0.2.0/pileoffeather/__init__.py
+-rw-rw-rw-   0        0        0     1209 2023-07-10 13:34:27.000000 pileoffeather-0.2.0/pileoffeather/pod.py
+-rw-rw-rw-   0        0        0     5288 2023-07-10 13:28:23.000000 pileoffeather-0.2.0/pileoffeather/pof.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:41:10.298520 pileoffeather-0.2.0/pileoffeather.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-07-10 13:41:10.000000 pileoffeather-0.2.0/pileoffeather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-07-10 13:41:10.000000 pileoffeather-0.2.0/pileoffeather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 13:41:10.000000 pileoffeather-0.2.0/pileoffeather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-10 13:41:10.000000 pileoffeather-0.2.0/pileoffeather.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-10 13:41:10.000000 pileoffeather-0.2.0/pileoffeather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 13:41:10.298520 pileoffeather-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      512 2023-07-10 13:40:24.000000 pileoffeather-0.2.0/setup.py
```

### Comparing `pileoffeather-0.0.1/LICENSE` & `pileoffeather-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pileoffeather-0.0.1/pileoffeather/pod.py` & `pileoffeather-0.2.0/pileoffeather/pod.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import cv2
 import numpy as np
 import os
 
-def loadImage(image_path, desired_size):
-    color_image = cv2.imread(image_path)
-    resized_image = cv2.resize(color_image, desired_size)
-    gray_image = cv2.cvtColor(resized_image, cv2.COLOR_BGR2GRAY)
-    vectorized_image = gray_image.flatten() / 255.0
+def saveImage(vector, image_path, image_size, color):
+    if color == "grayscale":
+        vector = (vector * 255.0).reshape(image_size).astype(np.uint8)
+        vector = cv2.cvtColor(vector, cv2.COLOR_GRAY2BGR)
+    else:
+        vector = (vector * 255.0).reshape(image_size + (3,)).astype(np.uint8)
+    cv2.imwrite(image_path, vector)
+
+def loadImage(image_path, desired_size, color):
+    image = cv2.imread(image_path)
+    image = cv2.resize(image, desired_size)
+    if color == "grayscale":
+        image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+    vectorized_image = image.flatten() / 255.0
     return vectorized_image
 
 def load(**options):
     data_type = options.get("data_type")
     match data_type:
         case "image":
             folder = options.get("folder")
             resize = options.get("resize")
             file_names = os.listdir(folder)
             all_images_vector = []
             for file_name in file_names:
-                image_vector = loadImage(folder + "/" + file_name, resize)
+                image_vector = loadImage(folder + "/" + file_name, resize, options.get("color"))
                 all_images_vector.append(image_vector)
             return np.vstack(all_images_vector)
```

### Comparing `pileoffeather-0.0.1/pileoffeather/pof.py` & `pileoffeather-0.2.0/pileoffeather/pof.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,66 +2,44 @@
 import concurrent.futures
 
 def initializeWeightsAndBiases(layers):
     model_weights = np.zeros(len(layers), dtype=object)
     model_biases = np.zeros(len(layers), dtype=object)
     for i in range(1, len(layers)):
         match layers[i][1]:
-            case "sigmoid":
-                model_weights[i] = np.random.uniform(low=-0.1, high=0.1, size=(layers[i][0], layers[i-1][0]))
-            case "relu":
-                std_dev = np.sqrt(2 / layers[i-1][0])
-                model_weights[i] = np.random.normal(loc=0, scale=std_dev, size=(layers[i][0], layers[i-1][0]))
-            case "leakyRelu":
-                std_dev = np.sqrt(2 / layers[i-1][0])
-                model_weights[i] = np.random.normal(loc=0, scale=std_dev, size=(layers[i][0], layers[i-1][0]))
-                model_weights[i] *= np.where(model_weights[i] > 0, 1, 0.1)
+            case "sigmoid": model_weights[i] = np.random.uniform(low=-0.1, high=0.1, size=(layers[i][0], layers[i-1][0]))
+            case "relu": model_weights[i] = np.random.normal(loc=0, scale=np.sqrt(2 / layers[i-1][0]), size=(layers[i][0], layers[i-1][0]))
+            case "leakyRelu": model_weights[i] = np.random.normal(loc=0, scale=np.sqrt(2 / layers[i-1][0]), size=(layers[i][0], layers[i-1][0]))*np.where(model_weights[i] > 0, 1, 0.1)
         model_biases[i] = np.zeros(layers[i][0])
     return model_weights, model_biases
 
-def runModel(model_weights, model_biases, layers, input):
-    for layer in range(1,len(layers)):
-        input = np.add(np.dot(model_weights[layer], input), model_biases[layer])
-        match layers[layer][1]:
-            case "sigmoid": input = 1 / (1 + np.exp(-input))
-            case "relu": lambda input: (abs(input) + input) / 2
-            case "leakyRelu": input = np.maximum(0.1 * input, input)
-    return input
-
-def runModelForTraining(model_weights, model_biases, layers, layer_history):
+def runModel(model_weights, model_biases, layers, layer_history):
     for layer in range(1,len(layers)):
         layer_history[layer] = np.add(np.dot(model_weights[layer], layer_history[layer-1]), model_biases[layer])
         match layers[layer][1]:
             case "sigmoid": layer_history[layer] = 1 / (1 + np.exp(-layer_history[layer]))
-            case "relu": lambda input: (abs(input) + input) / 2
+            case "relu": layer_history[layer] = np.maximum(0, layer_history[layer])
             case "leakyRelu": layer_history[layer] = np.maximum(0.1 * layer_history[layer], layer_history[layer])
     return layer_history
 
 def backprop(data_input, data_output, weights, biases, layers, learning_rate):
     layer_number = len(layers)
     layers_output_space = np.empty(layer_number, dtype=object)
     layers_output_space[0] = data_input
-    layers_output_space = runModelForTraining(weights, biases, layers, layers_output_space)
-    weights_mod = np.zeros_like(weights)
-    biases_mod = np.zeros_like(biases)
-    output_error = np.subtract(layers_output_space[-1], data_output)
-    match layers[-1][1]:
-        case "sigmoid": output_delta = output_error * layers_output_space[-1] * (1 - layers_output_space[-1])
-        case "relu": output_delta = output_error * np.where(layers_output_space[-1] > 0, 1, 0)
-        case "leakyRelu": output_delta = output_error * np.where(layers_output_space[-1] > 0, 1, 0.1)
-    weights_mod[-1] = np.multiply(np.outer(output_delta, layers_output_space[-2]), learning_rate)
-    biases_mod[-1] = np.multiply(output_delta, learning_rate)
-    for layer in range(layer_number - 2, 0, -1):
+    layers_output_space = runModel(weights, biases, layers, layers_output_space)
+    weights_mod, biases_mod = np.zeros_like(weights), np.zeros_like(biases)
+    error = np.subtract(layers_output_space[-1], data_output)
+    for layer in range(layer_number - 1, 0, -1):
         match layers[layer][1]:
-            case "sigmoid": delta = np.dot(weights[layer + 1].T, output_delta) * layers_output_space[layer] * (1 - layers_output_space[layer])
-            case "relu": delta = np.multiply(np.dot(weights[layer + 1].T, output_delta), np.where(layers_output_space[layer] > 0, 1, 0))
-            case "leakyRelu": delta = np.multiply(np.dot(weights[layer + 1].T, output_delta), np.where(layers_output_space[layer] > 0, 1, 0.1))
+            case "sigmoid": delta = np.multiply(error, layers_output_space[layer] * (1 - layers_output_space[layer]))
+            case "relu": delta = np.multiply(error, np.where(layers_output_space[layer] > 0, 1, 0))
+            case "leakyRelu": delta = np.multiply(error, np.where(layers_output_space[layer] > 0, 1, 0.1))
         weights_mod[layer] = np.multiply(np.outer(delta, layers_output_space[layer - 1]),learning_rate)
         biases_mod[layer] = np.multiply(delta,learning_rate)
-        output_delta = delta
+        if layer>1: error = np.dot(weights[layer].T, delta)
     return [weights_mod, biases_mod, abs(np.mean(layers_output_space[-1] - data_output))]
 
 def computeBatch(batch_input, batch_output, batch_size, weights, biases, layers, learning_rate):
     result = [None] * batch_size
     with concurrent.futures.ThreadPoolExecutor() as executor:
         for i in range(batch_size):
             result[i] = executor.submit(backprop, batch_input[i], batch_output[i], weights, biases, layers, learning_rate)
@@ -75,49 +53,42 @@
         else:
             if options.get("name") == None: self.name = "unknown"
             else: self.name = options.get("name")
             self.layers = options.get("layers")
             self.initializeWeights()
 
     def run(self, input):
-        return runModel(self.weights, self.biases, self.layers, input)
+        layers_output_space = np.empty(len(self.layers), dtype=object)
+        layers_output_space[0] = input
+        return runModel(self.weights, self.biases, self.layers, layers_output_space)[-1]
 
     def train(self, data_input, data_output, **options):
         batch_size = options.get("batch_size")
         epoch_number = options.get("epoch_number")
         learning_rate = options.get("rate")
         for epoch in range(epoch_number):
-            t_loss, t_counter = 0, 0
-            batch_start = 0
-            batch_end = batch_size
-            stopper = False
-            while not(stopper):
+            t_loss, t_counter, batch_start, batch_end = 0, 0, 0, batch_size
+            while not(batch_start>=len(data_input)):
                 batch_result = computeBatch(data_input[batch_start:batch_end], data_output[batch_start:batch_end], batch_end-batch_start, self.weights, self.biases, self.layers, learning_rate)
                 self.applyBatch(batch_result)
                 t_loss += np.mean([mod[2] for mod in batch_result])
                 t_counter += 1
                 batch_start += batch_size
                 batch_end += batch_size
-                if batch_end >= len(data_input):
-                    batch_end = len(data_input)
-                if batch_start>=len(data_input):
-                    stopper = True
+                if batch_end >= len(data_input): batch_end = len(data_input)
             print("Epoch " + str(epoch) + "        Loss = " + str(t_loss/t_counter), end='\r')
         self.save()
-        print("\nTraining finished, weights and biases saved.\n")
+        print("\nTraining finished, weights and biases saved.")
 
     def applyBatch(self, batch_result):
         self.weights -= np.mean([mod[0] for mod in batch_result], axis=0)
-        self.biases = np.subtract(self.biases, np.mean([mod[1] for mod in batch_result], axis=0))
+        self.biases -= np.mean([mod[1] for mod in batch_result], axis=0)
 
     def save(self):
         np.savez(self.name + ".npz", matrix1=self.weights, matrix2=self.biases, matrix3=self.layers)
 
     def load(self, filename):
         data = np.load(filename + ".npz", allow_pickle=True)
-        self.weights = data['matrix1']
-        self.biases = data['matrix2']
-        self.layers = data['matrix3']
-        self.name = filename
+        self.weights, self.biases, self.layers, self.name = data['matrix1'], data['matrix2'], data['matrix3'], filename
 
     def initializeWeights(self):
         self.weights, self.biases = initializeWeightsAndBiases(self.layers)
```

### Comparing `pileoffeather-0.0.1/setup.py` & `pileoffeather-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     name='pileoffeather',
-    version='0.0.1',
+    version='0.2.0',
     license='MIT',
     url = 'https://github.com/usedToBeTomas/pile-of-feather',
     author='Daniele Tomaselli',
-    description='Lightweight and easy to use ml library for small projects, create a neural network in minutes. (Fun project)',
+    description='Lightweight and easy to use ml library for small projects, create a neural network in minutes.',
     packages=['pileoffeather'],
     keywords = ['neural network', 'ml', 'ai', 'machine learning','simple','nn'],
     install_requires=[
         'opencv-python',
         'numpy'
     ]
 )
```

