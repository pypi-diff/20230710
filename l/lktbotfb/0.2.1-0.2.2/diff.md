# Comparing `tmp/lktbotfb-0.2.1.tar.gz` & `tmp/lktbotfb-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lktbotfb-0.2.1.tar", last modified: Mon Jul 10 17:32:23 2023, max compression
+gzip compressed data, was "lktbotfb-0.2.2.tar", last modified: Mon Jul 10 17:58:36 2023, max compression
```

## Comparing `lktbotfb-0.2.1.tar` & `lktbotfb-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 17:32:23.052124 lktbotfb-0.2.1/
--rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      885 2023-07-10 17:32:23.051172 lktbotfb-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.2.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 17:32:23.053155 lktbotfb-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-10 17:31:44.000000 lktbotfb-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 17:32:22.997130 lktbotfb-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 17:32:23.012126 lktbotfb-0.2.1/src/botfb/
--rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.2.1/src/botfb/__init__.py
--rw-rw-rw-   0        0        0     8424 2023-07-10 14:49:26.000000 lktbotfb-0.2.1/src/botfb/mylib.py
-drwxrwxrwx   0        0        0        0 2023-07-10 17:32:23.048130 lktbotfb-0.2.1/src/lktbotfb.egg-info/
--rw-rw-rw-   0        0        0      885 2023-07-10 17:32:22.000000 lktbotfb-0.2.1/src/lktbotfb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-10 17:32:22.000000 lktbotfb-0.2.1/src/lktbotfb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 17:32:22.000000 lktbotfb-0.2.1/src/lktbotfb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-10 17:32:22.000000 lktbotfb-0.2.1/src/lktbotfb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 17:32:22.000000 lktbotfb-0.2.1/src/lktbotfb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 17:58:36.756463 lktbotfb-0.2.2/
+-rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      885 2023-07-10 17:58:36.754463 lktbotfb-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.2.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 17:58:36.757461 lktbotfb-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-10 17:47:08.000000 lktbotfb-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 17:58:36.709467 lktbotfb-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 17:58:36.722464 lktbotfb-0.2.2/src/botfb/
+-rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.2.2/src/botfb/__init__.py
+-rw-rw-rw-   0        0        0     8200 2023-07-10 17:56:58.000000 lktbotfb-0.2.2/src/botfb/mylib.py
+drwxrwxrwx   0        0        0        0 2023-07-10 17:58:36.752463 lktbotfb-0.2.2/src/lktbotfb.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-07-10 17:58:36.000000 lktbotfb-0.2.2/src/lktbotfb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-10 17:58:36.000000 lktbotfb-0.2.2/src/lktbotfb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 17:58:36.000000 lktbotfb-0.2.2/src/lktbotfb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 17:58:36.000000 lktbotfb-0.2.2/src/lktbotfb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 17:58:36.000000 lktbotfb-0.2.2/src/lktbotfb.egg-info/top_level.txt
```

### Comparing `lktbotfb-0.2.1/LICENSE` & `lktbotfb-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lktbotfb-0.2.1/PKG-INFO` & `lktbotfb-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.2.1
+Version: 0.2.2
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lktbotfb-0.2.1/setup.py` & `lktbotfb-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='lktbotfb',
-  version='0.2.1',
+  version='0.2.2',
   description='This makes it easy for you to create a chatbot for your Facebook page',
   long_description=open('README.txt').read(),
   url='https://github.com/AmirLouktaila/lktbotfb',  
   author='Salah Louktaila',
   author_email='amir.Louktila@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `lktbotfb-0.2.1/src/botfb/mylib.py` & `lktbotfb-0.2.2/src/botfb/mylib.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         global keys
         token=self.token
         keys=self.keys
 
     def getHost(self, host):
         self.hostname = host
         global hostname
-
+        hostname=self.hostname
         file_path_setting = f"{current_path}\\{namebot_}\\{namebot_}"
         os.chdir(file_path_setting)
         name_setting = "settings.py"
         
         def replace_word_in_file(file_path, old_word, new_word):
             try:
                 with open(file_path, 'r') as file:
@@ -92,24 +92,21 @@
                 modified_content = content.replace(old_word, new_word)
     
                 with open(file_path, 'w') as file:
                     file.write(modified_content)
     
             except FileNotFoundError:
                 print("error in this file try again")
-        if hostname is not None:
-            file_path = name_setting
-            old_word = 'ALLOWED_HOSTS = []'
-            new_word ='ALLOWED_HOSTS = ' + "['{}','localhost']".format(str(hostname))
-            print('done add host')
-            replace_word_in_file(file_path, old_word, new_word)
-        else:
-            pass
 
         file_path = name_setting
+        old_word = 'ALLOWED_HOSTS = []'
+        new_word ='ALLOWED_HOSTS = ' + "['{}','localhost']".format(str(hostname))
+        print('done add host')
+        replace_word_in_file(file_path, old_word, new_word)
+        file_path = name_setting
         old_word_app = '''
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
@@ -245,21 +242,17 @@
 
         file_path = file_path_view
         old_word_event ='start_event{}'
         new_word_event =str(getevent)
         replace_word_in_file_view(file_path, old_word_event, new_word_event)
 
     def runbot(self):
-        if hostname is None:
-            os.chdir(f"{current_path}\\{namebot_}")
-            os.system("python manage.py runserver")    
-        else:
-            print(f"open this :https://{hostname}/fb/page{code_srt}")
-            os.chdir(f"{current_path}\\{namebot_}")
-            os.system("python manage.py runserver")
+        print(f"open this :https://{hostname}/fb/page{code_srt}")
+        os.chdir(f"{current_path}\\{namebot_}")
+        os.system("python manage.py runserver")
 
 class EditBot:
     def __init__(self, namebot):
         self.namebot_ = namebot
         global startapp
         global namebot_
         global startapp_edit
```

### Comparing `lktbotfb-0.2.1/src/lktbotfb.egg-info/PKG-INFO` & `lktbotfb-0.2.2/src/lktbotfb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.2.1
+Version: 0.2.2
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

