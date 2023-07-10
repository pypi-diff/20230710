# Comparing `tmp/lc-checkpoint-0.4.0.tar.gz` & `tmp/lc-checkpoint-0.4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.4.0.tar", last modified: Mon Jul 10 12:45:59 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.4.1.1.tar", last modified: Mon Jul 10 22:41:17 2023, max compression
```

## Comparing `lc-checkpoint-0.4.0.tar` & `lc-checkpoint-0.4.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-10 12:45:59.806147 lc-checkpoint-0.4.0/
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.4.0/LICENSE
--rw-r--r--   0 yeoshuheng   (501) staff       (20)     6026 2023-07-10 12:45:59.806259 lc-checkpoint-0.4.0/PKG-INFO
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     5680 2023-07-10 06:32:43.000000 lc-checkpoint-0.4.0/README.md
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.4.0/pyproject.toml
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      608 2023-07-10 12:45:59.806686 lc-checkpoint-0.4.0/setup.cfg
-drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-10 12:45:59.803390 lc-checkpoint-0.4.0/src/
-drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-10 12:45:59.804933 lc-checkpoint-0.4.0/src/lc_checkpoint/
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.4.0/src/lc_checkpoint/__init__.py
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     6051 2023-07-10 06:19:30.000000 lc-checkpoint-0.4.0/src/lc_checkpoint/main.py
-drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-10 12:45:59.805969 lc-checkpoint-0.4.0/src/lc_checkpoint.egg-info/
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     6026 2023-07-10 12:45:59.000000 lc-checkpoint-0.4.0/src/lc_checkpoint.egg-info/PKG-INFO
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      262 2023-07-10 12:45:59.000000 lc-checkpoint-0.4.0/src/lc_checkpoint.egg-info/SOURCES.txt
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)        1 2023-07-10 12:45:59.000000 lc-checkpoint-0.4.0/src/lc_checkpoint.egg-info/dependency_links.txt
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)       14 2023-07-10 12:45:59.000000 lc-checkpoint-0.4.0/src/lc_checkpoint.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 22:41:17.740987 lc-checkpoint-0.4.1.1/
+-rw-rw-rw-   0        0        0     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.4.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5464 2023-07-10 22:41:17.740987 lc-checkpoint-0.4.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4958 2023-06-06 17:29:43.000000 lc-checkpoint-0.4.1.1/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.4.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      637 2023-07-10 22:41:17.750992 lc-checkpoint-0.4.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 22:41:17.705711 lc-checkpoint-0.4.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 22:41:17.724198 lc-checkpoint-0.4.1.1/src/lc_checkpoint/
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.4.1.1/src/lc_checkpoint/__init__.py
+-rw-rw-rw-   0        0        0     4542 2023-06-06 17:09:16.000000 lc-checkpoint-0.4.1.1/src/lc_checkpoint/main.py
+drwxrwxrwx   0        0        0        0 2023-07-10 22:41:17.739987 lc-checkpoint-0.4.1.1/src/lc_checkpoint.egg-info/
+-rw-rw-rw-   0        0        0     5464 2023-07-10 22:41:17.000000 lc-checkpoint-0.4.1.1/src/lc_checkpoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-10 22:41:17.000000 lc-checkpoint-0.4.1.1/src/lc_checkpoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 22:41:17.000000 lc-checkpoint-0.4.1.1/src/lc_checkpoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-10 22:41:17.000000 lc-checkpoint-0.4.1.1/src/lc_checkpoint.egg-info/top_level.txt
```

### Comparing `lc-checkpoint-0.4.0/LICENSE` & `lc-checkpoint-0.4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.4.0/PKG-INFO` & `lc-checkpoint-0.4.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,143 @@
-Metadata-Version: 2.1
-Name: lc-checkpoint
-Version: 0.4.0
-Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
-Home-page: https://pypi.org/project/lc-checkpoint/
-Author: Dedy Van Hauten
-Author-email: dedy.van@ui.ac.id
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# LC-Checkpoint
-
-LC-Checkpoint is a Python package that implements the LC-Checkpoint method for compressing and checkpointing PyTorch models during training.
-
-## Installation
-
-You can install LC-Checkpoint using pip:
-
-```
-pip install lc_checkpoint
-```
-
-## Usage
-
-To use LC-Checkpoint in your PyTorch training script, you can follow these steps:
-
-1.  Import the LC-Checkpoint module:
-    
-    ```
-    from lc_checkpoint import main as lc
-    ```
-    
-
-    
-2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
-    
-    ```
-    model = model()
-    optimizer = optim.SGD(model.parameters(), lr=0.001, momentum=0.9)
-    criterion = nn.CrossEntropyLoss()
-    checkpoint_dir = 'checkpoints/lc-checkpoint'
-    num_buckets = 5
-    num_bits = 32
-
-    lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)
-    ```
-    
-    
-3.  Use the LC-Checkpoint method in your training loop:
-    
-    ```
-
-    # Save base model weights
-    init_save_dir = "checkpoints/initialstate.pt"
-    torch.save(model.state_dict(), init_save_dir)
-    prev_state_dict = model.state_dict()
-
-    for epoch in range(epochs):  # loop over the dataset multiple times
-
-        running_loss = 0.0
-        for i, data in enumerate(trainloader, 0):
-            # Load the previous checkpoints if exist
-            try:
-                # Find the latest checkpoint file
-                lc_checkpoint_files = glob.glob(os.path.join('checkpoints/lc-checkpoint', 'lc_checkpoint_epoch*.pt'))
-                latest_checkpoint_file = max(lc_checkpoint_files, key=os.path.getctime)
-                prev_state_dict, epoch_loaded = lc.load_checkpoint(latest_checkpoint_file)
-                print('Restored latest checkpoint:', latest_checkpoint_file)
-                latest_checkpoint_file_size = os.path.getsize(latest_checkpoint_file)
-                latest_checkpoint_file_size_kb = latest_checkpoint_file_size / 1024
-                print('Latest checkpoint file size:', latest_checkpoint_file_size_kb, 'KB')
-                restore_time = time.time() - start_time
-                total_restore_time += restore_time
-                print('Time taken to restore checkpoint:', restore_time)
-                start_time = time.time()  # reset the start time
-                print('-' * 50)
-            except:
-                pass
-
-            # Get the inputs and labels
-            inputs, labels = data
-
-            # Zero the parameter gradients
-            optimizer.zero_grad()
-
-            # Forward + backward + optimize
-            outputs = model(inputs)
-            loss = criterion(outputs, labels)
-            loss.backward()
-            optimizer.step()
-
-            new_state_dict = model.state_dict()
-            new_state_weights = np.concatenate([tensor.numpy().flatten() for tensor in new_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
-            prev_state_weights = np.concatenate([tensor.numpy().flatten() for tensor in prev_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
-            δt = new_state_weights - prev_state_weights # Get delta
-            prev_state_dict = new_state_dict
-
-            # Save the checkpoint
-            compressed_data = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
-            save_start_time = time.time()  # record the start time
-            lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i)
-            save_time = time.time() - save_start_time  # calculate the time taken to save the checkpoint
-
-            # Print statistics
-            running_loss += loss.item()
-            if i % 1 == 0:    # print every 1 mini-batches
-                print('[Epoch: %d, Iteration: %5d] loss: %.3f' %
-                      (epoch + 1, i + 1, running_loss / 1))
-                running_loss = 0.0
-                print('Time taken to save checkpoint:', save_time)
-    ```
-4. Using LC-Checkpoint to restore model.
-```
-last_epoch, last_iter = 30, 8
-max_iter = 10
-restored_model = restore_model(model(), last_epoch, last_iter, max_iter, init_save_dir)
-```
-
-## API Reference
-
-### `lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
-
-Initializes the LC-Checkpoint method with the given PyTorch model, optimizer, loss function, checkpoint directory, number of buckets, and number of bits.
-
-### `lc.compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True)`
-
-Compresses the model parameters and returns the compressed data.
-
-### `lc.decode_data(encoded)`
-
-Decodes the compressed data and returns the original model parameters.
-
-### `lc.save_checkpoint(filename, compressed_data, epoch, iteration)`
-
-Saves the compressed data to a file with the given filename, epoch, and iteration.
-
-### `lc.load_checkpoint(filename)`
-
-Loads the compressed data from a file with the given filename.
-
-### `lc.restore_model(model, last_epoch, last_iter, max_iter, init_filename, ckpt_name)`
-Loads the compressed data into a pytorch model.
-
-### `lc.calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets)`
-
-Calculates the compression rate of the LC-Checkpoint method based on the previous state dictionary and the current number of bits and buckets.
-
-## License
-
-LC-Checkpoint is licensed under the MIT License. See the LICENSE file for more information.
-
-## Acknowledgements
-
-LC-Checkpoint is based on paper "On Efficient Constructions of Checkpoints" authored by Yu Chen, Zhenming Liu, Bin Ren, Xin Jin.
+Metadata-Version: 2.1
+Name: lc-checkpoint
+Version: 0.4.1.1
+Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
+Home-page: https://pypi.org/project/lc-checkpoint/
+Author: Dedy Van Hauten
+Author-email: dedy.van@ui.ac.id
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# LC-Checkpoint
+
+LC-Checkpoint is a Python package that implements the LC-Checkpoint method for compressing and checkpointing PyTorch models during training.
+
+## Installation
+
+You can install LC-Checkpoint using pip:
+
+```
+pip install lc_checkpoint
+```
+
+## Usage
+
+To use LC-Checkpoint in your PyTorch training script, you can follow these steps:
+
+1.  Import the LC-Checkpoint module:
+    
+    ```
+    from lc_checkpoint import main as lc
+    ```
+    
+
+    
+2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
+    
+    ```
+    model = model
+    optimizer = optim.SGD(model.parameters(), lr=0.001, momentum=0.9)
+    criterion = nn.CrossEntropyLoss()
+    checkpoint_dir = 'checkpoints/lc-checkpoint'
+    num_buckets = 5
+    num_bits = 32
+    prev_state_dict = model.state_dict()
+
+    lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)
+    ```
+    
+    
+3.  Use the LC-Checkpoint method in your training loop:
+    
+    ```
+    for epoch in range(epochs):  # loop over the dataset multiple times
+
+        running_loss = 0.0
+        for i, data in enumerate(trainloader, 0):
+            # Load the previous checkpoints if exist
+            try:
+                # Find the latest checkpoint file
+                lc_checkpoint_files = glob.glob(os.path.join('checkpoints/lc-checkpoint', 'lc_checkpoint_epoch*.pt'))
+                latest_checkpoint_file = max(lc_checkpoint_files, key=os.path.getctime)
+                prev_state_dict, epoch_loaded = lc.load_checkpoint(latest_checkpoint_file)
+                print('Restored latest checkpoint:', latest_checkpoint_file)
+                latest_checkpoint_file_size = os.path.getsize(latest_checkpoint_file)
+                latest_checkpoint_file_size_kb = latest_checkpoint_file_size / 1024
+                print('Latest checkpoint file size:', latest_checkpoint_file_size_kb, 'KB')
+                restore_time = time.time() - start_time
+                total_restore_time += restore_time
+                print('Time taken to restore checkpoint:', restore_time)
+                start_time = time.time()  # reset the start time
+                print('-' * 50)
+            except:
+                pass
+
+            # Get the inputs and labels
+            inputs, labels = data
+
+            # Zero the parameter gradients
+            optimizer.zero_grad()
+
+            # Forward + backward + optimize
+            outputs = model(inputs)
+            loss = criterion(outputs, labels)
+            loss.backward()
+            optimizer.step()
+
+            new_state_dict = model.state_dict()
+            δt = np.concatenate([tensor.numpy().flatten() for tensor in new_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
+            prev_state_dict = new_state_dict
+
+            # Save the checkpoint
+            compressed_data = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
+            save_start_time = time.time()  # record the start time
+            lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i)
+            save_time = time.time() - save_start_time  # calculate the time taken to save the checkpoint
+
+            # Print statistics
+            running_loss += loss.item()
+            if i % 1 == 0:    # print every 1 mini-batches
+                print('[Epoch: %d, Iteration: %5d] loss: %.3f' %
+                      (epoch + 1, i + 1, running_loss / 1))
+                running_loss = 0.0
+                print('Time taken to save checkpoint:', save_time)
+    ```
+    
+
+## API Reference
+
+### `lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
+
+Initializes the LC-Checkpoint method with the given PyTorch model, optimizer, loss function, checkpoint directory, number of buckets, and number of bits.
+
+### `lc.compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True)`
+
+Compresses the model parameters and returns the compressed data.
+
+### `lc.decode_data(encoded)`
+
+Decodes the compressed data and returns the original model parameters.
+
+### `lc.save_checkpoint(filename, compressed_data, epoch, iteration)`
+
+Saves the compressed data to a file with the given filename, epoch, and iteration.
+
+### `lc.load_checkpoint(filename)`
+
+Loads the compressed data from a file with the given filename.
+
+### `lc.calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets)`
+
+Calculates the compression rate of the LC-Checkpoint method based on the previous state dictionary and the current number of bits and buckets.
+
+## License
+
+LC-Checkpoint is licensed under the MIT License. See the LICENSE file for more information.
+
+## Acknowledgements
+
+LC-Checkpoint is based on paper "On Efficient Constructions of Checkpoints" authored by Yu Chen, Zhenming Liu, Bin Ren, Xin Jin.
```

### Comparing `lc-checkpoint-0.4.0/README.md` & `lc-checkpoint-0.4.1.1/src/lc_checkpoint.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: lc-checkpoint
+Version: 0.4.1.1
+Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
+Home-page: https://pypi.org/project/lc-checkpoint/
+Author: Dedy Van Hauten
+Author-email: dedy.van@ui.ac.id
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # LC-Checkpoint
 
 LC-Checkpoint is a Python package that implements the LC-Checkpoint method for compressing and checkpointing PyTorch models during training.
 
 ## Installation
 
 You can install LC-Checkpoint using pip:
@@ -21,34 +35,29 @@
     ```
     
 
     
 2.  Initialize the LC-Checkpoint method with your PyTorch model, optimizer, loss function, and other hyperparameters:
     
     ```
-    model = model()
+    model = model
     optimizer = optim.SGD(model.parameters(), lr=0.001, momentum=0.9)
     criterion = nn.CrossEntropyLoss()
     checkpoint_dir = 'checkpoints/lc-checkpoint'
     num_buckets = 5
     num_bits = 32
+    prev_state_dict = model.state_dict()
 
     lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)
     ```
     
     
 3.  Use the LC-Checkpoint method in your training loop:
     
     ```
-
-    # Save base model weights
-    init_save_dir = "checkpoints/initialstate.pt"
-    torch.save(model.state_dict(), init_save_dir)
-    prev_state_dict = model.state_dict()
-
     for epoch in range(epochs):  # loop over the dataset multiple times
 
         running_loss = 0.0
         for i, data in enumerate(trainloader, 0):
             # Load the previous checkpoints if exist
             try:
                 # Find the latest checkpoint file
@@ -76,17 +85,15 @@
             # Forward + backward + optimize
             outputs = model(inputs)
             loss = criterion(outputs, labels)
             loss.backward()
             optimizer.step()
 
             new_state_dict = model.state_dict()
-            new_state_weights = np.concatenate([tensor.numpy().flatten() for tensor in new_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
-            prev_state_weights = np.concatenate([tensor.numpy().flatten() for tensor in prev_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
-            δt = new_state_weights - prev_state_weights # Get delta
+            δt = np.concatenate([tensor.numpy().flatten() for tensor in new_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
             prev_state_dict = new_state_dict
 
             # Save the checkpoint
             compressed_data = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
             save_start_time = time.time()  # record the start time
             lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i)
             save_time = time.time() - save_start_time  # calculate the time taken to save the checkpoint
@@ -95,20 +102,15 @@
             running_loss += loss.item()
             if i % 1 == 0:    # print every 1 mini-batches
                 print('[Epoch: %d, Iteration: %5d] loss: %.3f' %
                       (epoch + 1, i + 1, running_loss / 1))
                 running_loss = 0.0
                 print('Time taken to save checkpoint:', save_time)
     ```
-4. Using LC-Checkpoint to restore model.
-```
-last_epoch, last_iter = 30, 8
-max_iter = 10
-restored_model = restore_model(model(), last_epoch, last_iter, max_iter, init_save_dir)
-```
+    
 
 ## API Reference
 
 ### `lc.initialize(model, optimizer, criterion, checkpoint_dir, num_buckets, num_bits)`
 
 Initializes the LC-Checkpoint method with the given PyTorch model, optimizer, loss function, checkpoint directory, number of buckets, and number of bits.
 
@@ -124,21 +126,18 @@
 
 Saves the compressed data to a file with the given filename, epoch, and iteration.
 
 ### `lc.load_checkpoint(filename)`
 
 Loads the compressed data from a file with the given filename.
 
-### `lc.restore_model(model, last_epoch, last_iter, max_iter, init_filename, ckpt_name)`
-Loads the compressed data into a pytorch model.
-
 ### `lc.calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets)`
 
 Calculates the compression rate of the LC-Checkpoint method based on the previous state dictionary and the current number of bits and buckets.
 
 ## License
 
 LC-Checkpoint is licensed under the MIT License. See the LICENSE file for more information.
 
 ## Acknowledgements
 
-LC-Checkpoint is based on paper "On Efficient Constructions of Checkpoints" authored by Yu Chen, Zhenming Liu, Bin Ren, Xin Jin.
+LC-Checkpoint is based on paper "On Efficient Constructions of Checkpoints" authored by Yu Chen, Zhenming Liu, Bin Ren, Xin Jin.
```

### Comparing `lc-checkpoint-0.4.0/src/lc_checkpoint/main.py` & `lc-checkpoint-0.4.1.1/src/lc_checkpoint/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import pickle
 import math
 import numpy as np
 import torch.optim as optim
 import torch.nn as nn
 import dahuffman
-import torch
 
 __all__ = ['initialize', 'compress_data', 'decode_data', 'save_checkpoint', 'load_checkpoint', 'calculate_compression_rate']
 
 net = None
 optimizer = None
 criterion = None
 checkpoint_dir = None
@@ -23,23 +22,23 @@
     criterion = criterion
     checkpoint_dir = checkpoint_dir
     os.makedirs(checkpoint_dir, exist_ok=True)
     num_buckets = num_buckets
     num_bits = num_bits
     prev_state_dict = net.state_dict()
 
-def compress_data(δt, num_bits= 32, k = 5, treshold=True):
+def compress_data(δt, num_bits=num_bits, k=num_buckets, treshold=True):
     sign = np.sign(δt)
     x_abs = np.abs(δt)
-    exponent = np.floor(np.log2(x_abs, where = (x_abs != 0)))
+    exponent = np.floor(np.log2(x_abs))
     mantissa = x_abs / (2 ** exponent)
     quantized = sign * mantissa * (2 ** exponent)
-    smallest_value = 2 ** (-1 * num_bits)
+    smallest_value = 2 ** (-num_bits)
     quantized = np.round(quantized / smallest_value) * smallest_value
-
+    
     the_sign = np.zeros_like(δt)
     the_sign[δt < 0] = 1
 
     grouped_quantized = {}
     for i in range(len(δt)):
         key = (the_sign[i], int(exponent[i]))
         if key not in grouped_quantized:
@@ -80,28 +79,26 @@
         bucket_len = len(bucket)
         if bucket_len > 0:
             for key in bucket:
                 values = [round(val, 2) for val in grouped_quantized[key]]
                 bucket_mean += sum(values) / len(values)
             bucket_mean /= bucket_len
         bucket_means.append(bucket_mean)
-
+        
     new_δt = np.zeros_like(exponent)
     for i, bucket in enumerate(buckets):
         if len(bucket) > 0:
             bucket_mean = bucket_means[i]
             base_key = bucket[0][1]
             new_δt[(the_sign == bucket[0][0]) & (exponent == base_key)] = bucket_mean
-        
-    new_δt = np.nan_to_num(new_δt, 0)
     
     # Encode new_δt using Huffman coding
     encoder = dahuffman.HuffmanCodec.from_data(new_δt)
     encoded = encoder.encode(new_δt)
-
+    
     return encoded
 
 def decode_data(encoded):
     codec = dahuffman.HuffmanCodec.from_data(encoded)
     int_list = codec.decode(encoded)
     int_list = [int(x) for x in int_list]
     new_δt = np.array(int_list) / 100.0
@@ -121,44 +118,8 @@
         compressed_data, epoch = pickle.load(f)
     compressed_data = decode_data(compressed_data)  # decode the binary data
     return compressed_data, epoch
 
 def calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets):
     num_elements = len(prev_state_dict)
     compression_rate = num_elements * math.log(num_buckets, 2) + num_buckets * num_bits
-    return compression_rate
-
-def restore_model(init_model, last_epoch, last_iter, max_iter, init_filename, cpt_name = "lc_checkpoint"):
-    # Get initial model
-    init_model.load_state_dict(torch.load(init_filename))
-    deltas = np.concatenate([tensor.numpy().flatten() for tensor in init_model.state_dict().values()])
-
-    # Get deltas for last epoch.
-    for j in range(last_iter + 1):
-        ckpt = cpt_name + "_epoch{}_iter{}.pt".format(last_epoch, j)
-        cp, _ = load_checkpoint(ckpt)
-        deltas = np.add(deltas,cp)
-
-    # Get deltas for previous epochs
-    for e in range(last_epoch - 1):
-        for j in range(max_iter):
-            if e == 0 and j == 0:
-                continue
-            ckpt = cpt_name + "_epoch{}_iter{}.pt".format(e, j)
-            cp, _ = load_checkpoint(ckpt)
-            deltas = np.add(deltas,cp)
-
-    # Reshape based on model's state dictionary.
-    fin_dict = init_model.state_dict()
-    last_idx = 0
-    for layer_name, init_tensor in fin_dict.items():
-        # Extract appropriate elements
-        dim = init_tensor.numpy().shape
-        t_elements = np.prod(dim)
-        needed_ele = deltas[last_idx : last_idx + t_elements]
-        last_idx = t_elements # Reset the last index
-
-        # Reshape delta and reinsert into the dictionary.
-        fin_dict[layer_name] = torch.from_numpy(np.reshape(needed_ele, dim))
-        
-    init_model.load_state_dict(fin_dict)
-    return init_model
+    return compression_rate
```

