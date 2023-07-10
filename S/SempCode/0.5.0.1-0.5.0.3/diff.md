# Comparing `tmp/SempCode-0.5.0.1-py3-none-any.whl.zip` & `tmp/SempCode-0.5.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5550 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     1750 b- defN 23-Jul-08 11:17 Semp/Command.py
+Zip file size: 5634 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     1808 b- defN 23-Jul-10 12:58 Semp/Command.py
 -rw-rw-rw-  2.0 fat     2390 b- defN 23-Jul-08 10:25 Semp/SempWrite.py
--rw-rw-rw-  2.0 fat     3700 b- defN 23-Jul-10 10:58 Semp/__init__.py
+-rw-rw-rw-  2.0 fat     3938 b- defN 23-Jul-10 13:08 Semp/__init__.py
 -rw-rw-rw-  2.0 fat      370 b- defN 23-Jul-08 11:54 Semp/about.py
--rw-rw-rw-  2.0 fat     2660 b- defN 23-Jul-10 10:57 Semp/EasyTkinter/__init__.py
--rw-rw-rw-  2.0 fat      750 b- defN 23-Jul-10 10:58 SempCode-0.5.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-10 10:58 SempCode-0.5.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-10 10:58 SempCode-0.5.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      681 b- defN 23-Jul-10 10:58 SempCode-0.5.0.1.dist-info/RECORD
-9 files, 12398 bytes uncompressed, 4386 bytes compressed:  64.6%
+-rw-rw-rw-  2.0 fat     2594 b- defN 23-Jul-10 13:24 Semp/EasyTkinter/__init__.py
+-rw-rw-rw-  2.0 fat      842 b- defN 23-Jul-10 13:26 SempCode-0.5.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-10 13:26 SempCode-0.5.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-10 13:26 SempCode-0.5.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      681 b- defN 23-Jul-10 13:26 SempCode-0.5.0.3.dist-info/RECORD
+9 files, 12720 bytes uncompressed, 4470 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: Semp/about.py
 Comment: 
 
 Filename: Semp/EasyTkinter/__init__.py
 Comment: 
 
-Filename: SempCode-0.5.0.1.dist-info/METADATA
+Filename: SempCode-0.5.0.3.dist-info/METADATA
 Comment: 
 
-Filename: SempCode-0.5.0.1.dist-info/WHEEL
+Filename: SempCode-0.5.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: SempCode-0.5.0.1.dist-info/top_level.txt
+Filename: SempCode-0.5.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: SempCode-0.5.0.1.dist-info/RECORD
+Filename: SempCode-0.5.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Semp/Command.py

```diff
@@ -1,14 +1,15 @@
 """
     SempCommand Alpha
-    Version:a102
+    Version:a109
 """
 from subprocess import run
 from pathlib import Path
 from datetime import datetime
+from os import system
 
 
 EXIST_TRUE=True
 EXIST_FALSE=False
 class ModeError(Exception):
     def __init__(self, *args, **kwargs):
         pass
@@ -40,10 +41,12 @@
             self.date=datetime.utcfromtimestamp(self.time)
             return self.date.strftime("%Y.%m.%d %H:%M:%S")
         elif mode == 1:
             self.time = Path(path).stat().st_ctime
             self.date = datetime.utcfromtimestamp(self.time)
             return self.date.strftime("%Y.%m.%d %H:%M:%S")
         else:
-            raise ModeError("Mode 0:Edit Time,Mode 1:Create Time.Please enter someone.")
+            raise ModeError("Because not in 0&1")
     def rename(self,path: str = ...,new_name: str = ...):
-        Path(path).rename(new_name)
+        Path(path).rename(new_name)
+    def systemcommand(self,command: str = ...):
+        system(command)
```

## Semp/__init__.py

```diff
@@ -1,27 +1,31 @@
 """
     Semp Python Tool by Win12Home
-    Version:0.5.0.1 Alpha
+    Version:0.5.0.3 Beta
     
 """
 from PIL import Image,ImageTk
 from requests import *
 from sys import set_int_max_str_digits as max
+from subprocess import Popen
 
 
 max(0)
 BINARY_TRUE="BTRUE"
 BINARY_FALSE="BFALSE"
 
 class NumberError(Exception):
     def __init__(self, *args, **kwargs):
         pass
+
 class BoolError(Exception):
     def __init__(self, *args, **kwargs):
         pass
+
+ 
 def PhotoTk(file: str = ...):
     photo=Image.open(file)
     #Open Photo
     tkphoto=ImageTk.PhotoImage(image=photo)
     #Save Photo
     return tkphoto
 
@@ -35,14 +39,15 @@
         try:
             for x in range(b_from, to + 1,passnum):
                 a.append(x)
             return a
         except:
             raise NumberError("Name error.")
 
+ 
 class request_simplifies:
     def Download(website: str = ...,name: str = ...,binary: bool = ...):
         r = get(website)
         if binary == True or binary == BINARY_TRUE:
             with open(name, "wb") as f:
                 for chunk in r.iter_content(chunk_size=512):
                     f.write(chunk)
@@ -60,22 +65,24 @@
 
 def power_operation(num1: int = ...,num2: int = ...):
     num=num1
     for __count in range(num2-1):
         num*=num1
     return num
 
+ 
 def fibonacci_sequence(to: int = ...):
     numlist=[1,1,1]
     num=1
     for __count in range(to-3):
         num+=numlist[len(numlist)-2]
         numlist.append(num)
     return numlist
 
+ 
 class Requester:
     def __init__(self,website: str = ...):
         super().__init__()
         self.websitelink=website
     def Download(self,name: str = ...,binary=False):
         self.r = get(self.websitelink)
         if binary == True or binary == BINARY_TRUE:
@@ -90,14 +97,29 @@
         #This method can download TXT file, JSON file, JS file, etc
         else:
             raise BoolError("Not "+str(name)+".Expected BINARY_TRUE or BINARY_FALSE")
     def ResponseGet(self):
         self.r=get(self.websitelink)
         return {"status_code":self.r.status_code,"url":self.r.url,"text":self.r.text}
 
+ 
+def PyPrompt():
+    Popen(
+        "python.exe",
+        shell=True,
+        encoding="utf-8"
+    )
+
+ 
+def CmdPrompt():
+    Popen(
+        "cmd.exe",
+        shell=True
+    )
+
 """
 Here are some examples.
 Response(variable):
     response=Requester("https://1.1.1.1/")
     response.ResponseGet()
 Response(code):
     request_simplifies.ResponseGet("https://1.1.1.1/")
```

## Semp/EasyTkinter/__init__.py

```diff
@@ -66,12 +66,7 @@
     def Use(self,command:str = ...):
         self.runner=Popen(command,shell=True,stdout=PIPE,stderr=STDOUT,encoding="gb2312")
         self.text["state"]=NORMAL
         self.ms=self.runner.communicate()[0]
         self.msin=str(self.ms)[2:len(self.ms)-6]
         self.text.insert(END,f"{self.ms}\n")
         self.text["state"]=DISABLED
-
-
-
-if __name__ == '__main__':
-    CommandWindow().mainloop()
```

## Comparing `SempCode-0.5.0.1.dist-info/METADATA` & `SempCode-0.5.0.3.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: SempCode
-Version: 0.5.0.1
+Version: 0.5.0.3
 Summary: Simplified the Python Code
 Author: 是真的Win12Home
 Author-email: mcdhj-work@outlook.com
 License: Mozilla Public License Version 2.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Requires: requests
 Requires: pillow
 Requires: pathlib
 Requires: subprocess
 Requires: datetime
 Requires: ctypes
 Requires: ttkthemes
 Description-Content-Type: text/markdown
 
 ---
 Hello Semp!
 ---
 Semp is can simple some code in Python.\
 **1.Updates**\
-*v0.4.0.2(Update)*\
+*v0.5.0.3*(Update)\
+Add PyPrompt\
+Add CmdPrompt\
+Add systemcommand in Command.Commander\
+*v0.5.0.2(Update)*\
 Add Semp.EasyTkinter\
 *v0.3.7.5(Fix)*\
 Fix v0.3.7.2 bugs\
 *v0.3.7.2(Broken)*\
 Add NumberError,BoolError and ModeError\
 Add Command.Commander(Simplified pathlib,subprocess)\
 **2.Author**\
```

