# Comparing `tmp/easycompletion-0.1.4.tar.gz` & `tmp/easycompletion-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.1.4.tar", last modified: Mon Jul 10 21:46:29 2023, max compression
+gzip compressed data, was "easycompletion-0.1.5.tar", last modified: Mon Jul 10 21:51:37 2023, max compression
```

## Comparing `easycompletion-0.1.4.tar` & `easycompletion-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 21:46:29.387255 easycompletion-0.1.4/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.1.4/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)     7027 2023-07-10 21:46:29.387088 easycompletion-0.1.4/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     6418 2023-07-10 21:44:51.000000 easycompletion-0.1.4/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 21:46:29.385419 easycompletion-0.1.4/easycompletion/
--rw-r--r--   0 shawwalters   (501) staff       (20)      746 2023-07-10 21:46:25.000000 easycompletion-0.1.4/easycompletion/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)      511 2023-07-10 21:02:57.000000 easycompletion-0.1.4/easycompletion/constants.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    13811 2023-07-10 21:31:22.000000 easycompletion-0.1.4/easycompletion/model.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     5245 2023-07-10 21:05:34.000000 easycompletion-0.1.4/easycompletion/prompt.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     4499 2023-07-10 21:35:20.000000 easycompletion-0.1.4/easycompletion/test.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 21:46:29.386807 easycompletion-0.1.4/easycompletion.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)     7027 2023-07-10 21:46:29.000000 easycompletion-0.1.4/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      342 2023-07-10 21:46:29.000000 easycompletion-0.1.4/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-10 21:46:29.000000 easycompletion-0.1.4/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-10 21:46:29.000000 easycompletion-0.1.4/easycompletion.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-10 21:46:29.000000 easycompletion-0.1.4/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-10 21:46:29.387313 easycompletion-0.1.4/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1266 2023-07-10 21:46:25.000000 easycompletion-0.1.4/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 21:51:37.943402 easycompletion-0.1.5/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.1.5/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)     6663 2023-07-10 21:51:37.943232 easycompletion-0.1.5/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5917 2023-07-10 21:51:01.000000 easycompletion-0.1.5/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 21:51:37.941882 easycompletion-0.1.5/easycompletion/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      746 2023-07-10 21:51:34.000000 easycompletion-0.1.5/easycompletion/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)      511 2023-07-10 21:02:57.000000 easycompletion-0.1.5/easycompletion/constants.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)    13811 2023-07-10 21:31:22.000000 easycompletion-0.1.5/easycompletion/model.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5245 2023-07-10 21:05:34.000000 easycompletion-0.1.5/easycompletion/prompt.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     4499 2023-07-10 21:35:20.000000 easycompletion-0.1.5/easycompletion/test.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 21:51:37.942909 easycompletion-0.1.5/easycompletion.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     6663 2023-07-10 21:51:37.000000 easycompletion-0.1.5/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      342 2023-07-10 21:51:37.000000 easycompletion-0.1.5/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-10 21:51:37.000000 easycompletion-0.1.5/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       23 2023-07-10 21:51:37.000000 easycompletion-0.1.5/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-10 21:51:37.000000 easycompletion-0.1.5/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-10 21:51:37.943471 easycompletion-0.1.5/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1408 2023-07-10 21:51:34.000000 easycompletion-0.1.5/setup.py
```

### Comparing `easycompletion-0.1.4/LICENSE` & `easycompletion-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.4/PKG-INFO` & `easycompletion-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.1.4
-Summary: Easy-to-use agent memory, powered by chromadb
+Version: 0.1.5
+Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/lalalune/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # easycompletion
 
-Easy function calling using OpenAI's API. Handles a lot of the annoying boilerplate. Useful if you want a clean, validated response. Simple codebase, made after many hours of frustration with the various pitfalls and instabilities of the OpenAI API.
+Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 
 
 # Installation
 
 ```bash
 pip install easycompletion
 ```
@@ -32,14 +32,15 @@
 ## Importing
 
 ```python
 from easycompletion import openai_function_call, openai_text_call, compose_prompt
 ```
 
 ## Quickstart
+
 ```python
 from easycompletion import openai_function_call, openai_text_call, compose_prompt
 
 # Compose a function object
 test_function = compose_function(
     name="write_song",
     description="Write a song about AI",
@@ -79,14 +80,15 @@
 ```python
 from easycompletion import openai_text_call
 response = openai_text_call("Hello, how are you?")
 # response = "As an AI language model, I don't have feelings, but...""
 ```
 
 ## Compose a Function
+
 ```python
 
 Composes a function object for OpenAI API.
 
 test_function = compose_function(
     name="write_song",
     description="Write a song about AI",
@@ -112,30 +114,14 @@
 response = openai_function_call(text="Write a song about AI", functions=[test_function], function_call="write_song")
 # Response structure is { "text": string, "function_name": string, "arguments": dict  }
 print(response["arguments"]["lyrics"])
 ```
 
 # Advanced Usage
 
-### `parse_arguments(arguments)`
-
-Parses arguments that are expected to be either a JSON string, dictionary, or a list.
-
-```python
-arguments = parse_arguments('{"arg1": "value1", "arg2": "value2"}')
-```
-
-### `validate_functions(response, functions, function_call)`
-
-Validates if the function returned by the OpenAI API matches the intended function call.
-
-```python
-isValid = validate_functions(response, functions, function_call)
-```
-
 ### `compose_function(name, description, properties, required_properties)`
 
 Composes a function object for OpenAI API.
 
 ```python
 summarization_function = compose_function(
     name="summarize_text",
```

### Comparing `easycompletion-0.1.4/README.md` & `easycompletion-0.1.5/easycompletion.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,29 @@
+Metadata-Version: 2.1
+Name: easycompletion
+Version: 0.1.5
+Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
+Home-page: https://github.com/lalalune/easycompletion
+Author: Moon
+Author-email: shawmakesmagic@gmail.com
+License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # easycompletion
 
-Easy function calling using OpenAI's API. Handles a lot of the annoying boilerplate. Useful if you want a clean, validated response. Simple codebase, made after many hours of frustration with the various pitfalls and instabilities of the OpenAI API.
+Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 
-<img src="resources/image.jpg">
 
 # Installation
 
 ```bash
 pip install easycompletion
 ```
 
@@ -15,14 +32,15 @@
 ## Importing
 
 ```python
 from easycompletion import openai_function_call, openai_text_call, compose_prompt
 ```
 
 ## Quickstart
+
 ```python
 from easycompletion import openai_function_call, openai_text_call, compose_prompt
 
 # Compose a function object
 test_function = compose_function(
     name="write_song",
     description="Write a song about AI",
@@ -62,14 +80,15 @@
 ```python
 from easycompletion import openai_text_call
 response = openai_text_call("Hello, how are you?")
 # response = "As an AI language model, I don't have feelings, but...""
 ```
 
 ## Compose a Function
+
 ```python
 
 Composes a function object for OpenAI API.
 
 test_function = compose_function(
     name="write_song",
     description="Write a song about AI",
@@ -95,30 +114,14 @@
 response = openai_function_call(text="Write a song about AI", functions=[test_function], function_call="write_song")
 # Response structure is { "text": string, "function_name": string, "arguments": dict  }
 print(response["arguments"]["lyrics"])
 ```
 
 # Advanced Usage
 
-### `parse_arguments(arguments)`
-
-Parses arguments that are expected to be either a JSON string, dictionary, or a list.
-
-```python
-arguments = parse_arguments('{"arg1": "value1", "arg2": "value2"}')
-```
-
-### `validate_functions(response, functions, function_call)`
-
-Validates if the function returned by the OpenAI API matches the intended function call.
-
-```python
-isValid = validate_functions(response, functions, function_call)
-```
-
 ### `compose_function(name, description, properties, required_properties)`
 
 Composes a function object for OpenAI API.
 
 ```python
 summarization_function = compose_function(
     name="summarize_text",
```

### Comparing `easycompletion-0.1.4/easycompletion/__init__.py` & `easycompletion-0.1.5/easycompletion/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 easycompletion
 
 Leveraging conversational AI for bicameral decision making.
 """
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 __author__ = "Moon (https://github.com/lalalune)"
 __credits__ = "https://github.com/lalalune/easycompletion"
 
 from .model import (
     openai_function_call,
     openai_text_call,
     compose_function,
```

### Comparing `easycompletion-0.1.4/easycompletion/model.py` & `easycompletion-0.1.5/easycompletion/model.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.4/easycompletion/prompt.py` & `easycompletion-0.1.5/easycompletion/prompt.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.4/easycompletion/test.py` & `easycompletion-0.1.5/easycompletion/test.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.4/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-Metadata-Version: 2.1
-Name: easycompletion
-Version: 0.1.4
-Summary: Easy-to-use agent memory, powered by chromadb
-Home-page: https://github.com/lalalune/easycompletion
-Author: Moon
-Author-email: shawmakesmagic@gmail.com
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # easycompletion
 
-Easy function calling using OpenAI's API. Handles a lot of the annoying boilerplate. Useful if you want a clean, validated response. Simple codebase, made after many hours of frustration with the various pitfalls and instabilities of the OpenAI API.
+Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 
+<img src="resources/image.jpg">
 
 # Installation
 
 ```bash
 pip install easycompletion
 ```
 
@@ -32,14 +15,15 @@
 ## Importing
 
 ```python
 from easycompletion import openai_function_call, openai_text_call, compose_prompt
 ```
 
 ## Quickstart
+
 ```python
 from easycompletion import openai_function_call, openai_text_call, compose_prompt
 
 # Compose a function object
 test_function = compose_function(
     name="write_song",
     description="Write a song about AI",
@@ -79,14 +63,15 @@
 ```python
 from easycompletion import openai_text_call
 response = openai_text_call("Hello, how are you?")
 # response = "As an AI language model, I don't have feelings, but...""
 ```
 
 ## Compose a Function
+
 ```python
 
 Composes a function object for OpenAI API.
 
 test_function = compose_function(
     name="write_song",
     description="Write a song about AI",
@@ -112,30 +97,14 @@
 response = openai_function_call(text="Write a song about AI", functions=[test_function], function_call="write_song")
 # Response structure is { "text": string, "function_name": string, "arguments": dict  }
 print(response["arguments"]["lyrics"])
 ```
 
 # Advanced Usage
 
-### `parse_arguments(arguments)`
-
-Parses arguments that are expected to be either a JSON string, dictionary, or a list.
-
-```python
-arguments = parse_arguments('{"arg1": "value1", "arg2": "value2"}')
-```
-
-### `validate_functions(response, functions, function_call)`
-
-Validates if the function returned by the OpenAI API matches the intended function call.
-
-```python
-isValid = validate_functions(response, functions, function_call)
-```
-
 ### `compose_function(name, description, properties, required_properties)`
 
 Composes a function object for OpenAI API.
 
 ```python
 summarization_function = compose_function(
     name="summarize_text",
```

### Comparing `easycompletion-0.1.4/setup.py` & `easycompletion-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from setuptools import setup
 
 long_description = ""
 with open("README.md", "r") as fh:
     long_description = fh.read()
     # search for any lines that contain <img and remove them
-    long_description = long_description.split('\n')
-    long_description = [line for line in long_description if not '<img' in line]
+    long_description = long_description.split("\n")
+    long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
-    long_description = '\n'.join(long_description)
-    
+    long_description = "\n".join(long_description)
+
 
 setup(
-    name='easycompletion',
-    version='0.1.4',
-    description='Easy-to-use agent memory, powered by chromadb',
+    name="easycompletion",
+    version='0.1.5',
+    description="Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
-    url='https://github.com/lalalune/easycompletion',
-    author='Moon',
-    author_email='shawmakesmagic@gmail.com',
-    license='MIT',
-    packages=['easycompletion'],
-    install_requires=['chromadb'],
-    readme = "README.md",
+    url="https://github.com/lalalune/easycompletion",
+    author="Moon",
+    author_email="shawmakesmagic@gmail.com",
+    license="MIT",
+    packages=["easycompletion"],
+    install_requires=["openai", "tiktoken", "dotenv"],
+    readme="README.md",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',  
-        'Operating System :: POSIX :: Linux',        
-        'Programming Language :: Python :: 3',
-        'Operating System :: MacOS :: MacOS X',
-        'Operating System :: Microsoft :: Windows'
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: POSIX :: Linux",
+        "Programming Language :: Python :: 3",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
     ],
 )
```

