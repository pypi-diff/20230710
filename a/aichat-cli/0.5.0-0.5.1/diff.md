# Comparing `tmp/aichat-cli-0.5.0.tar.gz` & `tmp/aichat-cli-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aichat-cli-0.5.0.tar", last modified: Fri Jul  7 17:19:59 2023, max compression
+gzip compressed data, was "aichat-cli-0.5.1.tar", last modified: Mon Jul 10 18:21:47 2023, max compression
```

## Comparing `aichat-cli-0.5.0.tar` & `aichat-cli-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 17:19:59.100624 aichat-cli-0.5.0/
--rw-rw-rw-   0        0        0    35823 2023-05-23 15:04:57.000000 aichat-cli-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     5240 2023-07-07 17:19:59.099620 aichat-cli-0.5.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 17:19:59.098613 aichat-cli-0.5.0/aichat_cli.egg-info/
--rw-rw-rw-   0        0        0     5240 2023-07-07 17:19:59.000000 aichat-cli-0.5.0/aichat_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-07-07 17:19:59.000000 aichat-cli-0.5.0/aichat_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 17:19:59.000000 aichat-cli-0.5.0/aichat_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-07 17:19:59.000000 aichat-cli-0.5.0/aichat_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 17:19:59.000000 aichat-cli-0.5.0/aichat_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 17:19:59.100624 aichat-cli-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1063 2023-07-07 17:19:38.000000 aichat-cli-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:21:47.574262 aichat-cli-0.5.1/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 15:04:57.000000 aichat-cli-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     5273 2023-07-10 18:21:47.573260 aichat-cli-0.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-10 18:21:47.571260 aichat-cli-0.5.1/aichat_cli.egg-info/
+-rw-rw-rw-   0        0        0     5273 2023-07-10 18:21:47.000000 aichat-cli-0.5.1/aichat_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-07-10 18:21:47.000000 aichat-cli-0.5.1/aichat_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 18:21:47.000000 aichat-cli-0.5.1/aichat_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-07-10 18:21:47.000000 aichat-cli-0.5.1/aichat_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 18:21:47.000000 aichat-cli-0.5.1/aichat_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 18:21:47.575262 aichat-cli-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-07-10 18:21:14.000000 aichat-cli-0.5.1/setup.py
```

### Comparing `aichat-cli-0.5.0/LICENSE` & `aichat-cli-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aichat-cli-0.5.0/PKG-INFO` & `aichat-cli-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aichat-cli
-Version: 0.5.0
+Version: 0.5.1
 Summary: A CLI app that allows you to have interactive conversations with different AI bots
 Home-page: https://github.com/TheLime1/aichat-cli
 Author: TheLime1
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 
 A command-line interface chatbot. It allows you to have interactive conversations with different bots, including GPT4 FOR FREE
 
 Check the web version [here](https://github.com/TheLime1/gptCensorFree) (WIP).
 
 Thanks to [@Lomusire](https://github.com/Lomusire) for providing premium tokens ❤️.
 
-We are in a race with poe.com devs baning our tokens, you can help by [generating tokens](https://krakenfiles.com/view/kUx2jPXcZ0/file.html). 
+We are in a race with poe.com devs baning our tokens, you can help by [generating tokens](https://drive.google.com/file/d/1D9oHx_com_cn_XzZfcQ7XLGyQ9xUtSAG/view?usp=sharing). 
 
 Updated poe.com token list [here](https://raw.githubusercontent.com/TheLime1/online-proxy-list/main/poe_token_check/poe_tokens.txt).
 
 ## Features✨
 
 - Choose between different bots.
 - Input messages for the chatbot via command-line arguments or interactively.
```

### Comparing `aichat-cli-0.5.0/aichat_cli.egg-info/PKG-INFO` & `aichat-cli-0.5.1/aichat_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aichat-cli
-Version: 0.5.0
+Version: 0.5.1
 Summary: A CLI app that allows you to have interactive conversations with different AI bots
 Home-page: https://github.com/TheLime1/aichat-cli
 Author: TheLime1
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 
 A command-line interface chatbot. It allows you to have interactive conversations with different bots, including GPT4 FOR FREE
 
 Check the web version [here](https://github.com/TheLime1/gptCensorFree) (WIP).
 
 Thanks to [@Lomusire](https://github.com/Lomusire) for providing premium tokens ❤️.
 
-We are in a race with poe.com devs baning our tokens, you can help by [generating tokens](https://krakenfiles.com/view/kUx2jPXcZ0/file.html). 
+We are in a race with poe.com devs baning our tokens, you can help by [generating tokens](https://drive.google.com/file/d/1D9oHx_com_cn_XzZfcQ7XLGyQ9xUtSAG/view?usp=sharing). 
 
 Updated poe.com token list [here](https://raw.githubusercontent.com/TheLime1/online-proxy-list/main/poe_token_check/poe_tokens.txt).
 
 ## Features✨
 
 - Choose between different bots.
 - Input messages for the chatbot via command-line arguments or interactively.
```

### Comparing `aichat-cli-0.5.0/setup.py` & `aichat-cli-0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 long_description = (base_path / "README.md").read_text(encoding="utf-8")
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="aichat-cli",
-    version="0.5.0",
+    version="0.5.1",
     author="TheLime1",
     license="GPLv3",
     description="A CLI app that allows you to have interactive conversations with different AI bots",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

