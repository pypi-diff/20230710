# Comparing `tmp/language-agent-0.1.tar.gz` & `tmp/language-agent-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "language-agent-0.1.tar", last modified: Mon Jul 10 13:42:15 2023, max compression
+gzip compressed data, was "language-agent-0.2.tar", last modified: Mon Jul 10 13:53:57 2023, max compression
```

## Comparing `language-agent-0.1.tar` & `language-agent-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andi       (501) staff       (20)        0 2023-07-10 13:42:15.370245 language-agent-0.1/
--rw-r--r--   0 andi       (501) staff       (20)     1790 2023-07-10 13:42:15.370128 language-agent-0.1/PKG-INFO
-drwxr-xr-x   0 andi       (501) staff       (20)        0 2023-07-10 13:42:15.368713 language-agent-0.1/language_agent/
--rw-r--r--   0 andi       (501) staff       (20)        1 2023-07-10 13:14:29.000000 language-agent-0.1/language_agent/__init__.py
--rw-r--r--   0 andi       (501) staff       (20)      406 2023-07-10 13:06:34.000000 language-agent-0.1/language_agent/module.py
--rw-r--r--   0 andi       (501) staff       (20)      166 2023-07-10 13:18:31.000000 language-agent-0.1/language_agent/prompt.py
-drwxr-xr-x   0 andi       (501) staff       (20)        0 2023-07-10 13:42:15.369962 language-agent-0.1/language_agent.egg-info/
--rw-r--r--   0 andi       (501) staff       (20)     1790 2023-07-10 13:42:15.000000 language-agent-0.1/language_agent.egg-info/PKG-INFO
--rw-r--r--   0 andi       (501) staff       (20)      274 2023-07-10 13:42:15.000000 language-agent-0.1/language_agent.egg-info/SOURCES.txt
--rw-r--r--   0 andi       (501) staff       (20)        1 2023-07-10 13:42:15.000000 language-agent-0.1/language_agent.egg-info/dependency_links.txt
--rw-r--r--   0 andi       (501) staff       (20)       21 2023-07-10 13:42:15.000000 language-agent-0.1/language_agent.egg-info/requires.txt
--rw-r--r--   0 andi       (501) staff       (20)       15 2023-07-10 13:42:15.000000 language-agent-0.1/language_agent.egg-info/top_level.txt
--rw-r--r--   0 andi       (501) staff       (20)       38 2023-07-10 13:42:15.370286 language-agent-0.1/setup.cfg
--rw-r--r--   0 andi       (501) staff       (20)      504 2023-07-10 13:41:47.000000 language-agent-0.1/setup.py
+drwxr-xr-x   0 andi       (501) staff       (20)        0 2023-07-10 13:53:57.568781 language-agent-0.2/
+-rw-r--r--   0 andi       (501) staff       (20)     1812 2023-07-10 13:53:57.568648 language-agent-0.2/PKG-INFO
+drwxr-xr-x   0 andi       (501) staff       (20)        0 2023-07-10 13:53:57.567654 language-agent-0.2/language_agent/
+-rw-r--r--   0 andi       (501) staff       (20)        1 2023-07-10 13:14:29.000000 language-agent-0.2/language_agent/__init__.py
+-rw-r--r--   0 andi       (501) staff       (20)      406 2023-07-10 13:06:34.000000 language-agent-0.2/language_agent/module.py
+-rw-r--r--   0 andi       (501) staff       (20)      166 2023-07-10 13:18:31.000000 language-agent-0.2/language_agent/prompt.py
+drwxr-xr-x   0 andi       (501) staff       (20)        0 2023-07-10 13:53:57.568463 language-agent-0.2/language_agent.egg-info/
+-rw-r--r--   0 andi       (501) staff       (20)     1812 2023-07-10 13:53:57.000000 language-agent-0.2/language_agent.egg-info/PKG-INFO
+-rw-r--r--   0 andi       (501) staff       (20)      274 2023-07-10 13:53:57.000000 language-agent-0.2/language_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 andi       (501) staff       (20)        1 2023-07-10 13:53:57.000000 language-agent-0.2/language_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 andi       (501) staff       (20)       21 2023-07-10 13:53:57.000000 language-agent-0.2/language_agent.egg-info/requires.txt
+-rw-r--r--   0 andi       (501) staff       (20)       15 2023-07-10 13:53:57.000000 language-agent-0.2/language_agent.egg-info/top_level.txt
+-rw-r--r--   0 andi       (501) staff       (20)       38 2023-07-10 13:53:57.568823 language-agent-0.2/setup.cfg
+-rw-r--r--   0 andi       (501) staff       (20)      504 2023-07-10 13:51:48.000000 language-agent-0.2/setup.py
```

### Comparing `language-agent-0.1/PKG-INFO` & `language-agent-0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: language-agent
-Version: 0.1
+Version: 0.2
 Description-Content-Type: text/markdown
 
-# AI-Agent
+# Language-Agent
 
-AI-Agent is a Python package that allows for easy integration with OpenAI's GPT-4 model. The package provides a simple API to generate text completions given a user prompt.
+Language-Agent is a Python package that allows for easy integration with OpenAI's GPT-4 model. The package provides a simple API to generate text completions given a user prompt.
 
-AI-Agent is perfect for developers looking to utilize OpenAI's powerful language model in their applications without the need to directly interact with OpenAI's API.
+Lanuage-Agent is perfect for developers looking to utilize OpenAI's powerful language model in their applications without the need to directly interact with OpenAI's API.
 
 ## Key Features
 
 - Simple API for text generation
 - Automatic handling of API keys through environment variables
 - Easily customizable user prompt and context
 
 ## Installation
 
-To install AI-Agent, you can use pip:
+To install Lanuage-Agent, you can use pip:
 
-$$$ pip install $$$
+``` pip install ```
 
 Before using the package, you'll need to set your OpenAI API key in a `.env` file:
 
-$$$ OPENAI_API_KEY='your-key-here' $$$
+``` OPENAI_API_KEY='your-key-here' ```
 
 
 Make sure the `.env` file is in the root directory of your project.
 
 ## Usage
 
 Using AI-Agent is simple. Below is a sample code snippet:
```

### Comparing `language-agent-0.1/language_agent.egg-info/PKG-INFO` & `language-agent-0.2/language_agent.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: language-agent
-Version: 0.1
+Version: 0.2
 Description-Content-Type: text/markdown
 
-# AI-Agent
+# Language-Agent
 
-AI-Agent is a Python package that allows for easy integration with OpenAI's GPT-4 model. The package provides a simple API to generate text completions given a user prompt.
+Language-Agent is a Python package that allows for easy integration with OpenAI's GPT-4 model. The package provides a simple API to generate text completions given a user prompt.
 
-AI-Agent is perfect for developers looking to utilize OpenAI's powerful language model in their applications without the need to directly interact with OpenAI's API.
+Lanuage-Agent is perfect for developers looking to utilize OpenAI's powerful language model in their applications without the need to directly interact with OpenAI's API.
 
 ## Key Features
 
 - Simple API for text generation
 - Automatic handling of API keys through environment variables
 - Easily customizable user prompt and context
 
 ## Installation
 
-To install AI-Agent, you can use pip:
+To install Lanuage-Agent, you can use pip:
 
-$$$ pip install $$$
+``` pip install ```
 
 Before using the package, you'll need to set your OpenAI API key in a `.env` file:
 
-$$$ OPENAI_API_KEY='your-key-here' $$$
+``` OPENAI_API_KEY='your-key-here' ```
 
 
 Make sure the `.env` file is in the root directory of your project.
 
 ## Usage
 
 Using AI-Agent is simple. Below is a sample code snippet:
```

