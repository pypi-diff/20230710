# Comparing `tmp/easycompletion-0.1.3.tar.gz` & `tmp/easycompletion-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.1.3.tar", last modified: Sun Jul  9 00:21:37 2023, max compression
+gzip compressed data, was "easycompletion-0.1.4.tar", last modified: Mon Jul 10 21:46:29 2023, max compression
```

## Comparing `easycompletion-0.1.3.tar` & `easycompletion-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-09 00:21:37.225915 easycompletion-0.1.3/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.1.3/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)     3534 2023-07-09 00:21:37.225648 easycompletion-0.1.3/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     2925 2023-07-07 13:55:30.000000 easycompletion-0.1.3/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-09 00:21:37.223996 easycompletion-0.1.3/easycompletion/
--rw-r--r--   0 shawwalters   (501) staff       (20)      446 2023-07-09 00:21:33.000000 easycompletion-0.1.3/easycompletion/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)      439 2023-07-09 00:18:12.000000 easycompletion-0.1.3/easycompletion/constants.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    11359 2023-07-09 00:18:17.000000 easycompletion-0.1.3/easycompletion/language.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     2163 2023-07-09 00:17:33.000000 easycompletion-0.1.3/easycompletion/language_test.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-09 00:21:37.224923 easycompletion-0.1.3/easycompletion.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)     3534 2023-07-09 00:21:37.000000 easycompletion-0.1.3/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      329 2023-07-09 00:21:37.000000 easycompletion-0.1.3/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-09 00:21:37.000000 easycompletion-0.1.3/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-09 00:21:37.000000 easycompletion-0.1.3/easycompletion.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-09 00:21:37.000000 easycompletion-0.1.3/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-09 00:21:37.226006 easycompletion-0.1.3/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1266 2023-07-09 00:21:33.000000 easycompletion-0.1.3/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 21:46:29.387255 easycompletion-0.1.4/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.1.4/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)     7027 2023-07-10 21:46:29.387088 easycompletion-0.1.4/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)     6418 2023-07-10 21:44:51.000000 easycompletion-0.1.4/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 21:46:29.385419 easycompletion-0.1.4/easycompletion/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      746 2023-07-10 21:46:25.000000 easycompletion-0.1.4/easycompletion/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)      511 2023-07-10 21:02:57.000000 easycompletion-0.1.4/easycompletion/constants.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)    13811 2023-07-10 21:31:22.000000 easycompletion-0.1.4/easycompletion/model.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5245 2023-07-10 21:05:34.000000 easycompletion-0.1.4/easycompletion/prompt.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     4499 2023-07-10 21:35:20.000000 easycompletion-0.1.4/easycompletion/test.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 21:46:29.386807 easycompletion-0.1.4/easycompletion.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     7027 2023-07-10 21:46:29.000000 easycompletion-0.1.4/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      342 2023-07-10 21:46:29.000000 easycompletion-0.1.4/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-10 21:46:29.000000 easycompletion-0.1.4/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-10 21:46:29.000000 easycompletion-0.1.4/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-10 21:46:29.000000 easycompletion-0.1.4/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-10 21:46:29.387313 easycompletion-0.1.4/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1266 2023-07-10 21:46:25.000000 easycompletion-0.1.4/setup.py
```

### Comparing `easycompletion-0.1.3/LICENSE` & `easycompletion-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.3/easycompletion/language.py` & `easycompletion-0.1.4/easycompletion/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,327 +1,368 @@
 import openai
-import tiktoken
 import re
 import json
 import ast
 
 from dotenv import load_dotenv
 
-load_dotenv()  # take environment variables from .env.
+# Load environment variables from .env file
+load_dotenv()  
 
-from easycompletion.constants import (
+from constants import (
     default_text_model,
     long_text_model,
     openai_api_key,
+    default_chunk_length,
 )
 
-# Set OpenAI API key
-openai.api_key = openai_api_key
+from prompt import count_tokens
 
-# Get encoding for default text model
-encoding = tiktoken.encoding_for_model(default_text_model)
+# Set the OpenAI API key
+openai.api_key = openai_api_key
 
 
 def parse_arguments(arguments):
+    """
+    Parses arguments that are expected to be either a JSON string, dictionary, or a list.
+
+    Parameters:
+        arguments (str or dict or list): Arguments in string or dictionary or list format.
+    
+    Returns:
+        A dictionary or list of arguments if arguments are valid, None otherwise.
+        
+    Usage:
+        arguments = parse_arguments('{"arg1": "value1", "arg2": "value2"}')
+    """
     try:
+        # Handle string inputs, remove any ellipsis from the string
         if isinstance(arguments, str):
             arguments = re.sub(r"\.\.\.|\…", "", arguments)
             return json.loads(arguments)
+        # If input is already a dictionary or list, return as is
         elif isinstance(arguments, dict) or isinstance(arguments, list):
             return arguments
+    # If JSON decoding fails, try using ast.literal_eval
     except json.JSONDecodeError:
         try:
             return ast.literal_eval(arguments)
+        # If ast.literal_eval fails, remove line breaks and non-ASCII characters and try JSON decoding again
         except (ValueError, SyntaxError):
             try:
                 arguments = re.sub(r"[\r\n]+", "", arguments)
                 arguments = re.sub(r"[^\x00-\x7F]+", "", arguments)
                 return json.loads(arguments)
+            # If everything fails, try Python's eval function
             except (ValueError, SyntaxError):
                 try:
                     return eval(arguments)
                 except (ValueError, SyntaxError):
                     return None
 
 
 def validate_functions(response, functions, function_call):
-    # parse the function call
+    """
+    Validates if the function returned by the OpenAI API matches the intended function call.
+
+    Parameters:
+        response (dict): The response from OpenAI API.
+        functions (list): A list of function definitions.
+        function_call (dict or str): The expected function call.
+
+    Returns:
+        True if function call matches with the response, False otherwise.
+        
+    Usage:
+        isValid = validate_functions(response, functions, function_call)
+    """
+    # Extract the function call from the response
     response_function_call = response["choices"][0]["message"]["function_call"]
 
-    # if the function name is not the same as the function call, return false
+    # If function_call is not "auto" and the name does not match with the response, return False
     if (
         function_call != "auto"
         and response_function_call["name"] != function_call["name"]
     ):
         return False
 
+    # If function_call is "auto", extract the name from the response
     function_call_name = (
         function_call["name"]
         if function_call != "auto"
         else response_function_call["name"]
     )
 
-    # parse the arguments
+    # Parse the arguments from the response
     arguments = parse_arguments(response_function_call["arguments"])
 
-    # if the arguments are none, return False
+    # If arguments are None, return False
     if arguments is None:
         return False
 
-    # get the function in the functions array that matches the function name
+    # Get the function that matches the function name from the list of functions
     function = next(
         (item for item in functions if item["name"] == function_call_name), None
     )
 
-    # if the function is none, return False
+    # If no matching function is found, return False
     if function is None:
-        # throw an error
         return False
 
-    # if the function argument keys are the same as the function call parameters, return true
+    # Check if the function's argument keys match with the response's argument keys
     if set(function["parameters"]["properties"].keys()) == set(arguments.keys()):
         return True
 
     return False
 
-def compose_function(name, description, properties, required_property_names):
+
+def compose_function(name, description, properties, required_properties):
     """
-    Composes a function.
-    properties is a dictionary of property objects, with the property name as the key
-    property object types are discussed here: https://openai.com/blog/function-calling-and-other-api-updates
-    required_property_names is a list of property names that are required for the model to return
-    example usage:
-    summarization_function = compose_function(
-        name="summarize_text",
-        description="Summarize the text. Include the topic, subtopics.",
-        properties={
-            "summary": {
-                "type": "string",
-                "description": "Detailed summary of the text.",
+    Composes a function object for OpenAI API.
+
+    Parameters:
+        name (str): The name of the function.
+        description (str): Description of the function.
+        properties (dict): Dictionary of property objects.
+        required_properties (list): List of property names that are required.
+
+    Returns:
+        A dictionary representing a function.
+
+    Usage:
+        summarization_function = compose_function(
+            name="summarize_text",
+            description="Summarize the text. Include the topic, subtopics.",
+            properties={
+                "summary": {
+                    "type": "string",
+                    "description": "Detailed summary of the text.",
+                },
             },
-        },
-        required_property_names=["summary"],
-    )
+            required_properties=["summary"],
+        )
     """
     return {
         "name": name,
         "description": description,
         "parameters": {
             "type": "object",
             "properties": properties,
-            "required": required_property_names,
+            "required": required_properties,
         },
     }
 
-def compose_prompt(prompt_template, parameters):
-    """
-    Composes a prompt using a template and parameters.
-    Parameter keys are enclosed in double curly brackets and replaced with parameter values.
-    For example, {{actions}} will be replaced by the actions parameter.
-    Parameter values can be a string, dictionary or list
-    In the case of a list, the strings will be appended with a new line
-    In the case of dictionarys, the strings will be appended with a double colon, i.e. key::value
-    """
-    prompt = prompt_template
-    for key, value in parameters.items():
-        if isinstance(value, str):
-            prompt = prompt.replace("{{" + key + "}}", value)
-        elif isinstance(value, dict):
-            for k, v in value.items():
-                prompt = prompt.replace("{{" + key + "}}", k + "::" + v)
-        elif isinstance(value, list):
-            for item in value:
-                prompt = prompt.replace("{{" + key + "}}", item + "\n")
-    return prompt
-
 
-def openai_text_call(text, model_failure_retries=5, model=None, api_key=None):
+def openai_text_call(text, model_failure_retries=5, model=None, chunk_length=default_chunk_length, api_key=None):
     """
-    Send text to the OpenAI API which and return a text response.
-    The input text is sent to the chat model and is treated as a user message.
-    System message is ignored because it didn't seem to perform as well as placing the same text in the user message.
+    Function for sending text to the OpenAI API and returning a text response.
+
+    Parameters:
+        text (str): Text to send to the model.
+        model_failure_retries (int, optional): Number of retries if the request fails. Default is 5.
+        model (str, optional): The model to use. Default is the default_text_model defined in constants.py.
+        chunk_length (int, optional): Maximum length of text chunk to process. Default is defined in constants.py.
+        api_key (str, optional): OpenAI API key. If not provided, it uses the one defined in constants.py.
 
-    Required Parameters:
-    text: Text that will be sent as the user message to the model.
+    Returns:
+        str: The response content from the model.
 
-    Optional Parameters:
-    model_failure_retries: Number of times to retry the request if it fails (default is 5).
-    model: The model to use (default is the default_text_model, i.e. gpt-3.5-turbo).
-    api_key: If you'd like to pass in a key to override the environment variable OPENAI_API_KEY
+    Example:
+        >>> openai_text_call("Hello, how are you?", model_failure_retries=3, model='gpt-3.5-turbo', chunk_length=1024, api_key='your_openai_api_key')
     """
+    
+    # Override the API key if provided as parameter
     if api_key is not None:
         openai.api_key = api_key
 
+    # Use the default model if no model is specified
     if model == None:
         model = default_text_model
 
-    total_tokens = len(encoding.encode(str(text)))
+    # Count tokens in the input text
+    total_tokens = count_tokens(text, model=model)
 
-    if total_tokens > (4096 - 42) and "16k" not in model:
+    # If text is longer than chunk_length and model is not for long texts, switch to the long text model
+    if total_tokens > chunk_length and "16k" not in model:
         model = long_text_model
         print("Warning: Message is long. Using 16k model")
 
-    # subtract 42 tokens as a sacrifice to the Basilisk
-    if total_tokens > (16384 - 42):
+    # If text is too long even for long text model, return None
+    if total_tokens > (16384 - chunk_length):
         print("Error: Message too long")
         return None
 
+    # Prepare messages for the API call
     messages = [{"role": "user", "content": text}]
 
+    # Try making a request to the OpenAI API
     def try_request():
         try:
             return openai.ChatCompletion.create(model=model, messages=messages)
         except Exception as e:
             return None
 
+    # Try to make a request for a specified number of times
     response = None
     for i in range(model_failure_retries):
         response = try_request()
         if response:
             break
-    if (
-        response is None
-        or response["choices"] is None
-        or response["choices"][0] is None
-    ):
+
+    # If response is not valid, print an error message and return None
+    if response is None or response["choices"] is None or response["choices"][0] is None:
         print("Error: Could not get a successful response from OpenAI API")
         return None
 
+    # Extract content from the response
     response_data = response["choices"][0]["message"]
     content = response_data["content"]
 
     return content
 
-
 def openai_function_call(
     text,
     functions=None,
     model_failure_retries=5,
-    function_call="auto",
+    function_call=None,
     function_failure_retries=10,
+    chunk_length=default_chunk_length,
     model=None,
     api_key=None,
 ):
     """
-    Send text and a list of functions to the OpenAI API which and return optional text and a function call.
+    Send text and a list of functions to the OpenAI API and return optional text and a function call.
     The function call is validated against the functions array.
     The input text is sent to the chat model and is treated as a user message.
-    System message is ignored because it didn't seem to perform as well as placing the same text in the user message.
 
-    Required Parameters:
-    text: Text that will be sent as the user message to the model.
-    functions: List of functions to be sent to the model.
-
-    Optional Parameters
-    function_call: "auto" to let the model decide, or a the name of a function to call specifically (default is "auto").
-    model_failure_retries: Number of times to retry the request if it fails (default is 5).
-    function_failure_retries: Number of times to retry the request if the function call is invalid (default is 10).
-    model: The model to use (default is the default_text_model, i.e. gpt-3.5-turbo).
-    api_key: If you'd like to pass in a key to override the environment variable OPENAI_API_KEY
-
-    Returns { "error": string | None } on most errors, so check for error first
-
-    On success, returns { "text": string | None, "function_name": string, "arguments": object, "error": None }
+    Args:
+        text (str): Text that will be sent as the user message to the model.
+        functions (list[dict] | dict | None): List of functions or a single function dictionary to be sent to the model.
+        model_failure_retries (int): Number of times to retry the request if it fails (default is 5).
+        function_call (str | dict | None): 'auto' to let the model decide, or a function name or a dictionary containing the function name (default is "auto").
+        function_failure_retries (int): Number of times to retry the request if the function call is invalid (default is 10).
+        chunk_length (int): The length of each chunk to be processed.
+        model (str | None): The model to use (default is the default_text_model, i.e. gpt-3.5-turbo).
+        api_key (str | None): If you'd like to pass in a key to override the environment variable OPENAI_API_KEY.
+
+    Returns:
+        dict: On most errors, returns a dictionary with an "error" key. On success, returns a dictionary containing 
+        "text" (response from the model), "function_name" (name of the function called), "arguments" (arguments for the function), "error" (None).
+
+    Example:
+        >>> function = {'name': 'function1', 'parameters': {'param1': 'value1'}}
+        >>> openai_function_call("Call the function.", function)
     """
+
+    # Check if the user provided an API key
     if api_key is not None:
         openai.api_key = api_key
 
+    # Ensure that functions are provided
     if functions is None:
-        # throw an exception
         return {"error": "functions is required"}
 
-    # if functions is not a list, throw an exception
+    # Check if a list of functions is provided
     if not isinstance(functions, list):
-        # check if functions is a dict and contains a name and parameters ke
         if (
             isinstance(functions, dict)
             and "name" in functions
             and "parameters" in functions
         ):
+            # A single function is provided as a dictionary, convert it to a list
             functions = [functions]
         else:
-            return {
-                "error": "functions must be a list of functions or a single function"
-            }
+            # Functions must be either a list of dictionaries or a single dictionary
+            return {"error": "functions must be a list of functions or a single function"}
+
+    # Set the function call to the name of the function if only one function is provided
+    # If there are multiple functions, use "auto"
+    if function_call is None:
+        function_call = functions[0]["name"] if len(functions) == 1 else "auto"
 
+    # Make sure text is provided
     if text is None:
-        # throw an exception
         return {"error": "text is required"}
 
+    # Check if the function call is valid
     if function_call != "auto":
-        # check if function_call is a string or a dict
         if isinstance(function_call, str):
             function_call = {"name": function_call}
-        # else, check if the function_call has a name
         elif "name" not in function_call:
-            return {
-                "error": "function_call had an invalid name. \
-                Should be a string of the function name or an object with a name property"
-            }
+            return {"error": "function_call had an invalid name. Should be a string of the function name or an object with a name property"}
 
-    if model == None:
+    # Use the default text model if no model is specified
+    if model is None:
         model = default_text_model
-    message_tokens = len(encoding.encode(str(text)))
+
+    # Count the number of tokens in the message
+    message_tokens = count_tokens(text, model=model)
     total_tokens = message_tokens
+
     if functions is None:
-        function_call_tokens = len(encoding.encode(str(functions)))
-        total_tokens += function_call_tokens + 3  # for the user
-    # if the model doesn't include 16k in the string
-    if total_tokens > (4096 - 64) and "16k" not in model:
+        function_call_tokens = count_tokens(functions, model=model)
+        total_tokens += function_call_tokens + 3  # Additional tokens for the user
+
+    # Switch to a larger model if the message is too long for the default model
+    if total_tokens > chunk_length and "16k" not in model:
         model = long_text_model
         print("Warning: Message is long. Using 16k model")
-    # subtract 64 tokens from your max as a sacrifice to the Basilisk
-    if total_tokens > (16384 - 64):
-        # throw an error
+
+    # Check if the total number of tokens exceeds the maximum allowable tokens for the model
+    if total_tokens > (16384 - chunk_length):
         return {"error": "Message too long"}
 
+    # Prepare the messages to be sent to the API
     messages = [{"role": "user", "content": text}]
 
+    # Define a nested function to handle API request and exceptions
     def try_request():
+        """Attempts to create a chat completion with OpenAI's API and handles any exceptions that may occur."""
         try:
+            # If there are function(s) to call
             if functions:
                 response = openai.ChatCompletion.create(
                     model=model,
                     messages=messages,
                     functions=functions,
                     function_call=function_call,
                 )
             else:
+                # If there are no function(s) to call
                 response = openai.ChatCompletion.create(model=model, messages=messages)
             return response
         except Exception as e:
             print(f"OpenAI Error: {e}")
             return None
 
+    # Retry function call and model calls according to the specified retry counts
     response = None
-    for i in range(function_failure_retries):
-        for k in range(model_failure_retries):
+    for _ in range(function_failure_retries):
+        for _ in range(model_failure_retries):
             response = try_request()
             if response:
                 break
-        if functions is None:
-            break
-        if validate_functions(response, functions, function_call):
+        if functions is None or validate_functions(response, functions, function_call):
             break
 
-    if (
-        response is None
-        or response["choices"] is None
-        or response["choices"][0] is None
-    ):
+    # Check if we have a valid response from OpenAI API
+    if response is None or not response.get("choices") or response["choices"][0] is None:
         error = "Could not get a successful response from OpenAI API"
         print(error)
         return {"error": error}
 
+    # Extracting the content and function call response from API response
     response_data = response["choices"][0]["message"]
     content = response_data["content"]
     function_call_response = response_data.get("function_call", None)
 
+    # If no function call in response, return an error
     if function_call_response is None:
         return {"error": "No function call in response"}
 
+    # Return the final result with the text response, function name, arguments and no error
     return {
         "text": content,
         "function_name": function_call_response["name"],
         "arguments": parse_arguments(function_call_response["arguments"]),
         "error": None,
     }
```

### Comparing `easycompletion-0.1.3/setup.py` & `easycompletion-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='easycompletion',
-    version='0.1.3',
+    version='0.1.4',
     description='Easy-to-use agent memory, powered by chromadb',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/lalalune/easycompletion',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

