# Comparing `tmp/Pydule-3.3.5.tar.gz` & `tmp/Pydule-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pydule-3.3.5.tar", last modified: Thu May 25 09:38:55 2023, max compression
+gzip compressed data, was "Pydule-3.3.6.tar", last modified: Mon Jul 10 01:34:59 2023, max compression
```

## Comparing `Pydule-3.3.5.tar` & `Pydule-3.3.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 09:38:55.685967 Pydule-3.3.5/
--rw-rw-rw-   0        0        0     2543 2023-05-25 09:38:55.665796 Pydule-3.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     1779 2023-05-25 09:27:27.000000 Pydule-3.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 09:38:55.685967 Pydule-3.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1474 2023-05-25 09:27:52.000000 Pydule-3.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:38:55.597077 Pydule-3.3.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 09:38:55.661080 Pydule-3.3.5/src/Pydule.egg-info/
--rw-rw-rw-   0        0        0     2543 2023-05-25 09:38:54.000000 Pydule-3.3.5/src/Pydule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-05-25 09:38:54.000000 Pydule-3.3.5/src/Pydule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 09:38:54.000000 Pydule-3.3.5/src/Pydule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      237 2023-05-25 09:38:54.000000 Pydule-3.3.5/src/Pydule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-25 09:38:54.000000 Pydule-3.3.5/src/Pydule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    21890 2023-05-19 06:13:54.000000 Pydule-3.3.5/src/Pydule.py
+drwxrwxrwx   0        0        0        0 2023-07-10 01:34:59.679691 Pydule-3.3.6/
+-rw-rw-rw-   0        0        0     2606 2023-07-10 01:34:59.668770 Pydule-3.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1842 2023-07-09 13:47:24.000000 Pydule-3.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 01:34:59.679691 Pydule-3.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1507 2023-07-10 01:32:58.000000 Pydule-3.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 01:34:59.508017 Pydule-3.3.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 01:34:59.659743 Pydule-3.3.6/src/Pydule.egg-info/
+-rw-rw-rw-   0        0        0     2606 2023-07-10 01:34:58.000000 Pydule-3.3.6/src/Pydule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-07-10 01:34:59.000000 Pydule-3.3.6/src/Pydule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 01:34:58.000000 Pydule-3.3.6/src/Pydule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      258 2023-07-10 01:34:58.000000 Pydule-3.3.6/src/Pydule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 01:34:59.000000 Pydule-3.3.6/src/Pydule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    49497 2023-07-09 23:54:27.000000 Pydule-3.3.6/src/Pydule.py
```

### Comparing `Pydule-3.3.5/PKG-INFO` & `Pydule-3.3.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.3.5
+Version: 3.3.6
 Summary: Access ChatGPT,Track Location,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -22,15 +22,17 @@
 - Get Battery Percentage
 - Access ChatGPT
 - Get Any Website HTML
 - Encrypt and Decrypt a String
 - Record Screen,Internal Audio and Microphone
 - Seperate String
 - Insert Elements in Tuple & String
+- Check Internet Download and Upload Speed
 - Generate Qrcode
+- Print Emoji
 - Copy Text
 - Language Translation
 - Edit JSON Files
 - Replace Letters in String
 - Check Weather of any City
 - Open any File
 - Play Songs
@@ -76,15 +78,15 @@
 # to Get all Available Functions
 py.functions() 
 
 # to Open Calculator
 py.openapp('calculator')
 
 # to Copy Text
-py.copy('Hello World')
+py.copytext('Hello World')
 
 # to play mp3
 py.playmusic('PATH')
 
 # to Access ChatGPT
 from Pydule import AI
 print(AI.ChatGPT('Hi There','Your API Key'))
```

### Comparing `Pydule-3.3.5/README.md` & `Pydule-3.3.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 - Get Battery Percentage
 - Access ChatGPT
 - Get Any Website HTML
 - Encrypt and Decrypt a String
 - Record Screen,Internal Audio and Microphone
 - Seperate String
 - Insert Elements in Tuple & String
+- Check Internet Download and Upload Speed
 - Generate Qrcode
+- Print Emoji
 - Copy Text
 - Language Translation
 - Edit JSON Files
 - Replace Letters in String
 - Check Weather of any City
 - Open any File
 - Play Songs
@@ -62,15 +64,15 @@
 # to Get all Available Functions
 py.functions() 
 
 # to Open Calculator
 py.openapp('calculator')
 
 # to Copy Text
-py.copy('Hello World')
+py.copytext('Hello World')
 
 # to play mp3
 py.playmusic('PATH')
 
 # to Access ChatGPT
 from Pydule import AI
 print(AI.ChatGPT('Hi There','Your API Key'))
```

### Comparing `Pydule-3.3.5/setup.py` & `Pydule-3.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md','r') as fh:
 	long_description = fh.read()
 
 setup(
 	name='Pydule',
-	version='3.3.5',
+	version='3.3.6',
 	description="Access ChatGPT,Track Location,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..",
 	author='D.Tamil Mutharasan',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	packages=setuptools.find_packages(),
 	keywords=['python','PyDule','Module','Pydule','pydule','matrix','qrcode','youtube','weather','list','tuple','set','dictionary','clear','color','pick_color','open','app','search','play','mp3','song','restart','system','shutdown','date','time','text_to_speech','text','speech'],
 	classifiers=[
@@ -43,11 +43,13 @@
 		'wave',
 		'opencv-python',
 		'openai',
 		'phonenumbers',
 		'SpeechRecognition',
 		'Pillow',
 		'pyinstaller',
-		'pyfiglet'
+		'pyfiglet',
+		'pygame',
+		'speedtest-cli'
 	]
 
 )
```

### Comparing `Pydule-3.3.5/src/Pydule.egg-info/PKG-INFO` & `Pydule-3.3.6/src/Pydule.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.3.5
+Version: 3.3.6
 Summary: Access ChatGPT,Track Location,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -22,15 +22,17 @@
 - Get Battery Percentage
 - Access ChatGPT
 - Get Any Website HTML
 - Encrypt and Decrypt a String
 - Record Screen,Internal Audio and Microphone
 - Seperate String
 - Insert Elements in Tuple & String
+- Check Internet Download and Upload Speed
 - Generate Qrcode
+- Print Emoji
 - Copy Text
 - Language Translation
 - Edit JSON Files
 - Replace Letters in String
 - Check Weather of any City
 - Open any File
 - Play Songs
@@ -76,15 +78,15 @@
 # to Get all Available Functions
 py.functions() 
 
 # to Open Calculator
 py.openapp('calculator')
 
 # to Copy Text
-py.copy('Hello World')
+py.copytext('Hello World')
 
 # to play mp3
 py.playmusic('PATH')
 
 # to Access ChatGPT
 from Pydule import AI
 print(AI.ChatGPT('Hi There','Your API Key'))
```

