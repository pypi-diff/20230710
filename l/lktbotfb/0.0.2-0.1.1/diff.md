# Comparing `tmp/lktbotfb-0.0.2.tar.gz` & `tmp/lktbotfb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lktbotfb-0.0.2.tar", last modified: Mon Jul 10 16:33:01 2023, max compression
+gzip compressed data, was "lktbotfb-0.1.1.tar", last modified: Mon Jul 10 16:51:37 2023, max compression
```

## Comparing `lktbotfb-0.0.2.tar` & `lktbotfb-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 16:33:01.664227 lktbotfb-0.0.2/
--rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      844 2023-07-10 16:33:01.663227 lktbotfb-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-10 16:33:01.660228 lktbotfb-0.0.2/lktbotfb.egg-info/
--rw-rw-rw-   0        0        0      844 2023-07-10 16:33:01.000000 lktbotfb-0.0.2/lktbotfb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-07-10 16:33:01.000000 lktbotfb-0.0.2/lktbotfb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 16:33:01.000000 lktbotfb-0.0.2/lktbotfb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-10 16:33:01.000000 lktbotfb-0.0.2/lktbotfb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 16:33:01.000000 lktbotfb-0.0.2/lktbotfb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 16:33:01.665228 lktbotfb-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      683 2023-07-10 16:32:27.000000 lktbotfb-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 16:51:37.956783 lktbotfb-0.1.1/
+-rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      885 2023-07-10 16:51:37.954786 lktbotfb-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.1.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 16:51:37.950782 lktbotfb-0.1.1/lktbotfb.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-07-10 16:51:37.000000 lktbotfb-0.1.1/lktbotfb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-07-10 16:51:37.000000 lktbotfb-0.1.1/lktbotfb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 16:51:37.000000 lktbotfb-0.1.1/lktbotfb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 16:51:37.000000 lktbotfb-0.1.1/lktbotfb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 16:51:37.000000 lktbotfb-0.1.1/lktbotfb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 16:51:37.956783 lktbotfb-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      724 2023-07-10 16:49:50.000000 lktbotfb-0.1.1/setup.py
```

### Comparing `lktbotfb-0.0.2/LICENSE` & `lktbotfb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lktbotfb-0.0.2/PKG-INFO` & `lktbotfb-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.0.2
+Version: 0.1.1
 Summary: This makes it easy for you to create a chatbot for your Facebook page
-Home-page: 
+Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `lktbotfb-0.0.2/lktbotfb.egg-info/PKG-INFO` & `lktbotfb-0.1.1/lktbotfb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.0.2
+Version: 0.1.1
 Summary: This makes it easy for you to create a chatbot for your Facebook page
-Home-page: 
+Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `lktbotfb-0.0.2/setup.py` & `lktbotfb-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,18 +6,18 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='lktbotfb',
-  version='0.0.2',
+  version='0.1.1',
   description='This makes it easy for you to create a chatbot for your Facebook page',
   long_description=open('README.txt').read(),
-  url='',  
+  url='https://github.com/AmirLouktaila/lktbotfb',  
   author='Salah Louktaila',
   author_email='amir.Louktila@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='chatbot', 
   packages=find_packages(),
   install_requires=['django']
```

