# Comparing `tmp/lktbotfb-0.2.3.tar.gz` & `tmp/lktbotfb-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lktbotfb-0.2.3.tar", last modified: Mon Jul 10 18:42:29 2023, max compression
+gzip compressed data, was "lktbotfb-0.3.1.tar", last modified: Mon Jul 10 20:01:41 2023, max compression
```

## Comparing `lktbotfb-0.2.3.tar` & `lktbotfb-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 18:42:29.972245 lktbotfb-0.2.3/
--rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      885 2023-07-10 18:42:29.969246 lktbotfb-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.2.3/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 18:42:29.972245 lktbotfb-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-10 18:41:50.000000 lktbotfb-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:42:29.875250 lktbotfb-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 18:42:29.900244 lktbotfb-0.2.3/src/botfb/
--rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.2.3/src/botfb/__init__.py
--rw-rw-rw-   0        0        0     8441 2023-07-10 18:17:31.000000 lktbotfb-0.2.3/src/botfb/mylib.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:42:29.964251 lktbotfb-0.2.3/src/lktbotfb.egg-info/
--rw-rw-rw-   0        0        0      885 2023-07-10 18:42:29.000000 lktbotfb-0.2.3/src/lktbotfb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-10 18:42:29.000000 lktbotfb-0.2.3/src/lktbotfb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 18:42:29.000000 lktbotfb-0.2.3/src/lktbotfb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-10 18:42:29.000000 lktbotfb-0.2.3/src/lktbotfb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 18:42:29.000000 lktbotfb-0.2.3/src/lktbotfb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 20:01:41.715022 lktbotfb-0.3.1/
+-rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      885 2023-07-10 20:01:41.713021 lktbotfb-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.3.1/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 20:01:41.716021 lktbotfb-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-10 20:00:24.000000 lktbotfb-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:01:41.620027 lktbotfb-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 20:01:41.665075 lktbotfb-0.3.1/src/botfb/
+-rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.3.1/src/botfb/__init__.py
+-rw-rw-rw-   0        0        0     8446 2023-07-10 19:58:04.000000 lktbotfb-0.3.1/src/botfb/mylib.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:01:41.710027 lktbotfb-0.3.1/src/lktbotfb.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-07-10 20:01:41.000000 lktbotfb-0.3.1/src/lktbotfb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-10 20:01:41.000000 lktbotfb-0.3.1/src/lktbotfb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 20:01:41.000000 lktbotfb-0.3.1/src/lktbotfb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 20:01:41.000000 lktbotfb-0.3.1/src/lktbotfb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 20:01:41.000000 lktbotfb-0.3.1/src/lktbotfb.egg-info/top_level.txt
```

### Comparing `lktbotfb-0.2.3/LICENSE` & `lktbotfb-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lktbotfb-0.2.3/PKG-INFO` & `lktbotfb-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.2.3
+Version: 0.3.1
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lktbotfb-0.2.3/setup.py` & `lktbotfb-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='lktbotfb',
-  version='0.2.3',
+  version='0.3.1',
   description='This makes it easy for you to create a chatbot for your Facebook page',
   long_description=open('README.txt').read(),
   url='https://github.com/AmirLouktaila/lktbotfb',  
   author='Salah Louktaila',
   author_email='amir.Louktila@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `lktbotfb-0.2.3/src/botfb/mylib.py` & `lktbotfb-0.3.1/src/botfb/mylib.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,30 +26,30 @@
         startapp = str(namebot_ + "_")
         os.chdir(f"{namebot_}")
         creatbotapp = f"python manage.py startapp {startapp}"
         os.system(creatbotapp)
         startapp_edit="done create a app"   
         print(startapp_edit)
         time.sleep(2)
-        os.chdir(f"{current_path}\\{namebot_}\\{startapp}")
+        os.chdir(os.path.join(current_path, namebot_, startapp))
         name_urls = "urls.py"
         with open(name_urls, 'w') as files:
             files.write(
 f'''
 # yomamabot/fb_yomamabot/urls.py
 from django.urls import re_path, include
 from .views import YoMamaBotView
 urlpatterns = [
     re_path(r'^page{code_srt}/?$', YoMamaBotView.as_view()) 
 ]
 '''
             )
             files.close()
 
-        os.chdir(f"{current_path}\\{namebot_}\\{namebot_}")
+        os.chdir(os.path.join(current_path, namebot_, startapp))
         files_urls = "urls.py"
 
         with open(files_urls, 'w') as files:
             files.write(
 f'''
 from django.urls import re_path, include
 from django.contrib import admin
@@ -76,15 +76,15 @@
         token=self.token
         keys=self.keys
 
     def getHost(self, host):
         self.hostname = host
         global hostname
         hostname=self.hostname
-        file_path_setting = f"{current_path}\\{namebot_}\\{namebot_}"
+        file_path_setting =os.path.join(current_path, namebot_, namebot_)
         os.chdir(file_path_setting)
         name_setting = "settings.py"
         
         def replace_word_in_file(file_path, old_word, new_word):
             try:
                 with open(file_path, 'r') as file:
                     content = file.read()
@@ -131,15 +131,15 @@
         self.talking=talk
         talking = self.talking
         self.replying=relkt
         replying = self.replying
         
         self.funsing=funsme
         funsing = self.funsing
-        os.chdir(f"{current_path}\\{namebot_}\\{startapp}")
+        os.chdir(os.path.join(current_path, namebot_, startapp))
         file_path_view = "views.py"
         with open(file_path_view, 'w') as file_view:
             file_view.write('''
 
 from django.shortcuts import render
 from pprint import pprint
 import json, requests, random, re
@@ -250,31 +250,24 @@
         
         file_path = file_path_view
         old_word_event ='funme'
         new_word_event =str(funsing)
         replace_word_in_file_view(file_path, old_word_event, new_word_event)
     def runbot(self):
         print(f"open this :https://{hostname}/fb/page{code_srt}")
-        os.chdir(f"{current_path}\\{namebot_}")
+        os.chdir(os.path.join(current_path, namebot_))
         os.system("python manage.py runserver")
 
 class EditBot:
     def __init__(self, namebot):
         self.namebot_ = namebot
         global startapp
         global namebot_
         global startapp_edit
         global namebot_edit
         namebot_=self.namebot_
 
-        name_bot=f"{current_path}\\{namebot_}"
+        name_bot=os.path.join(current_path, namebot_)
         if os.path.exists(name_bot):
             #if os.access(name_bot, os.W_OK):
             shutil.rmtree(name_bot)
-            print("Editing")
-
-
-            
-
-
-
-
+            print("Editing")
```

### Comparing `lktbotfb-0.2.3/src/lktbotfb.egg-info/PKG-INFO` & `lktbotfb-0.3.1/src/lktbotfb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.2.3
+Version: 0.3.1
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

