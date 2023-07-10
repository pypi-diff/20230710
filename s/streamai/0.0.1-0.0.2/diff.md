# Comparing `tmp/streamai-0.0.1.tar.gz` & `tmp/streamai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamai-0.0.1.tar", last modified: Mon Jul 10 04:06:59 2023, max compression
+gzip compressed data, was "streamai-0.0.2.tar", last modified: Mon Jul 10 04:47:43 2023, max compression
```

## Comparing `streamai-0.0.1.tar` & `streamai-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 navdeep    (501) staff       (20)        0 2023-07-10 04:06:59.179737 streamai-0.0.1/
--rw-r--r--   0 navdeep    (501) staff       (20)     1071 2023-07-09 13:45:54.000000 streamai-0.0.1/LICENSE
--rw-r--r--   0 navdeep    (501) staff       (20)     1771 2023-07-10 04:06:59.179621 streamai-0.0.1/PKG-INFO
--rw-r--r--   0 navdeep    (501) staff       (20)       38 2023-07-10 04:06:59.179784 streamai-0.0.1/setup.cfg
--rw-r--r--   0 navdeep    (501) staff       (20)      733 2023-07-10 03:54:21.000000 streamai-0.0.1/setup.py
-drwxr-xr-x   0 navdeep    (501) staff       (20)        0 2023-07-10 04:06:59.175505 streamai-0.0.1/streamai/
--rw-r--r--   0 navdeep    (501) staff       (20)       69 2023-07-10 03:57:51.000000 streamai-0.0.1/streamai/__init__.py
-drwxr-xr-x   0 navdeep    (501) staff       (20)        0 2023-07-10 04:06:59.178326 streamai-0.0.1/streamai/alpacalora/
--rw-r--r--   0 navdeep    (501) staff       (20)      200 2023-07-10 03:58:30.000000 streamai-0.0.1/streamai/alpacalora/__init__.py
--rw-r--r--   0 navdeep    (501) staff       (20)     1422 2023-07-05 06:35:48.000000 streamai-0.0.1/streamai/alpacalora/export_hf_checkpoint.py
--rw-r--r--   0 navdeep    (501) staff       (20)     3601 2023-07-05 06:35:48.000000 streamai-0.0.1/streamai/alpacalora/export_state_dict_checkpoint.py
--rw-r--r--   0 navdeep    (501) staff       (20)     9823 2023-07-10 03:52:51.000000 streamai-0.0.1/streamai/alpacalora/finetune.py
--rw-r--r--   0 navdeep    (501) staff       (20)     7457 2023-07-10 03:52:51.000000 streamai-0.0.1/streamai/alpacalora/generate.py
--rw-r--r--   0 navdeep    (501) staff       (20)     4905 2023-07-10 03:52:51.000000 streamai-0.0.1/streamai/alpacalora/inference.py
--rw-r--r--   0 navdeep    (501) staff       (20)     4199 2023-07-10 03:52:51.000000 streamai-0.0.1/streamai/alpacalora/train.py
--rw-r--r--   0 navdeep    (501) staff       (20)     1849 2023-07-05 06:35:48.000000 streamai-0.0.1/streamai/alpacalora/uptest.py
-drwxr-xr-x   0 navdeep    (501) staff       (20)        0 2023-07-10 04:06:59.179032 streamai-0.0.1/streamai/alpacalora/utils/
--rw-r--r--   0 navdeep    (501) staff       (20)        0 2023-07-05 06:35:48.000000 streamai-0.0.1/streamai/alpacalora/utils/__init__.py
--rw-r--r--   0 navdeep    (501) staff       (20)     1833 2023-07-10 03:52:51.000000 streamai-0.0.1/streamai/alpacalora/utils/callbacks.py
--rw-r--r--   0 navdeep    (501) staff       (20)     1669 2023-07-05 06:35:48.000000 streamai-0.0.1/streamai/alpacalora/utils/prompter.py
--rw-r--r--   0 navdeep    (501) staff       (20)      984 2023-07-10 04:03:13.000000 streamai-0.0.1/streamai/app.py
-drwxr-xr-x   0 navdeep    (501) staff       (20)        0 2023-07-10 04:06:59.179392 streamai-0.0.1/streamai/llms/
--rw-r--r--   0 navdeep    (501) staff       (20)       52 2023-07-10 03:58:06.000000 streamai-0.0.1/streamai/llms/__init__.py
--rw-r--r--   0 navdeep    (501) staff       (20)     3605 2023-07-10 03:52:51.000000 streamai-0.0.1/streamai/llms/alpacalora.py
-drwxr-xr-x   0 navdeep    (501) staff       (20)        0 2023-07-10 04:06:59.176199 streamai-0.0.1/streamai.egg-info/
--rw-r--r--   0 navdeep    (501) staff       (20)     1771 2023-07-10 04:06:59.000000 streamai-0.0.1/streamai.egg-info/PKG-INFO
--rw-r--r--   0 navdeep    (501) staff       (20)      665 2023-07-10 04:06:59.000000 streamai-0.0.1/streamai.egg-info/SOURCES.txt
--rw-r--r--   0 navdeep    (501) staff       (20)        1 2023-07-10 04:06:59.000000 streamai-0.0.1/streamai.egg-info/dependency_links.txt
--rw-r--r--   0 navdeep    (501) staff       (20)       21 2023-07-10 04:06:59.000000 streamai-0.0.1/streamai.egg-info/requires.txt
--rw-r--r--   0 navdeep    (501) staff       (20)        9 2023-07-10 04:06:59.000000 streamai-0.0.1/streamai.egg-info/top_level.txt
+drwxr-xr-x   0 navdeep    (501) staff       (20)        0 2023-07-10 04:47:43.163368 streamai-0.0.2/
+-rw-r--r--   0 navdeep    (501) staff       (20)     1071 2023-07-09 13:45:54.000000 streamai-0.0.2/LICENSE
+-rw-r--r--   0 navdeep    (501) staff       (20)     1776 2023-07-10 04:47:43.163241 streamai-0.0.2/PKG-INFO
+-rw-r--r--   0 navdeep    (501) staff       (20)       38 2023-07-10 04:47:43.163416 streamai-0.0.2/setup.cfg
+-rw-r--r--   0 navdeep    (501) staff       (20)      740 2023-07-10 04:12:07.000000 streamai-0.0.2/setup.py
+drwxr-xr-x   0 navdeep    (501) staff       (20)        0 2023-07-10 04:47:43.160207 streamai-0.0.2/streamai/
+-rw-r--r--   0 navdeep    (501) staff       (20)       69 2023-07-10 03:57:51.000000 streamai-0.0.2/streamai/__init__.py
+drwxr-xr-x   0 navdeep    (501) staff       (20)        0 2023-07-10 04:47:43.162325 streamai-0.0.2/streamai/alpacalora/
+-rw-r--r--   0 navdeep    (501) staff       (20)      200 2023-07-10 03:58:30.000000 streamai-0.0.2/streamai/alpacalora/__init__.py
+-rw-r--r--   0 navdeep    (501) staff       (20)     1422 2023-07-05 06:35:48.000000 streamai-0.0.2/streamai/alpacalora/export_hf_checkpoint.py
+-rw-r--r--   0 navdeep    (501) staff       (20)     3601 2023-07-05 06:35:48.000000 streamai-0.0.2/streamai/alpacalora/export_state_dict_checkpoint.py
+-rw-r--r--   0 navdeep    (501) staff       (20)     9823 2023-07-10 03:52:51.000000 streamai-0.0.2/streamai/alpacalora/finetune.py
+-rw-r--r--   0 navdeep    (501) staff       (20)     7457 2023-07-10 03:52:51.000000 streamai-0.0.2/streamai/alpacalora/generate.py
+-rw-r--r--   0 navdeep    (501) staff       (20)     4905 2023-07-10 03:52:51.000000 streamai-0.0.2/streamai/alpacalora/inference.py
+-rw-r--r--   0 navdeep    (501) staff       (20)     4199 2023-07-10 03:52:51.000000 streamai-0.0.2/streamai/alpacalora/train.py
+-rw-r--r--   0 navdeep    (501) staff       (20)     1849 2023-07-05 06:35:48.000000 streamai-0.0.2/streamai/alpacalora/uptest.py
+drwxr-xr-x   0 navdeep    (501) staff       (20)        0 2023-07-10 04:47:43.162750 streamai-0.0.2/streamai/alpacalora/utils/
+-rw-r--r--   0 navdeep    (501) staff       (20)        0 2023-07-05 06:35:48.000000 streamai-0.0.2/streamai/alpacalora/utils/__init__.py
+-rw-r--r--   0 navdeep    (501) staff       (20)     1833 2023-07-10 03:52:51.000000 streamai-0.0.2/streamai/alpacalora/utils/callbacks.py
+-rw-r--r--   0 navdeep    (501) staff       (20)     1669 2023-07-05 06:35:48.000000 streamai-0.0.2/streamai/alpacalora/utils/prompter.py
+-rw-r--r--   0 navdeep    (501) staff       (20)      984 2023-07-10 04:03:13.000000 streamai-0.0.2/streamai/app.py
+drwxr-xr-x   0 navdeep    (501) staff       (20)        0 2023-07-10 04:47:43.163030 streamai-0.0.2/streamai/llms/
+-rw-r--r--   0 navdeep    (501) staff       (20)       52 2023-07-10 03:58:06.000000 streamai-0.0.2/streamai/llms/__init__.py
+-rw-r--r--   0 navdeep    (501) staff       (20)     3605 2023-07-10 03:52:51.000000 streamai-0.0.2/streamai/llms/alpacalora.py
+drwxr-xr-x   0 navdeep    (501) staff       (20)        0 2023-07-10 04:47:43.160808 streamai-0.0.2/streamai.egg-info/
+-rw-r--r--   0 navdeep    (501) staff       (20)     1776 2023-07-10 04:47:43.000000 streamai-0.0.2/streamai.egg-info/PKG-INFO
+-rw-r--r--   0 navdeep    (501) staff       (20)      665 2023-07-10 04:47:43.000000 streamai-0.0.2/streamai.egg-info/SOURCES.txt
+-rw-r--r--   0 navdeep    (501) staff       (20)        1 2023-07-10 04:47:43.000000 streamai-0.0.2/streamai.egg-info/dependency_links.txt
+-rw-r--r--   0 navdeep    (501) staff       (20)       21 2023-07-10 04:47:43.000000 streamai-0.0.2/streamai.egg-info/requires.txt
+-rw-r--r--   0 navdeep    (501) staff       (20)        9 2023-07-10 04:47:43.000000 streamai-0.0.2/streamai.egg-info/top_level.txt
```

### Comparing `streamai-0.0.1/LICENSE` & `streamai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamai-0.0.1/PKG-INFO` & `streamai-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: streamai
-Version: 0.0.1
-Summary: serve ai agents as api easily.
+Version: 0.0.2
+Summary: serve ai agents/models easily as api.
 Author: Navdeep Dhakar
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## 🌩️ Stream AI easily
 ### streamai let's you serve any AI agents/model(currently llms only) easily as api and integrate in fontend quickly.
-todo:
-- [ ] test alpaca lora with deployment
-- [ ] fix dynamic installation issue
-- [ ] add endpoint for info about deployed model
+
 #### deploy from custom model script
 ```py
 from streamai.app import endpointIO
-from streamai.models import Autoalpacalora
+from streamai.llms import Autoalpacalora
 def custom_model_IO(input:str):
     output = customodelinference(input) #depend on your inference function, just need to return string output from it.
     return f"this is output of {output}"
     
 model1 = endpointIO(custom_model_IO)
 model1.run() #this will create a server api endpoint for your model, at http://0.0.0.0:8000 see terminal logs for more info about endpoints
 ```
 #### deploy from inbuild models libs(you can also finetun inbuilt models)
 ```py
 from streamai.app import endpointIO
-from streamai.models import Autoalpacalora
+from streamai.llms import Autoalpacalora
     
 modelinstance = Autoalpacalora("decapoda/llama-7b", "./scroltest")
 #modelinstance.loadmodel() #required for deployment of model as api, not required during finetuning.
 #modelinstance.setparameters(input="use this as context", max_tokens=128, top_p=12, top_k=40) #optional, look into .info['available_methods']['setparameters'] for more details.
 print(modelinstance.info['available_methods'])
 model1 = endpointIO(modelinstance.testinferenceIO) #still some testing to do in actual alpaca inferneceIO.
 model1.run()
 ```
+todo:
+- [ ] test alpaca lora with deployment
+- [ ] fix dynamic installation issue
+- [ ] add endpoint for info about deployed model
+
```

### Comparing `streamai-0.0.1/setup.py` & `streamai-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from setuptools import setup, find_packages
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 setup(name='streamai',
-      version='0.0.1',
-      description='serve ai agents as api easily.',
+      version='0.0.2',
+      description='serve ai agents/models easily as api.',
       author='Navdeep Dhakar',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
```

### Comparing `streamai-0.0.1/streamai/alpacalora/export_hf_checkpoint.py` & `streamai-0.0.2/streamai/alpacalora/export_hf_checkpoint.py`

 * *Files identical despite different names*

### Comparing `streamai-0.0.1/streamai/alpacalora/export_state_dict_checkpoint.py` & `streamai-0.0.2/streamai/alpacalora/export_state_dict_checkpoint.py`

 * *Files identical despite different names*

### Comparing `streamai-0.0.1/streamai/alpacalora/finetune.py` & `streamai-0.0.2/streamai/alpacalora/finetune.py`

 * *Files identical despite different names*

### Comparing `streamai-0.0.1/streamai/alpacalora/generate.py` & `streamai-0.0.2/streamai/alpacalora/generate.py`

 * *Files identical despite different names*

### Comparing `streamai-0.0.1/streamai/alpacalora/inference.py` & `streamai-0.0.2/streamai/alpacalora/inference.py`

 * *Files identical despite different names*

### Comparing `streamai-0.0.1/streamai/alpacalora/train.py` & `streamai-0.0.2/streamai/alpacalora/train.py`

 * *Files identical despite different names*

### Comparing `streamai-0.0.1/streamai/alpacalora/uptest.py` & `streamai-0.0.2/streamai/alpacalora/uptest.py`

 * *Files identical despite different names*

### Comparing `streamai-0.0.1/streamai/alpacalora/utils/callbacks.py` & `streamai-0.0.2/streamai/alpacalora/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `streamai-0.0.1/streamai/alpacalora/utils/prompter.py` & `streamai-0.0.2/streamai/alpacalora/utils/prompter.py`

 * *Files identical despite different names*

### Comparing `streamai-0.0.1/streamai/app.py` & `streamai-0.0.2/streamai/app.py`

 * *Files identical despite different names*

### Comparing `streamai-0.0.1/streamai/llms/alpacalora.py` & `streamai-0.0.2/streamai/llms/alpacalora.py`

 * *Files identical despite different names*

### Comparing `streamai-0.0.1/streamai.egg-info/PKG-INFO` & `streamai-0.0.2/streamai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: streamai
-Version: 0.0.1
-Summary: serve ai agents as api easily.
+Version: 0.0.2
+Summary: serve ai agents/models easily as api.
 Author: Navdeep Dhakar
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## 🌩️ Stream AI easily
 ### streamai let's you serve any AI agents/model(currently llms only) easily as api and integrate in fontend quickly.
-todo:
-- [ ] test alpaca lora with deployment
-- [ ] fix dynamic installation issue
-- [ ] add endpoint for info about deployed model
+
 #### deploy from custom model script
 ```py
 from streamai.app import endpointIO
-from streamai.models import Autoalpacalora
+from streamai.llms import Autoalpacalora
 def custom_model_IO(input:str):
     output = customodelinference(input) #depend on your inference function, just need to return string output from it.
     return f"this is output of {output}"
     
 model1 = endpointIO(custom_model_IO)
 model1.run() #this will create a server api endpoint for your model, at http://0.0.0.0:8000 see terminal logs for more info about endpoints
 ```
 #### deploy from inbuild models libs(you can also finetun inbuilt models)
 ```py
 from streamai.app import endpointIO
-from streamai.models import Autoalpacalora
+from streamai.llms import Autoalpacalora
     
 modelinstance = Autoalpacalora("decapoda/llama-7b", "./scroltest")
 #modelinstance.loadmodel() #required for deployment of model as api, not required during finetuning.
 #modelinstance.setparameters(input="use this as context", max_tokens=128, top_p=12, top_k=40) #optional, look into .info['available_methods']['setparameters'] for more details.
 print(modelinstance.info['available_methods'])
 model1 = endpointIO(modelinstance.testinferenceIO) #still some testing to do in actual alpaca inferneceIO.
 model1.run()
 ```
+todo:
+- [ ] test alpaca lora with deployment
+- [ ] fix dynamic installation issue
+- [ ] add endpoint for info about deployed model
+
```

### Comparing `streamai-0.0.1/streamai.egg-info/SOURCES.txt` & `streamai-0.0.2/streamai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

